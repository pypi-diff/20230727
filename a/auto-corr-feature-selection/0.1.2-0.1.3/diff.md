# Comparing `tmp/auto_corr_feature_selection-0.1.2.tar.gz` & `tmp/auto_corr_feature_selection-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_corr_feature_selection-0.1.2.tar", max compression
+gzip compressed data, was "auto_corr_feature_selection-0.1.3.tar", max compression
```

## Comparing `auto_corr_feature_selection-0.1.2.tar` & `auto_corr_feature_selection-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3136 2023-07-19 14:13:50.699169 auto_corr_feature_selection-0.1.2/README.md
--rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/__init__.py
--rw-r--r--   0        0        0     3079 2023-07-27 14:27:34.277475 auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/auto_corr_feature_selection.py
--rw-r--r--   0        0        0      850 2023-07-27 14:31:33.745449 auto_corr_feature_selection-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3799 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3136 2023-07-19 14:13:50.699169 auto_corr_feature_selection-0.1.3/README.md
+-rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.3/auto_corr_feature_selection/__init__.py
+-rw-r--r--   0        0        0     3079 2023-07-27 14:27:34.277475 auto_corr_feature_selection-0.1.3/auto_corr_feature_selection/auto_corr_feature_selection.py
+-rw-r--r--   0        0        0      834 2023-07-27 14:37:08.984233 auto_corr_feature_selection-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.3/PKG-INFO
```

### Comparing `auto_corr_feature_selection-0.1.2/README.md` & `auto_corr_feature_selection-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `auto_corr_feature_selection-0.1.2/auto_corr_feature_selection/auto_corr_feature_selection.py` & `auto_corr_feature_selection-0.1.3/auto_corr_feature_selection/auto_corr_feature_selection.py`

 * *Files identical despite different names*

### Comparing `auto_corr_feature_selection-0.1.2/pyproject.toml` & `auto_corr_feature_selection-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 [tool.poetry]
 name = "auto_corr_feature_selection"
-version = "0.1.2"
+version = "0.1.3"
 description = "Automatically select the most relevant features based on correlation."
 authors = ["Andrés Di Giovanni <andresdigiovanni@gmail.com>"]
 readme = "README.md"
 license = "MIT"
+homepage = "https://github.com/andresdigiovanni/auto-corr-feature-selection"
 packages = [{include = "auto_corr_feature_selection"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 pandas = ">1.5.0"
 numpy = "^1.25.1"
 scikit-learn = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pre-commit = "^2.20.0"
 
-[project.urls]
-Homepage = "https://github.com/andresdigiovanni/auto-corr-feature-selection"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
 include = '\.pyi?$'
```

### Comparing `auto_corr_feature_selection-0.1.2/PKG-INFO` & `auto_corr_feature_selection-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: auto-corr-feature-selection
-Version: 0.1.2
+Version: 0.1.3
 Summary: Automatically select the most relevant features based on correlation.
+Home-page: https://github.com/andresdigiovanni/auto-corr-feature-selection
 License: MIT
 Author: Andrés Di Giovanni
 Author-email: andresdigiovanni@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

