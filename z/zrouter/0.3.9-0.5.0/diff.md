# Comparing `tmp/zrouter-0.3.9.tar.gz` & `tmp/zrouter-0.5.0.tar.gz`

## Comparing `zrouter-0.3.9.tar` & `zrouter-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 zrouter-0.3.9/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.9/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.9/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.9/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.9/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 zrouter-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 zrouter-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 zrouter-0.5.0/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 zrouter-0.5.0/src/zrouter/restful.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.0/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.0/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.0/LICENSE
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 zrouter-0.5.0/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 zrouter-0.5.0/PKG-INFO
```

### Comparing `zrouter-0.3.9/src/zrouter/__init__.py` & `zrouter-0.5.0/src/zrouter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,89 @@
+from zrouter.exceptions import MessagePrompt
+from zrouter.utils.json import to_lowcase, iter_lowcase, iter_camel
 from flask import Blueprint, request
-from zrouter.exception import MessagePrompt
-from inspirare import json as json_
-from json import JSONDecodeError
 from jsonschema.exceptions import ValidationError
+from abc import ABC, abstractmethod
 from functools import wraps
+import random
 
 
-class RouterUtility:
+class ParamMixin:
     @staticmethod
     def get_params():
-        """ 获取路由参数"""
         if request.method in ['GET', 'DELETE']:
-            return json_.to_lowcase(request.args)
+            return to_lowcase(request.args)
         elif 'multipart/form-data' in request.content_type:
             return {
                 'files': request.files,
-                'params': json_.to_lowcase(request.form.to_dict())
+                'params': to_lowcase(request.form.to_dict())
             }
         else:
             try:
                 params = request.get_json()
-                return json_.iter_lowcase(params)
+                return iter_lowcase(params)
             except:
                 return {
                     'data': request.get_data()
                 }
 
     @staticmethod
     def clean_params(params):
-        """空值参数清理"""
-        return {k: v for k, v in params.items() if v not in ('', 'null') and v is not None}
+        return {k: v for k, v in params.items() if v not in ('', 'null', None)}
 
 
-class Router(Blueprint, RouterUtility):
+class Router(ABC, ParamMixin, Blueprint):
     """路由"""
-
     def __init__(self, *args, **kwargs):
         Blueprint.__init__(self, *args, **kwargs)
 
-    @property
-    def authorized(self):
+    @abstractmethod
+    def verify_user(self):
         return True
 
+    @abstractmethod
+    def handle_error(self, e):
+        pass
+
+    def wrap_func(self, func, direct=False, open=False):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            params = self.clean_params(self.get_params())
+            if not self.verify_user() and not open:
+                return {'code': 401, 'msg': '用户无权限'}
+            try:
+                data = func(**params)
+            except MessagePrompt as e:
+                return {'code': 500, 'msg': str(e)}
+            except ValidationError as e:
+                return {'code': 400, 'msg': str(e)}
+            except Exception as e:
+                self.handle_error(e)
+                raise e
+            if direct:
+                return data
+            if isinstance(data, dict):
+                data = iter_camel(data)
+            elif isinstance(data, list):
+                data = [iter_camel(item) for item in data]
+            return {'code': 200, 'msg': '操作成功', 'data': data}
+        return wrapper
+
+    def add_resource(self, rule, resource_class):
+        http_methods = ['get', 'post', 'put', 'delete']
+        
+        for method in http_methods:
+            if method in dir(resource_class):
+                endpoint = str(random.randint(10000000, 99999999))
+                self.add_url_rule(rule, endpoint, self.wrap_func(
+                    getattr(resource_class, method)), methods=[method.upper()])
+
+    def add_resources(self, resource_map):
+        for rule, resource_class in resource_map.items():
+            self.add_resource(rule, resource_class)
+
     def add(self, rule, open=False, direct=False, **options):
         def decorator(f):
-            def func_wrapper(func):
-                @wraps(func)
-                def wrapper(*args, **kwargs):
-                    params = self.clean_params(self.get_params())
-                    if not self.authorized and not open:
-                        return {'code': 401, 'msg': '用户无权限'}
-                    try:
-                        data = func(**params)
-                    except MessagePrompt as e:
-                        return {'code': 500, 'msg': str(e)}
-                    except ValidationError as e:
-                        return {'code': 400, 'msg': str(e)}
-                    if direct:
-                        return data
-                    if isinstance(data, dict):
-                        data = json_.iter_camel(data)
-                    elif isinstance(data, list):
-                        data = [json_.iter_camel(item) for item in data]
-                    return {'code': 200, 'msg': '操作成功', 'data': data}
-                return wrapper
             endpoint = options.pop("endpoint", None)
-            self.add_url_rule(rule, endpoint, func_wrapper(f), **options)
+            self.add_url_rule(rule, endpoint, self.wrap_func(
+                f, open=open, direct=direct), **options)
         return decorator
```

### Comparing `zrouter-0.3.9/LICENSE` & `zrouter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.9/pyproject.toml` & `zrouter-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.3.9"
+version = "0.5.0"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "flask==2.2.2",
-  "inspirare",
-  "jsonschema"
+  "jsonschema==4.17.3",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

