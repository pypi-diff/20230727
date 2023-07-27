# Comparing `tmp/ez_cqrs-1.4.1.tar.gz` & `tmp/ez_cqrs-1.4.3.tar.gz`

## Comparing `ez_cqrs-1.4.1.tar` & `ez_cqrs-1.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/components.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/utilities/__init__.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/ez_cqrs/utilities/cli.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/requirements/core.txt
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/README.md
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/py.typed
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/requirements/core.txt
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/README.md
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ez_cqrs-1.4.3/PKG-INFO
```

### Comparing `ez_cqrs-1.4.1/.github/workflows/release.yml` & `ez_cqrs-1.4.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/.github/workflows/test.yml` & `ez_cqrs-1.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/.vscode/settings.json` & `ez_cqrs-1.4.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/acid_exec.py` & `ez_cqrs-1.4.3/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/components.py` & `ez_cqrs-1.4.3/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/error.py` & `ez_cqrs-1.4.3/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/framework.py` & `ez_cqrs-1.4.3/ez_cqrs/framework.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,22 +60,26 @@
         )
         if not isinstance(execution_result_or_err, Ok):
             return execution_result_or_err
 
         if app_database and max_transactions > 0:
             if ops_registry.is_empty():
                 msg = "No transactions to commit"
-                raise RuntimeError
+                raise RuntimeError(msg)
 
             commited_or_err = app_database.commit_as_transaction(
                 ops_registry=ops_registry,
             )
             if not isinstance(commited_or_err, Ok):
                 return commited_or_err
 
+            if not ops_registry.is_empty():
+                msg = "Ops registry didn't came empty after transactions commit."
+                raise RuntimeError(msg)
+
         event_dispatch_tasks = (
             self.event_dispatcher.dispatch(x) for x in event_registry
         )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
         return Ok(execution_result_or_err.unwrap())
```

### Comparing `ez_cqrs-1.4.1/ez_cqrs/handler.py` & `ez_cqrs-1.4.3/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/testing.py` & `ez_cqrs-1.4.3/ez_cqrs/testing.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/ez_cqrs/utilities/cli.py` & `ez_cqrs-1.4.3/ez_cqrs/utilities/cli.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/requirements/dev.txt` & `ez_cqrs-1.4.3/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/scripts/new_release.py` & `ez_cqrs-1.4.3/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/tests/integration/conftest.py` & `ez_cqrs-1.4.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/tests/integration/test_execution.py` & `ez_cqrs-1.4.3/tests/integration/test_execution.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/tests/unit/test_acid_exec.py` & `ez_cqrs-1.4.3/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/.gitignore` & `ez_cqrs-1.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/LICENSE` & `ez_cqrs-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.4.1/pyproject.toml` & `ez_cqrs-1.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,36 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.4.1"
+version = "1.4.3"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
-    { name = "Tomas Perez Alvarez", email = "tomasperezalvarez@gmail.com"}
-]
-dependencies = [
-    "mashumaro[orjson]",
-    "result",
-    "pydantic"
+    { name = "Tomas Perez Alvarez", email = "tomasperezalvarez@gmail.com" },
 ]
+dependencies = ["mashumaro[orjson]", "result", "pydantic"]
 
 [project.optional-dependencies]
-dev = [
-    "pyrgo>=0.3.0",
-    "pytest-cov",
-    "pytest-asyncio",
-    "tomli"
-]
+dev = ["pyrgo>=0.3.0", "pytest-cov", "pytest-asyncio", "tomli"]
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/ez-cqrs#readme"
 Issues = "https://github.com/Tomperez98/ez-cqrs/issues"
 Source = "https://github.com/Tomperez98/ez-cqrs"
 
 [tool.ruff]
 line-length = 88
-ignore = [
-    "ANN101",
-    "D203",
-    "D212",
-]
+ignore = ["ANN101", "D203", "D212"]
 select = ["ALL"]
 fix = false
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
@@ -93,28 +80,25 @@
     "--import-mode=importlib",
     "--strict-markers",
     "--cov-config=pyproject.toml",
     "--cov-fail-under=0",
     "--cov=ez_cqrs",
     "--cov-report=term-missing:skip-covered",
 ]
-markers = [
-    "integration: mark integration tests.",
-    "unit: mark unittest.",
-]
+markers = ["integration: mark integration tests.", "unit: mark unittest."]
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 precision = 1
 exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-  "@overload",
-  "raise NotImplementedError"
+    "no cov",
+    "if __name__ == .__main__.:",
+    "if TYPE_CHECKING:",
+    "@overload",
+    "raise NotImplementedError",
 ]
 
 
 [tool.mypy]
 show_error_codes = true
 follow_imports = "normal"
 strict_optional = true
```

### Comparing `ez_cqrs-1.4.1/PKG-INFO` & `ez_cqrs-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.4.1
+Version: 1.4.3
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

