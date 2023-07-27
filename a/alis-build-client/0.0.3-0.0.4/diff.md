# Comparing `tmp/alis_build_client-0.0.3.tar.gz` & `tmp/alis_build_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alis_build_client-0.0.3.tar", max compression
+gzip compressed data, was "alis_build_client-0.0.4.tar", max compression
```

## Comparing `alis_build_client-0.0.3.tar` & `alis_build_client-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      988 2023-07-20 09:59:34.978367 alis_build_client-0.0.3/README.md
--rw-r--r--   0        0        0       75 2023-07-14 08:48:39.896818 alis_build_client-0.0.3/alis/build/client/__init__.py
--rw-r--r--   0        0        0     2770 2023-07-16 16:35:27.451293 alis_build_client-0.0.3/alis/build/client/grpc.py
--rw-r--r--   0        0        0      809 2023-07-20 09:59:54.989952 alis_build_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 alis_build_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-27 13:10:16.687154 alis_build_client-0.0.4/README.md
+-rw-r--r--   0        0        0       75 2023-07-14 08:48:39.896818 alis_build_client-0.0.4/alis/build/client/__init__.py
+-rw-r--r--   0        0        0     3025 2023-07-27 12:59:03.151904 alis_build_client-0.0.4/alis/build/client/grpc.py
+-rw-r--r--   0        0        0      809 2023-07-27 13:05:18.746804 alis_build_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 alis_build_client-0.0.4/PKG-INFO
```

### Comparing `alis_build_client-0.0.3/README.md` & `alis_build_client-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 ## Usage
 Before you can use this project, you need to install [Poetry](https://python-poetry.org/docs/), a tool for dependency management and packaging in Python.
 On Unix-based systems (like Linux and MacOS), you can install Poetry using this command:
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 ```
 
-- To run tests, from `alis-build-client/alis/build`: ```python -m unittest discover test``` \
-- To install the package locally: ```poetry install``` \
-- To build the package: ```poetry build``` \
-- To publish the package: \
-    - Populate dist/ by building the package from source \
-    - Set up ~/.pypirc \
+- To run tests, from `python-client/alis/build`
+    - ```python -m unittest discover test```
+- To install the package locally: ```poetry install```
+- To build the package: ```poetry build```
+- To publish the package:
+    - Ensure the relevant version is set in `pyproject.toml`
+    - Populate dist/ by building the package from source
+    - Set up ~/.pypirc
     ```
     [pypi]
         username = __token__
         password = <API_KEY>
     ```
-    - Publish dist/ with twine \
-    ```pip install twine```
-    ```twine upload -r pypi dist/*```
+    - Publish dist/ with twine, from `python-client`
+        - ```pip install twine```
+        - ```twine upload -r pypi dist/*```
```

### Comparing `alis_build_client-0.0.3/alis/build/client/grpc.py` & `alis_build_client-0.0.4/alis/build/client/grpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import grpc
 import re
 import time
+import logging
 from google.auth.transport.grpc import AuthMetadataPlugin
 from google.auth.transport.requests import Request
 from google.auth.exceptions import DefaultCredentialsError
 from google.oauth2 import id_token
 
 class InvalidArgumentError(Exception):
-    print(f"Argument validation failed: {Exception}")
+    def __init__(self, message):
+        self.message = message
+
+    def __str__(self):
+        return f"Argument validation failed: {self.message}"
 
 def validate_argument(name: str, value: str, pattern: str) -> None:
     if not re.match(pattern, value):
         raise InvalidArgumentError(f"Invalid {name}. Expected format is {pattern}")
 
 def new_conn(host: str, insecure: bool) -> grpc.Channel:
     """
@@ -44,26 +49,31 @@
             self._token_expiry = id_token.verify_oauth2_token(token, request)['exp']
     
     validate_argument("host", host, r"^[a-zA-Z0-9.-]+:\d+$")
 
     if insecure:
         # Create an insecure Channel
         channel = grpc.insecure_channel(host)
+
+        logging.info(f"Established insecure channel to:{host}")
+
     else:
         # Make a secure Channel
         # The following URL will be used as the audience field in the JWT token authentication with the server.
         audience = f"https://{host.split(':')[0]}"
         try:
             # Create an AuthMetadataPlugin instance using the ID token credentials and the request
             auth = GrpcAuth(Request(), audience)
 
             # Create a set of grpc.CallCredentials using the AuthMetadataPlugin instance
             call_creds = grpc.metadata_call_credentials(auth)
 
             # Create a secure Channel using the call credentials
             channel = grpc.secure_channel(host, grpc.composite_channel_credentials(grpc.ssl_channel_credentials(), call_creds))
 
+            logging.info(f"Established secure channel to:{host}")
+
         except DefaultCredentialsError as e:
-            print(f"Failed to fetch identity token credentials: {e}")
+            logging.exception(f"Failed to fetch identity token credentials: {e}")
             return None
 
     return channel
```

### Comparing `alis_build_client-0.0.3/pyproject.toml` & `alis_build_client-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alis-build-client"
-version = "0.0.3"
+version = "0.0.4"
 description = "A grpc client package for python applications."
 authors = ["Thomas Scholtz <tom.scholtz@alisx.com>"]
 readme = "README.md"
 homepage = "https://github.com/yourusername/grpc_client"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `alis_build_client-0.0.3/PKG-INFO` & `alis_build_client-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alis-build-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: A grpc client package for python applications.
 Home-page: https://github.com/yourusername/grpc_client
 License: MIT
 Author: Thomas Scholtz
 Author-email: tom.scholtz@alisx.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,22 +26,24 @@
 ## Usage
 Before you can use this project, you need to install [Poetry](https://python-poetry.org/docs/), a tool for dependency management and packaging in Python.
 On Unix-based systems (like Linux and MacOS), you can install Poetry using this command:
 ```bash
 curl -sSL https://install.python-poetry.org | python3 -
 ```
 
-- To run tests, from `alis-build-client/alis/build`: ```python -m unittest discover test``` \
-- To install the package locally: ```poetry install``` \
-- To build the package: ```poetry build``` \
-- To publish the package: \
-    - Populate dist/ by building the package from source \
-    - Set up ~/.pypirc \
+- To run tests, from `python-client/alis/build`
+    - ```python -m unittest discover test```
+- To install the package locally: ```poetry install```
+- To build the package: ```poetry build```
+- To publish the package:
+    - Ensure the relevant version is set in `pyproject.toml`
+    - Populate dist/ by building the package from source
+    - Set up ~/.pypirc
     ```
     [pypi]
         username = __token__
         password = <API_KEY>
     ```
-    - Publish dist/ with twine \
-    ```pip install twine```
-    ```twine upload -r pypi dist/*```
+    - Publish dist/ with twine, from `python-client`
+        - ```pip install twine```
+        - ```twine upload -r pypi dist/*```
```

