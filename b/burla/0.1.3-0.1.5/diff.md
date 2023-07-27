# Comparing `tmp/burla-0.1.3.tar.gz` & `tmp/burla-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.1.3.tar", max compression
+gzip compressed data, was "burla-0.1.5.tar", max compression
```

## Comparing `burla-0.1.3.tar` & `burla-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      535 2023-07-26 21:20:40.795038 burla-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/config.py
--rw-r--r--   0        0        0     5560 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      535 2023-07-27 00:30:39.176725 burla-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/__init__.py
+-rw-r--r--   0        0        0      907 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_config.py
+-rw-r--r--   0        0        0     1352 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_logstream.py
+-rw-r--r--   0        0        0     5353 2023-07-27 00:30:39.176725 burla-0.1.5/src/burla/_remote_parallel_map.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.5/PKG-INFO
```

### Comparing `burla-0.1.3/pyproject.toml` & `burla-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burla"
-version = "0.1.3"
+version = "0.1.5"
 description = "Scale your program across 1000s of computers with one line of code."
 authors = ["Jake Zuliani <jake@burla.dev>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dill = "^0.3.6"
```

### Comparing `burla-0.1.3/src/burla/_logstream.py` & `burla-0.1.5/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.3/src/burla/config.py` & `burla-0.1.5/src/burla/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,13 +18,13 @@
 
 
 def load_api_key_from_local_config() -> Tuple[str, str]:
     if not CONFIG_PATH.exists():
         raise Exception(
             (
                 "No API key found.\n"
-                "To set an API key run: `burla set_api_key=<your API key>`\n"
+                "To set an API key run: `burla set_api_key <your API key>`\n"
                 "To request an API key email jake@burla.dev."
             )
         )
     config = json.loads(CONFIG_PATH.read_text())
     return config["API_KEY"]
```

### Comparing `burla-0.1.3/src/burla/remote_parallel_map.py` & `burla-0.1.5/src/burla/_remote_parallel_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,25 +9,20 @@
 from time import sleep, time
 from queue import PriorityQueue
 
 import dill
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
-from burla.config import load_api_key_from_local_config
+from burla._config import load_api_key_from_local_config
 
 pickling_support.install()
 
-# BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"  # prod
-# JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
-
-BURLA_SERVICE_URL = "https://burla-webservice-y66ufvpuua-uc.a.run.app"  # test
-JOB_ENV_REPO = "us-docker.pkg.dev/burla-test/burla-job-environments"
-
-# BURLA_SERVICE_URL = "http://127.0.0.1:5000"
+BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"
+JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
 
 MAX_CONCURRENCY = 100  # If your snooping on my code and want to increase this, don't, it wont work.
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
```

### Comparing `burla-0.1.3/PKG-INFO` & `burla-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.1.3
+Version: 0.1.5
 Summary: Scale your program across 1000s of computers with one line of code.
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

