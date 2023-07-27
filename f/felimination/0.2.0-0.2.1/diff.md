# Comparing `tmp/felimination-0.2.0.tar.gz` & `tmp/felimination-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felimination-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "felimination-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `felimination-0.2.0.tar` & `felimination-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     2167 2023-07-26 14:04:29.525784 felimination-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/__init__.py
--rw-r--r--   0        0        0    27093 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/drift.py
--rw-r--r--   0        0        0     3863 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/importance.py
--rw-r--r--   0        0        0    31512 2023-07-26 14:04:29.525784 felimination-0.2.0/felimination/rfe.py
--rw-r--r--   0        0        0     1413 2023-07-26 14:04:29.525784 felimination-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2167 2023-07-27 10:25:16.375560 felimination-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 10:25:16.375560 felimination-0.2.1/felimination/__init__.py
+-rw-r--r--   0        0        0    27098 2023-07-27 10:25:16.375560 felimination-0.2.1/felimination/drift.py
+-rw-r--r--   0        0        0     3863 2023-07-27 10:25:16.379560 felimination-0.2.1/felimination/importance.py
+-rw-r--r--   0        0        0    31517 2023-07-27 10:25:16.379560 felimination-0.2.1/felimination/rfe.py
+-rw-r--r--   0        0        0      249 2023-07-27 10:25:16.379560 felimination-0.2.1/felimination/utils/parallel.py
+-rw-r--r--   0        0        0     1413 2023-07-27 10:25:16.379560 felimination-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 felimination-0.2.1/PKG-INFO
```

### Comparing `felimination-0.2.0/README.md` & `felimination-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `felimination-0.2.0/felimination/drift.py` & `felimination-0.2.1/felimination/drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 
 import numpy as np
 from joblib import effective_n_jobs
 from sklearn.base import ClassifierMixin, clone
 from sklearn.metrics import check_scoring
 from sklearn.model_selection import check_cv
 from sklearn.utils._tags import _safe_tags
-from sklearn.utils.parallel import Parallel, delayed
 
 from felimination.importance import PermutationImportance
+from felimination.utils.parallel import Parallel, delayed
 from felimination.rfe import FeliminationRFECV, _train_score_get_importance
 
 
 class SampleSimilarityDriftRFE(FeliminationRFECV):
     """Recursively discards the features that introduce the highest drift.
 
     The algorithm of feature selection goes as follows:
```

### Comparing `felimination-0.2.0/felimination/importance.py` & `felimination-0.2.1/felimination/importance.py`

 * *Files identical despite different names*

### Comparing `felimination-0.2.0/felimination/rfe.py` & `felimination-0.2.1/felimination/rfe.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from sklearn.feature_selection import RFE
 from sklearn.linear_model._logistic import LogisticRegression
 from sklearn.metrics import check_scoring
 from sklearn.model_selection import check_cv, cross_validate
 from sklearn.model_selection._validation import _score
 from sklearn.utils import safe_sqr
 from sklearn.utils.metaestimators import _safe_split
-from sklearn.utils.parallel import Parallel, delayed
 from sklearn.utils.validation import check_is_fitted
 
 from felimination.importance import PermutationImportance
+from felimination.utils.parallel import Parallel, delayed
 
 
 def _train_score_get_importance(
     estimator, X, y, train, test, scorer, importance_getter
 ):
     """
     Train and test an estimator and get the feature importances.
```

### Comparing `felimination-0.2.0/pyproject.toml` & `felimination-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "felimination"
 description = "This library contains some useful scikit-learn compatible classes for feature selection."
-version = "0.2.0"
+version = "0.2.1"
 keywords = ["feature selection", "scikit-learn", "machine learning"]
 authors = [
     { name = "Claudio Salvatore Arcidiacono", email = "author@email.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `felimination-0.2.0/PKG-INFO` & `felimination-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felimination
-Version: 0.2.0
+Version: 0.2.1
 Summary: This library contains some useful scikit-learn compatible classes for feature selection.
 Keywords: feature selection,scikit-learn,machine learning
 Author-email: Claudio Salvatore Arcidiacono <author@email.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

