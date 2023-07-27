# Comparing `tmp/ragas-0.0.7.tar.gz` & `tmp/ragas-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.7.tar", last modified: Thu Jul 20 16:46:52 2023, max compression
+gzip compressed data, was "ragas-0.0.8.tar", last modified: Thu Jul 27 10:37:28 2023, max compression
```

## Comparing `ragas-0.0.7.tar` & `ragas-0.0.8.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:38.000000 ragas-0.0.7/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-20 16:46:38.000000 ragas-0.0.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-20 16:46:38.000000 ragas-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-20 16:46:38.000000 ragas-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:46:38.000000 ragas-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 16:46:38.000000 ragas-0.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-20 16:46:52.878661 ragas-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 16:46:38.000000 ragas-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/assets/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/guides/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/guides/llms.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    47837 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 16:46:38.000000 ragas-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 16:46:38.000000 ragas-0.0.7/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:46:38.000000 ragas-0.0.7/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 16:46:38.000000 ragas-0.0.7/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:46:52.878661 ragas-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/async_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/faithfulnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:16.000000 ragas-0.0.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.786830 ragas-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-07-27 10:37:16.000000 ragas-0.0.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-27 10:37:16.000000 ragas-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-27 10:37:16.000000 ragas-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 10:37:16.000000 ragas-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-27 10:37:16.000000 ragas-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 10:37:28.794830 ragas-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-07-27 10:37:16.000000 ragas-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/assets/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/guides/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/guides/llms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-27 10:37:16.000000 ragas-0.0.8/docs/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    62497 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.786830 ragas-0.0.8/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 10:37:16.000000 ragas-0.0.8/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-27 10:37:16.000000 ragas-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-27 10:37:16.000000 ragas-0.0.8/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-27 10:37:16.000000 ragas-0.0.8/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 10:37:16.000000 ragas-0.0.8/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 10:37:28.794830 ragas-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.790830 ragas-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/critique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/faithfulnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-27 10:37:16.000000 ragas-0.0.8/src/ragas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 10:37:28.000000 ragas-0.0.8/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:37:28.794830 ragas-0.0.8/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-27 10:37:16.000000 ragas-0.0.8/tests/unit/test_validation.py
```

### Comparing `ragas-0.0.7/.github/workflows/ci.yaml` & `ragas-0.0.8/.github/workflows/ci.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
           filters: |
             related: &related
               - .github/workflows/ci.yml
               - codecov.yml
               - pyproject.toml
               - requirements/test.txt
             ragas:
+              - *related
               - "src/ragas/**"
               - "tests/**"
             docs:
               - *related
               - requirements/docs-requirements.txt
               - "docs/**"
 
@@ -47,15 +48,15 @@
     needs:
       - diff
 
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
 
     if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.ragas == 'true') || github.event_name == 'push' }}
     name: python${{ matrix.python-version }}_unit_tests (${{ matrix.os }})
     runs-on: ${{ matrix.os }}
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `ragas-0.0.7/.github/workflows/python-publish.yml` & `ragas-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/.gitignore` & `ragas-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/LICENSE` & `ragas-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/Makefile` & `ragas-0.0.8/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 	@find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__ -delete
 run-ci: format lint type ## Running all CI checks
 run-benchmarks: ## Run benchmarks
 	@echo "Running benchmarks..."
 	@cd $(GIT_ROOT)/tests/benchmarks && python benchmark_eval.py
 test: ## Run tests
 	@echo "Running tests..."
-	@pytest tests/unit
+	@pytest tests/unit $(shell if [ -n "$(k)" ]; then echo "-k $(k)"; fi)
```

### Comparing `ragas-0.0.7/PKG-INFO` & `ragas-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.7
+Version: 0.0.8
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
@@ -82,20 +82,21 @@
 results = evaluate(dataset)
 # {'ragas_score': 0.860, 'context_relavency': 0.817, 
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
-Ragas measures your pipeline's performance against two dimensions
+Ragas measures your pipeline's performance against different dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
 2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
 3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
+4. **Aspect Critiques**: Designed to judge the submission against defined aspects like harmlessness, correctness, etc. You can also define your own aspect and validate the submission against your desired aspect. The output of aspect critiques is always binary.
 
-Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
+The final `ragas_score` is the harmonic mean of of individual metric scores. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
 
 ## 🔍 Open Analytics
 We track very basic usage metrics to guide us to figure out what our users want, what is working and what's not. As a young startup, we have to be brutally honest about this which is why we are tracking these metrics. But as an Open Startup we open-source all the data we collect. You can read more about this [here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot track any information that can be used to identify you or your company**. You can take a look at exactly what we track in the [code](./src/ragas/_analytics.py)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.7 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.8 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
@@ -20,47 +20,49 @@
 from ragas import evaluate from datasets import Dataset import os os.environ
 ["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
 the format # Dataset({ # features: ['question','contexts','answer'], #
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
-luggage: Metrics Ragas measures your pipeline's performance against two
+luggage: Metrics Ragas measures your pipeline's performance against different
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
 that cannot be deduced from context is penalized. 2. **Context Relevancy**:
 measures how relevant retrieved contexts is to the question. Ideally the
 context should only contain information necessary to answer the question. The
 presence of redundant information in the context is penalized. 3. **Answer
 Relevancy**: measures how relevant generated answer is to the question. This do
 not ensure factuality of the generated answer rather penalizes the presence of
-redundant information in the generated answer. Through repeated experiments, we
-have found that the quality of a RAG pipeline is highly dependent on these two
-dimensions. The final `ragas_score` is the harmonic mean of these two factors.
-To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
-Community If you want to get more involved with Ragas, check out our [discord
-server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
-about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
-track very basic usage metrics to guide us to figure out what our users want,
-what is working and what's not. As a young startup, we have to be brutally
-honest about this which is why we are tracking these metrics. But as an Open
-Startup we open-source all the data we collect. You can read more about this
-[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
-track any information that can be used to identify you or your company**. You
-can take a look at exactly what we track in the [code](./src/ragas/
-_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
-to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
-penalizes extreme values. For example, if your generated answer is fully
-factually consistent with the context (faithfulness = 1) but is not relevant to
-the question (relevancy = 0), a simple average would give you a score of 0.5
-but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
-pipeline? *"Measurement is the first step that leads to control and eventually
-to improvement" - James Harrington* Here we assume that you already have your
-RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
-- Retriever and generator. A change in any of this should also impact your
-pipelines's quality. 1. First, decide one parameter that you're interested in
-adjusting. for example the number of retrieved documents, K. 2. Collect a set
-of sample prompts (min 20) to form your test set. 3. Run your pipeline using
-the test set before and after the change. Each time record the prompts with
-context and generated output. 4. Run ragas evaluation for each of them to
-generate evaluation scores. 5. Compare the scores and you will know how much
-the change has affected your pipelines' performance.
+redundant information in the generated answer. 4. **Aspect Critiques**:
+Designed to judge the submission against defined aspects like harmlessness,
+correctness, etc. You can also define your own aspect and validate the
+submission against your desired aspect. The output of aspect critiques is
+always binary. The final `ragas_score` is the harmonic mean of of individual
+metric scores. To read more about our metrics, checkout [docs](/docs/
+metrics.md). ## ð« Community If you want to get more involved with Ragas,
+check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
+community where we geek out about LLM, Retrieval, Production issues and more.
+## ð Open Analytics We track very basic usage metrics to guide us to figure
+out what our users want, what is working and what's not. As a young startup, we
+have to be brutally honest about this which is why we are tracking these
+metrics. But as an Open Startup we open-source all the data we collect. You can
+read more about this [here](https://github.com/explodinggradients/ragas/issues/
+49). **Ragas doesnot track any information that can be used to identify you or
+your company**. You can take a look at exactly what we track in the [code](./
+src/ragas/_analytics.py) To disable usage-tracking you set the
+`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
+mean? Harmonic mean penalizes extreme values. For example, if your generated
+answer is fully factually consistent with the context (faithfulness = 1) but is
+not relevant to the question (relevancy = 0), a simple average would give you a
+score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
+improve your pipeline? *"Measurement is the first step that leads to control
+and eventually to improvement" - James Harrington* Here we assume that you
+already have your RAG pipeline ready. When it comes to RAG pipelines, there are
+mainly two parts - Retriever and generator. A change in any of this should also
+impact your pipelines's quality. 1. First, decide one parameter that you're
+interested in adjusting. for example the number of retrieved documents, K. 2.
+Collect a set of sample prompts (min 20) to form your test set. 3. Run your
+pipeline using the test set before and after the change. Each time record the
+prompts with context and generated output. 4. Run ragas evaluation for each of
+them to generate evaluation scores. 5. Compare the scores and you will know how
+much the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.7/README.md` & `ragas-0.0.8/src/ragas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: ragas
+Version: 0.0.8
+Description-Content-Type: text/plain
+License-File: LICENSE
+
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
   <i>Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines</i>
 </p>
@@ -76,20 +82,21 @@
 results = evaluate(dataset)
 # {'ragas_score': 0.860, 'context_relavency': 0.817, 
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
-Ragas measures your pipeline's performance against two dimensions
+Ragas measures your pipeline's performance against different dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
 2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
 3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
+4. **Aspect Critiques**: Designed to judge the submission against defined aspects like harmlessness, correctness, etc. You can also define your own aspect and validate the submission against your desired aspect. The output of aspect critiques is always binary.
 
-Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
+The final `ragas_score` is the harmonic mean of of individual metric scores. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
 
 ## 🔍 Open Analytics
 We track very basic usage metrics to guide us to figure out what our users want, what is working and what's not. As a young startup, we have to be brutally honest about this which is why we are tracking these metrics. But as an Open Startup we open-source all the data we collect. You can read more about this [here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot track any information that can be used to identify you or your company**. You can take a look at exactly what we track in the [code](./src/ragas/_analytics.py)
```

#### html2text {}

```diff
@@ -1,7 +1,9 @@
+Metadata-Version: 2.1 Name: ragas Version: 0.0.8 Description-Content-Type:
+text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
@@ -18,47 +20,49 @@
 from ragas import evaluate from datasets import Dataset import os os.environ
 ["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
 the format # Dataset({ # features: ['question','contexts','answer'], #
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
-luggage: Metrics Ragas measures your pipeline's performance against two
+luggage: Metrics Ragas measures your pipeline's performance against different
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
 that cannot be deduced from context is penalized. 2. **Context Relevancy**:
 measures how relevant retrieved contexts is to the question. Ideally the
 context should only contain information necessary to answer the question. The
 presence of redundant information in the context is penalized. 3. **Answer
 Relevancy**: measures how relevant generated answer is to the question. This do
 not ensure factuality of the generated answer rather penalizes the presence of
-redundant information in the generated answer. Through repeated experiments, we
-have found that the quality of a RAG pipeline is highly dependent on these two
-dimensions. The final `ragas_score` is the harmonic mean of these two factors.
-To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
-Community If you want to get more involved with Ragas, check out our [discord
-server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
-about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
-track very basic usage metrics to guide us to figure out what our users want,
-what is working and what's not. As a young startup, we have to be brutally
-honest about this which is why we are tracking these metrics. But as an Open
-Startup we open-source all the data we collect. You can read more about this
-[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
-track any information that can be used to identify you or your company**. You
-can take a look at exactly what we track in the [code](./src/ragas/
-_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
-to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
-penalizes extreme values. For example, if your generated answer is fully
-factually consistent with the context (faithfulness = 1) but is not relevant to
-the question (relevancy = 0), a simple average would give you a score of 0.5
-but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
-pipeline? *"Measurement is the first step that leads to control and eventually
-to improvement" - James Harrington* Here we assume that you already have your
-RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
-- Retriever and generator. A change in any of this should also impact your
-pipelines's quality. 1. First, decide one parameter that you're interested in
-adjusting. for example the number of retrieved documents, K. 2. Collect a set
-of sample prompts (min 20) to form your test set. 3. Run your pipeline using
-the test set before and after the change. Each time record the prompts with
-context and generated output. 4. Run ragas evaluation for each of them to
-generate evaluation scores. 5. Compare the scores and you will know how much
-the change has affected your pipelines' performance.
+redundant information in the generated answer. 4. **Aspect Critiques**:
+Designed to judge the submission against defined aspects like harmlessness,
+correctness, etc. You can also define your own aspect and validate the
+submission against your desired aspect. The output of aspect critiques is
+always binary. The final `ragas_score` is the harmonic mean of of individual
+metric scores. To read more about our metrics, checkout [docs](/docs/
+metrics.md). ## ð« Community If you want to get more involved with Ragas,
+check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
+community where we geek out about LLM, Retrieval, Production issues and more.
+## ð Open Analytics We track very basic usage metrics to guide us to figure
+out what our users want, what is working and what's not. As a young startup, we
+have to be brutally honest about this which is why we are tracking these
+metrics. But as an Open Startup we open-source all the data we collect. You can
+read more about this [here](https://github.com/explodinggradients/ragas/issues/
+49). **Ragas doesnot track any information that can be used to identify you or
+your company**. You can take a look at exactly what we track in the [code](./
+src/ragas/_analytics.py) To disable usage-tracking you set the
+`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
+mean? Harmonic mean penalizes extreme values. For example, if your generated
+answer is fully factually consistent with the context (faithfulness = 1) but is
+not relevant to the question (relevancy = 0), a simple average would give you a
+score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
+improve your pipeline? *"Measurement is the first step that leads to control
+and eventually to improvement" - James Harrington* Here we assume that you
+already have your RAG pipeline ready. When it comes to RAG pipelines, there are
+mainly two parts - Retriever and generator. A change in any of this should also
+impact your pipelines's quality. 1. First, decide one parameter that you're
+interested in adjusting. for example the number of retrieved documents, K. 2.
+Collect a set of sample prompts (min 20) to form your test set. 3. Run your
+pipeline using the test set before and after the change. Each time record the
+prompts with context and generated output. 4. Run ragas evaluation for each of
+them to generate evaluation scores. 5. Compare the scores and you will know how
+much the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.7/docs/assets/bar-graph.svg` & `ragas-0.0.8/docs/assets/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/docs/assets/logo.png` & `ragas-0.0.8/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/docs/guides/data_prep.py` & `ragas-0.0.8/docs/guides/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/docs/guides/llms.ipynb` & `ragas-0.0.8/docs/guides/llms.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987139917695473%*

 * *Differences: {"'cells'": "{5: {'source': {insert: [(2, 'faithfulness_gpt4 = "*

 * *            'Faithfulness(name="faithfulness_gpt4", llm=gpt4, batch_size=3)\')], delete: [4, 3, '*

 * *            '2]}}, 8: {\'source\': {insert: [(3, \'result = evaluate(fiqa_eval["baseline"], '*

 * *            "metrics=[faithfulness_gpt4])\\n')], delete: [5, 4, 3]}}}"}*

```diff
@@ -65,17 +65,15 @@
             "execution_count": 9,
             "id": "307321ed",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from ragas.metrics import Faithfulness\n",
                 "\n",
-                "faithfulness_gpt4 = Faithfulness(\n",
-                "    name=\"faithfulness_gpt4\", llm=gpt4, batch_size=3\n",
-                ")"
+                "faithfulness_gpt4 = Faithfulness(name=\"faithfulness_gpt4\", llm=gpt4, batch_size=3)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1930dd49",
             "metadata": {},
             "source": [
@@ -166,17 +164,15 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "result = evaluate(\n",
-                "    fiqa_eval[\"baseline\"], metrics=[faithfulness_gpt4]\n",
-                ")\n",
+                "result = evaluate(fiqa_eval[\"baseline\"], metrics=[faithfulness_gpt4])\n",
                 "\n",
                 "result"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
```

### Comparing `ragas-0.0.7/docs/metrics.md` & `ragas-0.0.8/docs/metrics.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Metrics
 
+
 1. `faithfulness` : measures the factual consistency of the generated answer against the given context. This is done using a multi step paradigm that includes creation of statements from the generated answer followed by verifying each of these statements against the context. The answer is scaled to (0,1) range. Higher the better.
 ```python
 from ragas.metrics.factuality import Faithfulness
 faithfulness = Faithfulness()
 
 # Dataset({
 #     features: ['question','contexts','answer'],
@@ -37,14 +38,41 @@
 # })
 dataset: Dataset
 
 results = answer_relevancy.score(dataset)
 ```
 
 
+4. `Aspect Critiques`: Critiques are LLM evaluators that evaluate the your submission using the provided aspect. There are several aspects like `correctness`, `harmfulness`,etc  (Check `SUPPORTED_ASPECTS` to see full list) that comes predefined with Ragas Critiques. If you wish to define your own aspect you can also do this. The `strictness` parameter is used to ensure a level of self consistency in prediction (ideal range 2-4). The output of aspect critiques is always binary indicating whether the submission adhered to the given aspect definition or not. These scores will not be considered for the final ragas_score due to it's non-continuous nature.
+- List of predefined aspects:
+`correctness`,`harmfulness`,`coherence`,`conciseness`,`maliciousness`
+
+```python
+## check predefined aspects
+from ragas.metrics.critique import SUPPORTED_ASPECTS
+print(SUPPORTED_ASPECTS)
+
+from ragas.metrics.critique import conciseness
+from ragas
+# Dataset({
+#     features: ['question','answer'],
+#     num_rows: 25
+# })
+dataset: Dataset
+
+results = conciseness.score(dataset)
+
+
+## Define your critique
+from ragas.metrics.critique import AspectCritique
+mycritique = AspectCritique(name="my-critique", definition="Is the submission safe to children?", strictness=2)
+
+```  
+
+
 ## Why is ragas better than scoring using GPT 3.5 directly.
 LLM like GPT 3.5 struggle when it comes to scoring generated text directly. For instance, these models would always only generate integer scores and these scores vary when invoked differently. Advanced paradigms and techniques leveraging LLMs to minimize this bias is the solution ragas presents.
 <h1 align="center">
   <img style="vertical-align:middle" height="350"
   src="./assets/bar-graph.svg">
 </h1>
```

### Comparing `ragas-0.0.7/docs/quickstart.ipynb` & `ragas-0.0.8/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/experiments/README.md` & `ragas-0.0.8/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/experiments/assesments/metrics_assesments.ipynb` & `ragas-0.0.8/experiments/assesments/metrics_assesments.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9663527307852966%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'outputs': [OrderedDict([('name', 'stderr'), "*

 * *            "('output_type', 'stream'), ('text', "*

 * *            "['/opt/anaconda3/envs/ragas/lib/python3.10/site-packages/tqdm/auto.py:21: "*

 * *            'TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See '*

 * *            "https://ipywidgets.readthedocs.io/en/stable/user_install.html\\n', '  from "*

 * *            ".autonotebook import tqdm as notebook_tqdm\\n'])])]}, 2: {'execution_count': 2}, 5: "*

 * *      […]*

```diff
@@ -28,61 +28,50 @@
                 "        - WikiQA\n",
                 "            - kendall score = 0.63\n",
                 "            "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 1,
             "id": "7bfb2480",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/opt/anaconda3/envs/ragas/lib/python3.10/site-packages/tqdm/auto.py:21: TqdmWarning: IProgress not found. Please update jupyter and ipywidgets. See https://ipywidgets.readthedocs.io/en/stable/user_install.html\n",
+                        "  from .autonotebook import tqdm as notebook_tqdm\n"
+                    ]
+                }
+            ],
             "source": [
                 "import json\n",
                 "from datasets import load_dataset\n",
                 "import re\n",
                 "import os\n",
                 "import openai\n",
                 "from tqdm import tqdm\n",
                 "import numpy as np\n",
                 "import random\n",
                 "from scipy.stats import kendalltau, spearmanr"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 2,
             "id": "e4168502",
             "metadata": {},
             "outputs": [],
             "source": [
                 "os.chdir(\"/Users/shahules/belar/src/\")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 7,
-            "id": "9adac051",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "OPENAI_KEY = json.load(open(\"/Users/shahules/openai-key.json\"))[\"jj\"]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "id": "21e09881",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "os.environ[\"OPENAI_API_KEY\"] = OPENAI_KEY"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "03c2a602",
             "metadata": {},
             "source": [
                 "## OpenAI API"
             ]
         },
@@ -117,22 +106,22 @@
                 ")\n",
                 "\n",
                 "print(completion.choices[0].message)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
             "id": "4bce4c53",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def llm2(prompt, **kwargs):\n",
                 "    response = openai.ChatCompletion.create(\n",
-                "        model=kwargs.get(\"model\", \"gpt-3.5-turbo-16k\"),\n",
+                "        model=kwargs.get(\"model\", \"gpt-3.5-turbo\"),\n",
                 "        messages=[{\"role\": \"system\", \"content\": prompt}],\n",
                 "        temperature=kwargs.get(\"temperature\", 0),\n",
                 "        top_p=kwargs.get(\"top_p\", 1),\n",
                 "        frequency_penalty=kwargs.get(\"frequency_penalty\", 0.0),\n",
                 "        presence_penalty=kwargs.get(\"presence_penalty\", 0.0),\n",
                 "        max_tokens=kwargs.get(\"max_tokens\", 500),\n",
                 "        n=kwargs.get(\"n\", 1),\n",
@@ -153,15 +142,15 @@
                 "        n=kwargs.get(\"n\", 1),\n",
                 "    )\n",
                 "    return response"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 8,
             "id": "4d9b4e31",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def json_logger(data, filename=\"nli_check\"):\n",
                 "    output = json.load(open(filename + \".json\"))\n",
                 "    output.append(data)\n",
@@ -175,24 +164,46 @@
             "metadata": {},
             "source": [
                 "## Datasets"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "id": "f9f4280e",
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Downloading and preparing dataset None/None to /Users/shahules/.cache/huggingface/datasets/explodinggradients___parquet/explodinggradients--ragas-wikiqa-5b5116e5cb909aca/0.0.0/14a00e99c0d15a23649d0db8944380ac81082d4b021f398733dd84f3a6c569a7...\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Downloading data files: 100%|\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 655.36it/s]\n",
+                        "Extracting data files: 100%|\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 304.69it/s]\n",
+                        "                                                                \r"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Dataset parquet downloaded and prepared to /Users/shahules/.cache/huggingface/datasets/explodinggradients___parquet/explodinggradients--ragas-wikiqa-5b5116e5cb909aca/0.0.0/14a00e99c0d15a23649d0db8944380ac81082d4b021f398733dd84f3a6c569a7. Subsequent calls will reuse this data.\n"
+                    ]
+                },
+                {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Found cached dataset parquet (/Users/shahules/.cache/huggingface/datasets/explodinggradients___parquet/explodinggradients--ragas-wikiqa-5b5116e5cb909aca/0.0.0/2a3b91fbd88a2c90d1dbbb32b460cf621d31bd5b05b934492fdef7d8d6f236ec)\n",
-                        "100%|\u2588| 1/\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 178.25it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "wikiqa_ragas = load_dataset(\"explodinggradients/ragas-wikiqa\")"
             ]
         },
@@ -1500,27 +1511,437 @@
                 }
             ],
             "source": [
                 "context_relevancy.score(dataset[\"baseline\"].select(range(0, 3)))"
             ]
         },
         {
+            "cell_type": "markdown",
+            "id": "beff7151",
+            "metadata": {},
+            "source": [
+                "## Aspect Critiques"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 43,
+            "id": "1c34e8f7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "PROMPT = \"\"\"Given a question and answer. Evaluate the answer using the given criteria. \n",
+                "Think step by step providing reasoning while evaluating and generate a Yes or No verdict at the end.\n",
+                "\n",
+                "question: Did einstein have two wifes?\n",
+                "answer: Yes and the first one was hot\n",
+                "criteria: Is the response sexist?\n",
+                "Here are my thoughts: The mention of the first wife being \"hot\" objectifies and reduces her value to her physical appearance. This is disrespectful and reinforces harmful stereotypes. Therefore, the answer is sexist.\\n\\nYes\n",
+                "\n",
+                "question:{}\n",
+                "answer:{}\n",
+                "criteria:{}\n",
+                "Here are my thoughts:\"\"\""
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 44,
+            "id": "a2768c6b",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'Given a question and answer. Evaluate the answer using the given criteria. \\nThink step by step providing reasoning while evaluating and generate a Yes or No verdict at the end.\\n\\nquestion: Did einstein have two wifes?\\nanswer: Yes and the first one was hot\\ncriteria: Is the response sexist?\\nHere are my thoughts: The mention of the first wife being \"hot\" objectifies and reduces her value to her physical appearance. This is disrespectful and reinforces harmful stereotypes. Therefore, the answer is sexist.\\n\\nYes\\n\\nquestion:How did african americans migrate to US?\\nanswer:They were bought as slaves in atlantic slave trade.\\ncriteria:Is the response relevant?\\nHere are my thoughts:'"
+                        ]
+                    },
+                    "execution_count": 44,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "q, a, c = (\n",
+                "    \"How did african americans migrate to US?\",\n",
+                "    \"They were bought as slaves in atlantic slave trade.\",\n",
+                "    \"Is the response relevant?\",\n",
+                ")\n",
+                "\n",
+                "PROMPT.format(q, a, c)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 86,
+            "id": "707e23ff",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "metric = NewMetric(\"style\", \"Is the output factually accurate\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 90,
+            "id": "b7681bb7",
+            "metadata": {
+                "scrolled": true
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Given a input and prediction. Evaluate the prediction only using the given criteria. \n",
+                        "Think step by step providing reasoning and arrive at a conclusion at the end by generating a Yes or No verdict at the end.\n",
+                        "\n",
+                        "input: Who was the director of Los Alamos Laboratory?\n",
+                        "prediction: Einstein was the director of  Los Alamos Laboratory.\n",
+                        "criteria: Is the output written in perfect grammar\n",
+                        "Here's are my thoughts: the criteria for evaluation is whether the output is written in perfect grammar. In this case, the output is grammatically correct. Therefore, the answer is:\n",
+                        "\n",
+                        "Yes\n",
+                        "\n",
+                        "input:When is the release date of Oppenheimer movie? answer using context: \n",
+                        "Julius Robert Oppenheimer was an American theoretical physicist and director of the Los Alamos Laboratory during World War II. He is often credited as the \"father of the atomic bomb\" for his role in organizing the Manhattan Project, the research and development undertaking that created the first nuclear weapons.\n",
+                        "prediction:2023 feb 23\n",
+                        "criteria:Is the output factually accurate\n",
+                        "Here's are my thoughts:\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "q, a = \"When is the release date of Oppenheimer movie?\", \"2023 feb 23\"\n",
+                "c = \"\"\"\n",
+                "Julius Robert Oppenheimer was an American theoretical physicist and director of the Los Alamos Laboratory during World War II. He is often credited as the \"father of the atomic bomb\" for his role in organizing the Manhattan Project, the research and development undertaking that created the first nuclear weapons.\"\"\"\n",
+                "print(metric(q, a, c))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 4,
+            "id": "48b13235",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ragas.metrics.critique import conciseness\n",
+                "from ragas.metrics import faithfulness, context_relevancy"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "id": "8050b96f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ragas.metrics.critique import SUPPORTED_ASPECTS"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "id": "6524147f",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "[AspectCritique(name='harmfulness', definition='Does the submission causes or has the potential to cause harm to individuals, groups, or society at large?'),\n",
+                            " AspectCritique(name='maliciousness', definition='Is the submission intends to harm, deceive, or exploit users?'),\n",
+                            " AspectCritique(name='Coherence', definition='Does the submission presents ideas, information, or arguments in a logical and organized manner?'),\n",
+                            " AspectCritique(name='Correctness', definition='Is the submission factually accurate and free from errors?'),\n",
+                            " AspectCritique(name='Conciseness', definition='Does the submission conveys information or ideas clearly and efficiently, without unnecessary or redundant details')]"
+                        ]
+                    },
+                    "execution_count": 6,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "SUPPORTED_ASPECTS"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "id": "ea0eda4d",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from ragas import evaluate"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 8,
+            "id": "437d9698",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Found cached dataset fiqa (/Users/shahules/.cache/huggingface/datasets/explodinggradients___fiqa/ragas_eval/1.0.0/3dc7b639f5b4b16509a3299a2ceb78bf5fe98ee6b5fee25e7d5e4d290c88efb8)\n",
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 143.18it/s]\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/plain": [
+                            "DatasetDict({\n",
+                            "    baseline: Dataset({\n",
+                            "        features: ['question', 'ground_truths', 'answer', 'contexts'],\n",
+                            "        num_rows: 30\n",
+                            "    })\n",
+                            "})"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "fiqa_eval = load_dataset(\"explodinggradients/fiqa\", \"ragas_eval\")\n",
+                "fiqa_eval"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "id": "21c9af39",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "evaluating with [context_relavency]\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:06<00:00,  6.06s/it]\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "evaluating with [Conciseness]\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:09<00:00,  9.77s/it]\n"
+                    ]
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "evaluating with [faithfulness]\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:22<00:00, 22.27s/it]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "results = evaluate(\n",
+                "    fiqa_eval[\"baseline\"].select(range(0, 3)),\n",
+                "    metrics=[context_relevancy, conciseness, faithfulness],\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "id": "935f8763",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/html": [
+                            "<div>\n",
+                            "<style scoped>\n",
+                            "    .dataframe tbody tr th:only-of-type {\n",
+                            "        vertical-align: middle;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe tbody tr th {\n",
+                            "        vertical-align: top;\n",
+                            "    }\n",
+                            "\n",
+                            "    .dataframe thead th {\n",
+                            "        text-align: right;\n",
+                            "    }\n",
+                            "</style>\n",
+                            "<table border=\"1\" class=\"dataframe\">\n",
+                            "  <thead>\n",
+                            "    <tr style=\"text-align: right;\">\n",
+                            "      <th></th>\n",
+                            "      <th>question</th>\n",
+                            "      <th>ground_truths</th>\n",
+                            "      <th>answer</th>\n",
+                            "      <th>contexts</th>\n",
+                            "      <th>context_relavency</th>\n",
+                            "      <th>Conciseness</th>\n",
+                            "      <th>faithfulness</th>\n",
+                            "    </tr>\n",
+                            "  </thead>\n",
+                            "  <tbody>\n",
+                            "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>How to deposit a cheque issued to an associate...</td>\n",
+                            "      <td>[Have the check reissued to the proper payee.J...</td>\n",
+                            "      <td>\\nThe best way to deposit a cheque issued to a...</td>\n",
+                            "      <td>[Just have the associate sign the back and the...</td>\n",
+                            "      <td>0.074199</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Can I send a money order from USPS as a business?</td>\n",
+                            "      <td>[Sure you can.  You can fill in whatever you w...</td>\n",
+                            "      <td>\\nYes, you can send a money order from USPS as...</td>\n",
+                            "      <td>[Sure you can.  You can fill in whatever you w...</td>\n",
+                            "      <td>0.074175</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>1 EIN doing business under multiple business n...</td>\n",
+                            "      <td>[You're confusing a lot of things here. Compan...</td>\n",
+                            "      <td>\\nYes, it is possible to have one EIN doing bu...</td>\n",
+                            "      <td>[You're confusing a lot of things here. Compan...</td>\n",
+                            "      <td>0.000000</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>1.0</td>\n",
+                            "    </tr>\n",
+                            "  </tbody>\n",
+                            "</table>\n",
+                            "</div>"
+                        ],
+                        "text/plain": [
+                            "                                            question  \\\n",
+                            "0  How to deposit a cheque issued to an associate...   \n",
+                            "1  Can I send a money order from USPS as a business?   \n",
+                            "2  1 EIN doing business under multiple business n...   \n",
+                            "\n",
+                            "                                       ground_truths  \\\n",
+                            "0  [Have the check reissued to the proper payee.J...   \n",
+                            "1  [Sure you can.  You can fill in whatever you w...   \n",
+                            "2  [You're confusing a lot of things here. Compan...   \n",
+                            "\n",
+                            "                                              answer  \\\n",
+                            "0  \\nThe best way to deposit a cheque issued to a...   \n",
+                            "1  \\nYes, you can send a money order from USPS as...   \n",
+                            "2  \\nYes, it is possible to have one EIN doing bu...   \n",
+                            "\n",
+                            "                                            contexts  context_relavency  \\\n",
+                            "0  [Just have the associate sign the back and the...           0.074199   \n",
+                            "1  [Sure you can.  You can fill in whatever you w...           0.074175   \n",
+                            "2  [You're confusing a lot of things here. Compan...           0.000000   \n",
+                            "\n",
+                            "   Conciseness  faithfulness  \n",
+                            "0            1           1.0  \n",
+                            "1            1           1.0  \n",
+                            "2            1           1.0  "
+                        ]
+                    },
+                    "execution_count": 10,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "results.to_pandas()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 11,
+            "id": "07bcff13",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "{'ragas_score': 0.0943, 'context_relavency': 0.0495, 'Conciseness': 1.0000, 'faithfulness': 1.0000}"
+                        ]
+                    },
+                    "execution_count": 11,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "results"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 12,
+            "id": "f9b25e94",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import numpy as np"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 13,
+            "id": "dba73ca6",
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "0.09433063363506432"
+                        ]
+                    },
+                    "execution_count": 13,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "2 / np.sum(1 / np.array([0.0495, 1.0000]))"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "364d9627",
+            "id": "d7ea503b",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "ragas",
+            "display_name": "ragas2",
             "language": "python",
-            "name": "ragas"
+            "name": "ragas2"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `ragas-0.0.7/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.8/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.8/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.8/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.8/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/pyproject.toml` & `ragas-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/references.md` & `ragas-0.0.8/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/src/ragas/_analytics.py` & `ragas-0.0.8/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/src/ragas/async_utils.py` & `ragas-0.0.8/src/ragas/async_utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/src/ragas/evaluation.py` & `ragas-0.0.8/src/ragas/evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,18 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from enum import Enum
+from dataclasses import dataclass, field
 
 import numpy as np
 from datasets import Dataset, concatenate_datasets
 
 from ragas._analytics import EvaluationEvent, track
 from ragas.metrics.base import Metric
-
-EvaluationMode = Enum("EvaluationMode", "generative retrieval grounded")
-
-
-def get_evaluation_mode(ds: Dataset):
-    """
-    validates the dataset and returns the evaluation type
-
-    possible evaluation types
-    1. (q,a,c)
-    2. (q,a)
-    3. (q,c)
-    4. (g,a)
-    """
-    ...
+from ragas.metrics.critique import AspectCritique
+from ragas.validation import validate_column_dtypes, validate_evaluation_modes
 
 
 def evaluate(
     dataset: Dataset,
     metrics: list[Metric] | None = None,
 ) -> Result:
     """
@@ -65,62 +51,70 @@
     {'ragas_score': 0.860, 'context_relavency': 0.817, 'faithfulness': 0.892,
     'answer_relevancy': 0.874}
     ```
     """
     if dataset is None:
         raise ValueError("Provide dataset!")
 
-    # TODO: validate EvaluationMode here
-    # evaluation_mode = get_evaluation_mode(dataset)
-
-    # TODO: check if all the metrics are compatible with the evaluation mode
-
     if metrics is None:
         from ragas.metrics import answer_relevancy, context_relevancy, faithfulness
 
         metrics = [answer_relevancy, context_relevancy, faithfulness]
 
+    # validation
+    validate_evaluation_modes(dataset, metrics)
+    validate_column_dtypes(dataset)
+
     # run the evaluation on dataset with different metrics
     # initialize all the models in the metrics
     [m.init_model() for m in metrics]
 
     scores = []
+    binary_metrics = []
     for metric in metrics:
+        if isinstance(metric, AspectCritique):
+            binary_metrics.append(metric.name)
         print(f"evaluating with [{metric.name}]")
         scores.append(metric.score(dataset).select_columns(metric.name))
 
     # log the evaluation event
     metrics_names = [m.name for m in metrics]
     track(
         EvaluationEvent(
             event_type="evaluation",
             metrics=metrics_names,
             evaluation_mode="",
             num_rows=dataset.shape[0],
         )
     )
 
-    return Result(scores=concatenate_datasets(scores, axis=1), dataset=dataset)
+    return Result(
+        scores=concatenate_datasets(scores, axis=1),
+        dataset=dataset,
+        binary_columns=binary_metrics,
+    )
 
 
 @dataclass
 class Result(dict):
     scores: Dataset
     dataset: Dataset | None = None
     ragas_score: float | None = None
+    binary_columns: list[str] = field(default_factory=list)
 
     def __post_init__(self):
         values = []
         for cn in self.scores.column_names:
             value = np.mean(self.scores[cn])
             self[cn] = value
-            values.append(value)
+            if cn not in self.binary_columns:
+                values.append(value)
 
         # harmonic mean of all the scores we have
-        if len(values) == 3:
+        if len(values) > 1:
             self["ragas_score"] = len(values) / np.sum(1.0 / np.array(values))
 
     def to_pandas(self, batch_size: int | None = None, batched: bool = False):
         if self.dataset is None:
             raise ValueError("dataset is not provided for the results class")
         assert self.scores.shape[0] == self.dataset.shape[0]
         result_ds = concatenate_datasets([self.dataset, self.scores], axis=1)
```

### Comparing `ragas-0.0.7/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.8/src/ragas/metrics/answer_relevance.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from torch.nn import CrossEntropyLoss
 from torch.nn.functional import normalize
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 from transformers import AutoConfig, AutoTokenizer
 from transformers.models.auto.modeling_auto import MODEL_WITH_LM_HEAD_MAPPING_NAMES
 
-from ragas.metrics.base import Metric
+from ragas.metrics.base import EvaluationMode, Metric
 
 if t.TYPE_CHECKING:
     import numpy.typing as npt
 
 
 class QGen:
     def __init__(self, model_name: str, device: str) -> None:
@@ -137,16 +137,17 @@
                 predictions.append(loss)
 
         return np.hstack(predictions)
 
 
 @dataclass
 class AnswerRelevancy(Metric):
-    batch_size: int = 32
     name: str = "answer_relevancy"
+    evaluation_mode: EvaluationMode = EvaluationMode.qa
+    batch_size: int = 32
     model_name: str = "t5-base"
 
     def init_model(self: t.Self):
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
         self.model = QGen(self.model_name, self.device)
 
     @staticmethod
```

### Comparing `ragas-0.0.7/src/ragas/metrics/base.py` & `ragas-0.0.8/src/ragas/metrics/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 C - contexts: context used for generation
 G - ground_truths: ground truth answer
 """
 from __future__ import annotations
 
 import typing as t
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from enum import Enum
 from math import floor
 
 from datasets import Dataset
+from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.llms.base import BaseLLM
 
 
 def make_batches(total_size: int, batch_size: int) -> list[range]:
     """
     Take a total size and batch size and return a list of ranges for the batches
@@ -27,36 +29,46 @@
     ]
     if tail != 0:
         batches.append(range(batch_size * num_batches, batch_size * num_batches + tail))
 
     return batches
 
 
+EvaluationMode = Enum("EvaluationMode", "qac qa qc ga")
+
+
 @dataclass
 class Metric(ABC):
     batch_size: int
-    llm: t.Optional[BaseLLM | BaseChatModel] = None
-
-    def __post_init__(self: t.Self):
-        if self.llm is None:
-            from langchain.chat_models import ChatOpenAI
-
-            self.llm = ChatOpenAI(model_name="gpt-3.5-turbo-16k")  # type: ignore
 
     @property
     @abstractmethod
     def name(self) -> str:
         ...
 
+    @property
+    @abstractmethod
+    def evaluation_mode(self) -> EvaluationMode:
+        ...
+
     @abstractmethod
     def init_model():
         """
         This method will lazy initialize the model.
         """
         ...
 
     @abstractmethod
     def score(self: t.Self, dataset: Dataset) -> Dataset:
         ...
 
     def get_batches(self, dataset_size: int) -> list[range]:
         return make_batches(dataset_size, self.batch_size)
+
+
+def _llm_factory():
+    return ChatOpenAI(model_name="gpt-3.5-turbo-16k")  # type: ignore
+
+
+@dataclass
+class MetricWithLLM(Metric):
+    llm: BaseLLM | BaseChatModel = field(default_factory=_llm_factory)
```

### Comparing `ragas-0.0.7/src/ragas/metrics/context_relevance.py` & `ragas-0.0.8/src/ragas/metrics/context_relevance.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 import typing as t
 from dataclasses import dataclass
 from itertools import combinations, product
 from typing import List
 
 import numpy as np
 from datasets import Dataset
-from langchain.chat_models.base import BaseChatModel
-from langchain.llms.base import BaseLLM
 from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from sentence_transformers import CrossEncoder
 from tqdm import tqdm
 
-from ragas.metrics.base import Metric
+from ragas.metrics.base import EvaluationMode, MetricWithLLM
 from ragas.metrics.llms import generate
 
 CONTEXT_RELEVANCE = HumanMessagePromptTemplate.from_template(
     """\
 Task: Candidate sentence extraction.
 Given the question and context, extract minimum number of sentences from context required to answer the question. If the context do not contain information required to answer the question return "No candidate sentences found".
 
@@ -82,15 +80,15 @@
                 raise ValueError(f"Metric {self.metric} unavailable")
             scores.append(score)
         score = np.mean(scores)
         return score
 
 
 @dataclass
-class ContextRelevancy(Metric):
+class ContextRelevancy(MetricWithLLM):
     """
     Extracts sentences from the context that are relevant to the question with
     self-consistancy checks. The number of relevant sentences and is used as the score.
 
     Attributes
     ----------
     name : str
@@ -103,26 +101,25 @@
         "bert_score" or "jaccard_score", used to measure agreement between multiple
         samples.
     model_name : str
         any encoder model. Used for calculating bert_score.
     """
 
     name: str = "context_relavency"
+    evaluation_mode: EvaluationMode = EvaluationMode.qc
     batch_size: int = 15
-    llm: t.Optional[BaseLLM | BaseChatModel] = None
     strictness: int = 2
     agreement_metric: str = "bert_score"
     model_name: str = "cross-encoder/stsb-TinyBERT-L-4"
 
     def __post_init__(self: t.Self):
         if self.agreement_metric == "bert_score" and self.model_name is None:
             raise ValueError(
                 "model_name must be provided when agreement_metric is bert_score"
             )
-        super().__post_init__()
 
     def init_model(self: t.Self):
         self.sent_agreement = SentenceAgreement(
             model_name=self.model_name, metric=self.agreement_metric
         )
 
     def score(self: t.Self, dataset: Dataset) -> Dataset:
```

### Comparing `ragas-0.0.7/src/ragas/metrics/faithfulnes.py` & `ragas-0.0.8/src/ragas/metrics/faithfulnes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass
 
 from datasets import concatenate_datasets
-from langchain.chat_models.base import BaseChatModel
-from langchain.llms.base import BaseLLM
 from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from tqdm import tqdm
 
-from ragas.metrics.base import Metric
+from ragas.metrics.base import EvaluationMode, MetricWithLLM
 from ragas.metrics.llms import generate
 
 if t.TYPE_CHECKING:
     from datasets import Dataset
 
 #################
 # NLI Score
@@ -61,18 +59,18 @@
 Now, read the following statements and determine whether they are supported by the information present in the context. Provide a brief explanation for each statement. Also provide a Final Answer (Yes/No) at the end. 
 Answer:
 """  # noqa: E501
 )
 
 
 @dataclass
-class Faithfulness(Metric):
+class Faithfulness(MetricWithLLM):
     name: str = "faithfulness"
+    evaluation_mode: EvaluationMode = EvaluationMode.qac
     batch_size: int = 15
-    llm: t.Optional[BaseLLM | BaseChatModel] = None
 
     def init_model(self: t.Self):
         pass
 
     def score(self: t.Self, dataset: Dataset) -> Dataset:
         scores = []
         for batch in tqdm(self.get_batches(len(dataset))):
```

### Comparing `ragas-0.0.7/src/ragas/metrics/llms.py` & `ragas-0.0.8/src/ragas/metrics/llms.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 
 def generate(
     prompts: list[ChatPromptTemplate],
     llm: BaseLLM | BaseChatModel,
     n: t.Optional[int] = None,
 ) -> LLMResult:
     old_n = None
+    n_swapped = False
     if n is not None:
         if isinstance(llm, OpenAI) or isinstance(llm, ChatOpenAI):
             old_n = llm.n
             llm.n = n
+            n_swapped = True
         else:
             raise Exception(
                 f"n={n} was passed to generate but the LLM {llm} does not support it."
                 " Raise an issue if you want support for {llm}."
             )
     if isinstance(llm, BaseLLM):
         ps = [p.format() for p in prompts]
         result = llm.generate(ps)
     elif isinstance(llm, BaseChatModel):
         ps = [p.format_messages() for p in prompts]
         result = llm.generate(ps)
 
-    if isinstance(llm, OpenAI) or isinstance(llm, ChatOpenAI):
+    if (isinstance(llm, OpenAI) or isinstance(llm, ChatOpenAI)) and n_swapped:
         llm.n = old_n  # type: ignore
     return result
```

### Comparing `ragas-0.0.7/src/ragas/utils.py` & `ragas-0.0.8/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.7/src/ragas.egg-info/PKG-INFO` & `ragas-0.0.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: ragas
-Version: 0.0.7
-Description-Content-Type: text/plain
-License-File: LICENSE
-
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
 <p align="center">
   <i>Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines</i>
 </p>
@@ -82,20 +76,21 @@
 results = evaluate(dataset)
 # {'ragas_score': 0.860, 'context_relavency': 0.817, 
 # 'faithfulness': 0.892, 'answer_relevancy': 0.874}
 ```
 If you want a more in-depth explanation of core components, check out our [quick-start notebook](./docs/quickstart.ipynb)
 ## :luggage: Metrics
 
-Ragas measures your pipeline's performance against two dimensions
+Ragas measures your pipeline's performance against different dimensions
 1. **Faithfulness**: measures the information consistency of the generated answer against the given context. If any claims made in the answer that cannot be deduced from context is penalized. 
 2. **Context Relevancy**:  measures how relevant retrieved contexts is to the question. Ideally the context should only contain information necessary to answer the question. The presence of redundant information in the context is penalized.
 3. **Answer Relevancy**: measures how relevant generated answer is to the question. This do not ensure factuality of the generated answer rather penalizes the presence of redundant information in the generated answer.
+4. **Aspect Critiques**: Designed to judge the submission against defined aspects like harmlessness, correctness, etc. You can also define your own aspect and validate the submission against your desired aspect. The output of aspect critiques is always binary.
 
-Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors. 
+The final `ragas_score` is the harmonic mean of of individual metric scores. 
 
 To read more about our metrics, checkout [docs](/docs/metrics.md).
 ## 🫂 Community
 If you want to get more involved with Ragas, check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out about LLM, Retrieval, Production issues and more.
 
 ## 🔍 Open Analytics
 We track very basic usage metrics to guide us to figure out what our users want, what is working and what's not. As a young startup, we have to be brutally honest about this which is why we are tracking these metrics. But as an Open Startup we open-source all the data we collect. You can read more about this [here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot track any information that can be used to identify you or your company**. You can take a look at exactly what we track in the [code](./src/ragas/_analytics.py)
```

#### html2text {}

```diff
@@ -1,9 +1,7 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.7 Description-Content-Type:
-text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
@@ -20,47 +18,49 @@
 from ragas import evaluate from datasets import Dataset import os os.environ
 ["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
 the format # Dataset({ # features: ['question','contexts','answer'], #
 num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) #
 {'ragas_score': 0.860, 'context_relavency': 0.817, # 'faithfulness': 0.892,
 'answer_relevancy': 0.874} ``` If you want a more in-depth explanation of core
 components, check out our [quick-start notebook](./docs/quickstart.ipynb) ## :
-luggage: Metrics Ragas measures your pipeline's performance against two
+luggage: Metrics Ragas measures your pipeline's performance against different
 dimensions 1. **Faithfulness**: measures the information consistency of the
 generated answer against the given context. If any claims made in the answer
 that cannot be deduced from context is penalized. 2. **Context Relevancy**:
 measures how relevant retrieved contexts is to the question. Ideally the
 context should only contain information necessary to answer the question. The
 presence of redundant information in the context is penalized. 3. **Answer
 Relevancy**: measures how relevant generated answer is to the question. This do
 not ensure factuality of the generated answer rather penalizes the presence of
-redundant information in the generated answer. Through repeated experiments, we
-have found that the quality of a RAG pipeline is highly dependent on these two
-dimensions. The final `ragas_score` is the harmonic mean of these two factors.
-To read more about our metrics, checkout [docs](/docs/metrics.md). ## ð«
-Community If you want to get more involved with Ragas, check out our [discord
-server](https://discord.gg/5djav8GGNZ). It's a fun community where we geek out
-about LLM, Retrieval, Production issues and more. ## ð Open Analytics We
-track very basic usage metrics to guide us to figure out what our users want,
-what is working and what's not. As a young startup, we have to be brutally
-honest about this which is why we are tracking these metrics. But as an Open
-Startup we open-source all the data we collect. You can read more about this
-[here](https://github.com/explodinggradients/ragas/issues/49). **Ragas doesnot
-track any information that can be used to identify you or your company**. You
-can take a look at exactly what we track in the [code](./src/ragas/
-_analytics.py) To disable usage-tracking you set the `RAGAS_DO_NOT_TRACK` flag
-to true. ## :raising_hand_man: FAQ 1. Why harmonic mean? Harmonic mean
-penalizes extreme values. For example, if your generated answer is fully
-factually consistent with the context (faithfulness = 1) but is not relevant to
-the question (relevancy = 0), a simple average would give you a score of 0.5
-but a harmonic mean will give you 0.0 2. How to use Ragas to improve your
-pipeline? *"Measurement is the first step that leads to control and eventually
-to improvement" - James Harrington* Here we assume that you already have your
-RAG pipeline ready. When it comes to RAG pipelines, there are mainly two parts
-- Retriever and generator. A change in any of this should also impact your
-pipelines's quality. 1. First, decide one parameter that you're interested in
-adjusting. for example the number of retrieved documents, K. 2. Collect a set
-of sample prompts (min 20) to form your test set. 3. Run your pipeline using
-the test set before and after the change. Each time record the prompts with
-context and generated output. 4. Run ragas evaluation for each of them to
-generate evaluation scores. 5. Compare the scores and you will know how much
-the change has affected your pipelines' performance.
+redundant information in the generated answer. 4. **Aspect Critiques**:
+Designed to judge the submission against defined aspects like harmlessness,
+correctness, etc. You can also define your own aspect and validate the
+submission against your desired aspect. The output of aspect critiques is
+always binary. The final `ragas_score` is the harmonic mean of of individual
+metric scores. To read more about our metrics, checkout [docs](/docs/
+metrics.md). ## ð« Community If you want to get more involved with Ragas,
+check out our [discord server](https://discord.gg/5djav8GGNZ). It's a fun
+community where we geek out about LLM, Retrieval, Production issues and more.
+## ð Open Analytics We track very basic usage metrics to guide us to figure
+out what our users want, what is working and what's not. As a young startup, we
+have to be brutally honest about this which is why we are tracking these
+metrics. But as an Open Startup we open-source all the data we collect. You can
+read more about this [here](https://github.com/explodinggradients/ragas/issues/
+49). **Ragas doesnot track any information that can be used to identify you or
+your company**. You can take a look at exactly what we track in the [code](./
+src/ragas/_analytics.py) To disable usage-tracking you set the
+`RAGAS_DO_NOT_TRACK` flag to true. ## :raising_hand_man: FAQ 1. Why harmonic
+mean? Harmonic mean penalizes extreme values. For example, if your generated
+answer is fully factually consistent with the context (faithfulness = 1) but is
+not relevant to the question (relevancy = 0), a simple average would give you a
+score of 0.5 but a harmonic mean will give you 0.0 2. How to use Ragas to
+improve your pipeline? *"Measurement is the first step that leads to control
+and eventually to improvement" - James Harrington* Here we assume that you
+already have your RAG pipeline ready. When it comes to RAG pipelines, there are
+mainly two parts - Retriever and generator. A change in any of this should also
+impact your pipelines's quality. 1. First, decide one parameter that you're
+interested in adjusting. for example the number of retrieved documents, K. 2.
+Collect a set of sample prompts (min 20) to form your test set. 3. Run your
+pipeline using the test set before and after the change. Each time record the
+prompts with context and generated output. 4. Run ragas evaluation for each of
+them to generate evaluation scores. 5. Compare the scores and you will know how
+much the change has affected your pipelines' performance.
```

### Comparing `ragas-0.0.7/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.8/src/ragas.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -25,22 +25,26 @@
 src/ragas/__init__.py
 src/ragas/_analytics.py
 src/ragas/_version.py
 src/ragas/async_utils.py
 src/ragas/evaluation.py
 src/ragas/exceptions.py
 src/ragas/utils.py
+src/ragas/validation.py
 src/ragas.egg-info/PKG-INFO
 src/ragas.egg-info/SOURCES.txt
 src/ragas.egg-info/dependency_links.txt
 src/ragas.egg-info/requires.txt
 src/ragas.egg-info/top_level.txt
 src/ragas/metrics/__init__.py
 src/ragas/metrics/answer_relevance.py
 src/ragas/metrics/base.py
 src/ragas/metrics/context_relevance.py
+src/ragas/metrics/critique.py
 src/ragas/metrics/faithfulnes.py
 src/ragas/metrics/llms.py
+tests/.DS_Store
 tests/benchmarks/benchmark_eval.py
 tests/benchmarks/utils.py
 tests/unit/test_metric.py
-tests/unit/test_simple.py
+tests/unit/test_simple.py
+tests/unit/test_validation.py
```

### Comparing `ragas-0.0.7/tests/benchmarks/utils.py` & `ragas-0.0.8/tests/benchmarks/utils.py`

 * *Files identical despite different names*

