# Comparing `tmp/hyperopt_prophet-0.1.5.tar.gz` & `tmp/hyperopt_prophet-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.5.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.6.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.5.tar` & `hyperopt_prophet-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/LICENSE
--rw-r--r--   0        0        0      980 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/README.md
--rw-r--r--   0        0        0      101 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0     5047 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21410 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9108 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/main.py
--rw-r--r--   0        0        0      797 2023-07-26 22:12:37.794354 hyperopt_prophet-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/README.md
+-rw-r--r--   0        0        0      101 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9129 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/main.py
+-rw-r--r--   0        0        0      797 2023-07-26 22:40:15.698201 hyperopt_prophet-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.6/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.5/LICENSE` & `hyperopt_prophet-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.5/README.md` & `hyperopt_prophet-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.5/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.6/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.5/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.6/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.5/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.6/hyperopt_prophet/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 import mlflow
 import mlflow.prophet
 import pandas as pd
 from hyperopt import hp
 from mlflowops import MLFlowOps
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
-from .model import (
-    MultiSeriesProphetModel,
-    ProphetHyperoptEstimator,
-    mlflow_prophet_log_model,
-)
+from .model import (MultiSeriesProphetModel, ProphetHyperoptEstimator,
+                    mlflow_prophet_log_model)
 from .utils import get_plotly_forecast, plotly_fig2pil
 
 warnings.filterwarnings("ignore")
 
 
 class ProphetTrainingParams(BaseSettings):
     """
@@ -97,15 +94,15 @@
 
 class ProphetHyperOptTrainer:
     def __init__(
         self, training_data: pd.DataFrame, training_params: ProphetTrainingParams
     ):
         self.training_data = training_data
         self.training_params = training_params
-        self.ts_id = str(training_data["ts_id"].iloc[0])
+        self.ts_id = str(training_data[training_params.id_cols].iloc[0])
 
     def register_model(self, training_loss, training_run_id):
         runs_names = "prophet_" + self.ts_id
         mlops = MLFlowOps(
             runs_names=[runs_names],
             experiment_ids=self.training_params.experiment_id,
             base_model_name=self.training_params.base_model_name,
```

### Comparing `hyperopt_prophet-0.1.5/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.6/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.5/pyproject.toml` & `hyperopt_prophet-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.5"
+version = "0.1.6"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
```

### Comparing `hyperopt_prophet-0.1.5/PKG-INFO` & `hyperopt_prophet-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.5
+Version: 0.1.6
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

