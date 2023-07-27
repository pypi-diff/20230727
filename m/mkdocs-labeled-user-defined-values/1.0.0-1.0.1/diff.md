# Comparing `tmp/mkdocs_labeled_user_defined_values-1.0.0.tar.gz` & `tmp/mkdocs_labeled_user_defined_values-1.0.1.tar.gz`

## Comparing `mkdocs_labeled_user_defined_values-1.0.0.tar` & `mkdocs_labeled_user_defined_values-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/src/mkdocs_labeled_user_defined_values/__init__.py
--rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/src/mkdocs_labeled_user_defined_values/plugin.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/LICENSE
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/README.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/src/mkdocs_labeled_user_defined_values/__init__.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/src/mkdocs_labeled_user_defined_values/plugin.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 mkdocs_labeled_user_defined_values-1.0.1/PKG-INFO
```

### Comparing `mkdocs_labeled_user_defined_values-1.0.0/src/mkdocs_labeled_user_defined_values/plugin.py` & `mkdocs_labeled_user_defined_values-1.0.1/src/mkdocs_labeled_user_defined_values/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from mkdocs import utils as mkdocs_utils
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 
 
-class UserDefinedValues(BasePlugin):
+class LabeledUserDefinedValues(BasePlugin):
 
     config_scheme = (
         ('keywords', config_options.Type(dict)),
         ('input-placeholder', config_options.Type(str, default='{{{user-defined-values}}}'))
     )
 
     def on_config(self, config, **kwards):
```

### Comparing `mkdocs_labeled_user_defined_values-1.0.0/LICENSE` & `mkdocs_labeled_user_defined_values-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_labeled_user_defined_values-1.0.0/README.md` & `mkdocs_labeled_user_defined_values-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_labeled_user_defined_values-1.0.0/pyproject.toml` & `mkdocs_labeled_user_defined_values-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "mkdocs-labeled-user-defined-values"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Alban MAZEROLLES", email="amazerol_dev@yahoo.com" },
 ]
 description = "An enhanced version of mkdocs-user-defined-values. Keywords can now be categorized."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mkdocs_labeled_user_defined_values-1.0.0/PKG-INFO` & `mkdocs_labeled_user_defined_values-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-labeled-user-defined-values
-Version: 1.0.0
+Version: 1.0.1
 Summary: An enhanced version of mkdocs-user-defined-values. Keywords can now be categorized.
 Project-URL: Homepage, https://github.com/amazerol/mkdocs-labeled-user-defined-values
 Project-URL: Bug Tracker, https://github.com/amazerol/mkdocs-labeled-user-defined-values/issues
 Author-email: Alban MAZEROLLES <amazerol_dev@yahoo.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

