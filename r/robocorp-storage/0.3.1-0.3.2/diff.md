# Comparing `tmp/robocorp_storage-0.3.1.tar.gz` & `tmp/robocorp_storage-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-0.3.1.tar", max compression
+gzip compressed data, was "robocorp_storage-0.3.2.tar", max compression
```

## Comparing `robocorp_storage-0.3.1.tar` & `robocorp_storage-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      385 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/README.md
--rw-r--r--   0        0        0      801 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7286 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6044 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_client.py
--rw-r--r--   0        0        0     2354 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_environment.py
--rw-r--r--   0        0        0     6343 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     1904 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_types.py
--rw-r--r--   0        0        0      170 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/_utils.py
--rw-r--r--   0        0        0        0 2023-07-18 10:56:47.998823 robocorp_storage-0.3.1/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 robocorp_storage-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      915 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/docs/README.md
+-rw-r--r--   0        0        0      803 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7286 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6063 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/_client.py
+-rw-r--r--   0        0        0     2354 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/_environment.py
+-rw-r--r--   0        0        0     6343 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     1904 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/_types.py
+-rw-r--r--   0        0        0      170 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-27 17:13:49.875287 robocorp_storage-0.3.2/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 robocorp_storage-0.3.2/PKG-INFO
```

### Comparing `robocorp_storage-0.3.1/pyproject.toml` & `robocorp_storage-0.3.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-storage"
-version = "0.3.1"
+version = "0.3.2"
 description = "Robocorp Asset Storage library"
 authors = [
 	"Cosmin P. <cosmin@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
@@ -15,15 +15,15 @@
 skip-string-normalization = false
 skip-magic-trailing-comma = false
 
 [tool.isort]
 profile = "black"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 requests = "^2.28.2"
 tenacity = "^8.0.1"
 typing-extensions = { version = "^4.6.3", python = "<3.8" }
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = { path = "../devutils/", develop = true }
 types-requests = "^2.30.0.0"
```

### Comparing `robocorp_storage-0.3.1/src/robocorp/storage/__init__.py` & `robocorp_storage-0.3.2/src/robocorp/storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ._client import AssetNotFound, AssetUploadFailed
 
 if TYPE_CHECKING:
     from ._client import AssetsClient
     from ._requests import Response
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 version_info = [int(x) for x in __version__.split(".")]
 
 JSON = Union[dict[str, "JSON"], list["JSON"], str, int, float, bool, None]
 
 LOGGER = logging.getLogger(__name__)
 
 # Known (additional) mimetypes from file extensions
```

### Comparing `robocorp_storage-0.3.1/src/robocorp/storage/_client.py` & `robocorp_storage-0.3.2/src/robocorp/storage/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import logging
 import math
 import time
 from typing import Optional, cast
-from urllib.parse import quote_plus
+from urllib.parse import quote as sanitize_id
 
 from ._requests import HTTPError, Requests, Response
 from ._types import (
     Asset,
     AssetDetails,
     AssetUploadResponse,
     AssetUploadState,
@@ -76,36 +76,36 @@
         """Create a new asset."""
         payload = {"name": name}
         response = self._client.post("", json=payload)
         return cast(AssetDetails, response.json())
 
     def get_asset(self, asset_id: str) -> AssetDetails:
         """Returns the details of a single asset, including its payload."""
-        path = quote_plus(asset_id)
+        path = sanitize_id(asset_id)
         handler = self._handle_asset_not_found(asset_id)
         response = self._client.get(path, _handle_error=handler)
         return cast(AssetDetails, response.json())
 
     def delete_asset(self, asset_id: str):
         """Delete the given asset."""
-        path = quote_plus(asset_id)
+        path = sanitize_id(asset_id)
         handler = self._handle_asset_not_found(asset_id)
         self._client.delete(path, _handle_error=handler)
 
     def upload_asset(
         self,
         asset_id: str,
         content: bytes,
         content_type: Optional[ContentType] = None,
         wait: bool = True,
         poll_interval: float = 0.5,
     ):
         """Upload an asset payload, and optionally wait for it to finish."""
         if _estimate_base64_size(len(content)) < DATA_LIMIT:
-            LOGGER.info("Content size under data limit, uploading directly")
+            LOGGER.debug("Content size under data limit, uploading directly")
             data_content = base64.b64encode(content).decode("ascii")
             response = self._create_upload(
                 asset_id,
                 content_type=content_type,
                 data=data_content,
             )
         else:
@@ -119,15 +119,15 @@
 
         # if response["status"] == "completed":
         #    return
 
         if not wait:
             return
 
-        LOGGER.info("Waiting for asset upload to complete")
+        LOGGER.info("Waiting for the asset upload to complete")
         while True:
             state = self._get_upload(asset_id, response["id"])
             status = state["status"]
 
             if status == "pending":
                 time.sleep(poll_interval)
                 continue
@@ -153,17 +153,17 @@
         """
         payload = {}
         if content_type is not None:
             payload["content_type"] = content_type
         if data is not None:
             payload["data"] = data
 
-        path = url_join(quote_plus(asset_id), "upload")
+        path = url_join(sanitize_id(asset_id), "upload")
         handler = self._handle_asset_not_found(asset_id)
         response = self._client.post(path, json=payload, _handle_error=handler)
         return cast(AssetUploadResponse, response.json())
 
     def _get_upload(self, asset_id: str, upload_id: str) -> AssetUploadState:
         """Return the details of a single asset upload."""
-        path = url_join(quote_plus(asset_id), "uploads", upload_id)
+        path = url_join(sanitize_id(asset_id), "uploads", upload_id)
         response = self._client.get(path)
         return cast(AssetUploadState, response.json())
```

### Comparing `robocorp_storage-0.3.1/src/robocorp/storage/_environment.py` & `robocorp_storage-0.3.2/src/robocorp/storage/_environment.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.1/src/robocorp/storage/_requests.py` & `robocorp_storage-0.3.2/src/robocorp/storage/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.1/src/robocorp/storage/_types.py` & `robocorp_storage-0.3.2/src/robocorp/storage/_types.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.3.1/PKG-INFO` & `robocorp_storage-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 0.3.1
+Version: 0.3.2
 Summary: Robocorp Asset Storage library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/robocorp/robo/
 Description-Content-Type: text/markdown
 
-# Robocorp Control Room Asset Storage API library
+# robocorp-storage
 
 `robocorp-storage` is a library which provides read and write access to the
-*Asset Storage* in Robocorp **Control Room**.
+*Asset Storage* in Robocorp Control Room.
 
-## Usage
+## Getting started
 
 ```python
 from robocorp import storage
 
 def store_email():
     storage.set_text("cosmin", "cosmin@robocorp.com")
     print("E-mail:", storage.get_text("cosmin"))
     storage.delete_asset("cosmin")
 ```
 
+## Guides
+
+- [Handling different asset types](https://github.com/robocorp/robo/blob/master/storage/docs/guides/asset-types.md)
+
+Further user guides and tutorials can be found in [Robocorp Docs](https://robocorp.com/docs).
+
+## API Reference
+
+Information on specific functions or classes: [robocorp.storage](https://github.com/robocorp/robo/blob/master/storage/docs/api/robocorp.storage.md)
+
+## Changelog
+
+A list of releases and corresponding changes can be found in the [changelog](https://github.com/robocorp/robo/blob/master/storage/docs/CHANGELOG.md).
+
```

