# Comparing `tmp/octoai_sdk-0.2.0.tar.gz` & `tmp/octoai_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai_sdk-0.2.0.tar", max compression
+gzip compressed data, was "octoai_sdk-0.2.1.tar", max compression
```

## Comparing `octoai_sdk-0.2.0.tar` & `octoai_sdk-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     3119 2023-07-18 16:44:57.986412 octoai_sdk-0.2.0/octoai/README.md
--rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.2.0/octoai/__init__.py
--rw-r--r--   0        0        0    13201 2023-07-26 19:32:26.932359 octoai_sdk-0.2.0/octoai/client.py
--rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.2.0/octoai/errors.py
--rw-r--r--   0        0        0       56 2023-07-11 00:00:05.180672 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/requirements.txt
--rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/service.py
--rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/test_request.py
--rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/requirements.txt
--rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/service.py
--rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/test_request.py
--rw-r--r--   0        0        0       34 2023-07-11 00:00:05.181513 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/requirements.txt
--rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/service.py
--rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/test_request.py
--rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/requirements.txt
--rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/service.py
--rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/test_request.py
--rw-r--r--   0        0        0     6788 2023-06-28 18:01:35.201394 octoai_sdk-0.2.0/octoai/server.py
--rw-r--r--   0        0        0     2698 2023-07-10 18:36:55.809355 octoai_sdk-0.2.0/octoai/service.py
--rw-r--r--   0        0        0    13192 2023-06-29 17:19:44.000199 octoai_sdk-0.2.0/octoai/types.py
--rw-r--r--   0        0        0     4000 2023-07-18 16:44:55.338153 octoai_sdk-0.2.0/octoai/utils.py
--rw-r--r--   0        0        0     1050 2023-07-26 19:33:12.234661 octoai_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3119 2023-07-18 16:44:57.986412 octoai_sdk-0.2.1/octoai/README.md
+-rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.2.1/octoai/__init__.py
+-rw-r--r--   0        0        0    13201 2023-07-26 19:32:26.932359 octoai_sdk-0.2.1/octoai/client.py
+-rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.2.1/octoai/errors.py
+-rw-r--r--   0        0        0       56 2023-07-11 00:00:05.180672 octoai_sdk-0.2.1/octoai/scaffolds/flan-t5/requirements.txt
+-rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.2.1/octoai/scaffolds/flan-t5/service.py
+-rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.2.1/octoai/scaffolds/flan-t5/test_request.py
+-rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.2.1/octoai/scaffolds/hello-world/requirements.txt
+-rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.2.1/octoai/scaffolds/hello-world/service.py
+-rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.2.1/octoai/scaffolds/hello-world/test_request.py
+-rw-r--r--   0        0        0       34 2023-07-11 00:00:05.181513 octoai_sdk-0.2.1/octoai/scaffolds/wav2vec/requirements.txt
+-rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.2.1/octoai/scaffolds/wav2vec/service.py
+-rw-r--r--   0        0        0     1464 2023-07-27 17:45:01.657527 octoai_sdk-0.2.1/octoai/scaffolds/wav2vec/test_request.py
+-rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.2.1/octoai/scaffolds/yolov8/requirements.txt
+-rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.2.1/octoai/scaffolds/yolov8/service.py
+-rw-r--r--   0        0        0     1815 2023-07-27 17:45:01.658903 octoai_sdk-0.2.1/octoai/scaffolds/yolov8/test_request.py
+-rw-r--r--   0        0        0     6794 2023-07-27 17:45:01.661171 octoai_sdk-0.2.1/octoai/server.py
+-rw-r--r--   0        0        0     2698 2023-07-10 18:36:55.809355 octoai_sdk-0.2.1/octoai/service.py
+-rw-r--r--   0        0        0    13192 2023-06-29 17:19:44.000199 octoai_sdk-0.2.1/octoai/types.py
+-rw-r--r--   0        0        0     4000 2023-07-18 16:44:55.338153 octoai_sdk-0.2.1/octoai/utils.py
+-rw-r--r--   0        0        0     1050 2023-07-27 17:50:18.792793 octoai_sdk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 octoai_sdk-0.2.1/PKG-INFO
```

### Comparing `octoai_sdk-0.2.0/octoai/README.md` & `octoai_sdk-0.2.1/octoai/README.md`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/client.py` & `octoai_sdk-0.2.1/octoai/client.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/errors.py` & `octoai_sdk-0.2.1/octoai/errors.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/service.py` & `octoai_sdk-0.2.1/octoai/scaffolds/flan-t5/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/test_request.py` & `octoai_sdk-0.2.1/octoai/scaffolds/flan-t5/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/hello-world/test_request.py` & `octoai_sdk-0.2.1/octoai/scaffolds/hello-world/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/service.py` & `octoai_sdk-0.2.1/octoai/scaffolds/wav2vec/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/test_request.py` & `octoai_sdk-0.2.1/octoai/scaffolds/wav2vec/test_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from octoai.client import Client
 from octoai.types import Audio
 
 audio = Audio.from_url(
     "https://datasets-server.huggingface.co/assets/patrickvonplaten/"
     "librispeech_asr_dummy/--/clean/validation/0/audio/audio.wav"
 )
-inputs = {"audio": audio.dict()}
+inputs = {"audio": audio.model_dump()}
 
 
 def main(endpoint):
     """Run inference against the endpoint."""
     # create an OctoAI client
     client = Client()
```

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/yolov8/service.py` & `octoai_sdk-0.2.1/octoai/scaffolds/yolov8/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/scaffolds/yolov8/test_request.py` & `octoai_sdk-0.2.1/octoai/scaffolds/yolov8/test_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import argparse
 import json
 
 from octoai.client import Client
 from octoai.types import Image
 
 image = Image.from_url("http://ultralytics.com/images/bus.jpg", follow_redirects=True)
-inputs = {"image": image.dict()}
+inputs = {"image": image.model_dump()}
 
 
 def main(endpoint):
     """Run inference against the endpoint."""
     # create an OctoAI client
     client = Client()
```

### Comparing `octoai_sdk-0.2.0/octoai/server.py` & `octoai_sdk-0.2.1/octoai/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 headers=self.response_headers,
                 content=Output(
                     output=prediction,
                     analytics=ResponseAnalytics(
                         inference_time_ms=inference_time_ms,
                         performance_time_ms=performance_time_ms,
                     ),
-                ).dict(),
+                ).model_dump(),
             )
 
     def get_api_schema(self) -> Dict[str, Any]:
         """Return the Open API schema for the underlying service."""
         return self.app.openapi()
 
     def init(self):
```

### Comparing `octoai_sdk-0.2.0/octoai/service.py` & `octoai_sdk-0.2.1/octoai/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/types.py` & `octoai_sdk-0.2.1/octoai/types.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/octoai/utils.py` & `octoai_sdk-0.2.1/octoai/utils.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.2.0/pyproject.toml` & `octoai_sdk-0.2.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "octoai-sdk"
-version = "0.2.0"
+version = "0.2.1"
 description = "A runtime library for OctoAI."
 authors = ["OctoML"]
 packages = [
     { include = "octoai" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
-fastapi = "^0.95.2"
+fastapi = "^0.100.0"
 httpx = "^0.24.0"
 numpy = "^1.24.3"
 pillow = "^9.5.0"
-pydantic = "^1.10.8"
+pydantic = "^2.1.1"
 pyyaml = "^6.0"
 soundfile = "^0.12.1"
 types-pyyaml = "^6.0.12.10"
 uvicorn = "^0.22.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.0.0"
```

### Comparing `octoai_sdk-0.2.0/PKG-INFO` & `octoai_sdk-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: octoai-sdk
-Version: 0.2.0
+Version: 0.2.1
 Summary: A runtime library for OctoAI.
 Author: OctoML
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: soundfile (>=0.12.1,<0.13.0)
 Requires-Dist: types-pyyaml (>=6.0.12.10,<7.0.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
```

