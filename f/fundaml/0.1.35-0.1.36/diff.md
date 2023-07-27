# Comparing `tmp/fundaml-0.1.35.tar.gz` & `tmp/fundaml-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundaml-0.1.35.tar", max compression
+gzip compressed data, was "fundaml-0.1.36.tar", max compression
```

## Comparing `fundaml-0.1.35.tar` & `fundaml-0.1.36.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0     1069 2023-07-26 23:07:33.180570 fundaml-0.1.35/LICENSE
--rw-r--r--   0        0        0     2284 2023-07-26 23:07:33.180570 fundaml-0.1.35/README.md
--rw-r--r--   0        0        0     1614 2023-07-26 23:23:40.752364 fundaml-0.1.35/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/__init__.py
--rw-r--r--   0        0        0     1058 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/eda.py
--rw-r--r--   0        0        0     3247 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/models.py
--rw-r--r--   0        0        0     1032 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/scores.py
--rw-r--r--   0        0        0     3050 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/tokenizers.py
--rw-r--r--   0        0        0    17645 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/trainers.py
--rw-r--r--   0        0        0    24833 2023-07-26 23:07:33.544575 fundaml-0.1.35/src/fundaml/transformer_from_scratch.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.35/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-07-27 00:19:23.374282 fundaml-0.1.36/LICENSE
+-rw-r--r--   0        0        0     2284 2023-07-27 00:19:23.374282 fundaml-0.1.36/README.md
+-rw-r--r--   0        0        0     1614 2023-07-27 00:34:08.709918 fundaml-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/__init__.py
+-rw-r--r--   0        0        0     1058 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/eda.py
+-rw-r--r--   0        0        0     3247 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/models.py
+-rw-r--r--   0        0        0     1032 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/scores.py
+-rw-r--r--   0        0        0     3050 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/tokenizers.py
+-rw-r--r--   0        0        0    17645 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/trainers.py
+-rw-r--r--   0        0        0    24833 2023-07-27 00:19:23.770293 fundaml-0.1.36/src/fundaml/transformer_from_scratch.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 fundaml-0.1.36/PKG-INFO
```

### Comparing `fundaml-0.1.35/LICENSE` & `fundaml-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/README.md` & `fundaml-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/pyproject.toml` & `fundaml-0.1.36/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fundaml"
-version = "0.1.35"
+version = "0.1.36"
 description = "A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks."
 authors = ["Tony Zoght"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `fundaml-0.1.35/src/fundaml/eda.py` & `fundaml-0.1.36/src/fundaml/eda.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/src/fundaml/models.py` & `fundaml-0.1.36/src/fundaml/models.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/src/fundaml/scores.py` & `fundaml-0.1.36/src/fundaml/scores.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/src/fundaml/tokenizers.py` & `fundaml-0.1.36/src/fundaml/tokenizers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/src/fundaml/trainers.py` & `fundaml-0.1.36/src/fundaml/trainers.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/src/fundaml/transformer_from_scratch.py` & `fundaml-0.1.36/src/fundaml/transformer_from_scratch.py`

 * *Files identical despite different names*

### Comparing `fundaml-0.1.35/PKG-INFO` & `fundaml-0.1.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundaml
-Version: 0.1.35
+Version: 0.1.36
 Summary: A foundational machine learning library designed to streamline the end-to-end process of developing and deploying machine learning models. FundAML offers a broad array of tools and utilities for data preprocessing, model training, evaluation, and deployment, making it a fundamental solution for machine learning tasks.
 License: MIT
 Author: Tony Zoght
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

