# Comparing `tmp/spark_calibration-1.0.1.tar.gz` & `tmp/spark_calibration-1.0.2.tar.gz`

## Comparing `spark_calibration-1.0.1.tar` & `spark_calibration-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/betacal.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/metrics.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/visualisation.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/LICENSE
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/src/spark_calibration/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/src/spark_calibration/betacal.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/src/spark_calibration/metrics.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/src/spark_calibration/visualisation.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 spark_calibration-1.0.2/PKG-INFO
```

### Comparing `spark_calibration-1.0.1/src/spark_calibration/betacal.py` & `spark_calibration-1.0.2/src/spark_calibration/betacal.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.1/src/spark_calibration/metrics.py` & `spark_calibration-1.0.2/src/spark_calibration/metrics.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.1/src/spark_calibration/visualisation.py` & `spark_calibration-1.0.2/src/spark_calibration/visualisation.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.1/LICENSE` & `spark_calibration-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.1/README.md` & `spark_calibration-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,26 @@
-# BetaCal pyspark
+Metadata-Version: 2.1
+Name: spark_calibration
+Version: 1.0.2
+Summary: Calibratiing model scores/probabilites with pyspark dataframes
+Project-URL: Homepage, https://github.com/kjsr7/spark_calibration
+Project-URL: Bug Tracker, https://github.com/kjsr7/spark_calibration/issues
+Author-email: jaya <jaya.kommuru@meesho.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: numpy>=1.20.3
+Requires-Dist: plotly>=5.9.0
+Requires-Dist: pyspark>=3.2.1
+Requires-Dist: scikit-learn>=1.0.2
+Description-Content-Type: text/markdown
+
+# Model calibration with pyspark
 
 This package provides a Betacal class which allows the user to fit the default beta calibration model and predict calibrated scores
 
 
 ## Setup
 
 spark-calibration is [uploaded to PyPi](https://pypi.org/project/spark-calibration/) and can be installed with this command:
```

### Comparing `spark_calibration-1.0.1/pyproject.toml` & `spark_calibration-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spark_calibration"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="jaya", email="jaya.kommuru@meesho.com" },
 ]
-description = "model scores calibration for pyspark dataframes"
+description = "Calibratiing model scores/probabilites with pyspark dataframes"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "pyspark>=3.2.1",
     "numpy>=1.20.3",
     "plotly>=5.9.0",
     "scikit-learn>=1.0.2"
```

