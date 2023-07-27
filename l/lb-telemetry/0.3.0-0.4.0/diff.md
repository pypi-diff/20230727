# Comparing `tmp/lb-telemetry-0.3.0.tar.gz` & `tmp/lb-telemetry-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-huk113xd/lb-telemetry-0.3.0.tar", last modified: Sun Jul 23 06:09:11 2023, max compression
+gzip compressed data, was "/builds/lhcb/lb-telemetry/dist/.tmp-kpa_0bwx/lb-telemetry-0.4.0.tar", last modified: Thu Jul 27 06:37:12 2023, max compression
```

## Comparing `lb-telemetry-0.3.0.tar` & `lb-telemetry-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     2191 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1967 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/.mypy.ini
--rw-r--r--   0 root         (0) root         (0)      594 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    18151 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)    35065 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2214 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1352 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry/
--rw-r--r--   0 root         (0) root         (0)     6386 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/src/lb_telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/src/lb_telemetry/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2214 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/src/lb_telemetry.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-23 06:09:11.000000 lb-telemetry-0.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6073 2023-07-23 06:09:03.000000 lb-telemetry-0.3.0/tests/test_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.mypy.ini
+-rw-r--r--   0 root         (0) root         (0)      594 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    18151 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)    35065 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry/
+-rw-r--r--   0 root         (0) root         (0)     7598 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/src/lb_telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/src/lb_telemetry/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/src/lb_telemetry.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 06:37:12.000000 lb-telemetry-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2023-07-27 06:37:03.000000 lb-telemetry-0.4.0/tests/test_logger.py
```

### Comparing `lb-telemetry-0.3.0/.gitignore` & `lb-telemetry-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.3.0/.gitlab-ci.yml` & `lb-telemetry-0.4.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.3.0/.pre-commit-config.yaml` & `lb-telemetry-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.3.0/.pylintrc` & `lb-telemetry-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.3.0/LICENSE` & `lb-telemetry-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lb-telemetry-0.3.0/PKG-INFO` & `lb-telemetry-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.3.0
+Version: 0.4.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -29,31 +29,44 @@
 pip install lb-telemetry
 ```
 
 ## Usage
 
 ### Adding to a package
 
-```py
+```python
+from lb_telemetry import Logger
+
 # Time execution (optional)
 start_time = time.perf_counter()
 do_some_task()
 exec_time = time.perf_counter() - start_time
 
 telemetry = {
     "exec_time": exec_time,
     "version": VERSION,
     "some_field": "field_value",
     "some_tag": "tag_value",
 }
 
-logger = Logger()
 Logger().log_to_monit(
     "NameOfThisPackage",  # Or other readable identifier
     telemetry,
-    tags=["version", "some_tag"],
+    tags=["version", "some_tag"],  # `exec_time` and `some_field` interpreted as fields
 )
 ```
 
+### Running the CLI
+
+The default value for `--table` is 'CLI'.
+```commandline
+lb-telemetry send '{"test_field": "test_value"}' --include-host-info
+```
+
+Tags can be specified by:
+```commandline
+lb-telemetry send '{"field1": 0, "tag1": 5, "tag2": 2}' --table some_table --tags tag1 tag2
+```
+
 ### Viewing the telemetry
 
 Logged telemetry is usually visible in under a minute and can be accessed via this [Grafana dashboard](https://monit-grafana.cern.ch/d/vQC-V7C4k/lb-telemetry?orgId=46&from=now-30d&to=now). Request permission to edit the dashboard from an LHCb Grafana org admin if necessary. Then create a new row on the dashboard for your package and add the desired graphs.
```

### Comparing `lb-telemetry-0.3.0/README.md` & `lb-telemetry-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,31 +15,44 @@
 pip install lb-telemetry
 ```
 
 ## Usage
 
 ### Adding to a package
 
-```py
+```python
+from lb_telemetry import Logger
+
 # Time execution (optional)
 start_time = time.perf_counter()
 do_some_task()
 exec_time = time.perf_counter() - start_time
 
 telemetry = {
     "exec_time": exec_time,
     "version": VERSION,
     "some_field": "field_value",
     "some_tag": "tag_value",
 }
 
-logger = Logger()
 Logger().log_to_monit(
     "NameOfThisPackage",  # Or other readable identifier
     telemetry,
-    tags=["version", "some_tag"],
+    tags=["version", "some_tag"],  # `exec_time` and `some_field` interpreted as fields
 )
 ```
 
+### Running the CLI
+
+The default value for `--table` is 'CLI'.
+```commandline
+lb-telemetry send '{"test_field": "test_value"}' --include-host-info
+```
+
+Tags can be specified by:
+```commandline
+lb-telemetry send '{"field1": 0, "tag1": 5, "tag2": 2}' --table some_table --tags tag1 tag2
+```
+
 ### Viewing the telemetry
 
 Logged telemetry is usually visible in under a minute and can be accessed via this [Grafana dashboard](https://monit-grafana.cern.ch/d/vQC-V7C4k/lb-telemetry?orgId=46&from=now-30d&to=now). Request permission to edit the dashboard from an LHCb Grafana org admin if necessary. Then create a new row on the dashboard for your package and add the desired graphs.
```

### Comparing `lb-telemetry-0.3.0/pyproject.toml` & `lb-telemetry-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -54,7 +54,10 @@
 ]
 
 [tool.ruff]
 select = ["E", "F", "B", "I", "PLE", "RUF", "UP"]
 target-version = "py39"
 [tool.ruff.isort]
 known-first-party = ["lb_telemetry"]
+
+[project.scripts]
+lb-telemetry = "lb_telemetry:lb_telemetry"
```

### Comparing `lb-telemetry-0.3.0/src/lb_telemetry/__init__.py` & `lb-telemetry-0.4.0/src/lb_telemetry/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-
+import argparse
 import json
+import os
 import platform
 import time
 from typing import Optional
 
 import requests
 from LbPlatformUtils import inspect
 from logzero import logger as logzero
@@ -61,19 +62,14 @@
                 return False
 
         # Every declared tag should also appear in the data dictionary
         for tag in tags:
             if tag not in data.keys():
                 logzero.warning(f"The tag {tag} does not appear in the data dictionary")
                 return False
-            elif not isinstance(data[tag], str):
-                logzero.warning(
-                    f"The tag {tag}: ({data[tag]}) has a value of type "
-                    f"{type(data[tag])} so will be converted to a string"
-                )
 
         return True
 
     @staticmethod
     def get_os_version() -> str:
         system = platform.system()
         if system == "Linux":
@@ -138,14 +134,16 @@
             tags: Which data entries are tags (the rest are assumed to be fields).
             include_host_info: Whether information about the caller's system should
                                be included in logging (Python version, OS, etc.)
 
         Returns:
             The timestamp of the created log entry.
         """
+        if "LBTELEMETRY_ENABLED" not in os.environ:
+            return None
         if not Logger.is_data_valid(data, tags):
             return None
 
         payload = self.build_payload(package, data, tags, include_host_info)
 
         # Send the data to MONIT
         try:
@@ -167,7 +165,51 @@
         if response.status_code != 200:
             logzero.warning(f"Unexpected status code: {response.status_code}")
             logzero.debug(f"Response: {response.text}")
             logzero.debug(f"Payload: {json.dumps(payload)}")
             return None
 
         return payload["timestamp"]
+
+
+def lb_telemetry():
+    parser = argparse.ArgumentParser(
+        usage="lb-telemetry [-h] send json_payload <table> "
+        "[--tags tag1 tag2] [--include-host-info]",
+        description="Manually send",
+    )
+    subparsers = parser.add_subparsers(dest="command")
+
+    send_parser = subparsers.add_parser("send", help="Send telemetry data")
+    send_parser.add_argument(
+        "payload", type=json.loads, help="Telemetry data to send in str JSON format"
+    )
+    send_parser.add_argument(
+        "-t", "--table", type=str, required=True, help="The destination table name"
+    )
+    send_parser.add_argument(
+        "--tags",
+        nargs="*",
+        default=[],
+        help="Which payload data are tags (the rest are fields)",
+    )
+    send_parser.add_argument(
+        "--include-host-info",
+        type=bool,
+        default=False,
+        action=argparse.BooleanOptionalAction,
+        help="Include for info about your system to be sent",
+    )
+
+    args = parser.parse_args()
+    if args.command == "send":
+        payload: dict = args.payload
+        table: str = args.table
+        tags: list[str] = args.tags
+        include_host_info: bool = args.include_host_info
+
+        Logger().log_to_monit(
+            package=table,
+            data=payload,
+            tags=tags,
+            include_host_info=include_host_info,
+        )
```

### Comparing `lb-telemetry-0.3.0/src/lb_telemetry.egg-info/PKG-INFO` & `lb-telemetry-0.4.0/src/lb_telemetry.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-telemetry
-Version: 0.3.0
+Version: 0.4.0
 Summary: A utility for logging telemetry data from LHCb packages to MONIT
 Author-email: Cameron McClymont <cameron.duncan.mcclymont@cern.ch>, Daniel Cervenkov <daniel.cervenkov@cern.ch>, Chris Burr <christopher.burr@cern.ch>
 Project-URL: Homepage, https://gitlab.cern.ch/lhcb/lb-telemetry
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb/lb-telemetry/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -29,31 +29,44 @@
 pip install lb-telemetry
 ```
 
 ## Usage
 
 ### Adding to a package
 
-```py
+```python
+from lb_telemetry import Logger
+
 # Time execution (optional)
 start_time = time.perf_counter()
 do_some_task()
 exec_time = time.perf_counter() - start_time
 
 telemetry = {
     "exec_time": exec_time,
     "version": VERSION,
     "some_field": "field_value",
     "some_tag": "tag_value",
 }
 
-logger = Logger()
 Logger().log_to_monit(
     "NameOfThisPackage",  # Or other readable identifier
     telemetry,
-    tags=["version", "some_tag"],
+    tags=["version", "some_tag"],  # `exec_time` and `some_field` interpreted as fields
 )
 ```
 
+### Running the CLI
+
+The default value for `--table` is 'CLI'.
+```commandline
+lb-telemetry send '{"test_field": "test_value"}' --include-host-info
+```
+
+Tags can be specified by:
+```commandline
+lb-telemetry send '{"field1": 0, "tag1": 5, "tag2": 2}' --table some_table --tags tag1 tag2
+```
+
 ### Viewing the telemetry
 
 Logged telemetry is usually visible in under a minute and can be accessed via this [Grafana dashboard](https://monit-grafana.cern.ch/d/vQC-V7C4k/lb-telemetry?orgId=46&from=now-30d&to=now). Request permission to edit the dashboard from an LHCb Grafana org admin if necessary. Then create a new row on the dashboard for your package and add the desired graphs.
```

### Comparing `lb-telemetry-0.3.0/tests/test_logger.py` & `lb-telemetry-0.4.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "test_field1": "test_value",
     "test_field2": False,
     "test_field3": 0,
     "test_field4": 3.5,
     "test_tag1": "some_tag",
 }
 TEST_TAGS = ["test_tag1"]
+os.environ["LBTELEMETRY_ENABLED"] = "x"
 
 
 class LogFetchError(Exception):
     pass
 
 
 def test_build_payload_valid():
```

