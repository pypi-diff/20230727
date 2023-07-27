# Comparing `tmp/pysigma_backend_sentinelone_pq-0.1.0.tar.gz` & `tmp/pysigma_backend_sentinelone_pq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_sentinelone_pq-0.1.0.tar", max compression
+gzip compressed data, was "pysigma_backend_sentinelone_pq-0.1.1.tar", max compression
```

## Comparing `pysigma_backend_sentinelone_pq-0.1.0.tar` & `pysigma_backend_sentinelone_pq-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/LICENSE
--rw-r--r--   0        0        0      583 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/sigma/backends/sentinelone/__init__.py
--rw-r--r--   0        0        0     5684 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/sigma/backends/sentinelone/sentinelone_pq.py
--rw-r--r--   0        0        0      120 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/sigma/pipelines/sentinelone/__init__.py
--rw-r--r--   0        0        0    15088 2023-07-27 19:22:43.505724 pysigma_backend_sentinelone_pq-0.1.0/sigma/pipelines/sentinelone/sentinelone_pq.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone_pq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/LICENSE
+-rw-r--r--   0        0        0      592 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/sigma/backends/sentinelone_pq/__init__.py
+-rw-r--r--   0        0        0     5687 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/sigma/backends/sentinelone_pq/sentinelone_pq.py
+-rw-r--r--   0        0        0      120 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/sigma/pipelines/sentinelone_pq/__init__.py
+-rw-r--r--   0        0        0    15088 2023-07-27 20:49:20.221072 pysigma_backend_sentinelone_pq-0.1.1/sigma/pipelines/sentinelone_pq/sentinelone_pq.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone_pq-0.1.1/PKG-INFO
```

### Comparing `pysigma_backend_sentinelone_pq-0.1.0/LICENSE` & `pysigma_backend_sentinelone_pq-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_sentinelone_pq-0.1.0/pyproject.toml` & `pysigma_backend_sentinelone_pq-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pySigma-backend-sentinelone-pq"
-version = "0.1.0"
-description = "pySigma SentinelOne PQ backend"
+version = "0.1.1"
+description = "pySigma SentinelOne PowerQuery backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-sentinelone-pq"
 packages = [
     { include = "sigma" }
 ]
 
@@ -18,8 +18,8 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pysigma_backend_sentinelone_pq-0.1.0/sigma/backends/sentinelone/sentinelone_pq.py` & `pysigma_backend_sentinelone_pq-0.1.1/sigma/backends/sentinelone_pq/sentinelone_pq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sigma.conversion.state import ConversionState
 from sigma.rule import SigmaRule
 from sigma.processing.pipeline import ProcessingPipeline
 from sigma.conversion.base import TextQueryBackend
 from sigma.conditions import ConditionItem, ConditionAND, ConditionOR, ConditionNOT, ConditionFieldEqualsValueExpression
 from sigma.types import SigmaCompareExpression, SigmaRegularExpression, SigmaString
-from sigma.pipelines.sentinelone import sentinelonepq_pipeline
+from sigma.pipelines.sentinelone_pq import sentinelonepq_pipeline
 from sigma.conversion.deferred import DeferredQueryExpression
 import re
 from typing import ClassVar, Dict, Tuple, Pattern, List, Any, Union
 
 class SentinelOnePQBackend(TextQueryBackend):
     """SentinelOne PowerQuery backend."""
```

### Comparing `pysigma_backend_sentinelone_pq-0.1.0/sigma/pipelines/sentinelone/sentinelone_pq.py` & `pysigma_backend_sentinelone_pq-0.1.1/sigma/pipelines/sentinelone_pq/sentinelone_pq.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_sentinelone_pq-0.1.0/PKG-INFO` & `pysigma_backend_sentinelone_pq-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-sentinelone-pq
-Version: 0.1.0
-Summary: pySigma SentinelOne PQ backend
+Version: 0.1.1
+Summary: pySigma SentinelOne PowerQuery backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-sentinelone-pq
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

