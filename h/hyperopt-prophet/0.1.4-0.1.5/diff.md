# Comparing `tmp/hyperopt_prophet-0.1.4.tar.gz` & `tmp/hyperopt_prophet-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.4.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.5.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.4.tar` & `hyperopt_prophet-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-26 04:48:12.823779 hyperopt_prophet-0.1.4/LICENSE
--rw-r--r--   0        0        0      980 2023-07-26 04:48:12.823779 hyperopt_prophet-0.1.4/README.md
--rw-r--r--   0        0        0      101 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0     5047 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21410 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9108 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/main.py
--rw-r--r--   0        0        0      818 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/README.md
+-rw-r--r--   0        0        0      101 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9108 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/main.py
+-rw-r--r--   0        0        0      797 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.5/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.4/LICENSE` & `hyperopt_prophet-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/README.md` & `hyperopt_prophet-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.5/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.5/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.5/hyperopt_prophet/training.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.5/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.4/pyproject.toml` & `hyperopt_prophet-0.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.4"
+version = "0.1.5"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
@@ -16,15 +16,14 @@
 pydantic = "^2.1.0"
 pydantic-settings = "^2.0.2"
 prophet = "^1.0.0"
 hyperopt = "^0.2.7"
 mlflow = "^2.5.0"
 cloudpickle = "^2.2.1"
 cython = "^3.0.0"
-pystan = "^2.19.1.1"
 mlflowops = '^0.1.2'
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.4.0"
 pylint = "^2.17.4"
```

### Comparing `hyperopt_prophet-0.1.4/PKG-INFO` & `hyperopt_prophet-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.4
+Version: 0.1.5
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,14 @@
 Requires-Dist: hyperopt (>=0.2.7,<0.3.0)
 Requires-Dist: mlflow (>=2.5.0,<3.0.0)
 Requires-Dist: mlflowops (>=0.1.2,<0.2.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: prophet (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=2.1.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
-Requires-Dist: pystan (>=2.19.1.1,<3.0.0.0)
 Description-Content-Type: text/markdown
 
 # Hyperopt Prophet
 
 **Integration of prophet forecasting with hyperopt, mlflow**
 This implementation is based on the [Databricks AutoML](https://github.com/databricks/automl) repository.
```

