# Comparing `tmp/probatus-2.0.1.tar.gz` & `tmp/probatus-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probatus-2.0.1.tar", last modified: Mon Jun 19 07:44:05 2023, max compression
+gzip compressed data, was "probatus-2.1.0.tar", last modified: Thu Jul 27 14:30:18 2023, max compression
```

## Comparing `probatus-2.0.1.tar` & `probatus-2.1.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-19 07:41:11.000000 probatus-2.0.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-19 07:44:05.726374 probatus-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-19 07:41:11.000000 probatus-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/binning/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/binning/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/feature_elimination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57143 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/feature_elimination/feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/interpret/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/interpret/shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29943 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/metric_volatility/volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/missing_values/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/missing_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/missing_values/imputation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/sample_similarity/resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/es.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/ks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/psi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/sw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/stat_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/probatus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/missing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/scoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/shap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-19 07:41:11.000000 probatus-2.0.1/probatus/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/probatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 07:44:05.000000 probatus-2.0.1/probatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-19 07:41:11.000000 probatus-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:44:05.726374 probatus-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.718374 probatus-2.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.722374 probatus-2.0.1/tests/binning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/binning/test_binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/docs/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/feature_elimination/test_feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/interpret/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/interpret/test_shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/metric_volatility/test_metric_volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/missing_values/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/missing_values/test_imputation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/sample_similarity/test_resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_stat_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/stat_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:44:05.726374 probatus-2.0.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-19 07:41:11.000000 probatus-2.0.1/tests/utils/test_utils_array_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.949736 probatus-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 14:26:30.000000 probatus-2.1.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-27 14:30:18.945737 probatus-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-27 14:26:30.000000 probatus-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.937736 probatus-2.1.0/probatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/binning/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/feature_elimination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67499 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/feature_elimination/feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/interpret/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/interpret/model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/interpret/shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/metric_volatility/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/metric_volatility/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29943 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/metric_volatility/volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/missing_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/missing_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/missing_values/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/sample_similarity/resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/ks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/psi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/sw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/stat_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/probatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/missing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/shap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-27 14:26:30.000000 probatus-2.1.0/probatus/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.941736 probatus-2.1.0/probatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-07-27 14:30:18.000000 probatus-2.1.0/probatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-27 14:30:18.000000 probatus-2.1.0/probatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:30:18.000000 probatus-2.1.0/probatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 14:30:18.000000 probatus-2.1.0/probatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 14:30:18.000000 probatus-2.1.0/probatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-27 14:26:30.000000 probatus-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:30:18.949736 probatus-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.937736 probatus-2.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/binning/test_binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/docs/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/feature_elimination/test_feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/interpret/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/interpret/test_model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/interpret/test_shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/metric_volatility/test_metric_volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/missing_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/missing_values/test_imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/sample_similarity/test_resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/stat_tests/test_distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/stat_tests/test_stat_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/stat_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:30:18.945737 probatus-2.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-07-27 14:26:30.000000 probatus-2.1.0/tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-2.0.1/LICENCE` & `probatus-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/PKG-INFO` & `probatus-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 2.0.1
+Version: 2.1.0
 Summary: Validation of binary classifiers and data used to develop them
-Author-email: "ING Bank N.V." <mateusz.garbacz@ing.com>
+Author-email: "ING Bank N.V." <reinier.koops@ing.com>
 License: Copyright (c) 2020 ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `probatus-2.0.1/README.md` & `probatus-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/__init__.py` & `probatus-2.1.0/probatus/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/binning/__init__.py` & `probatus-2.1.0/probatus/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/binning/binning.py` & `probatus-2.1.0/probatus/binning/binning.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/feature_elimination/__init__.py` & `probatus-2.1.0/probatus/feature_elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/feature_elimination/feature_elimination.py` & `probatus-2.1.0/probatus/feature_elimination/feature_elimination.py`

 * *Files 13% similar despite different names*

```diff
@@ -402,14 +402,15 @@
         self,
         X,
         y,
         sample_weight=None,
         columns_to_keep=None,
         column_names=None,
         groups=None,
+        shap_variance_penalty_factor=None,
         **shap_kwargs,
     ):
         """
         Fits the object with the provided data.
 
         The algorithm starts with the entire dataset, and then sequentially
              eliminates features. If sklearn compatible search CV is passed as clf e.g.
@@ -446,14 +447,20 @@
 
             groups (pd.Series, np.ndarray, list, optional):
                 array-like of shape (n_samples,)
                 Group labels for the samples used while splitting the dataset into train/test set.
                 Only used in conjunction with a "Group" `cv` instance.
                 (e.g. `sklearn.model_selection.GroupKFold`).
 
+            shap_variance_penalty_factor (int or float, optional):
+                Apply aggregation penalty when computing average of shap values for a given feature.
+                Results in a preference for features that have smaller standard deviation of shap
+                values (more coherent shap importance). Recommend value 0.5 - 1.0.
+                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
 
@@ -490,14 +497,27 @@
         if column_names is not None and columns_to_keep is not None:
             if (self.min_features_to_select + len_columns_to_keep) > len(self.column_names):
                 raise ValueError(
                     "Minimum features to select is greater than number of features."
                     "Lower the value for min_features_to_select or number of columns in columns_to_keep"
                 )
 
+        # Check shap_variance_penalty_factor has acceptable value
+        if shap_variance_penalty_factor is None:
+            _shap_variance_penalty_factor = 0
+        elif (
+            isinstance(shap_variance_penalty_factor, float) or isinstance(shap_variance_penalty_factor, int)
+        ) and shap_variance_penalty_factor >= 0:
+            _shap_variance_penalty_factor = shap_variance_penalty_factor
+        else:
+            warnings.warn(
+                "shap_variance_penalty_factor must be None, int or float. " "Setting shap_variance_penalty_factor = 0"
+            )
+            _shap_variance_penalty_factor = 0
+
         self.X, self.column_names = preprocess_data(X, X_name="X", column_names=column_names, verbose=self.verbose)
         self.y = preprocess_labels(y, y_name="y", index=self.X.index, verbose=self.verbose)
         if sample_weight is not None:
             if self.verbose > 0:
                 warnings.warn(
                     "sample_weight is passed only to the fit method of the model, not the evaluation metrics."
                 )
@@ -561,15 +581,17 @@
 
             shap_values = np.vstack([current_result[0] for current_result in results_per_fold])
             scores_train = [current_result[1] for current_result in results_per_fold]
             scores_val = [current_result[2] for current_result in results_per_fold]
 
             # Calculate the shap features with remaining features and features to keep.
 
-            shap_importance_df = calculate_shap_importance(shap_values, remaining_removeable_features)
+            shap_importance_df = calculate_shap_importance(
+                shap_values, remaining_removeable_features, shap_variance_penalty_factor=_shap_variance_penalty_factor
+            )
 
             # Get features to remove
             features_to_remove = self._get_current_features_to_remove(
                 shap_importance_df, columns_to_keep=columns_to_keep
             )
             # Ensures the order of the first list is kept as it was originally,
             # while removing elements which are present in both lists.
@@ -612,15 +634,24 @@
             (pd.DataFrame):
                 DataFrame with results of feature elimination for each round.
         """
         self._check_if_fitted()
 
         return self.report_df
 
-    def fit_compute(self, X, y, sample_weight=None, columns_to_keep=None, column_names=None, **shap_kwargs):
+    def fit_compute(
+        self,
+        X,
+        y,
+        sample_weight=None,
+        columns_to_keep=None,
+        column_names=None,
+        shap_variance_penalty_factor=None,
+        **shap_kwargs,
+    ):
         """
         Fits the object with the provided data.
 
         The algorithm starts with the entire dataset, and then sequentially
              eliminates features. If sklearn compatible search CV is passed as clf e.g.
              [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html),
              [RandomizedSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html)
@@ -648,14 +679,20 @@
                 List of columns to keep. If given, these columns will not be eliminated.
 
             column_names (list of str, optional):
                 List of feature names of the provided samples. If provided it will be used to overwrite the existing
                 feature names. If not provided the existing feature names are used or default feature names are
                 generated.
 
+            shap_variance_penalty_factor (int or float, optional):
+                Apply aggregation penalty when computing average of shap values for a given feature.
+                Results in a preference for features that have smaller standard deviation of shap
+                values (more coherent shap importance). Recommend value 0.5 - 1.0.
+                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
 
@@ -666,42 +703,216 @@
 
         self.fit(
             X,
             y,
             sample_weight=sample_weight,
             columns_to_keep=columns_to_keep,
             column_names=column_names,
+            shap_variance_penalty_factor=shap_variance_penalty_factor,
             **shap_kwargs,
         )
         return self.compute()
 
-    def get_reduced_features_set(self, num_features):
+    def get_reduced_features_set(self, num_features, standard_error_threshold=1.0, return_type="feature_names"):
         """
         Gets the features set after the feature elimination process, for a given number of features.
 
         Args:
-            num_features (int):
-                Number of features in the reduced features set.
+            num_features (int or str):
+                If int: Number of features in the reduced features set.
+                If str: One of the following automatic num feature selection methods supported:
+                    1. best: strictly selects the num_features with the highest model score.
+                    2. best_coherent: For iterations that are within standard_error_threshold of the highest
+                    score, select the iteration with the lowest standard deviation of model score.
+                    3. best_parsimonious: For iterations that are within standard_error_threshold of the
+                    highest score, select the iteration with the fewest features.
+
+            standard_error_threshold (float):
+                If num_features is 'best_coherent' or 'best_parsimonious', this parameter is used.
+
+            return_type:
+                Accepts possible values of 'feature_names', 'support' or 'ranking'. These are defined as:
+                    1. feature_names: returns column names
+                    2. support: returns boolean mask
+                    3. ranking: returns numeric ranking of features
 
         Returns:
             (list of str):
                 Reduced features set.
         """
         self._check_if_fitted()
 
+        if isinstance(num_features, str):
+            best_num_features = self._get_best_num_features(
+                best_method=num_features, standard_error_threshold=standard_error_threshold
+            )
+            if return_type == "feature_names":
+                return self._get_feature_names(best_num_features)
+            elif return_type == "support":
+                feature_names_selected = self._get_feature_names(best_num_features)
+                return self._get_feature_support(feature_names_selected)
+            elif return_type == "ranking":
+                return self._get_feature_ranking()
+
+        elif isinstance(num_features, int):
+            if return_type == "feature_names":
+                return self._get_feature_names(num_features)
+            elif return_type == "support":
+                feature_names_selected = self._get_feature_names(num_features)
+                return self._get_feature_support(feature_names_selected)
+            elif return_type == "ranking":
+                return self._get_feature_ranking()
+
+        else:
+            raise ValueError(
+                "Parameter num_features can be of type int, or of type str with"
+                "possible values of 'best', 'best_coherent' or 'best_parsimonious'"
+            )
+
+    def _get_best_num_features(self, best_method, standard_error_threshold=1.0):
+        """
+        Helper function to identify the best number of features to select as per some automatic
+        feature selection strategy. Strategies supported are:
+            1. best: strictly selects the num_features with the highest model score.
+            2. best_coherent: For iterations that are within standard_error_threshold of the highest
+            score, select the iteration with the lowest standard deviation of model score.
+            3. best_parsimonious: For iterations that are within standard_error_threshold of the
+            highest score, select the iteration with the fewest features.
+
+        Args:
+            best_method (str):
+                Automatic best feature selection strategy. One of "best", "best_coherent" or
+                "best_parsimonious".
+
+            standard_error_threshold (float):
+                Parameter used if best_method is 'best_coherent' or 'best_parsimonious'.
+                Numeric value greater than zero.
+
+        Returns:
+            (int)
+                num_features as per automatic feature selection strategy selected.
+        """
+
+        self._check_if_fitted()
+        shap_report = self.report_df.copy()
+
+        if (isinstance(standard_error_threshold, float) or isinstance(standard_error_threshold, int)) is not True:
+            raise ValueError("Parameter standard_error_threshold must be int or float")
+        elif standard_error_threshold < 0:
+            raise ValueError("Parameter standard_error_threshold must be >= zero.")
+
+        if best_method == "best":
+            shap_report["eval_metric"] = shap_report["val_metric_mean"]
+            best_iteration_idx = shap_report["eval_metric"].argmax()
+            best_num_features = shap_report["num_features"].iloc[best_iteration_idx]
+
+        elif best_method == "best_coherent":
+            shap_report["eval_metric"] = (
+                shap_report["val_metric_mean"] - shap_report["val_metric_std"] * standard_error_threshold
+            )
+            best_iteration_idx = shap_report["eval_metric"].argmax()
+            # Find standard error threshold above which we want to focus
+            best_val_metric_threshold = shap_report["eval_metric"].iloc[best_iteration_idx]
+            # Drop iterations with val_metric below threshold
+            shap_report = shap_report[shap_report["val_metric_mean"] >= best_val_metric_threshold]
+            # Get iteration with smallest val_metric_std
+            best_std_iteration_idx = shap_report["val_metric_std"].argmin()
+            best_num_features = shap_report["num_features"].iloc[best_std_iteration_idx]
+
+        elif best_method == "best_parsimonious":
+            shap_report["eval_metric"] = (
+                shap_report["val_metric_mean"] - shap_report["val_metric_std"] * standard_error_threshold
+            )
+            best_iteration_idx = shap_report["eval_metric"].argmax()
+            # Find standard error threshold above which we want to focus
+            best_val_metric_threshold = shap_report["eval_metric"].iloc[best_iteration_idx]
+            # Drop iterations with val_metric below threshold
+            shap_report = shap_report[shap_report["val_metric_mean"] >= best_val_metric_threshold]
+            # Get iteration with smallest num_features
+            best_parsimonious_iteration_idx = shap_report["num_features"].argmin()
+            best_num_features = shap_report["num_features"].iloc[best_parsimonious_iteration_idx]
+
+        else:
+            raise ValueError(
+                "The parameter best_method can take values of 'best', 'best_coherent' or 'best_parsimonious'"
+            )
+
+        # Log shap_report for users who want to inspect / debug
+        if self.verbose > 50:
+            print(shap_report)
+
+        return best_num_features
+
+    def _get_feature_names(self, num_features):
+        """
+        Helper function that takes num_features and returns the associated list of column/feature names.
+
+        Args:
+            num_features (int):
+                Represents the top N features to get the column names for.
+
+        Returns:
+            (list of feature names)
+                List of the names of the features representing top num_features
+        """
+        self._check_if_fitted()
         if num_features not in self.report_df.num_features.tolist():
             raise (
                 ValueError(
                     f"The provided number of features has not been achieved at any stage of the process. "
                     f"You can select one of the following: {self.report_df.num_features.tolist()}"
                 )
             )
         else:
             return self.report_df[self.report_df.num_features == num_features]["features_set"].values[0]
 
+    def _get_feature_support(self, feature_names_selected):
+        """
+        Helper function that takes feature_names_selected and returns a boolean mask representing the columns
+        that were selected by the RFECV method.
+
+        Args:
+            feature_names_selected (list):
+                Represents the top N features to get the column names for.
+
+        Returns:
+            (list of bools)
+                Boolean mask representing the features selected.
+        """
+        support = [True if col in feature_names_selected else False for col in self.column_names]
+        return support
+
+    def _get_feature_ranking(self):
+        """
+        Returns the feature ranking, such that ranking_[i] corresponds to the ranking position
+        of the i-th feature. Selected (i.e., estimated best) features are assigned rank 1.
+
+        Returns:
+            (list of bools)
+                Boolean mask representing the features selected.
+        """
+
+        flipped_report_df = self.report_df.iloc[::-1]
+
+        # Some features are not eliminated. All have importance of zero (highest importance)
+        features_not_eliminated = flipped_report_df["features_set"].iloc[0]
+        features_not_eliminated_dict = {v: 0 for v in features_not_eliminated}
+
+        # Eliminated features are ranked by shap importance
+        features_eliminated = np.concatenate(flipped_report_df["eliminated_features"].to_numpy())
+        features_eliminated_dict = {int(v): k + 1 for (k, v) in enumerate(features_eliminated)}
+
+        # Combine dicts with rank info
+        features_eliminated_dict.update(features_not_eliminated_dict)
+
+        # Get ranking per the order of columns
+        ranking = [features_eliminated_dict[col] for col in self.column_names]
+
+        return ranking
+
     def plot(self, show=True, **figure_kwargs):
         """
         Generates plot of the model performance for each iteration of feature elimination.
 
         Args:
             show (bool, optional):
                 If True, the plots are showed to the user, otherwise they are not shown. Not showing plot can be useful,
@@ -712,15 +923,15 @@
 
         Returns:
             (plt.axis):
                 Axis containing the performance plot.
         """
         x_ticks = list(reversed(self.report_df["num_features"].tolist()))
 
-        plt.figure(**figure_kwargs)
+        fig = plt.figure(**figure_kwargs)
 
         plt.plot(
             self.report_df["num_features"],
             self.report_df["train_metric_mean"],
             label="Train Score",
         )
         plt.fill_between(
@@ -742,22 +953,21 @@
             alpha=0.3,
         )
 
         plt.xlabel("Number of features")
         plt.ylabel(f"Performance {self.scorer.metric_name}")
         plt.title("Backwards Feature Elimination using SHAP & CV")
         plt.legend(loc="lower left")
-        ax = plt.gca()
-        ax.invert_xaxis()
-        ax.set_xticks(x_ticks)
+        fig.axes[0].invert_xaxis()
+        fig.axes[0].set_xticks(x_ticks)
         if show:
             plt.show()
         else:
             plt.close()
-        return ax
+        return fig
 
 
 class EarlyStoppingShapRFECV(ShapRFECV):
     """
     This class performs Backwards Recursive Feature Elimination, using SHAP feature importance.
 
     This is a child of ShapRFECV which allows early stopping of the training step, this class is compatible with
```

### Comparing `probatus-2.0.1/probatus/interpret/__init__.py` & `probatus-2.1.0/probatus/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/interpret/inspector.py` & `probatus-2.1.0/probatus/interpret/inspector.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/interpret/model_interpret.py` & `probatus-2.1.0/probatus/interpret/model_interpret.py`

 * *Files 11% similar despite different names*

```diff
@@ -102,15 +102,25 @@
                 - 51 - 100 - shows other warnings and prints
                 - above 100 - presents all prints and all warnings (including SHAP warnings).
         """
         self.clf = clf
         self.scorer = get_single_scorer(scoring)
         self.verbose = verbose
 
-    def fit(self, X_train, X_test, y_train, y_test, column_names=None, class_names=None, **shap_kwargs):
+    def fit(
+        self,
+        X_train,
+        X_test,
+        y_train,
+        y_test,
+        column_names=None,
+        class_names=None,
+        shap_variance_penalty_factor=None,
+        **shap_kwargs,
+    ):
         """
         Fits the object and calculates the shap values for the provided datasets.
 
         Args:
             X_train (pd.DataFrame):
                 Dataframe containing training data.
 
@@ -126,14 +136,20 @@
             column_names (None, or list of str, optional):
                 List of feature names for the dataset. If None, then column names from the X_train dataframe are used.
 
             class_names (None, or list of str, optional):
                 List of class names e.g. ['neg', 'pos']. If none, the default ['Negative Class', 'Positive Class'] are
                 used.
 
+            shap_variance_penalty_factor (int or float, optional):
+                Apply aggregation penalty when computing average of shap values for a given feature.
+                Results in a preference for features that have smaller standard deviation of shap
+                values (more coherent shap importance). Recommend value 0.5 - 1.0.
+                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
         """
@@ -228,38 +244,50 @@
             y,
             column_names=column_names,
             class_names=class_names,
             precalc_shap=shap_values,
         )
         return shap_values, expected_value, tdp
 
-    def compute(self, return_scores=False):
+    def compute(self, return_scores=False, shap_variance_penalty_factor=None):
         """
         Computes the DataFrame that presents the importance of each feature.
 
         Args:
             return_scores (bool, optional):
                 Flag indicating whether the method should return the train and test score of the model, together with
                 the model interpretation report. If true, the output of this method is a tuple of DataFrame, float,
                 float.
 
+            shap_variance_penalty_factor (int or float, optional):
+                Apply aggregation penalty when computing average of shap values for a given feature.
+                Results in a preference for features that have smaller standard deviation of shap
+                values (more coherent shap importance). Recommend value 0.5 - 1.0.
+                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
         Returns:
             (pd.DataFrame or tuple(pd.DataFrame, float, float)):
                 Dataframe with SHAP feature importance, or tuple containing the dataframe, train and test scores of the
                 model.
         """
         self._check_if_fitted()
 
         # Compute SHAP importance
         self.importance_df_train = calculate_shap_importance(
-            self.shap_values_train, self.column_names, output_columns_suffix="_train"
+            self.shap_values_train,
+            self.column_names,
+            output_columns_suffix="_train",
+            shap_variance_penalty_factor=shap_variance_penalty_factor,
         )
 
         self.importance_df_test = calculate_shap_importance(
-            self.shap_values_test, self.column_names, output_columns_suffix="_test"
+            self.shap_values_test,
+            self.column_names,
+            output_columns_suffix="_test",
+            shap_variance_penalty_factor=shap_variance_penalty_factor,
         )
 
         # Concatenate the train and test, sort by test set importance and reorder the columns
         self.importance_df = pd.concat([self.importance_df_train, self.importance_df_test], axis=1).sort_values(
             "mean_abs_shap_value_test", ascending=False
         )[
             [
@@ -280,14 +308,15 @@
         X_train,
         X_test,
         y_train,
         y_test,
         column_names=None,
         class_names=None,
         return_scores=False,
+        shap_variance_penalty_factor=None,
         **shap_kwargs,
     ):
         """
         Fits the object and calculates the shap values for the provided datasets.
 
         Args:
             X_train (pd.DataFrame):
@@ -314,14 +343,20 @@
             return_scores (bool, optional):
                 Flag indicating whether the method should return
                 the train and test score of the model,
                 together with the model interpretation report. If true,
                 the output of this method is a tuple of DataFrame, float,
                 float.
 
+            shap_variance_penalty_factor (int or float, optional):
+                Apply aggregation penalty when computing average of shap values for a given feature.
+                Results in a preference for features that have smaller standard deviation of shap
+                values (more coherent shap importance). Recommend value 0.5 - 1.0.
+                Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
 
@@ -333,17 +368,18 @@
         self.fit(
             X_train=X_train,
             X_test=X_test,
             y_train=y_train,
             y_test=y_test,
             column_names=column_names,
             class_names=class_names,
+            shap_variance_penalty_factor=shap_variance_penalty_factor,
             **shap_kwargs,
         )
-        return self.compute()
+        return self.compute(shap_variance_penalty_factor=shap_variance_penalty_factor)
 
     def plot(self, plot_type, target_set="test", target_columns=None, samples_index=None, show=True, **plot_kwargs):
         """
         Plots the appropriate SHAP plot.
 
         Args:
             plot_type (str):
```

### Comparing `probatus-2.0.1/probatus/interpret/shap_dependence.py` & `probatus-2.1.0/probatus/interpret/shap_dependence.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/metric_volatility/__init__.py` & `probatus-2.1.0/probatus/metric_volatility/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/metric_volatility/metric.py` & `probatus-2.1.0/probatus/metric_volatility/metric.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/metric_volatility/utils.py` & `probatus-2.1.0/probatus/metric_volatility/utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/metric_volatility/volatility.py` & `probatus-2.1.0/probatus/metric_volatility/volatility.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/missing_values/__init__.py` & `probatus-2.1.0/probatus/missing_values/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/missing_values/imputation.py` & `probatus-2.1.0/probatus/missing_values/imputation.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/sample_similarity/__init__.py` & `probatus-2.1.0/probatus/sample_similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/sample_similarity/resemblance_model.py` & `probatus-2.1.0/probatus/sample_similarity/resemblance_model.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/__init__.py` & `probatus-2.1.0/probatus/stat_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/ad.py` & `probatus-2.1.0/probatus/stat_tests/ad.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/distribution_statistics.py` & `probatus-2.1.0/probatus/stat_tests/distribution_statistics.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/es.py` & `probatus-2.1.0/probatus/stat_tests/es.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/ks.py` & `probatus-2.1.0/probatus/stat_tests/ks.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/psi.py` & `probatus-2.1.0/probatus/stat_tests/psi.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/sw.py` & `probatus-2.1.0/probatus/stat_tests/sw.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/stat_tests/utils.py` & `probatus-2.1.0/probatus/stat_tests/utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/__init__.py` & `probatus-2.1.0/probatus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/_utils.py` & `probatus-2.1.0/probatus/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/arrayfuncs.py` & `probatus-2.1.0/probatus/utils/arrayfuncs.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/exceptions.py` & `probatus-2.1.0/probatus/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/interface.py` & `probatus-2.1.0/probatus/utils/interface.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/missing_helpers.py` & `probatus-2.1.0/probatus/utils/missing_helpers.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/plots.py` & `probatus-2.1.0/probatus/utils/plots.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/scoring.py` & `probatus-2.1.0/probatus/utils/scoring.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus/utils/shap_helpers.py` & `probatus-2.1.0/probatus/utils/shap_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -152,50 +152,79 @@
     elif isinstance(X, np.ndarray) and len(X.shape) == 2:
         return pd.DataFrame(shap_values, columns=[f"col_{ix}" for ix in range(X.shape[1])])
 
     else:
         raise NotImplementedError("X must be a dataframe or a 2d array")
 
 
-def calculate_shap_importance(shap_values, columns, output_columns_suffix=""):
+def calculate_shap_importance(shap_values, columns, output_columns_suffix="", shap_variance_penalty_factor=None):
     """
     Returns the average shapley value for each column of the dataframe, as well as the average absolute shap value.
 
     Args:
         shap_values (np.array):
             Shap values.
 
         columns (list of str):
             Feature names.
 
         output_columns_suffix (str, optional):
             Suffix to be added at the end of column names in the output.
 
+        shap_variance_penalty_factor (int or float, optional):
+            Apply aggregation penalty when computing average of shap values for a given feature.
+            Results in a preference for features that have smaller standard deviation of shap
+            values (more coherent shap importance). Recommend value 0.5 - 1.0.
+            Formula: penalized_shap_mean = (mean_shap - (std_shap * shap_variance_penalty_factor))
+
     Returns:
         (pd.DataFrame):
             Mean absolute shap values and Mean shap values of features.
 
     """
     # Find average shap importance for neg and pos class
     shap_abs_mean = np.mean(np.abs(shap_values), axis=0)
     shap_mean = np.mean(shap_values, axis=0)
 
+    if shap_variance_penalty_factor is None:
+        _shap_variance_penalty_factor = 0
+    elif (
+        isinstance(shap_variance_penalty_factor, float) or isinstance(shap_variance_penalty_factor, int)
+    ) and shap_variance_penalty_factor >= 0:
+        _shap_variance_penalty_factor = shap_variance_penalty_factor
+    else:
+        warnings.warn(
+            "shap_variance_penalty_factor must be None, int or float. " "Setting shap_variance_penalty_factor = 0"
+        )
+        _shap_variance_penalty_factor = 0
+
+    penalized_shap_abs_mean = np.mean(np.abs(shap_values), axis=0) - (
+        np.std(np.abs(shap_values), axis=0) * _shap_variance_penalty_factor
+    )
+
     # Prepare importance values in a handy df
     importance_df = pd.DataFrame(
         {
             f"mean_abs_shap_value{output_columns_suffix}": shap_abs_mean.tolist(),
             f"mean_shap_value{output_columns_suffix}": shap_mean.tolist(),
+            f"penalized_mean_abs_shap_value{output_columns_suffix}": penalized_shap_abs_mean.tolist(),
         },
         index=columns,
     )
 
     # Set the correct column types
     importance_df[f"mean_abs_shap_value{output_columns_suffix}"] = importance_df[
         f"mean_abs_shap_value{output_columns_suffix}"
     ].astype(float)
     importance_df[f"mean_shap_value{output_columns_suffix}"] = importance_df[
         f"mean_shap_value{output_columns_suffix}"
     ].astype(float)
+    importance_df[f"penalized_mean_abs_shap_value{output_columns_suffix}"] = importance_df[
+        f"penalized_mean_abs_shap_value{output_columns_suffix}"
+    ].astype(float)
+
+    importance_df = importance_df.sort_values(f"penalized_mean_abs_shap_value{output_columns_suffix}", ascending=False)
 
-    importance_df = importance_df.sort_values(f"mean_abs_shap_value{output_columns_suffix}", ascending=False)
+    # Drop penalized column
+    importance_df = importance_df.drop(columns=[f"penalized_mean_abs_shap_value{output_columns_suffix}"])
 
     return importance_df
```

### Comparing `probatus-2.0.1/probatus/utils/warnings.py` & `probatus-2.1.0/probatus/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus.egg-info/PKG-INFO` & `probatus-2.1.0/probatus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 2.0.1
+Version: 2.1.0
 Summary: Validation of binary classifiers and data used to develop them
-Author-email: "ING Bank N.V." <mateusz.garbacz@ing.com>
+Author-email: "ING Bank N.V." <reinier.koops@ing.com>
 License: Copyright (c) 2020 ING Bank N.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `probatus-2.0.1/probatus.egg-info/SOURCES.txt` & `probatus-2.1.0/probatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/probatus.egg-info/requires.txt` & `probatus-2.1.0/probatus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/pyproject.toml` & `probatus-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "probatus"
-version = "2.0.1"
+version = "2.1.0"
 requires-python= ">=3.8"
 description = "Validation of binary classifiers and data used to develop them"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
-    { name = "ING Bank N.V.", email = "mateusz.garbacz@ing.com" }
+    { name = "ING Bank N.V.", email = "reinier.koops@ing.com" }
 ]
 license = { file = "LICENCE" }
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `probatus-2.0.1/tests/binning/test_binning.py` & `probatus-2.1.0/tests/binning/test_binning.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/docs/test_docstring.py` & `probatus-2.1.0/tests/docs/test_docstring.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/docs/test_notebooks.py` & `probatus-2.1.0/tests/docs/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/feature_elimination/test_feature_elimination.py` & `probatus-2.1.0/tests/feature_elimination/test_feature_elimination.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,14 +291,49 @@
         current_num_of_features=5, num_features_to_remove=1, min_num_features_to_keep=5
     )
     assert 4 == ShapRFECV._calculate_number_of_features_to_remove(
         current_num_of_features=5, num_features_to_remove=7, min_num_features_to_keep=1
     )
 
 
+def test_shap_automatic_num_feature_selection():
+    """
+    Test automatic num feature selection methods
+    """
+    X = pd.DataFrame(
+        {
+            "col_1": [1, 0, 1, 0, 1, 0, 1, 0],
+            "col_2": [0, 0, 0, 0, 0, 1, 1, 1],
+            "col_3": [1, 1, 1, 0, 0, 0, 0, 0],
+        }
+    )
+    y = pd.Series([0, 0, 0, 0, 1, 1, 1, 1])
+
+    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
+    shap_elimination = ShapRFECV(
+        clf,
+        random_state=1,
+        step=1,
+        cv=2,
+        scoring="roc_auc",
+        n_jobs=1,
+    )
+    _ = shap_elimination.fit_compute(X, y, approximate=True, check_additivity=False)
+
+    best_features = shap_elimination.get_reduced_features_set(num_features="best")
+    best_coherent_features = shap_elimination.get_reduced_features_set(
+        num_features="best_coherent",
+    )
+    best_parsimonious_features = shap_elimination.get_reduced_features_set(num_features="best_parsimonious")
+
+    assert best_features == ["col_3"]
+    assert best_coherent_features == ["col_1", "col_2", "col_3"]
+    assert best_parsimonious_features == ["col_3"]
+
+
 def test_get_feature_shap_values_per_fold(X, y):
     """
     Test with ShapRFECV with features per fold.
     """
     clf = DecisionTreeClassifier(max_depth=1)
     shap_elimination = ShapRFECV(clf)
     (
@@ -363,14 +398,37 @@
 
     kept_features = list(report.iloc[[report["val_metric_mean"].idxmax() - 1]]["features_set"].to_list()[0])
 
     # Results from the first run
     assert ["f6", "f10", "f12", "f14", "f15", "f17", "f18", "f20"] == kept_features
 
 
+def test_shap_rfe_penalty_factor(X, y):
+    """
+    Test ShapRFECV with shap_variance_penalty_factor
+    """
+    clf = DecisionTreeClassifier(max_depth=1, random_state=1)
+    shap_elimination = ShapRFECV(
+        clf,
+        random_state=1,
+        step=1,
+        cv=2,
+        scoring="roc_auc",
+        n_jobs=1,
+    )
+    shap_elimination = shap_elimination.fit(
+        X, y, shap_variance_penalty_factor=1.0, approximate=True, check_additivity=False
+    )
+
+    report = shap_elimination.compute()
+
+    assert report.shape[0] == 3
+    assert shap_elimination.get_reduced_features_set(1) == ["col_1"]
+
+
 @pytest.mark.skipif(os.environ.get("SKIP_LIGHTGBM") == "true", reason="LightGBM tests disabled")
 def test_complex_dataset(complex_data, complex_lightgbm):
     """
     Test on complex dataset.
     """
     X, y = complex_data
```

### Comparing `probatus-2.0.1/tests/interpret/test_inspector.py` & `probatus-2.1.0/tests/interpret/test_inspector.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/interpret/test_model_interpret.py` & `probatus-2.1.0/tests/interpret/test_model_interpret.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/interpret/test_shap_dependence.py` & `probatus-2.1.0/tests/interpret/test_shap_dependence.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/metric_volatility/test_metric_volatility.py` & `probatus-2.1.0/tests/metric_volatility/test_metric_volatility.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/missing_values/test_imputation.py` & `probatus-2.1.0/tests/missing_values/test_imputation.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/sample_similarity/test_resemblance_model.py` & `probatus-2.1.0/tests/sample_similarity/test_resemblance_model.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/stat_tests/test_distribution_statistics.py` & `probatus-2.1.0/tests/stat_tests/test_distribution_statistics.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/stat_tests/test_stat_tests.py` & `probatus-2.1.0/tests/stat_tests/test_stat_tests.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/stat_tests/test_utils.py` & `probatus-2.1.0/tests/stat_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-2.0.1/tests/utils/test_utils_array_funcs.py` & `probatus-2.1.0/tests/utils/test_utils_array_funcs.py`

 * *Files identical despite different names*

