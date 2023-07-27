# Comparing `tmp/spark_calibration-1.0.0.tar.gz` & `tmp/spark_calibration-1.0.1.tar.gz`

## Comparing `spark_calibration-1.0.0.tar` & `spark_calibration-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/src/spark_calibration/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/src/spark_calibration/betacal.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/src/spark_calibration/metrics.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/src/spark_calibration/visualisation.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/LICENSE
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 spark_calibration-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/betacal.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/metrics.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/src/spark_calibration/visualisation.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/README.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 spark_calibration-1.0.1/PKG-INFO
```

### Comparing `spark_calibration-1.0.0/src/spark_calibration/betacal.py` & `spark_calibration-1.0.1/src/spark_calibration/betacal.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.0/src/spark_calibration/metrics.py` & `spark_calibration-1.0.1/src/spark_calibration/metrics.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.0/src/spark_calibration/visualisation.py` & `spark_calibration-1.0.1/src/spark_calibration/visualisation.py`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.0/LICENSE` & `spark_calibration-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_calibration-1.0.0/README.md` & `spark_calibration-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,21 @@
 
 
 bc = Betacal(parameters="abm")
 
 # training
 train_df = spark.read.parquet("s3://train/")
 bc.fit(train_df)
+
+
+# Get the logistic regression model and individual coefficients
+print(bc.lr_model, a, b)
+
+# a,b -> coefficients of lr model
+# lr_model -> pyspark ml logistic regression model
 ```
 
 
 ### Prediction
 
 test_df is a pyspark dataframe with `score` as one of the columns. The `predict` function adds a new column `prediction` which has the calibrated score
```

### Comparing `spark_calibration-1.0.0/pyproject.toml` & `spark_calibration-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spark_calibration"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="jaya", email="jaya.kommuru@meesho.com" },
 ]
 description = "model scores calibration for pyspark dataframes"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `spark_calibration-1.0.0/PKG-INFO` & `spark_calibration-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_calibration
-Version: 1.0.0
+Version: 1.0.1
 Summary: model scores calibration for pyspark dataframes
 Project-URL: Homepage, https://github.com/kjsr7/spark_calibration
 Project-URL: Bug Tracker, https://github.com/kjsr7/spark_calibration/issues
 Author-email: jaya <jaya.kommuru@meesho.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -42,14 +42,21 @@
 
 
 bc = Betacal(parameters="abm")
 
 # training
 train_df = spark.read.parquet("s3://train/")
 bc.fit(train_df)
+
+
+# Get the logistic regression model and individual coefficients
+print(bc.lr_model, a, b)
+
+# a,b -> coefficients of lr model
+# lr_model -> pyspark ml logistic regression model
 ```
 
 
 ### Prediction
 
 test_df is a pyspark dataframe with `score` as one of the columns. The `predict` function adds a new column `prediction` which has the calibrated score
```

