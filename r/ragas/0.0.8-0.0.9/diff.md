# Comparing `tmp/ragas-0.0.8.tar.gz` & `tmp/ragas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.8.tar", last modified: Thu Jul 27 10:37:28 2023, max compression
+gzip compressed data, was "ragas-0.0.9.tar", last modified: Thu Jul 27 14:49:21 2023, max compression
```

## Comparing `ragas-0.0.8.tar` & `ragas-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:16.000000 ragas-0.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.786830 ragas-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 10:37:16.000000 ragas-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-27 10:37:16.000000 ragas-0.0.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-27 10:37:16.000000 ragas-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 10:37:16.000000 ragas-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-27 10:37:16.000000 ragas-0.0.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 10:37:28.794830 ragas-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-27 10:37:16.000000 ragas-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/assets/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/guides/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/guides/llms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    62497 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.786830 ragas-0.0.8/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 10:37:16.000000 ragas-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 10:37:16.000000 ragas-0.0.8/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 10:37:16.000000 ragas-0.0.8/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 10:37:16.000000 ragas-0.0.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:37:28.794830 ragas-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/critique.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/faithfulnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:06.000000 ragas-0.0.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.032121 ragas-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.036121 ragas-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 14:49:06.000000 ragas-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-27 14:49:06.000000 ragas-0.0.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-27 14:49:06.000000 ragas-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 14:49:06.000000 ragas-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-27 14:49:06.000000 ragas-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 14:49:21.044122 ragas-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-27 14:49:06.000000 ragas-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.036121 ragas-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/assets/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/guides/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/guides/llms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-27 14:49:06.000000 ragas-0.0.9/docs/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    62497 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.036121 ragas-0.0.9/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 14:49:06.000000 ragas-0.0.9/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 14:49:06.000000 ragas-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 14:49:06.000000 ragas-0.0.9/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 14:49:06.000000 ragas-0.0.9/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 14:49:06.000000 ragas-0.0.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:49:21.044122 ragas-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.036121 ragas-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.040122 ragas-0.0.9/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 14:49:20.000000 ragas-0.0.9/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/critique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/faithfulnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-27 14:49:06.000000 ragas-0.0.9/src/ragas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 14:49:21.000000 ragas-0.0.9/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-27 14:49:21.000000 ragas-0.0.9/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:49:21.000000 ragas-0.0.9/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 14:49:21.000000 ragas-0.0.9/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 14:49:21.000000 ragas-0.0.9/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/e2e/test_fullflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:49:21.044122 ragas-0.0.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/unit/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-27 14:49:06.000000 ragas-0.0.9/tests/unit/test_validation.py
```

### Comparing `ragas-0.0.8/.github/workflows/ci.yaml` & `ragas-0.0.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/.github/workflows/python-publish.yml` & `ragas-0.0.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/.gitignore` & `ragas-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/LICENSE` & `ragas-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/Makefile` & `ragas-0.0.9/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,10 @@
 run-ci: format lint type ## Running all CI checks
 run-benchmarks: ## Run benchmarks
 	@echo "Running benchmarks..."
 	@cd $(GIT_ROOT)/tests/benchmarks && python benchmark_eval.py
 test: ## Run tests
 	@echo "Running tests..."
 	@pytest tests/unit $(shell if [ -n "$(k)" ]; then echo "-k $(k)"; fi)
+test-e2e: ## Run end2end tests
+	echo "running end2end tests..."
+	@pytest tests/e2e -s
```

### Comparing `ragas-0.0.8/PKG-INFO` & `ragas-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.8 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.9 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
```

### Comparing `ragas-0.0.8/README.md` & `ragas-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/assets/bar-graph.svg` & `ragas-0.0.9/docs/assets/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/assets/logo.png` & `ragas-0.0.9/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/guides/data_prep.py` & `ragas-0.0.9/docs/guides/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/guides/llms.ipynb` & `ragas-0.0.9/docs/guides/llms.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/metrics.md` & `ragas-0.0.9/docs/metrics.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/docs/quickstart.ipynb` & `ragas-0.0.9/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/README.md` & `ragas-0.0.9/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/assesments/metrics_assesments.ipynb` & `ragas-0.0.9/experiments/assesments/metrics_assesments.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.9/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.9/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.9/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.9/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/pyproject.toml` & `ragas-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/references.md` & `ragas-0.0.9/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/_analytics.py` & `ragas-0.0.9/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/async_utils.py` & `ragas-0.0.9/src/ragas/async_utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/evaluation.py` & `ragas-0.0.9/src/ragas/evaluation.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
     Returns
     -------
     result : Result
         Result object containing the scores of each metric. You can use this do analysis
         later. If the top 3 metrics are provided then it also returns the `ragas_score`
         for the entire pipeline.
 
+    Raises
+    ------
+    ValueError
+        if validation fails because the columns required for the metrics are missing or
+        if the columns are of the wrong format.
+
     Examples
     --------
     the basic usage is as follows:
     ```
     from ragas import evaluate
 
     >>> dataset
```

### Comparing `ragas-0.0.8/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.9/src/ragas/metrics/answer_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/metrics/base.py` & `ragas-0.0.9/src/ragas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/metrics/context_relevance.py` & `ragas-0.0.9/src/ragas/metrics/context_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/metrics/critique.py` & `ragas-0.0.9/src/ragas/metrics/critique.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/metrics/faithfulnes.py` & `ragas-0.0.9/src/ragas/metrics/faithfulnes.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/metrics/llms.py` & `ragas-0.0.9/src/ragas/metrics/llms.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/utils.py` & `ragas-0.0.9/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/src/ragas/validation.py` & `ragas-0.0.9/src/ragas/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,13 +43,13 @@
     3. (q,c)
     4. (g,a)
     """
 
     for m in metrics:
         required_columns = set(EVALMODE_TO_COLUMNS[m.evaluation_mode])
         available_columns = set(ds.features.keys())
-        if required_columns.symmetric_difference(available_columns):
+        if not required_columns.issubset(available_columns):
             raise ValueError(
                 f"The metric [{m.name}] that that is used requires the following "
                 f"additional columns {list(required_columns - available_columns)} "
                 "to be present in the dataset."
             )
```

### Comparing `ragas-0.0.8/src/ragas.egg-info/PKG-INFO` & `ragas-0.0.9/src/ragas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.8 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.9 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
```

### Comparing `ragas-0.0.8/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.9/src/ragas.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,10 +41,11 @@
 src/ragas/metrics/context_relevance.py
 src/ragas/metrics/critique.py
 src/ragas/metrics/faithfulnes.py
 src/ragas/metrics/llms.py
 tests/.DS_Store
 tests/benchmarks/benchmark_eval.py
 tests/benchmarks/utils.py
+tests/e2e/test_fullflow.py
 tests/unit/test_metric.py
 tests/unit/test_simple.py
 tests/unit/test_validation.py
```

### Comparing `ragas-0.0.8/tests/.DS_Store` & `ragas-0.0.9/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/tests/benchmarks/benchmark_eval.py` & `ragas-0.0.9/tests/benchmarks/benchmark_eval.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/tests/benchmarks/utils.py` & `ragas-0.0.9/tests/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.8/tests/unit/test_validation.py` & `ragas-0.0.9/tests/unit/test_validation.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 CaseToTest = namedtuple(
     "TestCase", ["q", "a", "c", "g", "is_valid_columns", "metrics", "is_valid_metrics"]
 )
 
 TEST_CASES = [
     CaseToTest("a", "b", ["c"], None, True, [faithfulness], True),
-    CaseToTest("a", "b", ["c"], ["g"], True, [faithfulness], False),
+    CaseToTest("a", "b", ["c"], ["g"], True, [faithfulness], True),
     CaseToTest("a", None, ["c"], None, True, [context_relevancy], True),
     CaseToTest("a", None, "c", None, False, [context_relevancy], True),
     CaseToTest(
         "a", None, [["c"]], None, False, [context_relevancy, answer_relevancy], False
     ),
-    CaseToTest("a", None, ["c"], "g", False, [context_relevancy], False),
-    CaseToTest("a", None, ["c"], [["g"]], False, [context_relevancy], False),
-    CaseToTest(1, None, ["c"], ["g"], False, [context_relevancy], False),
+    CaseToTest("a", None, ["c"], "g", False, [context_relevancy], True),
+    CaseToTest("a", None, ["c"], [["g"]], False, [context_relevancy], True),
+    CaseToTest(1, None, ["c"], ["g"], False, [context_relevancy], True),
     CaseToTest(1, None, None, None, False, [context_relevancy], False),
 ]
 
 
 @pytest.mark.parametrize("testcase", TEST_CASES)
 def test_validate_column_dtypes(testcase):
     dataset_dict = {}
```

