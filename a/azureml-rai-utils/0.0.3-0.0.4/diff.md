# Comparing `tmp/azureml_rai_utils-0.0.3-py3-none-any.whl.zip` & `tmp/azureml_rai_utils-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,44 @@
-Zip file size: 11338 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      183 b- defN 23-Jun-29 15:51 azureml/__init__.py
--rw-rw-rw-  2.0 fat      183 b- defN 23-Jun-29 15:51 azureml/rai/__init__.py
--rw-rw-rw-  2.0 fat      319 b- defN 23-Jun-29 15:51 azureml/rai/utils/__init__.py
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jun-29 15:55 azureml/rai/utils/_version.py
--rw-rw-rw-  2.0 fat      680 b- defN 23-Jun-29 15:51 azureml/rai/utils/constants.py
--rw-rw-rw-  2.0 fat     7431 b- defN 23-Jun-29 15:51 azureml/rai/utils/dataset_manager.py
--rw-rw-rw-  2.0 fat     5364 b- defN 23-Jun-29 15:51 azureml/rai/utils/model_serializer.py
--rw-rw-rw-  2.0 fat      318 b- defN 23-Jun-29 15:51 azureml/rai/utils/pyfunc_model.py
--rw-rw-rw-  2.0 fat      274 b- defN 23-Jun-29 15:51 azureml/rai/utils/telemetry/__init__.py
--rw-rw-rw-  2.0 fat     6811 b- defN 23-Jun-29 15:51 azureml/rai/utils/telemetry/loggerfactory.py
--rw-rw-rw-  2.0 fat      675 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1629 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1443 b- defN 23-Jun-29 16:10 azureml_rai_utils-0.0.3.dist-info/RECORD
-16 files, 26526 bytes uncompressed, 8934 bytes compressed:  66.3%
+Zip file size: 36850 bytes, number of entries: 42
+-rw-rw-rw-  2.0 fat      247 b- defN 23-Jul-27 18:13 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      183 b- defN 23-Jul-27 18:13 azureml/rai/__init__.py
+-rw-rw-rw-  2.0 fat      319 b- defN 23-Jul-27 18:13 azureml/rai/utils/__init__.py
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Jul-27 18:15 azureml/rai/utils/_version.py
+-rw-rw-rw-  2.0 fat      864 b- defN 23-Jul-27 18:13 azureml/rai/utils/constants.py
+-rw-rw-rw-  2.0 fat     7431 b- defN 23-Jul-27 18:13 azureml/rai/utils/dataset_manager.py
+-rw-rw-rw-  2.0 fat     8697 b- defN 23-Jul-27 18:13 azureml/rai/utils/mlflow_model_wrapper.py
+-rw-rw-rw-  2.0 fat     6559 b- defN 23-Jul-27 18:13 azureml/rai/utils/model_serializer.py
+-rw-rw-rw-  2.0 fat      318 b- defN 23-Jul-27 18:13 azureml/rai/utils/pyfunc_model.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/__init__.py
+-rw-rw-rw-  2.0 fat     2864 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/e2e.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/benchmarkutils/__init__.py
+-rw-rw-rw-  2.0 fat     2239 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/benchmarkutils/azure_connector.py
+-rw-rw-rw-  2.0 fat      628 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/benchmarkutils/constants.py
+-rw-rw-rw-  2.0 fat      806 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/benchmarkutils/http_client.py
+-rw-rw-rw-  2.0 fat      677 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/benchmarkutils/tokenizer.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/__init__.py
+-rw-rw-rw-  2.0 fat     2482 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/data_preparer.py
+-rw-rw-rw-  2.0 fat     7551 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/experiment_runner.py
+-rw-rw-rw-  2.0 fat     1791 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/metrics_generator.py
+-rw-rw-rw-  2.0 fat    10925 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/prompt_formatter.py
+-rw-rw-rw-  2.0 fat     6106 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/request_manager.py
+-rw-rw-rw-  2.0 fat     4743 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/response_parser.py
+-rw-rw-rw-  2.0 fat     5378 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/scoring_manager.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/model/__init__.py
+-rw-rw-rw-  2.0 fat      319 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/model/input_sample.py
+-rw-rw-rw-  2.0 fat      833 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/model/job.py
+-rw-rw-rw-  2.0 fat      744 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/common/model/prompt_data.py
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/configs/__init__.py
+-rw-rw-rw-  2.0 fat      142 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/configs/aml_workspace_config.json
+-rw-rw-rw-  2.0 fat      148 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/configs/request_config.json
+-rw-rw-rw-  2.0 fat      181 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/groundedness/__init__.py
+-rw-rw-rw-  2.0 fat     2338 b- defN 23-Jul-27 18:13 azureml/rai/utils/llm_eval_benchmark/groundedness/groundedness_benchmark_runner.py
+-rw-rw-rw-  2.0 fat      274 b- defN 23-Jul-27 18:13 azureml/rai/utils/telemetry/__init__.py
+-rw-rw-rw-  2.0 fat     6811 b- defN 23-Jul-27 18:13 azureml/rai/utils/telemetry/loggerfactory.py
+-rw-rw-rw-  2.0 fat      675 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat       80 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat     1446 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2046 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     4516 b- defN 23-Jul-27 18:29 azureml_rai_utils-0.0.4.dist-info/RECORD
+42 files, 92390 bytes uncompressed, 29310 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -12,38 +12,116 @@
 
 Filename: azureml/rai/utils/constants.py
 Comment: 
 
 Filename: azureml/rai/utils/dataset_manager.py
 Comment: 
 
+Filename: azureml/rai/utils/mlflow_model_wrapper.py
+Comment: 
+
 Filename: azureml/rai/utils/model_serializer.py
 Comment: 
 
 Filename: azureml/rai/utils/pyfunc_model.py
 Comment: 
 
+Filename: azureml/rai/utils/llm_eval_benchmark/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/e2e.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/benchmarkutils/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/benchmarkutils/azure_connector.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/benchmarkutils/constants.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/benchmarkutils/http_client.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/benchmarkutils/tokenizer.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/data_preparer.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/experiment_runner.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/metrics_generator.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/prompt_formatter.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/request_manager.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/response_parser.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/scoring_manager.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/model/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/model/input_sample.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/model/job.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/common/model/prompt_data.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/configs/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/configs/aml_workspace_config.json
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/configs/request_config.json
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/groundedness/__init__.py
+Comment: 
+
+Filename: azureml/rai/utils/llm_eval_benchmark/groundedness/groundedness_benchmark_runner.py
+Comment: 
+
 Filename: azureml/rai/utils/telemetry/__init__.py
 Comment: 
 
 Filename: azureml/rai/utils/telemetry/loggerfactory.py
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/DESCRIPTION.rst
+Filename: azureml_rai_utils-0.0.4.dist-info/DESCRIPTION.rst
+Comment: 
+
+Filename: azureml_rai_utils-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/metadata.json
+Filename: azureml_rai_utils-0.0.4.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/top_level.txt
+Filename: azureml_rai_utils-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/WHEEL
+Filename: azureml_rai_utils-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/METADATA
+Filename: azureml_rai_utils-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: azureml_rai_utils-0.0.3.dist-info/RECORD
+Filename: azureml_rai_utils-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/__init__.py

```diff
@@ -1,3 +1,4 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
+__path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

## azureml/rai/utils/_version.py

```diff
@@ -1 +1 @@
-VERSION = "0.0.3"
+VERSION = "0.0.4"
```

## azureml/rai/utils/constants.py

```diff
@@ -6,16 +6,24 @@
 
 
 AUTOML_MLIMAGES_MLFLOW_MODEL_IDENTIFIER = (
     "azureml.automl.dnn.vision.common.mlflow.mlflow_model_wrapper."
     "MLFlowImagesModelWrapper'>"
 )
 
+
 class ModelTypes:
     FASTAI = "fastai"
     PYTORCH = "pytorch"
     PYFUNC = "pyfunc"
+    HFTRANSFORMERS = "hftransformers"
+
+
+class TaskType:
+    TEXT_CLASSIFICATION = "text_classification"
+    MULTILABEL_TEXT_CLASSIFICATION = "multilabel_text_classification"
+
 
 class CredentialType(str, Enum):
     AZUREML_ON_BEHALF_OF_CREDENTIAL = "AzureMLOnBehalfOfCredential"
     DEFAULT_AZURE_CREDENTIAL = "DefaultAzureCredential"
     MANAGED_IDENTITY_CREDENTIAL = "ManagedIdentityCredential"
```

## azureml/rai/utils/model_serializer.py

```diff
@@ -8,17 +8,27 @@
 
 import os
 import subprocess
 import sys
 import mlflow
 
 from azureml.rai.utils.constants import (
-    AUTOML_MLIMAGES_MLFLOW_MODEL_IDENTIFIER, 
-    ModelTypes
+    AUTOML_MLIMAGES_MLFLOW_MODEL_IDENTIFIER,
+    ModelTypes,
+    TaskType
 )
+from azureml.rai.utils.mlflow_model_wrapper import (
+    get_predictor
+)
+
+try:
+    import azureml.evaluate.mlflow as aml_mlflow
+    aml_mlflow_installed = True
+except ImportError:
+    aml_mlflow_installed = False
 
 _logger = logging.getLogger(__file__)
 logging.basicConfig(level=logging.INFO)
 
 
 def log_info(message):
     _logger.info(message)
@@ -27,20 +37,24 @@
 
 class ModelSerializer:
     def __init__(self,
                  model_id: str,
                  model_type: str = "pyfunc",
                  use_model_dependency: bool = False,
                  use_conda: bool = True,
-                 tracking_uri: str = None):
+                 tracking_uri: str = None,
+                 mlflow_model: str = None,
+                 task_type: TaskType = None):
         self._model_id = model_id
+        self._mlflow_model = mlflow_model
         self._model_type = model_type
         self._use_model_dependency = use_model_dependency
         self._use_conda = use_conda
         self._tracking_uri = tracking_uri
+        self._task_type = task_type
 
     def save(self, model, path):
         # Nothing to do, since model is saved in AzureML
         pass
 
     def load(self, path):
         return self.load_mlflow_model(self._model_id)
@@ -51,14 +65,29 @@
             log_info("Current non azureml tracking uri: " + tracking_uri)
             log_info("Setting mlflow tracking uri to: " + self._tracking_uri)
             mlflow.set_tracking_uri(self._tracking_uri)
         client = mlflow.tracking.MlflowClient()
 
         split_model_id = model_id.rsplit(":", 1)
         model_name = split_model_id[0]
+
+        if self._model_type == ModelTypes.HFTRANSFORMERS:
+            if not aml_mlflow_installed:
+                error = "azureml.evaluate.mlflow package is required to \
+                         load HFTransformers model"
+                raise RuntimeError(error)
+            if self._task_type == TaskType.TEXT_CLASSIFICATION:
+                aml_mlflow_model = aml_mlflow.aml.load_model(
+                    self._mlflow_model, "text-classifier")
+                log_info("mlflow_loaded: {0}".format(type(aml_mlflow_model)))
+                log_info(f"dir(mlflow_loaded): {dir(aml_mlflow_model)}")
+                predictor_cls = get_predictor(TaskType.TEXT_CLASSIFICATION)
+                predictor = predictor_cls(aml_mlflow_model)
+                return predictor
+
         if model_name == model_id:
             model = client.get_registered_model(model_id)
             model_uri_name = model.name
             model_uri_version = model.latest_versions[0].version
         else:
             version = split_model_id[1]
             model = client.get_model_version(model_name, version=version)
```

## Comparing `azureml_rai_utils-0.0.3.dist-info/DESCRIPTION.rst` & `azureml_rai_utils-0.0.4.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `azureml_rai_utils-0.0.3.dist-info/metadata.json` & `azureml_rai_utils-0.0.4.dist-info/metadata.json`

 * *Files 26% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8782051282051282%*

 * *Differences: {"'extensions'": "{'python.commands': OrderedDict([('wrap_console', OrderedDict([('rai-benchmark', "*

 * *                 "'azureml.rai.utils.llm_eval_benchmark.e2e:main')]))]), 'python.exports': "*

 * *                 "OrderedDict([('console_scripts', OrderedDict([('rai-benchmark', "*

 * *                 "'azureml.rai.utils.llm_eval_benchmark.e2e:main')]))])}",*

 * * "'extras'": "['benchmark']",*

 * * "'run_requires'": "{insert: [(1, OrderedDict([('extra', 'benchmark'), ('requires', "*

 * *                   "['azure-keyvault', 'cli […]*

```diff
@@ -9,30 +9,42 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License"
     ],
     "description_content_type": "text/markdown",
     "extensions": {
+        "python.commands": {
+            "wrap_console": {
+                "rai-benchmark": "azureml.rai.utils.llm_eval_benchmark.e2e:main"
+            }
+        },
         "python.details": {
             "contacts": [
                 {
                     "name": "Microsoft Corporation",
                     "role": "author"
                 }
             ],
             "document_names": {
                 "description": "DESCRIPTION.rst"
             },
             "project_urls": {
                 "Home": "https://github.com/Azure/azureml-examples/tree/main/cli/responsible-ai"
             }
+        },
+        "python.exports": {
+            "console_scripts": {
+                "rai-benchmark": "azureml.rai.utils.llm_eval_benchmark.e2e:main"
+            }
         }
     },
-    "extras": [],
+    "extras": [
+        "benchmark"
+    ],
     "generator": "bdist_wheel (0.30.0)",
     "keywords": [
         "AzureMachineLearning"
     ],
     "license": "MIT License",
     "metadata_version": "2.0",
     "name": "azureml-rai-utils",
@@ -42,12 +54,25 @@
             "requires": [
                 "azure-ai-ml",
                 "azure-identity",
                 "azureml-mlflow",
                 "mlflow",
                 "mltable"
             ]
+        },
+        {
+            "extra": "benchmark",
+            "requires": [
+                "azure-keyvault",
+                "click",
+                "jinja2",
+                "json5",
+                "numpy",
+                "pandas",
+                "scikit-learn",
+                "tiktoken"
+            ]
         }
     ],
     "summary": "Azure Machine Learning Responsible AI Utils SDK",
-    "version": "0.0.3"
+    "version": "0.0.4"
 }
```

## Comparing `azureml_rai_utils-0.0.3.dist-info/METADATA` & `azureml_rai_utils-0.0.4.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-rai-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Azure Machine Learning Responsible AI Utils SDK
 Home-page: https://github.com/Azure/azureml-examples/tree/main/cli/responsible-ai
 Author: Microsoft Corporation
 License: MIT License
 Keywords: AzureMachineLearning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: benchmark
 Requires-Dist: azure-ai-ml
 Requires-Dist: azure-identity
 Requires-Dist: mlflow
 Requires-Dist: azureml-mlflow
 Requires-Dist: mltable
+Provides-Extra: benchmark
+Requires-Dist: click; extra == 'benchmark'
+Requires-Dist: jinja2; extra == 'benchmark'
+Requires-Dist: json5; extra == 'benchmark'
+Requires-Dist: azure-keyvault; extra == 'benchmark'
+Requires-Dist: scikit-learn; extra == 'benchmark'
+Requires-Dist: pandas; extra == 'benchmark'
+Requires-Dist: numpy; extra == 'benchmark'
+Requires-Dist: tiktoken; extra == 'benchmark'
 
 # Azure Machine Learning Responsible AI Utils Python SDK
 
 The `azureml-rai-utils` package provides the SDK interface that works along with the AzureML Responsible AI Dashboard experience.
 
 The [Responsible AI dashboard](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-responsible-ai-dashboard) includes a robust, rich set of visualizations and functionality to help you analyze your machine learning model or make data-driven business decisions:
```

