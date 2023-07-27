# Comparing `tmp/spark_calibration-0.0.2.tar.gz` & `tmp/spark_calibration-0.0.3.tar.gz`

## Comparing `spark_calibration-0.0.2.tar` & `spark_calibration-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/__init__.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/betacal.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/metrics.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/src/spark_calibration/visualisation.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/LICENSE
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/README.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 spark_calibration-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/src/spark_calibration/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/src/spark_calibration/betacal.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/src/spark_calibration/metrics.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/src/spark_calibration/visualisation.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/README.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 spark_calibration-0.0.3/PKG-INFO
```

### Comparing `spark_calibration-0.0.2/src/spark_calibration/betacal.py` & `spark_calibration-0.0.3/src/spark_calibration/betacal.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 
 from pyspark.ml.classification import LogisticRegression
 from pyspark.ml.feature import VectorAssembler
 from pyspark.sql.types import DoubleType
 
 from pyspark.sql.dataframe import DataFrame
 
-class Betacal():
-    
+
+class Betacal:
     def __init__(self, parameters):
         assert parameters == "abm"
-        
+
         self.parameters = parameters
         self.a = None
         self.b = None
         self.lr_model = None
-    
+
     def fit(self, df: DataFrame):
-        
-        assert "score" in df.columns and "label" in df.columns, "score and label columns should be present in the dataframe"
-    
-        if self.parameters == "abm":
+        assert (
+            "score" in df.columns and "label" in df.columns
+        ), "score and label columns should be present in the dataframe"
 
-            df = df.withColumn("score2", 1-F.col("score"))
-            df = df.withColumn("score", F.log("score")).withColumn("score2", -1 * F.log("score2"))
+        if self.parameters == "abm":
+            df = df.withColumn("score2", 1 - F.col("score"))
+            df = df.withColumn("score", F.log("score")).withColumn(
+                "score2", -1 * F.log("score2")
+            )
             lr = LogisticRegression()
-            featurizer = VectorAssembler(inputCols=["score", "score2"], outputCol="features")
+            featurizer = VectorAssembler(
+                inputCols=["score", "score2"], outputCol="features"
+            )
 
             train_data = featurizer.transform(df)["label", "features"]
 
             lr_fitted = lr.fit(train_data)
 
             lr_coef = lr_fitted.coefficients
 
@@ -47,51 +51,55 @@
                 train_data = featurizer.transform(df)["label", "features"]
                 lr_fitted = lr.fit(train_data)
                 b = 0
                 a = lr_fitted.coefficients[0]
             else:
                 a = lr_coef[0]
                 b = lr_coef[1]
-                
+
             self.a = a
             self.b = b
             self.lr_model = lr_fitted
 
     def predict(self, df: DataFrame):
-        
         cols = df.columns
-        
+
         assert "score" in cols, "score column should be present in the dataframe"
-        
+
         if self.parameters == "abm":
 
             def pick_value(v):
                 return float(v[1])
 
             pick_value = F.udf(pick_value, DoubleType())
-            
 
             df = df.withColumn("orig_score", F.col("score"))
 
-            df = df.withColumn("score2", 1-F.col("score"))
+            df = df.withColumn("score2", 1 - F.col("score"))
 
-            df = df.withColumn("score", F.log("score")).withColumn("score2", -1 * F.log("score2"))
+            df = df.withColumn("score", F.log("score")).withColumn(
+                "score2", -1 * F.log("score2")
+            )
 
             if self.a == 0:
                 featurizer = VectorAssembler(inputCols=["score2"], outputCol="features")
 
             elif self.b == 0:
                 featurizer = VectorAssembler(inputCols=["score"], outputCol="features")
 
             else:
-                featurizer = VectorAssembler(inputCols=["score", "score2"], outputCol="features")
+                featurizer = VectorAssembler(
+                    inputCols=["score", "score2"], outputCol="features"
+                )
 
             test_data = featurizer.transform(df)
-            
-            df = (self.lr_model.transform(test_data)
+
+            df = (
+                self.lr_model.transform(test_data)
                 .withColumn("prediction", pick_value("probability"))
                 .drop("score")
-                .withColumnRenamed("orig_score", "score"))                        
-            
+                .withColumnRenamed("orig_score", "score")
+            )
+
             df = df.select(cols + ["prediction"])
-            
-            return df
+
+            return df
```

### Comparing `spark_calibration-0.0.2/src/spark_calibration/metrics.py` & `spark_calibration-0.0.3/src/spark_calibration/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,67 @@
 from pyspark.ml.evaluation import BinaryClassificationEvaluator
 import pyspark.sql.functions as F
 
 from pyspark.sql.dataframe import DataFrame
 
+
 def display_classification_calib_metrics(df: DataFrame):
     """Print pre and post calibration metrics for comparison
 
     Args:
         df: dataframe with score, label and prediction(calibratied score) columns
     """
-    
-    assert "score" in df.columns and "label" in df.columns and  "prediction" in df.columns, "score and label columns should be present in the dataframe"
-        
-    model_bs = df.select(F.avg(F.pow(df["label"] - df["score"], 2))).collect()[0][0]
-    model_ll = df.select(F.avg(-F.col('label')*F.log(F.col('score')) - (1-F.col('label'))*F.log(1-F.col('score')))).collect()[0][0]
 
-    model_aucpr = BinaryClassificationEvaluator(rawPredictionCol="score", metricName="areaUnderPR").evaluate(df)
-    model_roc_auc = BinaryClassificationEvaluator(rawPredictionCol="score", metricName="areaUnderROC").evaluate(df)
+    assert (
+        "score" in df.columns and "label" in df.columns and "prediction" in df.columns
+    ), "score and label columns should be present in the dataframe"
+
+    model_bs = df.select(F.avg(F.pow(df["label"] - df["score"], 2))).collect()[0][0]
+    model_ll = df.select(
+        F.avg(
+            -F.col("label") * F.log(F.col("score"))
+            - (1 - F.col("label")) * F.log(1 - F.col("score"))
+        )
+    ).collect()[0][0]
+
+    model_aucpr = BinaryClassificationEvaluator(
+        rawPredictionCol="score", metricName="areaUnderPR"
+    ).evaluate(df)
+    model_roc_auc = BinaryClassificationEvaluator(
+        rawPredictionCol="score", metricName="areaUnderROC"
+    ).evaluate(df)
     iso_bs = df.select(F.avg(F.pow(df["label"] - df["prediction"], 2))).collect()[0][0]
 
     print(f"model brier score loss: {model_bs}")
     print(f"calibrated model brier score loss: {iso_bs}")
 
     print(f"delta: {round((iso_bs/model_bs - 1) * 100, 2)}%")
-    iso_ll = df.select(F.avg(-F.col('label')*F.log(F.col('prediction')) - (1-F.col('label'))*F.log(1-F.col('prediction')))).collect()[0][0]
+    iso_ll = df.select(
+        F.avg(
+            -F.col("label") * F.log(F.col("prediction"))
+            - (1 - F.col("label")) * F.log(1 - F.col("prediction"))
+        )
+    ).collect()[0][0]
 
     print("")
 
     print(f"model log loss: {model_ll}")
     print(f"calibrated model log loss: {iso_ll}")
     print(f"delta: {round((iso_ll/model_ll - 1) * 100, 2)}%")
-    iso_aucpr = BinaryClassificationEvaluator(rawPredictionCol="prediction", metricName="areaUnderPR").evaluate(df)
+    iso_aucpr = BinaryClassificationEvaluator(
+        rawPredictionCol="prediction", metricName="areaUnderPR"
+    ).evaluate(df)
 
     print("")
 
     print(f"model aucpr: {model_aucpr}")
     print(f"calibrated model aucpr: {iso_aucpr}")
     print(f"delta: {round((iso_aucpr/model_aucpr - 1) * 100, 2)}%")
-    iso_roc_auc = BinaryClassificationEvaluator(rawPredictionCol="prediction", metricName="areaUnderROC").evaluate(df)
+    iso_roc_auc = BinaryClassificationEvaluator(
+        rawPredictionCol="prediction", metricName="areaUnderROC"
+    ).evaluate(df)
 
     print("")
 
     print(f"model roc_auc: {model_roc_auc}")
     print(f"calibrated model roc_auc: {iso_roc_auc}")
-    print(f"delta: {round((iso_roc_auc/model_roc_auc - 1) * 100, 2)}%")
+    print(f"delta: {round((iso_roc_auc/model_roc_auc - 1) * 100, 2)}%")
```

### Comparing `spark_calibration-0.0.2/src/spark_calibration/visualisation.py` & `spark_calibration-0.0.3/src/spark_calibration/visualisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import plotly.graph_objects as go
 from sklearn.calibration import calibration_curve
 from pyspark.sql.dataframe import DataFrame
 
 
 def plot_calibration_curve(df: DataFrame):
-    
-    assert "score" in df.columns and "label" in df.columns and  "prediction" in df.columns, "score and label columns should be present in the dataframe"
-    
+    assert (
+        "score" in df.columns and "label" in df.columns and "prediction" in df.columns
+    ), "score and label columns should be present in the dataframe"
+
     df_p_v = df.select("label", "score", "prediction").toPandas().values
 
     y_test_true, y_test_pred, y_test_pred_cal = df_p_v[:, 0], df_p_v[:, 1], df_p_v[:, 2]
 
     fig = go.Figure()
 
     fig.add_trace(
@@ -24,28 +25,29 @@
     )
 
     prob_true, prob_pred = calibration_curve(
         y_test_true, y_test_pred, n_bins=50, strategy="quantile"
     )
     print(f"number of bins for pre-calibration scores: {prob_true.shape[0]}")
 
-    fig.add_trace(go.Scatter(x=prob_pred, y=prob_true, mode="lines+markers", name="Model"))
-
+    fig.add_trace(
+        go.Scatter(x=prob_pred, y=prob_true, mode="lines+markers", name="Model")
+    )
 
     prob_true, prob_pred = calibration_curve(
         y_test_true, y_test_pred_cal, n_bins=50, strategy="quantile"
     )
     print(f"number of bins for post-calibration scores: {prob_true.shape[0]}")
 
     fig.add_trace(
-        go.Scatter(x=prob_pred, y=prob_true, mode="lines+markers", name="Calibrated Model")
+        go.Scatter(
+            x=prob_pred, y=prob_true, mode="lines+markers", name="Calibrated Model"
+        )
     )
 
     fig.update_layout(
         title=dict(text="Calibration Curve on test data (quantile bins)", x=0.5),
         xaxis_title="Mean Predicted Probability",
         yaxis_title="Fraction of Positives",
     )
 
-
     fig.show()
-
```

### Comparing `spark_calibration-0.0.2/LICENSE` & `spark_calibration-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_calibration-0.0.2/pyproject.toml` & `spark_calibration-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spark_calibration"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="jaya", email="jaya.kommuru@meesho.com" },
 ]
 description = "model scores calibration for pyspark dataframes"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `spark_calibration-0.0.2/PKG-INFO` & `spark_calibration-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_calibration
-Version: 0.0.2
+Version: 0.0.3
 Summary: model scores calibration for pyspark dataframes
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: jaya <jaya.kommuru@meesho.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,33 +27,51 @@
 
 ```
 pip install spark-calibration
 ```
 
 ## Usage
 
+### Training
+
+train_df should be a pyspark dataframe with `score` and `label` columns
+
 ```
 from spark_calibration import Betacal
 from spark_calibration import display_classification_calib_metrics
 from spark_calibration import plot_calibration_curve
 
+
 bc = Betacal(parameters="abm")
 
 # training
 train_df = spark.read.parquet("s3://train/")
 bc.fit(train_df)
+```
 
-# prediction
-test_df = spark.read.parquet("s3://test/")
-test_df = bc.predict(test_df)
 
+### Prediction
 
-display_classification_calib_metrics(test_df)
+test_df is a pyspark dataframe with `score` as one of the columns. The `predict` function adds a new column `prediction` which has the calibrated score
+
+```
+test_df = spark.read.parquet("s3://test/")
+test_df = bc.predict(test_df)
+```
 
-plot_calibration_curve(test_df)
 
+### Pre post calibration metrics comparison
 
+The test_df should have `score`, `prediction` & `label` columns. 
+The `display_classification_calib_metrics` functions displays `brier_score_loss`, `log_loss`, `area_under_PR_curve` and `area_under_ROC_curve`
+```
+display_classification_calib_metrics(test_df)
 ```
 
 
+### plot the calibration curve
 
+Computes true, predicted probabilites (pre & post calibration) using quantile binning strategy with 50 bins and plots the calibration curve
 
+```
+plot_calibration_curve(test_df)
+```
```

