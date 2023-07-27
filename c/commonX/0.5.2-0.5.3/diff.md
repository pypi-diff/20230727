# Comparing `tmp/commonX-0.5.2.tar.gz` & `tmp/commonX-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonX-0.5.2.tar", last modified: Mon Jul 24 03:00:27 2023, max compression
+gzip compressed data, was "commonX-0.5.3.tar", last modified: Thu Jul 27 07:46:33 2023, max compression
```

## Comparing `commonX-0.5.2.tar` & `commonX-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 03:00:27.986121 commonX-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 03:00:18.000000 commonX-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 03:00:18.000000 commonX-0.5.2/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/base/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/genor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-24 03:00:18.000000 commonX-0.5.2/common/base/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/cookie_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/iphone_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/ocr_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 03:00:18.000000 commonX-0.5.2/common/ext/qq_email.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.982121 commonX-0.5.2/common/postman/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-24 03:00:18.000000 commonX-0.5.2/common/postman/postman_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/common/util/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/args_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/assert_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/decorator_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/exception_utll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/image_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/json_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/requests_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/sys_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/time_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-24 03:00:18.000000 commonX-0.5.2/common/util/typing_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:00:27.986121 commonX-0.5.2/commonX.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 03:00:27.000000 commonX-0.5.2/commonX.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:00:27.986121 commonX-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-24 03:00:18.000000 commonX-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.013275 commonX-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-27 07:46:33.013275 commonX-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 07:46:23.000000 commonX-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.001275 commonX-0.5.3/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-27 07:46:23.000000 commonX-0.5.3/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.001275 commonX-0.5.3/common/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/genor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-27 07:46:23.000000 commonX-0.5.3/common/base/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.005275 commonX-0.5.3/common/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-27 07:46:23.000000 commonX-0.5.3/common/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-27 07:46:23.000000 commonX-0.5.3/common/ext/cookie_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-27 07:46:23.000000 commonX-0.5.3/common/ext/iphone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-27 07:46:23.000000 commonX-0.5.3/common/ext/ocr_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-27 07:46:23.000000 commonX-0.5.3/common/ext/qq_email.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.005275 commonX-0.5.3/common/postman/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 07:46:23.000000 commonX-0.5.3/common/postman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-27 07:46:23.000000 commonX-0.5.3/common/postman/postman_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-27 07:46:23.000000 commonX-0.5.3/common/postman/postman_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-27 07:46:23.000000 commonX-0.5.3/common/postman/postman_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.005275 commonX-0.5.3/common/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/args_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/assert_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/decorator_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/exception_utll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/image_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/requests_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/sys_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 07:46:23.000000 commonX-0.5.3/common/util/typing_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 07:46:33.013275 commonX-0.5.3/commonX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-27 07:46:32.000000 commonX-0.5.3/commonX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-27 07:46:32.000000 commonX-0.5.3/commonX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 07:46:32.000000 commonX-0.5.3/commonX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 07:46:32.000000 commonX-0.5.3/commonX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 07:46:33.013275 commonX-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-27 07:46:23.000000 commonX-0.5.3/setup.py
```

### Comparing `commonX-0.5.2/PKG-INFO` & `commonX-0.5.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.5.2
+Version: 0.5.3
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.5.2/common/base/__init__.py` & `commonX-0.5.3/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/entity.py` & `commonX-0.5.3/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/genor.py` & `commonX-0.5.3/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/hook.py` & `commonX-0.5.3/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/logger.py` & `commonX-0.5.3/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/mapper.py` & `commonX-0.5.3/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/multi_task.py` & `commonX-0.5.3/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/packer.py` & `commonX-0.5.3/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/base/registry.py` & `commonX-0.5.3/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/ext/cookie_parser.py` & `commonX-0.5.3/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/ext/iphone_client.py` & `commonX-0.5.3/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/ext/qq_email.py` & `commonX-0.5.3/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/postman/postman_api.py` & `commonX-0.5.3/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/postman/postman_impl.py` & `commonX-0.5.3/common/postman/postman_impl.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/postman/postman_proxy.py` & `commonX-0.5.3/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/args_util.py` & `commonX-0.5.3/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/assert_util.py` & `commonX-0.5.3/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/decorator_util.py` & `commonX-0.5.3/common/util/decorator_util.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,8 +88,22 @@
 ):
     def wrapper(func):
         return SimpleCacheWrapper(func, cache_dict, cache_miss_msg, cache_hit_msg)
 
     return wrapper
 
 
-enable_cache = cache
+def field_cache(field_name, miss=None):
+    def wrapper(func):
+        def func_exec(*args, **kwargs):
+            obj = args[0]
+            attr = getattr(obj, field_name, None)
+            if attr != miss:
+                return attr
+
+            attr = func(*args, **kwargs)
+            setattr(obj, field_name, attr)
+            return attr
+
+        return func_exec
+
+    return wrapper
```

### Comparing `commonX-0.5.2/common/util/exception_utll.py` & `commonX-0.5.3/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/file_util.py` & `commonX-0.5.3/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/image_util.py` & `commonX-0.5.3/common/util/image_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/json_util.py` & `commonX-0.5.3/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/requests_util.py` & `commonX-0.5.3/common/util/requests_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/sys_util.py` & `commonX-0.5.3/common/util/sys_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/time_util.py` & `commonX-0.5.3/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/common/util/typing_util.py` & `commonX-0.5.3/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/commonX.egg-info/PKG-INFO` & `commonX-0.5.3/commonX.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.5.2
+Version: 0.5.3
 Summary: python common toolkit
 Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `commonX-0.5.2/commonX.egg-info/SOURCES.txt` & `commonX-0.5.3/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.5.2/setup.py` & `commonX-0.5.3/setup.py`

 * *Files identical despite different names*

