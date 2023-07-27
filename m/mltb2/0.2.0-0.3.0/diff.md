# Comparing `tmp/mltb2-0.2.0.tar.gz` & `tmp/mltb2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltb2-0.2.0.tar", last modified: Wed Jul 19 16:04:16 2023, max compression
+gzip compressed data, was "mltb2-0.3.0.tar", last modified: Thu Jul 27 18:58:47 2023, max compression
```

## Comparing `mltb2-0.2.0.tar` & `mltb2-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:04:16.425852 mltb2-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-19 16:04:01.000000 mltb2-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-19 16:04:01.000000 mltb2-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-19 16:04:16.425852 mltb2-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-19 16:04:01.000000 mltb2-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:04:16.421852 mltb2-0.2.0/mltb2/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-19 16:04:01.000000 mltb2-0.2.0/mltb2/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:04:16.421852 mltb2-0.2.0/mltb2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-19 16:04:16.000000 mltb2-0.2.0/mltb2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-19 16:04:16.000000 mltb2-0.2.0/mltb2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 16:04:16.000000 mltb2-0.2.0/mltb2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-19 16:04:16.000000 mltb2-0.2.0/mltb2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-19 16:04:16.000000 mltb2-0.2.0/mltb2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-19 16:04:01.000000 mltb2-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-19 16:04:16.425852 mltb2-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-19 16:04:01.000000 mltb2-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 16:04:16.425852 mltb2-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_optuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_somajo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_somajo_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 16:04:01.000000 mltb2-0.2.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:58:47.674665 mltb2-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-27 18:58:36.000000 mltb2-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 18:58:36.000000 mltb2-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-27 18:58:47.674665 mltb2-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 18:58:36.000000 mltb2-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:58:47.670665 mltb2-0.3.0/mltb2/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-27 18:58:36.000000 mltb2-0.3.0/mltb2/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:58:47.670665 mltb2-0.3.0/mltb2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-27 18:58:47.000000 mltb2-0.3.0/mltb2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-27 18:58:47.000000 mltb2-0.3.0/mltb2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:58:47.000000 mltb2-0.3.0/mltb2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-27 18:58:47.000000 mltb2-0.3.0/mltb2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 18:58:47.000000 mltb2-0.3.0/mltb2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-27 18:58:36.000000 mltb2-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-27 18:58:47.674665 mltb2-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-27 18:58:36.000000 mltb2-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:58:47.674665 mltb2-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_somajo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_somajo_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 18:58:36.000000 mltb2-0.3.0/tests/test_transformers.py
```

### Comparing `mltb2-0.2.0/LICENSE` & `mltb2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/PKG-INFO` & `mltb2-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.2.0
+Version: 0.3.0
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -32,14 +32,15 @@
 Provides-Extra: files
 Provides-Extra: fasttext
 Provides-Extra: optuna
 Provides-Extra: plot
 Provides-Extra: somajo
 Provides-Extra: transformers
 Provides-Extra: somajo_transformers
+Provides-Extra: openai
 Provides-Extra: optional
 Provides-Extra: checking
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `mltb2-0.2.0/README.md` & `mltb2-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/fasttext.py` & `mltb2-0.3.0/mltb2/fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/files.py` & `mltb2-0.3.0/mltb2/files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/optuna.py` & `mltb2-0.3.0/mltb2/optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/plot.py` & `mltb2-0.3.0/mltb2/plot.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/somajo.py` & `mltb2-0.3.0/mltb2/somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/somajo_transformers.py` & `mltb2-0.3.0/mltb2/somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2/transformers.py` & `mltb2-0.3.0/mltb2/transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/mltb2.egg-info/PKG-INFO` & `mltb2-0.3.0/mltb2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltb2
-Version: 0.2.0
+Version: 0.3.0
 Summary: Machine Learning Toolbox
 Home-page: https://github.com/telekom/mltb2
 Author: Philip May
 Author-email: philip@may.la
 Maintainer: Philip May
 Project-URL: Bug Tracker, https://github.com/telekom/mltb2/issues
 Project-URL: Documentation, https://telekom.github.io/mltb2/
@@ -32,14 +32,15 @@
 Provides-Extra: files
 Provides-Extra: fasttext
 Provides-Extra: optuna
 Provides-Extra: plot
 Provides-Extra: somajo
 Provides-Extra: transformers
 Provides-Extra: somajo_transformers
+Provides-Extra: openai
 Provides-Extra: optional
 Provides-Extra: checking
 Provides-Extra: testing
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `mltb2-0.2.0/mltb2.egg-info/SOURCES.txt` & `mltb2-0.3.0/mltb2.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 mltb2/__init__.py
 mltb2/fasttext.py
 mltb2/files.py
+mltb2/openai.py
 mltb2/optuna.py
 mltb2/plot.py
 mltb2/somajo.py
 mltb2/somajo_transformers.py
 mltb2/transformers.py
 mltb2.egg-info/PKG-INFO
 mltb2.egg-info/SOURCES.txt
 mltb2.egg-info/dependency_links.txt
 mltb2.egg-info/requires.txt
 mltb2.egg-info/top_level.txt
 tests/__init__.py
 tests/test__init__.py
 tests/test_fasttext.py
 tests/test_files.py
+tests/test_openai.py
 tests/test_optuna.py
 tests/test_somajo.py
 tests/test_somajo_transformers.py
 tests/test_transformers.py
```

### Comparing `mltb2-0.2.0/pyproject.toml` & `mltb2-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/setup.py` & `mltb2-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,39 @@
 files_requires = {"platformdirs", "scikit-learn"}
 fasttext_requires = files_requires | {"fasttext-wheel"}
 optuna_requires = {"numpy", "optuna", "scipy"}
 plot_requires = {"matplotlib"}
 somajo_requires = {"SoMaJo", "tqdm"}
 transformers_requires = {"scikit-learn", "torch", "tqdm", "transformers"}
 somajo_transformers_requires = somajo_requires | transformers_requires | {"tqdm"}
+openai_requires = {"tiktoken"}
 optional_requires = (
     somajo_transformers_requires
     | transformers_requires
     | somajo_requires
     | plot_requires
     | optuna_requires
     | fasttext_requires
     | files_requires
+    | openai_requires
 )
 
 project_name = "mltb2"
 source_code = "https://github.com/telekom/mltb2"
 keywords = "optuna deep-learning ml ai machine-learning hyperparameter-optimization"
 install_requires = ["numpy", "scipy", "tqdm"]
 extras_require = {
     "files": files_requires,
     "fasttext": fasttext_requires,
     "optuna": optuna_requires,
     "plot": plot_requires,
     "somajo": somajo_requires,
     "transformers": transformers_requires,
     "somajo_transformers": somajo_transformers_requires,
+    "openai": openai_requires,
     "optional": optional_requires,
     "checking": [
         "black",
         "flake8",
         "isort",
         "mdformat",
         "pydocstyle",
```

### Comparing `mltb2-0.2.0/tests/test_fasttext.py` & `mltb2-0.3.0/tests/test_fasttext.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/tests/test_files.py` & `mltb2-0.3.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/tests/test_optuna.py` & `mltb2-0.3.0/tests/test_optuna.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/tests/test_somajo.py` & `mltb2-0.3.0/tests/test_somajo.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/tests/test_somajo_transformers.py` & `mltb2-0.3.0/tests/test_somajo_transformers.py`

 * *Files identical despite different names*

### Comparing `mltb2-0.2.0/tests/test_transformers.py` & `mltb2-0.3.0/tests/test_transformers.py`

 * *Files identical despite different names*

