# Comparing `tmp/another_sd_client-1.4.0.tar.gz` & `tmp/another_sd_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.4.0.tar", max compression
+gzip compressed data, was "another_sd_client-1.5.0.tar", max compression
```

## Comparing `another_sd_client-1.4.0.tar` & `another_sd_client-1.5.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     6296 2023-07-13 09:41:00.108048 another_sd_client-1.4.0/README.md
--rw-r--r--   0        0        0      919 2023-07-13 09:41:01.342161 another_sd_client-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 09:41:00.148051 another_sd_client-1.4.0/sdclient/__init__.py
--rw-r--r--   0        0        0     5018 2023-07-13 09:41:00.109048 another_sd_client-1.4.0/sdclient/client.py
--rw-r--r--   0        0        0     1017 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/exceptions.py
--rw-r--r--   0        0        0     4937 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/requests.py
--rw-r--r--   0        0        0     2697 2023-07-13 09:41:00.110048 another_sd_client-1.4.0/sdclient/responses.py
--rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-07-27 12:17:40.989938 another_sd_client-1.5.0/README.md
+-rw-r--r--   0        0        0      950 2023-07-27 12:17:42.328061 another_sd_client-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-27 12:17:41.032942 another_sd_client-1.5.0/sdclient/__init__.py
+-rw-r--r--   0        0        0     5018 2023-07-27 12:17:40.990938 another_sd_client-1.5.0/sdclient/client.py
+-rw-r--r--   0        0        0     1017 2023-07-27 12:17:40.990938 another_sd_client-1.5.0/sdclient/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:17:41.032942 another_sd_client-1.5.0/sdclient/py.typed
+-rw-r--r--   0        0        0     4937 2023-07-27 12:17:40.990938 another_sd_client-1.5.0/sdclient/requests.py
+-rw-r--r--   0        0        0     2697 2023-07-27 12:17:40.990938 another_sd_client-1.5.0/sdclient/responses.py
+-rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.5.0/PKG-INFO
```

### Comparing `another_sd_client-1.4.0/README.md` & `another_sd_client-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.4.0/pyproject.toml` & `another_sd_client-1.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
-
 [tool.poetry]
 name = "another-sd-client"
-version = "1.4.0"
+version = "1.5.0"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
+include = ["sdclient/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.4"
 more-itertools = ">=8.14.0"
 click = "^8.1.3"
 httpx = ">=0.22.0"
```

### Comparing `another_sd_client-1.4.0/sdclient/client.py` & `another_sd_client-1.5.0/sdclient/client.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.4.0/sdclient/exceptions.py` & `another_sd_client-1.5.0/sdclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.4.0/sdclient/requests.py` & `another_sd_client-1.5.0/sdclient/requests.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.4.0/sdclient/responses.py` & `another_sd_client-1.5.0/sdclient/responses.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.4.0/PKG-INFO` & `another_sd_client-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.4.0
+Version: 1.5.0
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

