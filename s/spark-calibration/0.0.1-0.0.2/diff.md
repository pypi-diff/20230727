# Comparing `tmp/spark_calibration-0.0.1.tar.gz` & `tmp/spark_calibration-0.0.2.tar.gz`

## Comparing `spark_calibration-0.0.1.tar` & `spark_calibration-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/src/spark_calibration/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/src/spark_calibration/betacal.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/src/spark_calibration/metrics.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/src/spark_calibration/visualisation.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/LICENSE
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/README.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 spark_calibration-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/__init__.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/betacal.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/metrics.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/visualisation.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/LICENSE
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/README.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/PKG-INFO
```

### Comparing `spark_calibration-0.0.1/src/spark_calibration/betacal.py` & `spark_calibration-0.0.2/src/spark_calibration/betacal.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-0.0.1/src/spark_calibration/metrics.py` & `spark_calibration-0.0.2/src/spark_calibration/metrics.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-0.0.1/src/spark_calibration/visualisation.py` & `spark_calibration-0.0.2/src/spark_calibration/visualisation.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-0.0.1/LICENSE` & `spark_calibration-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_calibration-0.0.1/pyproject.toml` & `spark_calibration-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spark_calibration"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="jaya", email="jaya.kommuru@meesho.com" },
 ]
 description = "model scores calibration for pyspark dataframes"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

