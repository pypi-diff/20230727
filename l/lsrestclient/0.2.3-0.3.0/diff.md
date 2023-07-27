# Comparing `tmp/lsrestclient-0.2.3.tar.gz` & `tmp/lsrestclient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-0.2.3.tar", max compression
+gzip compressed data, was "lsrestclient-0.3.0.tar", max compression
```

## Comparing `lsrestclient-0.2.3.tar` & `lsrestclient-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.3/README.md
--rw-r--r--   0        0        0     3313 2023-07-26 07:12:24.295402 lsrestclient-0.2.3/lsrestclient/__init__.py
--rw-r--r--   0        0        0      706 2023-07-26 07:13:21.278761 lsrestclient-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 lsrestclient-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.3.0/README.md
+-rw-r--r--   0        0        0     3463 2023-07-27 13:55:03.321953 lsrestclient-0.3.0/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      212 2023-07-27 13:55:03.321953 lsrestclient-0.3.0/lsrestclient/exceptions.py
+-rw-r--r--   0        0        0      706 2023-07-27 13:55:33.098831 lsrestclient-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 lsrestclient-0.3.0/PKG-INFO
```

### Comparing `lsrestclient-0.2.3/README.md` & `lsrestclient-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-0.2.3/lsrestclient/__init__.py` & `lsrestclient-0.3.0/lsrestclient/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from typing import Optional, Dict, Any
 
 import lsjsonclasses
 import requests
 from requests import Session, Response
 from requests.structures import CaseInsensitiveDict
 
+from lsrestclient import exceptions
+
 find_parameters_regex = re.compile('{(.*?)}')
 
 
 @dataclass
 class LsRestClientResponse:
     status_code: int
     content: str
@@ -76,23 +78,23 @@
 
         # params
         if params is None:
             params = {}
         if body is not None:
             kwargs['data'] = lsjsonclasses.LSoftJSONEncoder.dumps(body).encode("utf8")
 
-        return LsRestClientResponse.from_requests_response(
-            requests.request(
-                method.upper(),
-                self.full_url(url, params),
-                *args,
-                params=params,
-                **kwargs
-            )
-        )
+        full_url = self.full_url(url, params)
+
+        try:
+            requests_response = requests.request(method.upper(), full_url, *args, params=params, **kwargs)
+            response = LsRestClientResponse.from_requests_response(requests_response)
+            return response
+
+        except requests.ConnectionError:
+            raise exceptions.ConnectionError(url=full_url)
 
     def get(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('GET', *args, **kwargs)
 
     def post(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('POST', *args, **kwargs)
```

### Comparing `lsrestclient-0.2.3/pyproject.toml` & `lsrestclient-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "0.2.3"
+version = "0.3.0"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
```

### Comparing `lsrestclient-0.2.3/PKG-INFO` & `lsrestclient-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 0.2.3
+Version: 0.3.0
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

