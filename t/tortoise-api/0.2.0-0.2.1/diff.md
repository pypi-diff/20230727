# Comparing `tmp/tortoise-api-0.2.0.tar.gz` & `tmp/tortoise-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.2.0.tar", last modified: Sun Jul 23 16:25:20 2023, max compression
+gzip compressed data, was "tortoise-api-0.2.1.tar", last modified: Thu Jul 27 10:59:42 2023, max compression
```

## Comparing `tortoise-api-0.2.0.tar` & `tortoise-api-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-23 16:25:20.259421 tortoise-api-0.2.0/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.0/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-23 16:25:20.259193 tortoise-api-0.2.0/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.0/README.md
--rw-r--r--   0 sol        (501) staff       (20)      679 2023-07-23 11:38:30.000000 tortoise-api-0.2.0/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-23 16:25:20.259477 tortoise-api-0.2.0/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-23 16:25:20.257853 tortoise-api-0.2.0/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.0/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     3136 2023-07-23 11:37:57.000000 tortoise-api-0.2.0/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)     1663 2023-07-23 11:35:37.000000 tortoise-api-0.2.0/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-23 16:25:20.258933 tortoise-api-0.2.0/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-23 16:25:20.000000 tortoise-api-0.2.0/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-23 16:25:20.000000 tortoise-api-0.2.0/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-23 16:25:20.000000 tortoise-api-0.2.0/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       59 2023-07-23 16:25:20.000000 tortoise-api-0.2.0/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-23 16:25:20.000000 tortoise-api-0.2.0/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.174822 tortoise-api-0.2.1/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.2.1/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-27 10:59:42.174587 tortoise-api-0.2.1/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.2.1/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      686 2023-07-27 10:59:05.000000 tortoise-api-0.2.1/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-27 10:59:42.174881 tortoise-api-0.2.1/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.173206 tortoise-api-0.2.1/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.2.1/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     3186 2023-07-27 10:21:50.000000 tortoise-api-0.2.1/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)     1979 2023-07-27 10:21:50.000000 tortoise-api-0.2.1/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-27 10:59:42.174286 tortoise-api-0.2.1/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2410 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       66 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-27 10:59:42.000000 tortoise-api-0.2.1/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.2.0/LICENSE` & `tortoise-api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.0/PKG-INFO` & `tortoise-api-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.2.0/README.md` & `tortoise-api-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.2.0/pyproject.toml` & `tortoise-api-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
     "asyncpg",
     "python-dotenv",
     "starlette",
-    "tortoise-api-model",
+    "tortoise-api-model>=0.0.4",
     "uvicorn"
 ]
-version = "0.2.0"
+version = "0.2.1"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.2.0/tortoise_api/api.py` & `tortoise-api-0.2.1/tortoise_api/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 from os import getenv as env
 from dotenv import load_dotenv
 from starlette.applications import Starlette
 from starlette.requests import Request
-from starlette.responses import JSONResponse, Response
+from starlette.responses import JSONResponse, Response, RedirectResponse
 from starlette.routing import Route
 from starlette.templating import Jinja2Templates
 from tortoise.contrib.starlette import register_tortoise
 from tortoise_api_model import Model
 
-from tortoise_api.util import jsonify, upsert, update, delete
+from tortoise_api.util import jsonify, update, delete, parse_qs
 
 
 class Api:
     app: Starlette
     models: {str: Model}
 
     def __init__(
@@ -47,16 +47,17 @@
     # ROUTES
     async def api_menu(self, _: Request):
         return JSONResponse(list(self.models))
 
     async def all_create(self, request: Request):
         model: type[Model] = self._get_model(request)
         if request.method == 'POST':
-            res = await upsert(model, await request.json())
-            return JSONResponse(jsonify(res[0]), status_code={True: 201, False: 202}[res[1]]) # create
+            data = parse_qs(await request.body())
+            await model.create(**data)
+            return RedirectResponse('/'+model.__name__, 303) # create # {True: 201, False: 202}[res[1]]
         objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
         data = [jsonify(obj) for obj in objects]
         return JSONResponse({'data': data}) # show all
 
     async def one_update(self, request: Request):
         model: type[Model] = self._get_model(request)
         oid = request.path_params['oid']
```

### Comparing `tortoise-api-0.2.0/tortoise_api/util.py` & `tortoise-api-0.2.1/tortoise_api/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from datetime import date
+from urllib.parse import parse_qsl, unquote
+
 from tortoise.fields import Field
 from tortoise.fields.relational import RelationalField, ReverseRelation
-from tortoise.models import MetaInfo
 from tortoise_api_model import Model
 
+
 def jsonify(obj: Model) -> dict:
     def check(field: Field, key: str):
         def rel_pack(mod: Model) -> dict:
             return {'id': mod.id, 'type': mod.__class__.__name__, 'repr': mod.repr()}
 
         prop = getattr(obj, key)
         if isinstance(prop, date):
@@ -21,22 +23,34 @@
                 return ''
             return None
         else:
             return getattr(obj, key)
 
     return {key: check(field, key) for key, field in obj._meta.fields_map.items() if not key.endswith('_id')}
 
-async def upsert(model: type[Model], dct: dict):
-    meta: MetaInfo = model._meta
-    # if pk := meta.pk_attr in dct.keys():
-    #     unq = {pk: dct.pop(pk)}
-    # else:
-    unq = {key: dct.pop(key) for key, ft in meta.fields_map.items() if ft.unique and key in dct.keys()}
-    # unq = meta.unique_together
-    res = await model.update_or_create(dct, **unq)
-    return res
+def parse_qs(s: str) -> dict:
+    data = {}
+    for k, v in parse_qsl(unquote(s)):
+        if k in data:
+            if isinstance(data[k], tuple):
+                data[k] += (v,)
+            else:
+                data[k] = data[k], v
+        else:
+            data[k] = v
+    return data
+
+# async def upsert(model: type[Model], dct: dict):
+#     meta: MetaInfo = model._meta
+#     if pk := meta.pk_attr in dct.keys():
+#         unq = {pk: dct.pop(pk)}
+#     else:
+#         unq = {key: dct.pop(key) for key, ft in meta.fields_map.items() if ft.unique and key in dct.keys()}
+#     # unq = meta.unique_together
+#     res = await model.update_or_create(dct, **unq)
+#     return res
 
 async def update(model: type[Model], dct: dict, oid):
     return await model.update_or_create(dct, **{model._meta.pk_attr: oid})
 
 async def delete(model: type[Model], oid):
-    return await (await model[oid]).delete()
+    return await (await model[oid]).delete()
```

### Comparing `tortoise-api-0.2.0/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.2.1/tortoise_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,generator,db-model,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

