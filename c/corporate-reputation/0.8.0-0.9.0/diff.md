# Comparing `tmp/corporate_reputation-0.8.0.tar.gz` & `tmp/corporate_reputation-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corporate_reputation-0.8.0.tar", max compression
+gzip compressed data, was "corporate_reputation-0.9.0.tar", max compression
```

## Comparing `corporate_reputation-0.8.0.tar` & `corporate_reputation-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0     1071 2023-07-26 19:11:27.879430 corporate_reputation-0.8.0/LICENSE
--rw-r--r--   0        0        0     3898 2023-07-26 19:11:27.879430 corporate_reputation-0.8.0/README.md
--rw-r--r--   0        0        0     3324 2023-07-26 19:12:03.036127 corporate_reputation-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      182 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/__cli__.py
--rw-r--r--   0        0        0      484 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/__init__.py
--rw-r--r--   0        0        0       22 2023-07-26 19:12:02.992127 corporate_reputation-0.8.0/src/corprep/_version.py
--rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/agent.py
--rw-r--r--   0        0        0     4793 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/absa/config.py
--rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/__init__.py
--rw-r--r--   0        0        0      286 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/about/corprep.yaml
--rw-r--r--   0        0        0      259 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/absa/default.yaml
--rw-r--r--   0        0        0     2930 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/absa/prompts/default.yaml
--rw-r--r--   0        0        0      113 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/absa_agent_predict.yaml
--rw-r--r--   0        0        0      156 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/dataset_filter.yaml
--rw-r--r--   0        0        0      107 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/pipe/dataset_load_raw.yaml
--rw-r--r--   0        0        0      230 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/absa_agent_predict.yaml
--rw-r--r--   0        0        0      171 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/filter_dataset.yaml
--rw-r--r--   0        0        0      138 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/conf/run/load_raw_dataset.yaml
--rw-r--r--   0        0        0      204 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/__init__.py
--rw-r--r--   0        0        0     1013 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/io.py
--rw-r--r--   0        0        0     1790 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/similarity.py
--rw-r--r--   0        0        0     2606 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/datasets/tokenize.py
--rw-r--r--   0        0        0        0 2023-07-26 19:11:27.883430 corporate_reputation-0.8.0/src/corprep/py.typed
--rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 corporate_reputation-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-27 09:12:13.325415 corporate_reputation-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3898 2023-07-27 09:12:13.325415 corporate_reputation-0.9.0/README.md
+-rw-r--r--   0        0        0     3407 2023-07-27 09:12:48.754425 corporate_reputation-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      182 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/__cli__.py
+-rw-r--r--   0        0        0      496 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-27 09:12:48.706424 corporate_reputation-0.9.0/src/corprep/_version.py
+-rw-r--r--   0        0        0        0 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/absa/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/absa/agent.py
+-rw-r--r--   0        0        0     4793 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/absa/config.py
+-rw-r--r--   0        0        0        0 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/__init__.py
+-rw-r--r--   0        0        0      286 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/about/corprep.yaml
+-rw-r--r--   0        0        0      259 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/absa/default.yaml
+-rw-r--r--   0        0        0     2930 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/absa/prompts/default.yaml
+-rw-r--r--   0        0        0      113 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      116 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/dataframe_save.yaml
+-rw-r--r--   0        0        0      156 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/dataset_filter.yaml
+-rw-r--r--   0        0        0      107 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/dataset_load_raw.yaml
+-rw-r--r--   0        0        0       85 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/dataset_to_pandas.yaml
+-rw-r--r--   0        0        0      112 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/find_similar_docs.yaml
+-rw-r--r--   0        0        0      101 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/pipe/pandas_print_head.yaml
+-rw-r--r--   0        0        0      206 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/run/absa_agent_predict.yaml
+-rw-r--r--   0        0        0      147 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/run/filter_dataset.yaml
+-rw-r--r--   0        0        0      364 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/run/find_similar_docs.yaml
+-rw-r--r--   0        0        0      114 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/run/load_raw_dataset.yaml
+-rw-r--r--   0        0        0      169 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/conf/run/save_dataframes.yaml
+-rw-r--r--   0        0        0      204 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/datasets/__init__.py
+-rw-r--r--   0        0        0     1013 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/datasets/io.py
+-rw-r--r--   0        0        0     9362 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/datasets/similarity.py
+-rw-r--r--   0        0        0     2606 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/datasets/tokenize.py
+-rw-r--r--   0        0        0        0 2023-07-27 09:12:13.329416 corporate_reputation-0.9.0/src/corprep/py.typed
+-rw-r--r--   0        0        0     4853 1970-01-01 00:00:00.000000 corporate_reputation-0.9.0/PKG-INFO
```

### Comparing `corporate_reputation-0.8.0/LICENSE` & `corporate_reputation-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/README.md` & `corporate_reputation-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/pyproject.toml` & `corporate_reputation-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corporate-reputation"
-version = "0.8.0"
+version = "0.9.0"
 description = "Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/corporate-reputation"
 repository = "https://github.com/entelecheia/corporate-reputation"
 readme = "README.md"
 packages = [{ include = "corprep", from = "src" }]
@@ -16,14 +16,16 @@
 python = ">=3.8.1,<3.12"
 hyfi = "^1.11.0"
 openai = "^0.27.8"
 backoff = "^2.2.1"
 scikit-learn = "^1.3.0"
 lexikanon = "^0.3.1"
 # lexikanon = { path = "../lexikanon", develop = true }
+# hyfi = { path = "../hyfi", develop = true }
+thematos = "^0.2.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
@@ -68,14 +70,15 @@
     "node_modules",
     "_build",
     "docs",
     "tests",
     "venv",
     ".copier-template",
     ".refs",
+    "workspace",
 ]
 per-file-ignores = ['__init__.py:F401', '_version.py:W292']
 
 [tool.mypy]
 namespace_packages = true
 exclude = [
     "node_modules",
```

### Comparing `corporate_reputation-0.8.0/src/corprep/absa/agent.py` & `corporate_reputation-0.9.0/src/corprep/absa/agent.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/src/corprep/absa/config.py` & `corporate_reputation-0.9.0/src/corprep/absa/config.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/src/corprep/conf/absa/prompts/default.yaml` & `corporate_reputation-0.9.0/src/corprep/conf/absa/prompts/default.yaml`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/src/corprep/datasets/io.py` & `corporate_reputation-0.9.0/src/corprep/datasets/io.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/src/corprep/datasets/tokenize.py` & `corporate_reputation-0.9.0/src/corprep/datasets/tokenize.py`

 * *Files identical despite different names*

### Comparing `corporate_reputation-0.8.0/PKG-INFO` & `corporate_reputation-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corporate-reputation
-Version: 0.8.0
+Version: 0.9.0
 Summary: Unraveling Corporate and CEO Reputation using Aspect-Based Sentiment Analysis and Signal Modeling
 Home-page: https://entelecheia.github.io/corporate-reputation
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: hyfi (>=1.11.0,<2.0.0)
 Requires-Dist: lexikanon (>=0.3.1,<0.4.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
+Requires-Dist: thematos (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/entelecheia/corporate-reputation
 Description-Content-Type: text/markdown
 
 # Reputation Analysis of Companies and CEOs
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

