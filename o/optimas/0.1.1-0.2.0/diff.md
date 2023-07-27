# Comparing `tmp/optimas-0.1.1.tar.gz` & `tmp/optimas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimas-0.1.1.tar", last modified: Fri Jun 16 07:35:09 2023, max compression
+gzip compressed data, was "optimas-0.2.0.tar", last modified: Thu Jul 27 10:43:46 2023, max compression
```

## Comparing `optimas-0.1.1.tar` & `optimas-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.305848 optimas-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 07:35:09.301848 optimas-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-16 07:34:57.000000 optimas-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.297848 optimas-0.1.1/optimas/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/core/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/multitask_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/evaluators/template_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/explorations/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/explorations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/explorations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/gen_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/developer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/ax_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/developer/multitask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/generators/ax/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/ax/service/single_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/generators/random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/sim_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/optimas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 07:34:57.000000 optimas-0.1.1/optimas/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.297848 optimas-0.1.1/optimas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:35:09.000000 optimas-0.1.1/optimas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-16 07:34:57.000000 optimas-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:35:09.305848 optimas-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:34:57.000000 optimas-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:35:09.301848 optimas-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_analyzed_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_ax_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_grid_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_line_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_random_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-16 07:34:57.000000 optimas-0.1.1/tests/test_template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.458181 optimas-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-27 10:43:46.458181 optimas-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-27 10:43:34.000000 optimas-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.450181 optimas-0.2.0/optimas/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.450181 optimas-0.2.0/optimas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/core/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/evaluators/function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/evaluators/multitask_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/evaluators/template_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/explorations/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/explorations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/explorations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/gen_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/generators/ax/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/generators/ax/developer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/developer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/developer/ax_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18514 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/developer/multitask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/generators/ax/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/service/ax_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/service/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/ax/service/single_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/generators/random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/sim_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.454181 optimas-0.2.0/optimas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 10:43:34.000000 optimas-0.2.0/optimas/utils/other.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.450181 optimas-0.2.0/optimas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-27 10:43:46.000000 optimas-0.2.0/optimas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-27 10:43:46.000000 optimas-0.2.0/optimas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:43:46.000000 optimas-0.2.0/optimas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-27 10:43:46.000000 optimas-0.2.0/optimas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 10:43:46.000000 optimas-0.2.0/optimas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 10:43:34.000000 optimas-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:43:46.458181 optimas-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:43:34.000000 optimas-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:43:46.458181 optimas-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_analyzed_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_ax_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_grid_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_line_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_random_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-27 10:43:34.000000 optimas-0.2.0/tests/test_template_evaluator.py
```

### Comparing `optimas-0.1.1/PKG-INFO` & `optimas-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.1.1
+Version: 0.2.0
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optimas-0.1.1/README.md` & `optimas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/core/evaluation.py` & `optimas-0.2.0/optimas/core/evaluation.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/core/parameter.py` & `optimas-0.2.0/optimas/core/parameter.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/core/task.py` & `optimas-0.2.0/optimas/core/task.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/core/trial.py` & `optimas-0.2.0/optimas/core/trial.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/evaluators/base.py` & `optimas-0.2.0/optimas/evaluators/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,42 @@
     """Base class for all evaluators.
 
     Parameters
     ----------
     sim_function : callable
         The simulation function (as defined in libEnsemble) to be used for
         carrying out the evaluations.
+    n_procs : int, optional
+        The number of processes that will be used for each evaluation. By
+        default, ``n_procs=1`` if ``n_gpus`` is not given. Otherwise, the
+        default behavior is to match the number of processes to the number
+        of GPUs, i.e., ``n_procs=n_gpus``.
     n_gpus : int, optional
-        The number of GPUs that will be made available for each evaluation. BY
-        default, 1.
+        The number of GPUs that will be made available for each evaluation. By
+        default, 0.
     """
     def __init__(
         self,
         sim_function: Callable,
-        n_gpus: Optional[int] = 1
+        n_procs: Optional[int] = None,
+        n_gpus: Optional[int] = None
     ) -> None:
         self.sim_function = sim_function
+        # If no resources are specified, use 1 CPU an 0 GPUs.
+        if n_procs is None and n_gpus is None:
+            n_procs = 1
+            n_gpus = 0
+        # If `n_gpus` is given without specifying `n_procs`, match processes
+        # to GPUs.
+        elif n_procs is None:
+            n_procs = n_gpus
+        # If `n_procs` is given without specifying `n_gpus`, do not use GPUs.
+        elif n_gpus is None:
+            n_gpus = 0
+        self._n_procs = n_procs
         self._n_gpus = n_gpus
         self._initialized = False
 
     def get_sim_specs(
         self,
         varying_parameters: List[VaryingParameter],
         objectives: List[Objective],
@@ -51,26 +69,35 @@
                 [(obj.name, float) for obj in objectives]
                 # f is the single float output that LibEnsemble minimizes.
                 + [(par.name, par.dtype) for par in analyzed_parameters]
                 # input parameters
                 + [(var.name, float) for var in varying_parameters]
             ),
             'user': {
+                'n_procs': self._n_procs,
                 'n_gpus': self._n_gpus,
             }
         }
         return sim_specs
 
     def get_libe_specs(self) -> Dict:
         """Get a dictionary with the ``libE_specs`` as expected
         by ``libEnsemble``
         """
         libE_specs = {}
         return libE_specs
 
+    def get_run_params(self) -> Dict:
+        """Return run parameters for this evaluator."""
+        run_params = {
+            'num_procs': self._n_procs,
+            'num_gpus': self._n_gpus
+        }
+        return run_params
+
     def initialize(self) -> None:
         """Initialize the evaluator."""
         if not self._initialized:
             self._initialize()
             self._initialized = True
 
     def _initialize(self) -> None:
```

### Comparing `optimas-0.1.1/optimas/evaluators/multitask_evaluator.py` & `optimas-0.2.0/optimas/evaluators/multitask_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,21 @@
             libE_specs_1['sim_dir_copy_files'] = list(
                 set(libE_specs_1['sim_dir_copy_files'] +
                     libE_specs_2['sim_dir_copy_files'])
             )
         # Use only the combined specs.
         return libE_specs_1
 
+    def get_run_params(self) -> Dict:
+        """Return run parameters for this evaluator."""
+        run_params = {}
+        for task, evaluator in zip(self.tasks, self.task_evaluators):
+            run_params[task.name] = evaluator.get_run_params()
+        return run_params
+
     def _initialize(self) -> None:
         """Initialize the evaluator."""
         if isinstance(self.task_evaluators[0], TemplateEvaluator):
             for task, evaluator in zip(self.tasks, self.task_evaluators):
                 evaluator.app_name = task.name
         for evaluator in self.task_evaluators:
             evaluator.initialize()
```

### Comparing `optimas-0.1.1/optimas/evaluators/template_evaluator.py` & `optimas-0.2.0/optimas/evaluators/template_evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,38 +23,41 @@
         of the objective(s) and other analyzed parameters.
     executable : str, optional.
         Path to the executable that will run the simulation. Only needed if
         the simulation template is not a Python script.
     sim_files : list of str, optional.
         List of files that are needed to carry out the simulation and that
         will be copied to the simulation directory.
+    n_procs : int, optional
+        The number of processes that will be used for each evaluation. By
+        default, ``n_procs=1`` if ``n_gpus`` is not given. Otherwise, the
+        default behavior is to match the number of processes to the number
+        of GPUs, i.e., ``n_procs=n_gpus``.
     n_gpus : int, optional
-        The number of GPUs that will be made available for each simulation. By
-        default, 1.
-    n_proc : int, optional
-        The number of processes that will be made used for each simulation. By
-        default, 1. (Currently unused)
+        The number of GPUs that will be made available for each evaluation. By
+        default, 0.
     """
     def __init__(
         self,
         sim_template: str,
         analysis_func: Callable,
         executable: Optional[str] = None,
         sim_files: Optional[List[str]] = None,
-        n_gpus: Optional[int] = 1,
-        n_proc: Optional[int] = 1
+        n_procs: Optional[int] = None,
+        n_gpus: Optional[int] = None
     ) -> None:
         super().__init__(
             sim_function=run_template_simulation,
-            n_gpus=n_gpus)
+            n_procs=n_procs,
+            n_gpus=n_gpus
+        )
         self.sim_template = sim_template
         self.analysis_func = analysis_func
         self.executable = executable
         self.sim_files = [] if sim_files is None else sim_files
-        self.n_proc = n_proc
         self._app_name = 'sim'
 
     @property
     def app_name(self) -> str:
         return self._app_name
 
     @app_name.setter
@@ -76,24 +79,27 @@
         # Get base sim_specs.
         sim_specs = super().get_sim_specs(varying_parameters, objectives,
                                           analyzed_parameters)
         # Add parameters specific to the template evaluator.
         sim_specs['user']['analysis_func'] = self.analysis_func
         sim_specs['user']['sim_template'] = os.path.basename(self.sim_template)
         sim_specs['user']['app_name'] = self._app_name
-        sim_specs['user']['n_proc'] = self.n_proc
         return sim_specs
 
     def get_libe_specs(self) -> Dict:
         """Get a dictionary with the ``libE_specs`` as expected
         by ``libEnsemble``
         """
         libE_specs = super().get_libe_specs()
-        # Add sim_template and sim_files to the list of files to be copied
-        libE_specs['sim_dir_copy_files'] = [self.sim_template] + self.sim_files
+        # Add sim_template and sim_files to the list of files to be copied.
+        # Use the absolute path to the files to get around a libEnsemble bug
+        # when using a workflow dir.
+        sim_files = [self.sim_template] + self.sim_files
+        sim_files = [os.path.abspath(file) for file in sim_files]
+        libE_specs['sim_dir_copy_files'] = sim_files
         # Force libEnsemble to create a directory for each simulation
         # default value, if not defined
         libE_specs['sim_dirs_make'] = True
         return libE_specs
 
     def _initialize(self) -> None:
         self._register_app()
```

### Comparing `optimas-0.1.1/optimas/explorations/base.py` & `optimas-0.2.0/optimas/explorations/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 import numpy as np
 
 from libensemble.libE import libE
 from libensemble.tools import save_libE_output, add_unique_random_streams
 from libensemble.alloc_funcs.start_only_persistent import only_persistent_gens
 from libensemble.executors.mpi_executor import MPIExecutor
+from libensemble.resources.resources import Resources
+from libensemble.executors.executor import Executor
+from libensemble.logger import LogConfig
 
 from optimas.generators.base import Generator
 from optimas.evaluators.base import Evaluator
 
 
 class Exploration():
     """Base class in charge of launching an exploration (i.e., an optimization
@@ -63,100 +66,114 @@
         libe_comms: Optional[str] = 'local'
     ) -> None:
         self.generator = generator
         self.evaluator = evaluator
         self.max_evals = max_evals
         self.sim_workers = sim_workers
         self.run_async = run_async
-        self.history = self._load_history(history)
         if history_save_period is None:
             self.history_save_period = sim_workers
         else:
             self.history_save_period = history_save_period
         self.exploration_dir_path = exploration_dir_path
         self.libe_comms = libe_comms
+        self._load_history(history)
         self._create_alloc_specs()
         self._create_executor()
         self._initialize_evaluator()
         self._set_default_libe_specs()
 
     def run(self) -> None:
         """Run the exploration."""
         # Set exit criteria to maximum number of evaluations.
         exit_criteria = {'sim_max': self.max_evals}
 
         # Create persis_info.
         persis_info = add_unique_random_streams({}, self.sim_workers + 2)
 
         # If specified, allocate dedicated resources for the generator.
-        if self.generator.dedicated_resources:
+        if self.generator.dedicated_resources and self.generator.use_cuda:
             persis_info['gen_resources'] = 1
+            persis_info['gen_use_gpus'] = True
+        else:
+            self.libE_specs['zero_resource_workers'] = [1]
 
         # Get gen_specs and sim_specs.
-        gen_specs = self.generator.get_gen_specs(self.sim_workers)
+        run_params = self.evaluator.get_run_params()
+        gen_specs = self.generator.get_gen_specs(self.sim_workers, run_params)
         sim_specs = self.evaluator.get_sim_specs(
             self.generator.varying_parameters,
             self.generator.objectives,
             self.generator.analyzed_parameters
         )
 
-        # If provided, incorporate history into generator.
-        if self.history is not None:
-            self.generator.incorporate_history(self.history)
-
         # Launch exploration with libEnsemble.
         history, persis_info, flag = libE(
             sim_specs,
             gen_specs,
             exit_criteria,
             persis_info,
             self.alloc_specs,
             self.libE_specs,
             H0=self.history
         )
 
         # Update history.
         self.history = history
 
+        # Update generator with the one received from libE.
+        self.generator._update(persis_info[1]['generator'])
+
         # Determine if current rank is master.
         if self.libE_specs["comms"] == "local":
             is_master = True
             nworkers = self.sim_workers + 1
         else:
             from mpi4py import MPI
             is_master = (MPI.COMM_WORLD.Get_rank() == 0)
             nworkers = MPI.COMM_WORLD.Get_size() - 1
 
         # Save history.
         if is_master:
-            save_libE_output(history, persis_info, __file__, nworkers)
+            save_libE_output(
+                history, persis_info, __file__, nworkers,
+                dest_path=os.path.abspath(self.exploration_dir_path))
+
+        # Reset state of libEnsemble.
+        self._reset_libensemble()
 
     def _create_executor(self) -> None:
         """Create libEnsemble executor."""
         self.executor = MPIExecutor()
 
     def _initialize_evaluator(self) -> None:
         """Initialize exploration evaluator."""
         self.evaluator.initialize()
 
-    def _load_history(self, history: Union[str, np.ndarray, None]) -> None:
+    def _load_history(
+        self,
+        history: Union[str, np.ndarray, None]
+    ) -> None:
         """Load history file."""
         if isinstance(history, str):
             if os.path.exists(history):
                 # Load array.
                 history = np.load(history)
                 # Only include runs that completed
                 history = history[history['sim_ended']]
             else:
                 raise ValueError(
                     'History file {} does not exist.'.format(history))
         assert history is None or isinstance(history, np.ndarray), (
             'Type {} not valid for `history`'.format(type(history))
         )
-        return history
+        # Incorporate history into generator.
+        if history is not None:
+            self.generator.incorporate_history(history)
+        self.history = history
 
     def _set_default_libe_specs(self) -> None:
         """Set default exploration libe_specs."""
         libE_specs = {}
         # Save H to file every N simulation evaluations
         # default value, if not defined
         libE_specs['save_every_k_sims'] = self.history_save_period
@@ -180,15 +197,17 @@
                     '(Windows) instead.')
         else:
             raise ValueError(
                 "Communication mode '{}'".format(self.libe_comms)
                 + " not recognized. Possible values are 'local' or 'mpi'."
             )
         # Set exploration directory path.
-        libE_specs['ensemble_dir_path'] = self.exploration_dir_path
+        libE_specs['ensemble_dir_path'] = 'evaluations'
+        libE_specs['use_workflow_dir'] = True
+        libE_specs['workflow_dir_path'] = self.exploration_dir_path
 
         # get specs from generator and evaluator
         gen_libE_specs = self.generator.get_libe_specs()
         ev_libE_specs = self.evaluator.get_libe_specs()
         self.libE_specs = {**gen_libE_specs, **ev_libE_specs, **libE_specs}
 
     def _create_alloc_specs(self) -> None:
@@ -196,7 +215,23 @@
         self.alloc_specs = {
             'alloc_f': only_persistent_gens,
             'out': [('given_back', bool)],
             'user': {
                 'async_return': self.run_async
             }
         }
+
+    def _reset_libensemble(self) -> None:
+        """Reset the state of libEnsemble.
+
+        After calling `libE`, some libEnsemble attributes do not come back to
+        their original states. This leads to issues if another `Exploration`
+        run is launched within the same script. This method resets the
+        necessary libEnsemble attributes to their original state.
+        """
+        if Resources.resources is not None:
+            del Resources.resources
+            Resources.resources = None
+        if Executor.executor is not None:
+            del Executor.executor
+            Executor.executor = None
+        LogConfig.config.logger_set = False
```

### Comparing `optimas-0.1.1/optimas/gen_functions.py` & `optimas-0.2.0/optimas/gen_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         if resources.slot_count is None:
             gpu_id = str(gen_specs['user']['gpu_id'])
             os.environ['CUDA_VISIBLE_DEVICES'] = gpu_id
         # If there is a dedicated slot for the generator, use the corresponding
         # GPU. This GPU will only be used for the generator and will not be
         # available for the simulation workers.
         else:
-            resources.set_env_to_slots('CUDA_VISIBLE_DEVICES')
+            resources.set_env_to_gpus('CUDA_VISIBLE_DEVICES')
 
     # Get generator, objectives, and parameters to analyze.
     generator = gen_specs['user']['generator']
     objectives = generator.objectives
     analyzed_parameters = generator.analyzed_parameters
 
     ps = PersistentSupport(libE_info, EVAL_GEN_TAG)
@@ -53,23 +53,27 @@
         for i in range(number_of_gen_points):
             generated_trials = generator.ask(1)
             if generated_trials:
                 trial = generated_trials[0]
                 for var, val in zip(trial.varying_parameters,
                                     trial.parameter_values):
                     H_o[var.name][i] = val
+                run_params = gen_specs['user']['run_params']
                 if 'task' in H_o.dtype.names:
                     H_o['task'][i] = trial.trial_type
+                    run_params = run_params[trial.trial_type]
                 if trial.custom_parameters is not None:
                     for par in trial.custom_parameters:
                         H_o[par.save_name][i] = getattr(trial, par.name)
                 H_o['trial_index'][i] = trial.index
-                H_o['resource_sets'][i] = 1
-        n_failed_gens = np.sum(H_o['resource_sets'] == 0)
-        H_o = H_o[H_o['resource_sets'] > 0]
+                H_o['num_procs'][i] = run_params["num_procs"]
+                H_o['num_gpus'][i] = run_params["num_gpus"]
+
+        n_failed_gens = np.sum(H_o['num_procs'] == 0)
+        H_o = H_o[H_o['num_procs'] > 0]
 
         # Send data and get results from finished simulation
         # Blocking call: waits for simulation results to be sent by the manager
         tag, Work, calc_in = ps.send_recv(H_o)
         if calc_in is not None:
             # Check how many simulations have returned
             n = len(calc_in['sim_id'])
@@ -85,8 +89,12 @@
                 generator.tell([trial])
             # Set the number of points to generate to that number:
             number_of_gen_points = n + n_failed_gens
             n_failed_gens = 0
         else:
             number_of_gen_points = 0
 
+    # Add updated generator to `persis_info`.
+    generator._prepare_to_send()
+    persis_info['generator'] = generator
+
     return H_o, persis_info, FINISHED_PERSISTENT_GEN_TAG
```

### Comparing `optimas-0.1.1/optimas/generators/__init__.py` & `optimas-0.2.0/optimas/generators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from .ax.service.single_fidelity import AxSingleFidelityGenerator
 from .ax.service.multi_fidelity import AxMultiFidelityGenerator
+from .ax.service.ax_client import AxClientGenerator
 from .ax.developer.multitask import AxMultitaskGenerator
 from .grid_sampling import GridSamplingGenerator
 from .line_sampling import LineSamplingGenerator
 from .random_sampling import RandomSamplingGenerator
 
 
 __all__ = ['AxSingleFidelityGenerator', 'AxMultiFidelityGenerator',
-           'AxMultitaskGenerator', 'GridSamplingGenerator',
-           'LineSamplingGenerator', 'RandomSamplingGenerator']
+           'AxMultitaskGenerator', 'AxClientGenerator',
+           'GridSamplingGenerator', 'LineSamplingGenerator',
+           'RandomSamplingGenerator']
```

### Comparing `optimas-0.1.1/optimas/generators/ax/base.py` & `optimas-0.2.0/optimas/generators/ax/base.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/generators/ax/developer/ax_metric.py` & `optimas-0.2.0/optimas/generators/ax/developer/ax_metric.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/generators/ax/developer/multitask.py` & `optimas-0.2.0/optimas/generators/ax/developer/multitask.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,23 +113,25 @@
         self.n_gen_lofi = 0
         self.n_gen_hifi = 0
         self.gen_state = NOT_STARTED
         self.returned_lofi_trials = 0
         self.returned_hifi_trials = 0
         self.init_batch_limit = 1000
         self.current_trial = None
+        self.gr_lofi = None
         self._experiment = self._create_experiment()
 
     def get_gen_specs(
         self,
-        sim_workers: int
+        sim_workers: int,
+        run_params: dict
     ) -> Dict:
         """Get the libEnsemble gen_specs."""
         # Get base specs.
-        gen_specs = super().get_gen_specs(sim_workers)
+        gen_specs = super().get_gen_specs(sim_workers, run_params)
         # Add task to output parameters.
         max_length = max([len(self.lofi_task.name), len(self.hifi_task.name)])
         gen_specs['out'].append(('task', str, max_length))
         return gen_specs
 
     def _check_inputs(
         self,
@@ -435,14 +437,23 @@
         )
         save_experiment(
             experiment=self._experiment,
             filepath=file_path,
             encoder_registry=self._encoder_registry
         )
 
+    def _prepare_to_send(self) -> None:
+        """Prepare generator to send to another process.
+
+        Delete stored generator run. It can contain pytorch tensors that
+        prevent serialization.
+        """
+        del self.gr_lofi
+        self.gr_lofi = None
+
 
 def max_utility_from_GP(
     n: int,
     m: TorchModelBridge,
     gr: GeneratorRun,
     hifi_task: str
 ) -> GeneratorRun:
```

### Comparing `optimas-0.1.1/optimas/generators/ax/service/base.py` & `optimas-0.2.0/optimas/generators/ax/service/single_fidelity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-"""Contains the definition of the base Ax generator using the service API."""
+"""Contains the definition of the single-fidelity Ax generator."""
 
 from typing import List, Optional
 
-import os
-
+import torch
 from ax.service.ax_client import AxClient
-
-from optimas.core import Objective, Trial, VaryingParameter, Parameter
-from optimas.generators.ax.base import AxGenerator
+from ax.modelbridge.generation_strategy import (
+    GenerationStep, GenerationStrategy)
+from ax.modelbridge.registry import Models
+from ax.service.utils.instantiation import ObjectiveProperties
+
+from optimas.core import Objective, VaryingParameter, Parameter
+from .base import AxServiceGenerator
 
 
-class AxServiceGenerator(AxGenerator):
-    """Base class for all Ax generators using the service API.
+class AxSingleFidelityGenerator(AxServiceGenerator):
+    """Generator for performing single-fidelity Bayesian optimization using the
+    Ax service API.
 
     Parameters
     ----------
     varying_parameters : list of VaryingParameter
         List of input parameters to vary.
     objectives : list of Objective
         List of optimization objectives.
@@ -57,63 +61,71 @@
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
     ) -> None:
         super().__init__(
             varying_parameters=varying_parameters,
             objectives=objectives,
             analyzed_parameters=analyzed_parameters,
+            n_init=n_init,
             use_cuda=use_cuda,
             gpu_id=gpu_id,
             dedicated_resources=dedicated_resources,
             save_model=save_model,
             model_save_period=model_save_period,
             model_history_dir=model_history_dir
         )
-        self._n_init = n_init
-        self._ax_client = self._create_ax_client()
 
-    def _ask(
-        self,
-        trials: List[Trial]
-    ) -> List[Trial]:
-        """Fill in the parameter values of the requested trials."""
-        for trial in trials:
-            parameters, trial_id = self._ax_client.get_next_trial()
-            trial.parameter_values = [
-                parameters.get(var.name) for var in self._varying_parameters]
-            trial.ax_trial_id = trial_id
-        return trials
+    def _create_ax_client(self):
+        """Create single-fidelity Ax client."""
+        # Create parameter list.
+        parameters = list()
+        for var in self._varying_parameters:
+            parameters.append(
+                {
+                    'name': var.name,
+                    'type': 'range',
+                    'bounds': [var.lower_bound, var.upper_bound],
+                    # Suppresses warning when the type is not given explicitly
+                    'value_type': var.dtype.__name__
+                }
+            )
+
+        # Make generation strategy:
+        steps = []
+
+        # If there is no past history,
+        # adds Sobol initialization with `n_init` random trials:
+        # if self.history is None:
+        steps.append(
+            GenerationStep(
+                model=Models.SOBOL,
+                num_trials=self._n_init
+            )
+        )
 
-    def _tell(
-        self,
-        trials: List[Trial]
-    ) -> None:
-        """Incorporate evaluated trials into Ax client."""
-        for trial in trials:
-            objective_eval = {}
-            for ev in trial.objective_evaluations:
-                objective_eval[ev.parameter.name] = (ev.value, ev.sem)
-            try:
-                self._ax_client.complete_trial(
-                            trial_index=trial.ax_trial_id,
-                            raw_data=objective_eval
-                )
-            except AttributeError:
-                params = {}
-                for var, value in zip(trial.varying_parameters,
-                                      trial.parameter_values):
-                    params[var.name] = value
-                _, trial_id = self._ax_client.attach_trial(params)
-                self._ax_client.complete_trial(trial_id, objective_eval)
-
-    def _create_ax_client(self) -> AxClient:
-        """Create Ax client (must be implemented by subclasses)"""
-        raise NotImplementedError
-
-    def _save_model_to_file(self) -> None:
-        """Save Ax client to json file."""
-        file_path = os.path.join(
-            self._model_history_dir,
-            'ax_client_at_eval_{}.json'.format(
-                self._n_completed_trials_last_saved)
+        # continue indefinitely with GPEI.
+        steps.append(
+            GenerationStep(
+                model=Models.GPEI,
+                num_trials=-1,
+                model_kwargs={
+                    'torch_dtype': torch.double,
+                    'torch_device': torch.device(self.torch_device)
+                }
+            )
         )
-        self._ax_client.save_to_json_file(file_path)
+
+        gs = GenerationStrategy(steps)
+
+        ax_objectives = {}
+        for obj in self.objectives:
+            ax_objectives[obj.name] = ObjectiveProperties(
+                minimize=obj.minimize)
+
+        # Create client and experiment.
+        ax_client = AxClient(generation_strategy=gs, verbose_logging=False)
+        ax_client.create_experiment(
+            parameters=parameters,
+            objectives=ax_objectives
+        )
+
+        return ax_client
```

### Comparing `optimas-0.1.1/optimas/generators/ax/service/multi_fidelity.py` & `optimas-0.2.0/optimas/generators/ax/service/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/generators/ax/service/single_fidelity.py` & `optimas-0.2.0/optimas/generators/ax/service/ax_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,152 @@
-"""Contains the definition of the single-fidelity Ax generator."""
-
+"""Contains the definition of the Ax generator that uses a custom AxClient."""
 from typing import List, Optional
 
-import torch
 from ax.service.ax_client import AxClient
-from ax.modelbridge.generation_strategy import (
-    GenerationStep, GenerationStrategy)
-from ax.modelbridge.registry import Models
-from ax.service.utils.instantiation import ObjectiveProperties
+from ax.core.objective import MultiObjective
 
 from optimas.core import Objective, VaryingParameter, Parameter
 from .base import AxServiceGenerator
 
 
-class AxSingleFidelityGenerator(AxServiceGenerator):
-    """Generator for performing single-fidelity Bayesian optimization using the
-    Ax service API.
+class AxClientGenerator(AxServiceGenerator):
+    """Bayesian optimization generator with a user-defined ``AxClient``.
+
+    This generator allows the user to provide a custom ``AxClient``,
+    allowing for maximum control of the optimization.
+
+    For this generator there is no need to provide the list of
+    ``varying_parameters`` or ``objectives``. The generator will obtain
+    these parameters directly from the ``AxClient``.
 
     Parameters
     ----------
-    varying_parameters : list of VaryingParameter
-        List of input parameters to vary.
-    objectives : list of Objective
-        List of optimization objectives.
+    ax_client : AxClient
+        The Ax client from which the trials will be generated.
     analyzed_parameters : list of Parameter, optional
         List of parameters to analyze at each trial, but which are not
         optimization objectives. By default ``None``.
-    n_init : int, optional
-        Number of evaluations to perform during the initialization phase using
-        Sobol sampling. By default, ``4``.
-    use_cuda : bool, optional
-        Whether to allow the generator to run on a CUDA GPU. By default
-        ``False``.
     gpu_id : int, optional
         The ID of the GPU in which to run the generator. By default, ``0``.
+        This parameter will only have an effect if any ``GenerationStep`` in
+        the ``AxClient`` uses a GPU.
     dedicated_resources : bool, optional
         Whether to allocated dedicated resources (e.g., the GPU) for the
         generator. These resources will not be available to the
         simulation workers. By default, ``False``.
+        This parameter will only have an effect if any ``GenerationStep`` in
+        the ``AxClient`` uses a GPU.
     save_model : bool, optional
         Whether to save the optimization model (in this case, the Ax client) to
         disk. By default ``True``.
     model_save_period : int, optional
         Periodicity, in number of evaluated Trials, with which to save the
         model to disk. By default, ``5``.
     model_history_dir : str, optional
         Name of the directory in which the model will be saved. By default,
         ``'model_history'``.
+
+    Notes
+    -----
+    If the ``AxClient`` contains ``outcome_constraints``, these will appear in
+    the ``optimas`` log as optimization objectives. They are still being
+    correctly used as constraints by the ``AxClient``, and the optimization
+    will work as expected. This is only an issue on ``optimas``, which fails to
+    properly recognize them because optimization constraints have not yet been
+    implemented.
     """
     def __init__(
         self,
-        varying_parameters: List[VaryingParameter],
-        objectives: List[Objective],
+        ax_client: AxClient,
         analyzed_parameters: Optional[List[Parameter]] = None,
-        n_init: Optional[int] = 4,
-        use_cuda: Optional[bool] = False,
         gpu_id: Optional[int] = 0,
         dedicated_resources: Optional[bool] = False,
         save_model: Optional[bool] = True,
         model_save_period: Optional[int] = 5,
         model_history_dir: Optional[str] = 'model_history',
-    ) -> None:
+    ):
+        varying_parameters = self._get_varying_parameters(ax_client)
+        objectives = self._get_objectives(ax_client)
+        self._add_constraints_to_objectives(objectives, ax_client)
+        use_cuda = self._use_cuda(ax_client)
+        self._ax_client = ax_client
         super().__init__(
             varying_parameters=varying_parameters,
             objectives=objectives,
             analyzed_parameters=analyzed_parameters,
-            n_init=n_init,
             use_cuda=use_cuda,
             gpu_id=gpu_id,
             dedicated_resources=dedicated_resources,
             save_model=save_model,
             model_save_period=model_save_period,
             model_history_dir=model_history_dir
         )
 
-    def _create_ax_client(self):
-        """Create single-fidelity Ax client."""
-        # Create parameter list.
-        parameters = list()
-        for var in self._varying_parameters:
-            parameters.append(
-                {
-                    'name': var.name,
-                    'type': 'range',
-                    'bounds': [var.lower_bound, var.upper_bound],
-                    # Suppresses warning when the type is not given explicitly
-                    'value_type': var.dtype.__name__
-                }
+    def _get_varying_parameters(
+        self,
+        ax_client: AxClient
+    ):
+        """Obtain the list of varying parameters from the AxClient."""
+        varying_parameters = []
+        for _, p in ax_client.experiment.search_space.parameters.items():
+            vp = VaryingParameter(
+                name=p.name,
+                lower_bound=p.lower,
+                upper_bound=p.upper,
+                is_fidelity=p.is_fidelity,
+                fidelity_target_value=p.target_value,
+                dtype=p.python_type
             )
+            varying_parameters.append(vp)
+        return varying_parameters
 
-        # Make generation strategy:
-        steps = []
-
-        # If there is no past history,
-        # adds Sobol initialization with `n_init` random trials:
-        # if self.history is None:
-        steps.append(
-            GenerationStep(
-                model=Models.SOBOL,
-                num_trials=self._n_init
+    def _get_objectives(
+        self,
+        ax_client: AxClient
+    ):
+        """Obtain the list of objectives from the AxClient."""
+        objectives = []
+        ax_objective = ax_client.experiment.optimization_config.objective
+        if isinstance(ax_objective, MultiObjective):
+            ax_objectives = ax_objective.objectives
+        else:
+            ax_objectives = [ax_objective]
+        for ax_obj in ax_objectives:
+            obj = Objective(
+                name=ax_obj.metric_names[0],
+                minimize=ax_obj.minimize
             )
-        )
+            objectives.append(obj)
+        return objectives
 
-        # continue indefinitely with GPEI.
-        steps.append(
-            GenerationStep(
-                model=Models.GPEI,
-                num_trials=-1,
-                model_kwargs={
-                    'torch_dtype': torch.double,
-                    'torch_device': torch.device(self.torch_device)
-                }
+    def _add_constraints_to_objectives(
+        self,
+        objectives: List[Objective],
+        ax_client: AxClient
+    ):
+        """Add outcome constraints in the AxClient to the list of objectives.
+
+        This is currently needed because optimas does not yet have a
+        proper definition of constraints. The constraints will be correctly
+        handled and given to the AxClient, but will appear as objectives
+        in the optimization log.
+        """
+        ax_config = ax_client.experiment.optimization_config
+        for constraint in ax_config.outcome_constraints:
+            objectives.append(
+                Objective(name=constraint.metric.name)
             )
-        )
 
-        gs = GenerationStrategy(steps)
+    def _create_ax_client(self) -> AxClient:
+        """Overrides the base function to simply return the given"""
+        return self._ax_client
 
-        ax_objectives = {}
-        for obj in self.objectives:
-            ax_objectives[obj.name] = ObjectiveProperties(
-                minimize=obj.minimize)
-
-        # Create client and experiment.
-        ax_client = AxClient(generation_strategy=gs, verbose_logging=False)
-        ax_client.create_experiment(
-            parameters=parameters,
-            objectives=ax_objectives
-        )
-
-        return ax_client
+    def _use_cuda(
+        self,
+        ax_client: AxClient
+    ):
+        """Determine whether the AxClient uses CUDA."""
+        for step in ax_client.generation_strategy._steps:
+            if "torch_device" in step.model_kwargs:
+                if step.model_kwargs["torch_device"] == "cuda":
+                    return True
+        return False
```

### Comparing `optimas-0.1.1/optimas/generators/base.py` & `optimas-0.2.0/optimas/generators/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Contains the definition of the base Generator class."""
 
+from __future__ import annotations
 import os
 from typing import List, Dict, Optional
 
 import numpy as np
 
 from optimas.utils.logger import get_logger
+from optimas.utils.other import update_object
 from optimas.gen_functions import persistent_generator
 from optimas.core import (Objective, Trial, Evaluation, VaryingParameter,
                           Parameter, TrialParameter)
 
 logger = get_logger(__name__)
 
 
@@ -237,57 +239,96 @@
             logger.info(
                 'Saved model to file after {} completed trials.'.format(
                     n_completed_trials)
             )
 
     def get_gen_specs(
         self,
-        sim_workers: int
+        sim_workers: int,
+        run_params: dict
     ) -> Dict:
         """Get the libEnsemble gen_specs.
 
         Parameters
         ----------
         sim_workers : int
             Total number of parallel simulation workers.
         """
+        self._prepare_to_send()
         gen_specs = {
             # Generator function.
             'gen_f': self._gen_function,
             # Generator input. This is a RNG, no need for inputs.
             'in': ['sim_id'],
             'persis_in': (
                 ['sim_id', 'trial_index'] +
                 [obj.name for obj in self._objectives] +
                 [par.name for par in self._analyzed_parameters]
             ),
             'out': (
                 [(var.name, var.dtype) for var in self._varying_parameters] +
-                [('resource_sets', int), ('trial_index', int)] +
+                [('num_procs', int), ('num_gpus', int)] +
+                [('trial_index', int)] +
                 [(par.save_name, par.dtype)
                  for par in self._custom_trial_parameters]
             ),
             'user': {
                 # Store the generator itself in gen_specs.
                 'generator': self,
                 # Total max number of sims running concurrently.
                 'gen_batch_size': sim_workers,
                 # Allow generator to run on GPU.
                 'use_cuda': self._use_cuda,
                 # GPU in which to run generator.
-                'gpu_id': self._gpu_id
+                'gpu_id': self._gpu_id,
+                # num of procs and gpus required
+                'run_params': run_params
             }
         }
         return gen_specs
 
     def get_libe_specs(self) -> Dict:
         """Get the libEnsemble libe_specs."""
         libE_specs = {}
         return libE_specs
 
+    def _prepare_to_send(self) -> None:
+        """Prepare generator to send to another process.
+
+        This method is necessary because the generator, when given to
+        libEnsemble, is sent to another process (the process of the generator
+        worker) and then sent back to optimas at the end of the run. In order
+        for it to be sent, the generator must be serialized, and sometimes
+        some of the contents of the generator cannot be serialized. The
+        purpose of this method is to take care of the attributes that prevent
+        serialization, and is always called before the generator is sent
+        to/from libEnsemble.
+
+        It must be implemented by the subclasses, if needed.
+        """
+        pass
+
+    def _update(
+        self,
+        new_generator: Generator
+    ) -> None:
+        """Update generator with the attributes of a newer one.
+
+        This method is only intended to be used internally by an
+        ``Exploration`` after a run is completed. It is needed because the
+        ``Generator`` given to ``libEnsemble`` is passed as a copy to the
+        generator worker and is therefore not updated during the run.
+
+        Parameters
+        ----------
+        new_generator : Generator
+            The newer version of the generator returned in ``persis_info``.
+        """
+        update_object(self, new_generator)
+
     def _ask(
         self,
         trials: List[Trial]
     ) -> List[Trial]:
         """Ask method to be implemented by the Generator subclasses.
 
         Parameters
```

### Comparing `optimas-0.1.1/optimas/generators/grid_sampling.py` & `optimas-0.2.0/optimas/generators/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/generators/line_sampling.py` & `optimas-0.2.0/optimas/generators/line_sampling.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas/generators/random_sampling.py` & `optimas-0.2.0/optimas/generators/random_sampling.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 from optimas.core import Objective, Trial, VaryingParameter, Parameter
 from .base import Generator
 
 
 class RandomSamplingGenerator(Generator):
     """Generator for sampling an n-dimensional space with random distributions.
 
-    This generator uses a random distribution to generate sample of
+    This generator uses a random distribution to generate a sample of
     configurations where to evaluate the given objectives.
 
     Parameters
     ----------
     varying_parameters : list of VaryingParameter
         List of input parameters to vary.
     objectives : list of Objective
         List of optimization objectives.
     distribution : {'uniform', 'normal'}, optional
-        The random distribution to use. By default, ``'uniform'``.
+        The random distribution to use. The ``'uniform'`` option draws samples
+        from a uniform distribution within the lower :math:`l_b` and upper
+        :math:`u_b` bounds of each parameter. The ``'normal'`` option draws
+        samples from a normal distribution that, for each parameter, is
+        centered at :math:`c = l_b - u_b` with standard deviation
+        :math:`\\sigma = u_b - c`. By default, ``'uniform'``.
     seed : int, optional
         Seed to initialize the random generator.
     analyzed_parameters : list of Parameter, optional
         List of parameters to analyze at each trial, but which are not
         optimization objectives. By default ``None``.
     """
     def __init__(
```

### Comparing `optimas-0.1.1/optimas/post_processing.py` & `optimas-0.2.0/optimas/post_processing.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/optimas.egg-info/PKG-INFO` & `optimas-0.2.0/optimas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimas
-Version: 0.1.1
+Version: 0.2.0
 Summary: Optimization at scale, powered by libEnsemble
 Author-email: Optimas Developers <angel.ferran.pousa@desy.de>
 License: BSD-3-Clause-LBNL
 Project-URL: Documentation, https://optimas.readthedocs.io/
 Keywords: optimization,scale,bayesian
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `optimas-0.1.1/optimas.egg-info/SOURCES.txt` & `optimas-0.2.0/optimas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,21 @@
 optimas/generators/random_sampling.py
 optimas/generators/ax/__init__.py
 optimas/generators/ax/base.py
 optimas/generators/ax/developer/__init__.py
 optimas/generators/ax/developer/ax_metric.py
 optimas/generators/ax/developer/multitask.py
 optimas/generators/ax/service/__init__.py
+optimas/generators/ax/service/ax_client.py
 optimas/generators/ax/service/base.py
 optimas/generators/ax/service/multi_fidelity.py
 optimas/generators/ax/service/single_fidelity.py
 optimas/utils/__init__.py
 optimas/utils/logger.py
+optimas/utils/other.py
 tests/test_analyzed_parameters.py
 tests/test_ax_generators.py
 tests/test_function_evaluator.py
 tests/test_grid_sampling.py
 tests/test_line_sampling.py
 tests/test_random_sampling.py
 tests/test_template_evaluator.py
```

### Comparing `optimas-0.1.1/pyproject.toml` & `optimas-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
-    'libensemble == 0.9.3',
+    'libensemble >= 0.10.2',
     'jinja2',
     'ax-platform >= 0.2.9',
     'mpi4py',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
```

### Comparing `optimas-0.1.1/tests/test_analyzed_parameters.py` & `optimas-0.2.0/tests/test_analyzed_parameters.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/tests/test_ax_generators.py` & `optimas-0.2.0/tests/test_ax_generators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
+from ax.service.ax_client import AxClient, ObjectiveProperties
+from ax.utils.measurement.synthetic_functions import hartmann6
 
 from optimas.explorations import Exploration
 from optimas.generators import (
-    AxSingleFidelityGenerator, AxMultiFidelityGenerator, AxMultitaskGenerator)
+    AxSingleFidelityGenerator, AxMultiFidelityGenerator, AxMultitaskGenerator,
+    AxClientGenerator)
 from optimas.evaluators import FunctionEvaluator, MultitaskEvaluator
 from optimas.core import VaryingParameter, Objective, Task
 
 
 def eval_func_sf(input_params, output_params):
     """Evaluation function for single-fidelity test"""
     x0 = input_params['x0']
@@ -21,14 +24,21 @@
     x1 = input_params['x1']
     resolution = input_params['res']
     result = -((x0 + 10 * np.cos(x0 + 0.1 * resolution)) *
                (x1 + 5 * np.cos(x1 - 0.2 * resolution)))
     output_params['f'] = result
 
 
+def eval_func_ax_client(input_params, output_params):
+    """Evaluation function for the AxClient test"""
+    x = np.array([input_params.get(f"x{i+1}") for i in range(6)])
+    output_params['hartmann6'] = hartmann6(x)
+    output_params['l2norm'] = np.sqrt((x ** 2).sum())
+
+
 def eval_func_task_1(input_params, output_params):
     """Evaluation function for task1 in multitask test"""
     x0 = input_params['x0']
     x1 = input_params['x1']
     result = -(x0 + 10 * np.cos(x0)) * (x1 + 5 * np.cos(x1))
     output_params['f'] = result
 
@@ -38,15 +48,18 @@
     x0 = input_params['x0']
     x1 = input_params['x1']
     result = - 0.5 * (x0 + 10 * np.cos(x0)) * (x1 + 5 * np.cos(x1))
     output_params['f'] = result
 
 
 def test_ax_single_fidelity():
-    """Test that an exploration with a single-fidelity generator runs"""
+    """
+    Test that an exploration with a single-fidelity generator runs
+    and that the generator and Ax client are updated after running.
+    """
 
     var1 = VaryingParameter('x0', -50., 5.)
     var2 = VaryingParameter('x1', -5., 15.)
     obj = Objective('f', minimize=False)
 
     gen = AxSingleFidelityGenerator(varying_parameters=[var1, var2], objectives=[obj])
     ev = FunctionEvaluator(function=eval_func_sf)
@@ -54,16 +67,27 @@
         generator=gen,
         evaluator=ev,
         max_evals=10,
         sim_workers=2,
         exploration_dir_path='./tests_output/test_ax_single_fidelity'
     )
 
+    # Get reference to original AxClient.
+    ax_client = gen._ax_client
+
+    # Run exploration.
     exploration.run()
 
+    # Check that the generator has been updated.
+    assert len(gen._trials) == exploration.history.shape[0]
+
+    # Check that the original ax client has been updated.
+    n_ax_trials = ax_client.get_trials_data_frame().shape[0]
+    assert n_ax_trials == exploration.history.shape[0]
+
     # Save history for later restart test
     np.save('./tests_output/ax_sf_history' , exploration.history)
 
 
 def test_ax_multi_fidelity():
     """Test that an exploration with a multifidelity generator runs"""
 
@@ -122,14 +146,73 @@
 
     exploration.run()
 
     # Save history for later restart test
     np.save('./tests_output/ax_mt_history' , exploration.history)
 
 
+def test_ax_client():
+    """Test that an exploration with a user-given AxClient runs"""
+    # Create the AxClient from https://ax.dev/tutorials/gpei_hartmann_service.html.
+    ax_client = AxClient()
+    ax_client.create_experiment(
+        name="hartmann_test_experiment",
+        parameters=[
+            {
+                "name": "x1",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+            {
+                "name": "x2",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+            {
+                "name": "x3",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+            {
+                "name": "x4",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+            {
+                "name": "x5",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+            {
+                "name": "x6",
+                "type": "range",
+                "bounds": [0.0, 1.0],
+            },
+        ],
+        objectives={
+            "hartmann6": ObjectiveProperties(minimize=True),
+            },
+        parameter_constraints=["x1 + x2 <= 2.0"],  # Optional.
+        outcome_constraints=["l2norm <= 1.25"],  # Optional.
+    )
+
+    gen = AxClientGenerator(ax_client=ax_client)
+    ev = FunctionEvaluator(function=eval_func_ax_client)
+    exploration = Exploration(
+        generator=gen,
+        evaluator=ev,
+        max_evals=6,
+        sim_workers=2,
+        run_async=False,
+        exploration_dir_path='./tests_output/test_ax_client'
+    )
+
+    exploration.run()
+
+
 def test_ax_single_fidelity_with_history():
     """
     Test that an exploration with a single-fidelity generator runs when
     restarted from a history file
     """
 
     var1 = VaryingParameter('x0', -50., 5.)
@@ -216,10 +299,11 @@
     exploration.run()
 
 
 if __name__ == '__main__':
     test_ax_single_fidelity()
     test_ax_multi_fidelity()
     test_ax_multitask()
+    test_ax_client()
     test_ax_single_fidelity_with_history()
     test_ax_multi_fidelity_with_history()
     test_ax_multitask_with_history()
```

### Comparing `optimas-0.1.1/tests/test_function_evaluator.py` & `optimas-0.2.0/tests/test_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `optimas-0.1.1/tests/test_grid_sampling.py` & `optimas-0.2.0/tests/test_grid_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         n_steps=n_steps
     )
     ev = FunctionEvaluator(function=eval_func)
     exploration = Exploration(
         generator=gen,
         evaluator=ev,
         max_evals=n_evals,
-        sim_workers=4,
+        sim_workers=2,
         exploration_dir_path='./tests_output/test_grid_sampling'
     )
     exploration.run()
 
     # Get generated points.
     h = exploration.history
     h = h[h['sim_ended']]
```

### Comparing `optimas-0.1.1/tests/test_line_sampling.py` & `optimas-0.2.0/tests/test_line_sampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         n_steps=n_steps
     )
     ev = FunctionEvaluator(function=eval_func)
     exploration = Exploration(
         generator=gen,
         evaluator=ev,
         max_evals=n_evals,
-        sim_workers=4,
+        sim_workers=2,
         exploration_dir_path='./tests_output/test_line_sampling'
     )
     exploration.run()
 
     # Get generated points.
     h = exploration.history
     h = h[h['sim_ended']]
```

### Comparing `optimas-0.1.1/tests/test_random_sampling.py` & `optimas-0.2.0/tests/test_random_sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         seed=1
     )
     ev = FunctionEvaluator(function=eval_func)
     exploration = Exploration(
         generator=gen,
         evaluator=ev,
         max_evals=n_evals,
-        sim_workers=4,
+        sim_workers=2,
         exploration_dir_path='./tests_output/test_uniform_sampling'
     )
     exploration.run()
 
     # Get generated points.
     h = exploration.history
     h = h[h['sim_ended']]
@@ -98,15 +98,15 @@
         seed=1
     )
     ev = FunctionEvaluator(function=eval_func)
     exploration = Exploration(
         generator=gen,
         evaluator=ev,
         max_evals=n_evals,
-        sim_workers=4,
+        sim_workers=2,
         exploration_dir_path='./tests_output/test_normal_sampling'
     )
     exploration.run()
 
     # Get generated points.
     h = exploration.history
     h = h[h['sim_ended']]
```

### Comparing `optimas-0.1.1/tests/test_template_evaluator.py` & `optimas-0.2.0/tests/test_template_evaluator.py`

 * *Files identical despite different names*

