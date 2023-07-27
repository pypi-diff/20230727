# Comparing `tmp/mypyllant-0.4.0.tar.gz` & `tmp/mypyllant-0.4.1.tar.gz`

## Comparing `mypyllant-0.4.0.tar` & `mypyllant-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.0/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.0/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.0/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/api.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/export.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.4.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.0/LICENSE
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 mypyllant-0.4.0/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 mypyllant-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.1/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.1/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.1/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19167 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2782 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8659 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7808 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 mypyllant-0.4.1/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7088 2020-02-02 00:00:00.000000 mypyllant-0.4.1/PKG-INFO
```

### Comparing `mypyllant-0.4.0/.pre-commit-config.yaml` & `mypyllant-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/logo.png` & `mypyllant-0.4.1/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/.github/workflows/build-test.yaml` & `mypyllant-0.4.1/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/api.py` & `mypyllant-0.4.1/src/myPyllant/api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/const.py` & `mypyllant-0.4.1/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/export.py` & `mypyllant-0.4.1/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/models.py` & `mypyllant-0.4.1/src/myPyllant/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     system_id: str
     index: int
     current_dhw_temperature: float | None
     current_special_function: DHWCurrentSpecialFunction
     max_setpoint: float
     min_setpoint: float
     operation_mode_dhw: DHWOperationMode
-    tapping_setpoint: float
+    tapping_setpoint: float | None
     time_program_dhw: dict
     time_program_circulation_pump: dict
 
 
 class System(BaseModel):
     id: str
     claim: Claim | None
```

### Comparing `mypyllant-0.4.0/src/myPyllant/sample.py` & `mypyllant-0.4.1/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/utils.py` & `mypyllant-0.4.1/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.1/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.1/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.1/src/myPyllant/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.1/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.1/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.1/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/update_sample.py` & `mypyllant-0.4.1/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/utils.py` & `mypyllant-0.4.1/src/myPyllant/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json` & `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.1/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/.gitignore` & `mypyllant-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/LICENSE` & `mypyllant-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/README.md` & `mypyllant-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/pyproject.toml` & `mypyllant-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.0/PKG-INFO` & `mypyllant-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

