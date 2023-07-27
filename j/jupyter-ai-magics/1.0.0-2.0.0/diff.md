# Comparing `tmp/jupyter_ai_magics-1.0.0.tar.gz` & `tmp/jupyter_ai_magics-2.0.0.tar.gz`

## Comparing `jupyter_ai_magics-1.0.0.tar` & `jupyter_ai_magics-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/setup.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/_version.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/aliases.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/embedding_providers.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/exception.py
--rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/magics.py
--rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/parsers.py
--rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/providers.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/jupyter_ai_magics/tests/__init__.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/LICENSE
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/README.md
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 jupyter_ai_magics-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/setup.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/_version.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/aliases.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/embedding_providers.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/exception.py
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/magics.py
+-rw-r--r--   0        0        0     6098 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/parsers.py
+-rw-r--r--   0        0        0    14514 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/providers.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/jupyter_ai_magics/tests/__init__.py
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/LICENSE
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/README.md
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 jupyter_ai_magics-2.0.0/PKG-INFO
```

### Comparing `jupyter_ai_magics-1.0.0/package.json` & `jupyter_ai_magics-2.0.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'2.0.0'"}*

```diff
@@ -16,9 +16,9 @@
         "type": "git",
         "url": "https://github.com/jupyterlab/jupyter-ai.git"
     },
     "scripts": {
         "dev-install": "pip install -e \".[dev,all]\"",
         "dev-uninstall": "pip uninstall jupyter_ai_magics -y"
     },
-    "version": "1.0.0"
+    "version": "2.0.0"
 }
```

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/__init__.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/embedding_providers.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/embedding_providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/exception.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/exception.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/magics.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/magics.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/parsers.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/parsers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/providers.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/providers.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/jupyter_ai_magics/utils.py` & `jupyter_ai_magics-2.0.0/jupyter_ai_magics/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/.gitignore` & `jupyter_ai_magics-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/LICENSE` & `jupyter_ai_magics-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/pyproject.toml` & `jupyter_ai_magics-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai_magics-1.0.0/PKG-INFO` & `jupyter_ai_magics-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai_magics
-Version: 1.0.0
+Version: 2.0.0
 Summary: Jupyter AI magics Python package. Not published on NPM.
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

