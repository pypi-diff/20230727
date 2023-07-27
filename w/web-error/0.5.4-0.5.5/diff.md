# Comparing `tmp/web_error-0.5.4.tar.gz` & `tmp/web_error-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_error-0.5.4.tar", max compression
+gzip compressed data, was "web_error-0.5.5.tar", max compression
```

## Comparing `web_error-0.5.4.tar` & `web_error-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.4/LICENSE
--rw-r--r--   0        0        0     3068 2023-07-12 12:38:27.008882 web_error-0.5.4/README.md
--rw-r--r--   0        0        0     1772 2023-07-12 12:38:27.006882 web_error-0.5.4/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-12 12:38:27.009882 web_error-0.5.4/web_error/__init__.py
--rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.4/web_error/constant.py
--rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.4/web_error/error.py
--rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.4/web_error/handler/__init__.py
--rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.4/web_error/handler/aiohttp.py
--rw-r--r--   0        0        0     2758 2023-07-12 12:38:02.330747 web_error-0.5.4/web_error/handler/fastapi.py
--rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.4/web_error/handler/flask.py
--rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.4/web_error/handler/pyramid.py
--rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.4/web_error/handler/starlette.py
--rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    11307 2020-10-05 08:06:50.313394 web_error-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3068 2023-07-27 11:32:37.697399 web_error-0.5.5/README.md
+-rw-r--r--   0        0        0     1772 2023-07-27 11:32:37.697399 web_error-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-27 11:32:37.697399 web_error-0.5.5/web_error/__init__.py
+-rw-r--r--   0        0        0       76 2023-02-19 13:27:57.835626 web_error-0.5.5/web_error/constant.py
+-rw-r--r--   0        0        0     1700 2023-02-19 13:32:08.909713 web_error-0.5.5/web_error/error.py
+-rw-r--r--   0        0        0        0 2020-10-05 09:05:22.710518 web_error-0.5.5/web_error/handler/__init__.py
+-rw-r--r--   0        0        0     1268 2023-02-19 13:23:27.856394 web_error-0.5.5/web_error/handler/aiohttp.py
+-rw-r--r--   0        0        0     2857 2023-07-27 11:31:31.079041 web_error-0.5.5/web_error/handler/fastapi.py
+-rw-r--r--   0        0        0     1116 2023-02-19 13:20:25.477898 web_error-0.5.5/web_error/handler/flask.py
+-rw-r--r--   0        0        0     1528 2023-02-19 13:19:46.823583 web_error-0.5.5/web_error/handler/pyramid.py
+-rw-r--r--   0        0        0     3725 2023-02-19 13:25:07.941219 web_error-0.5.5/web_error/handler/starlette.py
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 web_error-0.5.5/PKG-INFO
```

### Comparing `web_error-0.5.4/LICENSE` & `web_error-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/README.md` & `web_error-0.5.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Web Errors v0.5.4
+# Web Errors v0.5.5
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
 ![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
```

### Comparing `web_error-0.5.4/pyproject.toml` & `web_error-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web_error"
-version = "0.5.4"
+version = "0.5.5"
 description = "Web based error utils"
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/EdgyEdgemond/web-error/"
 homepage="https://github.com/EdgyEdgemond/web-error/"
 readme = "README.md"
```

### Comparing `web_error-0.5.4/web_error/error.py` & `web_error-0.5.5/web_error/error.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/web_error/handler/aiohttp.py` & `web_error-0.5.5/web_error/handler/aiohttp.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/web_error/handler/fastapi.py` & `web_error-0.5.5/web_error/handler/fastapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     status = constant.SERVER_ERROR
     message = "Unhandled exception occurred."
     response = {
         "message": message,
         "debug_message": str(exc),
         "code": None,
     }
+    headers = {}
 
     if isinstance(exc, HTTPException):
         response["message"] = exc.detail
         status = exc.status_code
+        headers = exc.headers
 
     if isinstance(exc, RequestValidationError):
         response["message"] = "Request validation error."
         response["debug_message"] = json.loads(json.dumps(exc.errors(), default=str))
         status = 422
 
     if isinstance(exc, HttpException):
@@ -36,41 +38,42 @@
 
     if status >= constant.SERVER_ERROR:
         logger.exception(message, exc_info=(type(exc), exc, exc.__traceback__))
 
     if not debug_enabled:
         response.pop("debug_message", None)
 
-    return response, status
+    return response, status, headers
 
 
 class ExceptionHandler:
     def __init__(self, unhandled_code: str, request_validation_code: str, *, debug_enabled: bool = True) -> None:
         self.unhandled_code = unhandled_code
         self.request_validation_code = request_validation_code
         self.debug_enabled = debug_enabled
 
     def __call__(self, request: starlette.Request, exc: Exception) -> starlette.JSONResponse:  # noqa: ARG002
-        response, status = _handle_exception(exc, debug_enabled=self.debug_enabled)
+        response, status, headers = _handle_exception(exc, debug_enabled=self.debug_enabled)
 
         if response["code"] is None:
             response["code"] = self.request_validation_code if status == 422 else self.unhandled_code  # noqa: PLR2004
 
         return starlette.JSONResponse(
             status_code=status,
             content=response,
         )
 
 
 def exception_handler(request: starlette.Request, exc: Exception) -> starlette.JSONResponse:  # noqa: ARG001
-    response, status = _handle_exception(exc)
+    response, status, headers = _handle_exception(exc)
 
     return starlette.JSONResponse(
         status_code=status,
         content=response,
+        headers=headers,
     )
 
 
 def generate_handler_with_cors(
     allow_origins: Optional[List[str]] = None,
     allow_credentials: bool = True,
     allow_methods: Optional[List[str]] = None,
```

### Comparing `web_error-0.5.4/web_error/handler/flask.py` & `web_error-0.5.5/web_error/handler/flask.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/web_error/handler/pyramid.py` & `web_error-0.5.5/web_error/handler/pyramid.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/web_error/handler/starlette.py` & `web_error-0.5.5/web_error/handler/starlette.py`

 * *Files identical despite different names*

### Comparing `web_error-0.5.4/PKG-INFO` & `web_error-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-error
-Version: 0.5.4
+Version: 0.5.5
 Summary: Web based error utils
 Home-page: https://github.com/EdgyEdgemond/web-error/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/EdgyEdgemond/web-error/
 Description-Content-Type: text/markdown
 
-# Web Errors v0.5.4
+# Web Errors v0.5.5
 [![image](https://img.shields.io/pypi/v/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/l/web_error.svg)](https://pypi.org/project/web_error/)
 [![image](https://img.shields.io/pypi/pyversions/web_error.svg)](https://pypi.org/project/web_error/)
 ![style](https://github.com/EdgyEdgemond/web-error/workflows/style/badge.svg)
 ![tests](https://github.com/EdgyEdgemond/web-error/workflows/tests/badge.svg)
 [![codecov](https://codecov.io/gh/EdgyEdgemond/web-error/branch/master/graph/badge.svg)](https://codecov.io/gh/EdgyEdgemond/web-error)
```

