# Comparing `tmp/pydrawise-2023.7.0.tar.gz` & `tmp/pydrawise-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2023.7.0.tar", last modified: Thu Jul  6 20:18:43 2023, max compression
+gzip compressed data, was "pydrawise-2023.7.1.tar", last modified: Thu Jul 27 12:57:11 2023, max compression
```

## Comparing `pydrawise-2023.7.0.tar` & `pydrawise-2023.7.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.523273 pydrawise-2023.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/reference/schema.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/hydrawise.graphql
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:18:43.000000 pydrawise-2023.7.0/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:43.527273 pydrawise-2023.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 20:18:28.000000 pydrawise-2023.7.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.819867 pydrawise-2023.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.819867 pydrawise-2023.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/pydrawise/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:57:11.000000 pydrawise-2023.7.1/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:57:11.823868 pydrawise-2023.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18279 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 12:56:50.000000 pydrawise-2023.7.1/tests/test_schema.py
```

### Comparing `pydrawise-2023.7.0/.devcontainer.json` & `pydrawise-2023.7.1/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/.github/workflows/build-and-test.yml` & `pydrawise-2023.7.1/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/.github/workflows/publish-python.yml` & `pydrawise-2023.7.1/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/.gitignore` & `pydrawise-2023.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/.pre-commit-config.yaml` & `pydrawise-2023.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/LICENSE` & `pydrawise-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/PKG-INFO` & `pydrawise-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2023.7.0/README.md` & `pydrawise-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/docs/index.md` & `pydrawise-2023.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/hydrawise.graphql` & `pydrawise-2023.7.1/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/mkdocs.yml` & `pydrawise-2023.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise/auth.py` & `pydrawise-2023.7.1/pydrawise/auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise/client.py` & `pydrawise-2023.7.1/pydrawise/client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise/exceptions.py` & `pydrawise-2023.7.1/pydrawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise/legacy/__init__.py` & `pydrawise-2023.7.1/pydrawise/legacy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,17 +70,18 @@
     def sensors(self) -> list[dict]:
         return self.controller_status.get("sensors", [])
 
     @property
     def running(self) -> str | None:
         return self.controller_status.get("running")
 
-    def update_controller_info(self) -> None:
+    def update_controller_info(self) -> bool:
         self.controller_info = self._get_controller_info()
         self.controller_status = self._get_controller_status()
+        return True
 
     def _get(self, path: str, **kwargs) -> dict:
         url = f"{_BASE_URL}/{path}"
         params = {"api_key": self._api_key}
         params.update(kwargs)
         resp = requests.get(url, params=params, timeout=_TIMEOUT)
```

### Comparing `pydrawise-2023.7.0/pydrawise/schema.py` & `pydrawise-2023.7.1/pydrawise/schema.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise/schema_utils.py` & `pydrawise-2023.7.1/pydrawise/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pydrawise.egg-info/PKG-INFO` & `pydrawise-2023.7.1/pydrawise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2023.7.0/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2023.7.1/pydrawise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/pyproject.toml` & `pydrawise-2023.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/tests/test_auth.py` & `pydrawise-2023.7.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/tests/test_client.py` & `pydrawise-2023.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.7.0/tests/test_legacy.py` & `pydrawise-2023.7.1/tests/test_legacy.py`

 * *Files identical despite different names*

