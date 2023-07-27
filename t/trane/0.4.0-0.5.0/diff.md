# Comparing `tmp/trane-0.4.0.tar.gz` & `tmp/trane-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trane-0.4.0.tar", last modified: Sat Jul  8 21:53:52 2023, max compression
+gzip compressed data, was "trane-0.5.0.tar", last modified: Thu Jul 27 19:25:19 2023, max compression
```

## Comparing `trane-0.4.0.tar` & `trane-0.5.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-08 21:53:36.000000 trane-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-08 21:53:52.792954 trane-0.4.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2875 2023-07-08 21:53:36.000000 trane-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-08 21:53:36.000000 trane-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:53:52.792954 trane-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.788954 trane-0.4.0/trane/
--rwxr-xr-x   0 runner    (1001) docker     (123)      383 2023-07-08 21:53:36.000000 trane-0.4.0/trane/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/core/
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/cutoff_strategy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3123 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/labeler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9443 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8038 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem_evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7909 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/prediction_problem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-08 21:53:36.000000 trane-0.4.0/trane/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 21:53:36.000000 trane-0.4.0/trane/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-08 21:53:36.000000 trane-0.4.0/trane/datasets/load_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/ops/
--rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/aggregation_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2665 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/filter_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2965 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/op_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/threshold_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:36.000000 trane-0.4.0/trane/ops/threshold_functions.test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/typing/
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/1-1000.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/column_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/inference_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-08 21:53:36.000000 trane-0.4.0/trane/typing/logical_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.792954 trane-0.4.0/trane/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      301 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/data_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1861 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/featuretools_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5495 2023-07-08 21:53:36.000000 trane-0.4.0/trane/utils/table_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 21:53:36.000000 trane-0.4.0/trane/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:53:52.788954 trane-0.4.0/trane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:53:52.000000 trane-0.4.0/trane.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.102540 trane-0.5.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1076 2023-07-27 19:25:00.000000 trane-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 19:25:19.102540 trane-0.5.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2875 2023-07-27 19:25:00.000000 trane-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-27 19:25:00.000000 trane-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 19:25:19.102540 trane-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.094539 trane-0.5.0/trane/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      372 2023-07-27 19:25:00.000000 trane-0.5.0/trane/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.098540 trane-0.5.0/trane/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/cutoff_strategy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3099 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/labeler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10017 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/prediction_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8038 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/prediction_problem_evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6971 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/prediction_problem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-27 19:25:00.000000 trane-0.5.0/trane/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.098540 trane-0.5.0/trane/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1957148 2023-07-27 19:25:00.000000 trane-0.5.0/trane/datasets/USvideos.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 19:25:00.000000 trane-0.5.0/trane/datasets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   748996 2023-07-27 19:25:00.000000 trane-0.5.0/trane/datasets/covid19.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-27 19:25:00.000000 trane-0.5.0/trane/datasets/load_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.102540 trane-0.5.0/trane/ops/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4153 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/aggregation_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2651 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/filter_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/op_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/threshold_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/threshold_functions.test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-27 19:25:00.000000 trane-0.5.0/trane/ops/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.102540 trane-0.5.0/trane/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 19:25:00.000000 trane-0.5.0/trane/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-07-27 19:25:00.000000 trane-0.5.0/trane/parsing/denormalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.102540 trane-0.5.0/trane/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/1-1000.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/column_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/inference_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-27 19:25:00.000000 trane-0.5.0/trane/typing/logical_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.102540 trane-0.5.0/trane/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      169 2023-07-27 19:25:00.000000 trane-0.5.0/trane/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2389 2023-07-27 19:25:00.000000 trane-0.5.0/trane/utils/featuretools_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1254 2023-07-27 19:25:00.000000 trane-0.5.0/trane/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 19:25:00.000000 trane-0.5.0/trane/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 19:25:19.094539 trane-0.5.0/trane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-27 19:25:19.000000 trane-0.5.0/trane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-27 19:25:19.000000 trane-0.5.0/trane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 19:25:19.000000 trane-0.5.0/trane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-27 19:25:19.000000 trane-0.5.0/trane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 19:25:19.000000 trane-0.5.0/trane.egg-info/top_level.txt
```

### Comparing `trane-0.4.0/LICENSE` & `trane-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/PKG-INFO` & `trane-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: trane
-Version: 0.4.0
+Version: 0.5.0
 Summary: automatically generate prediction problems and labels for supervised learning.
 Author-email: MIT Data to AI Lab <dai-lab-trane@mit.edu>
 Maintainer-email: MIT Data to AI Lab <dai-lab-trane@mit.edu>
 License: MIT License
-Project-URL: Source Code, https://github.com/HDI-Project/Trane/
-Project-URL: Changes, https://github.com/HDI-Project/Trane/blob/main/docs/changelog.md
-Project-URL: Issue Tracker, https://github.com/HDI-Project/Trane/issues
+Project-URL: Source Code, https://github.com/trane-dev/Trane/
+Project-URL: Changes, https://github.com/trane-dev/Trane/blob/main/docs/changelog.md
+Project-URL: Issue Tracker, https://github.com/trane-dev/Trane/issues
 Project-URL: Twitter, https://twitter.com/lab_dai
+Project-URL: Chat, https://join.slack.com/t/trane-dev/shared_invite/zt-1zglnh25c-ryuQFarw0rVgKHC6ywUOlg
 Keywords: trane,data science,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: trane Version: 0.4.0 Summary: automatically
+Metadata-Version: 2.1 Name: trane Version: 0.5.0 Summary: automatically
 generate prediction problems and labels for supervised learning. Author-email:
 MIT Data to AI Lab
 mit.edu> Maintainer-email: MIT Data to AI Lab
-mit.edu> License: MIT License Project-URL: Source Code, https://github.com/HDI-
-Project/Trane/ Project-URL: Changes, https://github.com/HDI-Project/Trane/blob/
-main/docs/changelog.md Project-URL: Issue Tracker, https://github.com/HDI-
-Project/Trane/issues Project-URL: Twitter, https://twitter.com/lab_dai
-Keywords: trane,data science,machine learning Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS Classifier: License :: OSI Approved ::
-MIT License Classifier: Natural Language :: English Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-dev License-File: LICENSE
+mit.edu> License: MIT License Project-URL: Source Code, https://github.com/
+trane-dev/Trane/ Project-URL: Changes, https://github.com/trane-dev/Trane/blob/
+main/docs/changelog.md Project-URL: Issue Tracker, https://github.com/trane-
+dev/Trane/issues Project-URL: Twitter, https://twitter.com/lab_dai Project-URL:
+Chat, https://join.slack.com/t/trane-dev/shared_invite/zt-1zglnh25c-
+ryuQFarw0rVgKHC6ywUOlg Keywords: trane,data science,machine learning
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Science/Research Classifier: Intended Audience :: Developers Classifier:
+Topic :: Software Development Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Requires-Python: <4,>=3.8 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev License-File: LICENSE
                               [âTrane_Logoâ]
        [Tests] [https://codecov.io/gh/trane-dev/Trane/branch/main/graph/
           badge.svg?token=HafAlYGH8F] [PyPI_Version] [PyPI_Downloads]
 ===============================================================================
     Automatically formulating machine learning tasks for temporal datasets
 Trane is a software package for automatically generating prediction problems
 and generating labels for supervised learning. Trane is a system designed to
```

### Comparing `trane-0.4.0/README.md` & `trane-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/pyproject.toml` & `trane-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -32,25 +32,26 @@
 license = {text = "MIT License"}
 requires-python = ">=3.8,<4"
 dependencies = [
     "numpy >= 1.13.0",
     "pandas >= 0.21.0",
     "scipy >= 1.0.0",
     "composeml >= 0.10.1",
-    "featuretools",
-    "scikit-learn",
-    "tqdm",
-    "ipywidgets",
+    "scikit-learn >= 1.3.0",
+    "tqdm >= 4.65.0",
+    "featuretools >= 1.0.0",
+    "ipywidgets >= 8.0.0",
 ]
 
 [project.urls]
-"Source Code"= "https://github.com/HDI-Project/Trane/"
-"Changes" = "https://github.com/HDI-Project/Trane/blob/main/docs/changelog.md"
-"Issue Tracker" = "https://github.com/HDI-Project/Trane/issues"
+"Source Code"= "https://github.com/trane-dev/Trane/"
+"Changes" = "https://github.com/trane-dev/Trane/blob/main/docs/changelog.md"
+"Issue Tracker" = "https://github.com/trane-dev/Trane/issues"
 "Twitter" = "https://twitter.com/lab_dai"
+"Chat" = "https://join.slack.com/t/trane-dev/shared_invite/zt-1zglnh25c-ryuQFarw0rVgKHC6ywUOlg"
 
 [project.optional-dependencies]
 test = [
     "pytest >= 3.4.2",
     "pytest-cov >= 2.5.1",
     "pytest-xdist >= 3.1.0",
     "pytest-runner >= 2.11.1",
@@ -59,28 +60,30 @@
     "ruff >= 0.0.260" ,
     "black[jupyter] >= 22.12.0",
     "pre-commit == 2.20.0",
 ]
 
 [tool.setuptools]
 include-package-data = true
-license-files = [
-    "LICENSE",
-]
+license-files = ["LICENSE"]
 
 [tool.setuptools.packages.find]
 namespaces = true
 
 [tool.setuptools.package-data]
 "*" = [
     "*.txt",
-    "*.md",
+    "*.csv",
     "README.md",
     "Makefile",
 ]
+"trane" = [
+    "datasets/data/covid19.csv",
+    "datasets/data/USvideos.csv",
+]
 
 [tool.setuptools.exclude-package-data]
 "*" = [
     "* __pycache__",
     "*.py[co]",
 ]
```

### Comparing `trane-0.4.0/trane/core/labeler.py` & `trane-0.5.0/trane/core/labeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-__all__ = ["Labeler"]
-
-
 class Labeler:
     """
     Object for executing prediction problems on data in order
     to generate labels for many prediction problems.
     The execute method performs the labelling operation.
     """
```

### Comparing `trane-0.4.0/trane/core/prediction_problem.py` & `trane-0.5.0/trane/core/prediction_problem.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,33 @@
         self._label_maker = cp.LabelMaker(
             target_dataframe_index=entity_col,
             time_index=time_col,
             labeling_function=self._execute_operations_on_df,
             window_size=window_size,
         )
 
+    def __lt__(self, other):
+        return self.__str__() < (other.__str__())
+
+    def __le__(self, other):
+        return self.__str__() <= (other.__str__())
+
+    def __gt__(self, other):
+        return self.__str__() > (other.__str__())
+
+    def __ge__(self, other):
+        return self.__str__() >= (other.__str__())
+
+    def __hash__(self) -> int:
+        # TODO: why is the opbase hash function not working
+        attributes = ()
+        for op in self.operations:
+            attributes += (type(op), op.column_name, op.threshold)
+        return hash(attributes)
+
     def is_valid(self, table_meta=None):
         """
         Typechecking for operations. Insures that their input and output types
         match. Allows a user to use the problem's existing table_meta, or pass
         in a new one
 
         Parameters
@@ -89,15 +108,15 @@
         if result:
             return True
         return False
 
     def execute(
         self,
         df,
-        num_examples_per_instance,
+        num_examples_per_instance=-1,
         minimum_data=None,
         maximum_data=None,
         gap=None,
         drop_empty=True,
         verbose=True,
         *args,
         **kwargs,
@@ -179,15 +198,14 @@
         description += self._describe_aggop(self.operations[-1])
 
         # cycle through ops, pick out filters and describe them
         filterop_desc_arr = []
         for op in self.operations:
             if issubclass(type(op), FilterOpBase):
                 filterop_desc_arr.append(self._describe_filter(op))
-
         # join filter ops with ands and append to the description
         if len(filterop_desc_arr) > 0:
             description += " and ".join(filterop_desc_arr)
 
         # add the cutoff strategy description if it exists
         if self.cutoff_strategy:
             description += " " + self.cutoff_strategy.description
```

### Comparing `trane-0.4.0/trane/core/prediction_problem_evaluator.py` & `trane-0.5.0/trane/core/prediction_problem_evaluator.py`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/trane/core/prediction_problem_generator.py` & `trane-0.5.0/trane/core/prediction_problem_generator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import copy
-import itertools
 
 from tqdm.notebook import tqdm
 
 from trane.core.prediction_problem import PredictionProblem
-from trane.core.utils import _parse_table_meta, get_semantic_tags
-from trane.ops import aggregation_ops as agg_ops
-from trane.ops import filter_ops
+from trane.core.utils import (
+    _generate_possible_operations,
+    _parse_table_meta,
+    get_semantic_tags,
+)
 from trane.ops.filter_ops import AllFilterOp
 from trane.ops.threshold_functions import get_k_most_frequent
 from trane.typing.column_schema import ColumnSchema
 from trane.typing.inference import infer_table_meta
 from trane.typing.logical_types import (
     Categorical,
     Datetime,
     Integer,
 )
 
-__all__ = ["PredictionProblemGenerator"]
-
 
 class PredictionProblemGenerator:
     """
     Object for generating prediction problems on data.
     """
 
     def __init__(self, df, entity_col, time_col, table_meta=None, cutoff_strategy=None):
@@ -63,17 +62,17 @@
             assert isinstance(column_schema, ColumnSchema)
             assert col in self.df.columns
             assert column_schema.logical_type.dtype == str(self.df[col].dtype)
 
         entity_col_type = self.table_meta[self.entity_col]
         assert entity_col_type.logical_type in [Integer, Categorical]
         if inferred_table_meta is False:
-            assert "index" in entity_col_type.semantic_tags
+            assert "primary_key" in entity_col_type.semantic_tags
         else:
-            self.table_meta[self.entity_col].semantic_tags.add("index")
+            self.table_meta[self.entity_col].semantic_tags.add("primary_key")
 
         time_col_type = self.table_meta[self.time_col]
         assert time_col_type.logical_type == Datetime
 
     def transform_data(self):
         """
         Transform the data to the correct types.
@@ -106,51 +105,31 @@
         Returns
         -------
         problems: a list of Prediction Problem objects.
         """
         if generate_thresholds and df is None:
             raise ValueError("Must provide a dataframe sample to generate thresholds")
 
-        # a list of problems that will eventually be returned
+        exclude_columns = [self.entity_col, self.time_col]
         problems = []
-        all_columns = list(self.table_meta.keys())
+        possible_operations = _generate_possible_operations(
+            table_meta=self.table_meta,
+            exclude_columns=exclude_columns,
+        )
 
-        possible_ops = []
-        for agg, filter_ in itertools.product(
-            agg_ops.AGGREGATION_OPS,
-            filter_ops.FILTER_OPS,
-        ):
-            filter_columns = all_columns
-            if filter_ == "AllFilterOp":
-                filter_columns = [None]
-
-            agg_columns = all_columns
-            if agg == "CountAggregationOp":
-                agg_columns = [None]
-            for filter_col, agg_col in itertools.product(
-                filter_columns,
-                agg_columns,
-            ):
-                if filter_col == self.time_col or agg_col == self.time_col:
-                    continue
-                if filter_col != self.entity_col and agg_col != self.entity_col:
-                    possible_ops.append((agg_col, filter_col, agg, filter_))
-        total_attempts = len(possible_ops)
+        total_attempts = len(possible_operations)
         all_attempts = 0
         success_attempts = 0
         for op_col_combo in tqdm(
-            possible_ops,
+            possible_operations,
             total=total_attempts,
             position=pbar_position,
         ):
             all_attempts += 1
-            ag_col, filter_col, agg_op_name, filter_op_name = op_col_combo
-
-            agg_op_obj = getattr(agg_ops, agg_op_name)(ag_col)  # noqa
-            filter_op_obj = getattr(filter_ops, filter_op_name)(filter_col)  # noqa
+            filter_op_obj, agg_op_obj = op_col_combo
 
             # Note: the order of the operations matters, the filter operation must be first
             operations = [filter_op_obj, agg_op_obj]
 
             problem = PredictionProblem(
                 operations=operations,
                 entity_col=self.entity_col,
```

### Comparing `trane-0.4.0/trane/datasets/load_functions.py` & `trane-0.5.0/trane/datasets/load_functions.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,23 +29,14 @@
     ]
     df = df.fillna(0)
     df = df.sort_values(by=["Date"])
     df = df.reset_index(drop=True)
     return df
 
 
-def load_bike():
-    filepath = generate_local_filepath("bike-sampled.csv")
-    df = pd.read_csv(filepath)
-    df["date"] = pd.to_datetime(df["date"], format="%Y-%m-%d")
-    df = df.sort_values(by=["date"])
-    df = df.fillna(0)
-    return df
-
-
 def load_youtube():
     time_col = "trending_date"
     filepath = generate_local_filepath("USvideos.csv")
     df = pd.read_csv(filepath)
     df[time_col] = pd.to_datetime(df[time_col], format="%y.%d.%m")
     df = df.sort_values(by=[time_col])
     df = df.fillna(0)
@@ -56,15 +47,15 @@
     table_meta = {
         "Province/State": ColumnSchema(
             logical_type=Categorical,
             semantic_tags={"category"},
         ),
         "Country/Region": ColumnSchema(
             logical_type=Categorical,
-            semantic_tags={"category", "index"},
+            semantic_tags={"category", "primary_key"},
         ),
         "Lat": ColumnSchema(logical_type=Double, semantic_tags={"numeric"}),
         "Long": ColumnSchema(logical_type=Double, semantic_tags={"numeric"}),
         "Date": ColumnSchema(logical_type=Datetime),
         "Confirmed": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
         "Deaths": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
         "Recovered": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
@@ -73,49 +64,24 @@
 
 
 def load_youtube_metadata():
     table_meta = {
         "trending_date": ColumnSchema(logical_type=Datetime),
         "channel_title": ColumnSchema(
             logical_type=Categorical,
-            semantic_tags={"index"},
+            semantic_tags={"primary_key"},
         ),
         "category_id": ColumnSchema(
             logical_type=Categorical,
-            semantic_tags={"category", "index"},
+            semantic_tags={"category", "primary_key"},
         ),
         "views": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
         "likes": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
         "dislikes": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
         "comment_count": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
     }
     return table_meta
 
 
-def load_bike_metadata():
-    table_meta = {
-        "date": ColumnSchema(logical_type=Datetime),
-        "hour": ColumnSchema(logical_type=Categorical, semantic_tags={"category"}),
-        "usertype": ColumnSchema(logical_type=Categorical, semantic_tags={"category"}),
-        "gender": ColumnSchema(logical_type=Categorical, semantic_tags={"category"}),
-        "tripduration": ColumnSchema(logical_type=Double, semantic_tags={"numeric"}),
-        "temperature": ColumnSchema(logical_type=Double, semantic_tags={"numeric"}),
-        "from_station_id": ColumnSchema(
-            logical_type=Categorical,
-            semantic_tags={"index"},
-        ),
-        "dpcapacity_start": ColumnSchema(
-            logical_type=Integer,
-            semantic_tags={"numeric"},
-        ),
-        "to_station_id": ColumnSchema(
-            logical_type=Categorical,
-            semantic_tags={"index"},
-        ),
-        "dpcapacity_end": ColumnSchema(logical_type=Integer, semantic_tags={"numeric"}),
-    }
-    return table_meta
-
-
 def generate_local_filepath(key):
     dir_path = os.path.dirname(os.path.realpath(__file__))
     return os.path.join(dir_path, key)
```

### Comparing `trane-0.4.0/trane/ops/aggregation_ops.py` & `trane-0.5.0/trane/ops/aggregation_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,9 @@
 from trane.ops.op_base import OpBase
 
-AGGREGATION_OPS = [
-    "CountAggregationOp",
-    "SumAggregationOp",
-    "AvgAggregationOp",
-    "MaxAggregationOp",
-    "MinAggregationOp",
-    "MajorityAggregationOp",
-]
-
 
 class AggregationOpBase(OpBase):
     """
     Given a dataframe, and column, return 1 value.
 
     Super class for all Aggregation Operations. The class is empty and is
     currently a placeholder for any AggregationOpBase level methods we want to
@@ -46,16 +37,17 @@
     """
     CountAggregation will not be given any columns.
     It will apply to the whole dataslice and return 1 number (integer).
     Basically, its then number of rows in the dataslice.
     So a customer's transactions (within the window_size).
     """
 
-    input_output_types = [(None, "Integer")]
+    input_output_types = [("None", "Integer")]
     description = " the number of records"
+    restricted_semantic_tags = {"time_index", "primary_key"}
 
     def label_function(self, dataslice):
         return len(dataslice)
 
 
 class SumAggregationOp(AggregationOpBase):
     input_output_types = [("numeric", "Double")]
@@ -95,24 +87,36 @@
         if len(dataslice) == 0:
             return None
         return dataslice[self.column_name].min()
 
 
 class MajorityAggregationOp(AggregationOpBase):
     input_output_types = [("category", "category")]
-    # input_output_types = [("category", "category"), ("index", "index")]
+    # input_output_types = [("category", "category"), ("primary_key", "primary_key")]
     description = " the majority <{}> in all related records"
 
     def label_function(self, dataslice):
         if len(dataslice) == 0:
             return None
         return str(dataslice[self.column_name].mode()[0])
 
 
-AGG_OPS = [
-    CountAggregationOp,
-    SumAggregationOp,
-    AvgAggregationOp,
-    MaxAggregationOp,
-    MinAggregationOp,
-    MajorityAggregationOp,
-]
+class ExistsAggregationOp(AggregationOpBase):
+    input_output_types = [("None", "Boolean")]
+    description = " if there exists a record"
+    restricted_semantic_tags = {"time_index", "primary_key"}
+
+    def label_function(self, dataslice):
+        return len(dataslice) > 0
+
+
+# class FirstAggregationOp(AggregationOpBase):
+#     input_output_types = [("category", "category")]
+#     description = " the first <{}> in all related records"
+#     def label_function(self, dataslice):
+#         return dataslice[self.column_name].iloc[0]
+
+# class LastAggregationOp(AggregationOpBase):
+#     input_output_types = [("category", "category")]
+#     description = " the last <{}> in all related records"
+#     def label_function(self, dataslice):
+#         return dataslice[self.column_name].iloc[-1]
```

### Comparing `trane-0.4.0/trane/ops/filter_ops.py` & `trane-0.5.0/trane/ops/filter_ops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,94 +1,82 @@
 import pandas as pd
 
 from trane.ops.op_base import OpBase
 
-FILTER_OPS = [
-    "AllFilterOp",
-    "GreaterFilterOp",
-    "EqFilterOp",
-    "NeqFilterOp",
-    "LessFilterOp",
-]
-
 
 class FilterOpBase(OpBase):
     """
     Super class for all Filter Operations. The class is empty and is currently
     a placeholder for any FilterOpBase level methods we want to make.
 
     Filter operations represent the 1st operation in a prediction problem.
     They filter out rows based on values in the filter_column. Filter
     operations are defined as classes that inherit the FilterOpBase class and
     instantiate the execute method.
 
+    Old, v1 version
     Filter operations filter data
     row operations transform data within a row and return a dataframe of the same dimensions,
     transformation operations transform data across rows and return a new dataset with fewer rows,
     aggregation operations accumulate the dataframe into a single row.
 
+    New, v2 version
+    Filter operations filter data (return a subset of the rows)
+    Aggregation operations aggregate data from many rows into a single row.
+
     """
 
 
 class AllFilterOp(FilterOpBase):
-    input_output_types = [(None, None)]
+    input_output_types = [("None", "None")]
     description = ""
 
     def label_function(self, dataslice):
         if len(dataslice) == 0:
             return pd.NA
         return dataslice
 
 
 class EqFilterOp(FilterOpBase):
     input_output_types = [("category", "category")]
-    # input_output_types = [("category", "category"), ("index", "index")]
+    # input_output_types = [("category", "category"), ("primary_key", "primary_key")]
     description = "equal to"
 
     def set_parameters(self, threshold: float):
         self.threshold = threshold
 
     def label_function(self, dataslice):
         return dataslice[dataslice[self.column_name] == self.threshold]
 
 
 class NeqFilterOp(FilterOpBase):
     input_output_types = [("category", "category")]
-    # input_output_types = [("category", "category"), ("index", "index")]
+    # input_output_types = [("category", "category"), ("primary_key", "primary_key")]
     description = "not equal to"
 
     def set_parameters(self, threshold: float):
         self.threshold = threshold
 
-    def label_function(self, dataframe):
-        return dataframe[dataframe[self.column_name] != self.threshold]
+    def label_function(self, dataslice):
+        return dataslice[dataslice[self.column_name] != self.threshold]
 
 
 class GreaterFilterOp(FilterOpBase):
     input_output_types = [("numeric", "Double")]
     description = "greater than"
 
     def set_parameters(self, threshold: float):
         self.threshold = threshold
 
-    def label_function(self, dataframe):
-        return dataframe[dataframe[self.column_name] > self.threshold]
+    def label_function(self, dataslice):
+        return dataslice[dataslice[self.column_name] > self.threshold]
 
 
 class LessFilterOp(FilterOpBase):
     input_output_types = [("numeric", "Double")]
     description = "less than"
 
     def set_parameters(self, threshold: float):
         self.threshold = threshold
 
-    def label_function(self, dataframe):
-        return dataframe[dataframe[self.column_name] < self.threshold]
-
-
-FILT_OPS = [
-    AllFilterOp,
-    GreaterFilterOp,
-    EqFilterOp,
-    NeqFilterOp,
-    LessFilterOp,
-]
+    def label_function(self, dataslice):
+        return dataslice[dataslice[self.column_name] < self.threshold]
```

### Comparing `trane-0.4.0/trane/ops/op_base.py` & `trane-0.5.0/trane/ops/op_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+from typing import Union
+
 import pandas as pd
 
 from trane.ops.threshold_functions import sample_unique_values
 
-__all__ = ["OpBase"]
+
+class Meta(type):
+    def __repr__(self):
+        return f"{self.__name__}"
 
 
-class OpBase(object):
+class OpBase(object, metaclass=Meta):
     """
     Super class of all operations.
     """
 
     description = None
     threshold = None
+    restricted_semantic_tags = {"time_index", "foreign_key", "primary_key"}
 
     def __init__(self, column_name, input_type=None, output_type=None):
         """
         Initalization of all operations.
         Subclasses shouldn't have their own init.
 
         Parameters
@@ -29,23 +35,49 @@
         None
         """
         self.column_name = column_name
 
     def __call__(self, dataslice):
         return self.label_function(dataslice)
 
+    def __lt__(self, other):
+        return (type(self).__name__) < (type(other).__name__)
+
+    def __le__(self, other):
+        return (type(self).__name__) <= (type(other).__name__)
+
+    def __gt__(self, other):
+        return (type(self).__name__) > (type(other).__name__)
+
+    def __ge__(self, other):
+        return (type(self).__name__) >= (type(other).__name__)
+
+    def __hash__(self):
+        return hash((type(self).__name__, self.column_name, self.threshold))
+
+    def __repr__(self) -> str:
+        if self.column_name is not None:
+            return "{}({})".format(type(self).__name__, self.column_name)
+        return "{}".format(type(self).__name__)
+
+    def __eq__(self, other):
+        """Overrides the default implementation"""
+        if isinstance(self, other.__class__):
+            return self.__dict__ == other.__dict__
+        return False
+
     def label_function(self, dataslice):
         raise NotImplementedError
 
     def generate_description(self):
         if self.description:
             return self.description.format(self.column_name)
         return self.description
 
-    def set_parameters(self, threshold: float):
+    def set_parameters(self, threshold: Union[float, str]):
         raise NotImplementedError
 
     def find_threshold_by_fraction_of_data_to_keep(
         self,
         fraction_of_data_target: float,
         df: pd.DataFrame,
         label_col: str,
@@ -72,24 +104,7 @@
             score = abs(fraction_of_data_left - fraction_of_data_target)
             # minimize the score (reduce the difference)
             if score < best_score:
                 best_score = score
                 best_threshold = unique_val
         self.set_parameters(threshold=original_threshold)
         return best_threshold
-
-    def __hash__(self):
-        return hash((type(self).__name__, self.column_name))
-
-    # def __repr__(self):
-    #     hyper_param_str = ",".join(
-    #         [str(x) for x in list(self.hyper_parameter_settings.values())],
-    #     )
-    #     if len(hyper_param_str) > 0:
-    #         hyper_param_str = "@" + hyper_param_str
-    #     return "%s(%s%s)" % (type(self).__name__, self.column_name, hyper_param_str)
-
-    def __eq__(self, other):
-        """Overrides the default implementation"""
-        if isinstance(self, other.__class__):
-            return self.__dict__ == other.__dict__
-        return False
```

### Comparing `trane-0.4.0/trane/ops/threshold_functions.py` & `trane-0.5.0/trane/ops/threshold_functions.py`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/trane/typing/1-1000.txt` & `trane-0.5.0/trane/typing/1-1000.txt`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/trane/typing/column_schema.py` & `trane-0.5.0/trane/typing/column_schema.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,28 @@
         if isclass(logical_type):
             self.logical_type = logical_type()
         semantic_tags = self._parse_column_tags(semantic_tags)
         self.logical_type = logical_type
         self.semantic_tags = semantic_tags
 
     def __eq__(self, other, deep=True):
-        if self.logical_type != other.logical_type:
+        if not isinstance(other, ColumnSchema):
             return False
-        if self.semantic_tags != other.semantic_tags:
+        if (
+            self.logical_type
+            and other.logical_type
+            and self.logical_type != other.logical_type
+        ):
+            return False
+        if (
+            self.semantic_tags != other.semantic_tags
+            or self.semantic_tags.issubset(other.semantic_tags) is False
+            or other.semantic_tags.issubset(self.semantic_tags) is False
+            or len(self.semantic_tags) != len(other.semantic_tags)
+        ):
             return False
         return True
 
     def __repr__(self):
         msg = "<ColumnSchema"
         if self.logical_type is not None:
             msg += " (Logical Type = {})".format(self.logical_type)
```

### Comparing `trane-0.4.0/trane/typing/inference.py` & `trane-0.5.0/trane/typing/inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,13 +36,21 @@
     }
     for infer_func, column_schema in inference_functions.items():
         if infer_func(series) is True:
             return column_schema
     return ColumnSchema(logical_type=Unknown)
 
 
-def infer_table_meta(df: pd.DataFrame) -> Dict[str, ColumnSchema]:
+def infer_table_meta(
+    df: pd.DataFrame,
+    entity_col=None,
+    time_col=None,
+) -> Dict[str, ColumnSchema]:
     table_meta = {}
     for col in df.columns:
         column_schema = _infer_series_schema(df[col])
         table_meta[col] = column_schema
+    if entity_col:
+        table_meta[entity_col].semantic_tags.add("primary_key")
+    if time_col:
+        table_meta[time_col].semantic_tags.add("time_index")
     return table_meta
```

### Comparing `trane-0.4.0/trane/typing/inference_functions.py` & `trane-0.5.0/trane/typing/inference_functions.py`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/trane/utils/featuretools_wrapper.py` & `trane-0.5.0/trane/utils/featuretools_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,80 @@
-from datetime import timedelta
-
 import featuretools as ft
 import pandas as pd
 
-__all__ = ["FeaturetoolsWrapper"]
 
+def create_unique_ids_df(df, entity_col):
+    unique_entity_ids = df[entity_col].unique()
+    entity_df = pd.Series(unique_entity_ids, name=entity_col).to_frame()
+    return entity_df
 
-class FeaturetoolsWrapper(object):
-    """docstring for FeaturetoolsWrapper."""
 
-    def __init__(self, df, entity_col, time_col, name, logical_types=None):
-        assert name != entity_col
+class FeaturetoolsWrapper(object):
+    def __init__(
+        self,
+        dataframe_name: str,
+        dataframe: pd.DataFrame,
+        entity_col: str,
+        time_col: str,
+        entityset_name,
+        logical_types=None,
+    ):
+        assert dataframe_name != entity_col
 
         self.entity_col = entity_col
-        self.es = ft.EntitySet(id=name)
+        self.es = ft.EntitySet(id=entityset_name)
         self.es = self.es.add_dataframe(
-            dataframe_name=name,
-            dataframe=df,
+            dataframe_name=dataframe_name,
+            dataframe=dataframe,
             time_index=time_col,
             index="__id__",
             make_index=True,
             logical_types=logical_types,
         )
 
-        entity_df = pd.Series(df[entity_col].unique(), name=entity_col).to_frame()
-        # entity_df = pd.DataFrame(
-        #     [[i] for i in set(df[entity_col])],
-        #     columns=[entity_col],
-        # )
+        entity_df = create_unique_ids_df(dataframe, entity_col)
         self.es = self.es.add_dataframe(
             dataframe_name=entity_col,
             dataframe=entity_df,
             index=entity_col,
         )
+        # each entity has multiple values in the base dataframe
+        self.es = self.es.add_relationship(
+            entity_col,
+            entity_col,
+            dataframe_name,
+            entity_col,
+        )
 
-        self.es = self.es.add_relationship(entity_col, entity_col, name, entity_col)
-
-    def compute_features(self, cutoff_strategy, feature_window):
+    def compute_features(
+        self,
+        label_times: pd.DataFrame,
+        agg_primitives=None,
+        trans_primitives=None,
+        max_depth=2,
+        n_jobs=1,
+        verbose=False,
+        max_features=-1,
+    ):
         feature_matrix, features = ft.dfs(
             target_dataframe_name=self.entity_col,
-            cutoff_time=cutoff_strategy,
+            cutoff_time=label_times,
             entityset=self.es,
             cutoff_time_in_index=True,
-            verbose=True,
+            agg_primitives=agg_primitives,
+            trans_primitives=trans_primitives,
+            max_depth=max_depth,
+            n_jobs=n_jobs,
+            max_features=max_features,
+            verbose=verbose,
         )
         return feature_matrix, features
 
     def encode_features(self, feature_matrix, features):
         feature_matrix_encoded, features_encoded = ft.encode_features(
             feature_matrix,
             features,
         )
-        features = feature_matrix_encoded.fillna(0)
-        return feature_matrix_encoded, features_encoded
+        return feature_matrix_encoded.fillna(0), features_encoded
 
-    def get_feature(self, entity_name, cutoff_st):
-        return list(self.features.loc[entity_name, cutoff_st - timedelta(days=1)])
+    # def get_feature(self, entity_name, cutoff_st):
+    #     return list(self.features.loc[entity_name, cutoff_st - timedelta(days=1)])
```

### Comparing `trane-0.4.0/trane/utils/helper.py` & `trane-0.5.0/trane/utils/helper.py`

 * *Files identical despite different names*

### Comparing `trane-0.4.0/trane.egg-info/PKG-INFO` & `trane-0.5.0/trane.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: trane
-Version: 0.4.0
+Version: 0.5.0
 Summary: automatically generate prediction problems and labels for supervised learning.
 Author-email: MIT Data to AI Lab <dai-lab-trane@mit.edu>
 Maintainer-email: MIT Data to AI Lab <dai-lab-trane@mit.edu>
 License: MIT License
-Project-URL: Source Code, https://github.com/HDI-Project/Trane/
-Project-URL: Changes, https://github.com/HDI-Project/Trane/blob/main/docs/changelog.md
-Project-URL: Issue Tracker, https://github.com/HDI-Project/Trane/issues
+Project-URL: Source Code, https://github.com/trane-dev/Trane/
+Project-URL: Changes, https://github.com/trane-dev/Trane/blob/main/docs/changelog.md
+Project-URL: Issue Tracker, https://github.com/trane-dev/Trane/issues
 Project-URL: Twitter, https://twitter.com/lab_dai
+Project-URL: Chat, https://join.slack.com/t/trane-dev/shared_invite/zt-1zglnh25c-ryuQFarw0rVgKHC6ywUOlg
 Keywords: trane,data science,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: trane Version: 0.4.0 Summary: automatically
+Metadata-Version: 2.1 Name: trane Version: 0.5.0 Summary: automatically
 generate prediction problems and labels for supervised learning. Author-email:
 MIT Data to AI Lab
 mit.edu> Maintainer-email: MIT Data to AI Lab
-mit.edu> License: MIT License Project-URL: Source Code, https://github.com/HDI-
-Project/Trane/ Project-URL: Changes, https://github.com/HDI-Project/Trane/blob/
-main/docs/changelog.md Project-URL: Issue Tracker, https://github.com/HDI-
-Project/Trane/issues Project-URL: Twitter, https://twitter.com/lab_dai
-Keywords: trane,data science,machine learning Classifier: Development Status ::
-2 - Pre-Alpha Classifier: Intended Audience :: Science/Research Classifier:
-Intended Audience :: Developers Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS Classifier: License :: OSI Approved ::
-MIT License Classifier: Natural Language :: English Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-dev License-File: LICENSE
+mit.edu> License: MIT License Project-URL: Source Code, https://github.com/
+trane-dev/Trane/ Project-URL: Changes, https://github.com/trane-dev/Trane/blob/
+main/docs/changelog.md Project-URL: Issue Tracker, https://github.com/trane-
+dev/Trane/issues Project-URL: Twitter, https://twitter.com/lab_dai Project-URL:
+Chat, https://join.slack.com/t/trane-dev/shared_invite/zt-1zglnh25c-
+ryuQFarw0rVgKHC6ywUOlg Keywords: trane,data science,machine learning
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
+:: Science/Research Classifier: Intended Audience :: Developers Classifier:
+Topic :: Software Development Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
+Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
+:: English Requires-Python: <4,>=3.8 Description-Content-Type: text/markdown
+Provides-Extra: test Provides-Extra: dev License-File: LICENSE
                               [âTrane_Logoâ]
        [Tests] [https://codecov.io/gh/trane-dev/Trane/branch/main/graph/
           badge.svg?token=HafAlYGH8F] [PyPI_Version] [PyPI_Downloads]
 ===============================================================================
     Automatically formulating machine learning tasks for temporal datasets
 Trane is a software package for automatically generating prediction problems
 and generating labels for supervised learning. Trane is a system designed to
```

### Comparing `trane-0.4.0/trane.egg-info/SOURCES.txt` & `trane-0.5.0/trane.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,26 +11,29 @@
 trane/core/__init__.py
 trane/core/cutoff_strategy.py
 trane/core/labeler.py
 trane/core/prediction_problem.py
 trane/core/prediction_problem_evaluator.py
 trane/core/prediction_problem_generator.py
 trane/core/utils.py
+trane/datasets/USvideos.csv
 trane/datasets/__init__.py
+trane/datasets/covid19.csv
 trane/datasets/load_functions.py
 trane/ops/__init__.py
 trane/ops/aggregation_ops.py
 trane/ops/filter_ops.py
 trane/ops/op_base.py
 trane/ops/threshold_functions.py
 trane/ops/threshold_functions.test.py
+trane/ops/utils.py
+trane/parsing/__init__.py
+trane/parsing/denormalize.py
 trane/typing/1-1000.txt
 trane/typing/__init__.py
 trane/typing/column_schema.py
 trane/typing/inference.py
 trane/typing/inference_functions.py
 trane/typing/logical_types.py
 trane/utils/__init__.py
-trane/utils/data_parser.py
 trane/utils/featuretools_wrapper.py
-trane/utils/helper.py
-trane/utils/table_meta.py
+trane/utils/helper.py
```

