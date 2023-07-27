# Comparing `tmp/pydgn-1.4.0.tar.gz` & `tmp/pydgn-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgn-1.4.0.tar", last modified: Thu Jul 27 15:08:04 2023, max compression
+gzip compressed data, was "pydgn-1.4.1.tar", last modified: Thu Jul 27 15:56:37 2023, max compression
```

## Comparing `pydgn-1.4.0.tar` & `pydgn-1.4.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-07-27 15:07:53.000000 pydgn-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 15:08:04.684171 pydgn-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-27 15:07:53.000000 pydgn-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.676171 pydgn-1.4.0/pydgn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/build_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29659 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    40974 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/provider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/semi_supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/launch_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/log/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/log/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/dgn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/toy_dgn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/toy_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/readout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/graph_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/link_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/node_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/pydgn/training/callback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/engine_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)    47277 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/pydgn/training/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.676171 pydgn-1.4.0/pydgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 15:07:53.000000 pydgn-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-27 15:08:04.684171 pydgn-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 15:07:53.000000 pydgn-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/test_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/test_data_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/test_search_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/integration/test_full_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-07-27 15:56:22.000000 pydgn-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-27 15:56:37.456648 pydgn-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-27 15:56:22.000000 pydgn-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.448648 pydgn-1.4.1/pydgn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/build_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.448648 pydgn-1.4.1/pydgn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29659 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40974 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/evaluation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/experiment/semi_supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/experiment/supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/experiment/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/launch_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/log/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/log/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/model/dgn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/dgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/dgn/toy_dgn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/dgn/toy_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/model/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/readout/graph_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/readout/link_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/model/readout/node_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.452648 pydgn-1.4.1/pydgn/training/callback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/engine_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47277 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/callback/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/pydgn/training/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/event/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/event/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 15:56:22.000000 pydgn-1.4.1/pydgn/training/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.448648 pydgn-1.4.1/pydgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:56:37.000000 pydgn-1.4.1/pydgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 15:56:22.000000 pydgn-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-27 15:56:37.456648 pydgn-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-27 15:56:22.000000 pydgn-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/data/test_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/data/test_data_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/evaluation/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/evaluation/test_search_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/integration/test_full_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:37.456648 pydgn-1.4.1/tests/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/training/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-27 15:56:22.000000 pydgn-1.4.1/tests/training/test_metric.py
```

### Comparing `pydgn-1.4.0/LICENSE` & `pydgn-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/PKG-INFO` & `pydgn-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python Package for Deep Graph Networks
 Home-page: https://pydgn.readthedocs.io/en/latest/
 Author: Federico Errica
 Author-email: f.errica@protonmail.com
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8,<=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydgn-1.4.0/README.md` & `pydgn-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/build_dataset.py` & `pydgn-1.4.1/pydgn/build_dataset.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/dataset.py` & `pydgn-1.4.1/pydgn/data/dataset.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/provider.py` & `pydgn-1.4.1/pydgn/data/provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/sampler.py` & `pydgn-1.4.1/pydgn/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/splitter.py` & `pydgn-1.4.1/pydgn/data/splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/transform.py` & `pydgn-1.4.1/pydgn/data/transform.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/data/util.py` & `pydgn-1.4.1/pydgn/data/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/evaluation/config.py` & `pydgn-1.4.1/pydgn/evaluation/config.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/evaluation/evaluator.py` & `pydgn-1.4.1/pydgn/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/evaluation/grid.py` & `pydgn-1.4.1/pydgn/evaluation/grid.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/evaluation/random_search.py` & `pydgn-1.4.1/pydgn/evaluation/random_search.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/evaluation/util.py` & `pydgn-1.4.1/pydgn/evaluation/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/experiment/experiment.py` & `pydgn-1.4.1/pydgn/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/experiment/semi_supervised_task.py` & `pydgn-1.4.1/pydgn/experiment/semi_supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/experiment/supervised_task.py` & `pydgn-1.4.1/pydgn/experiment/supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/launch_experiment.py` & `pydgn-1.4.1/pydgn/launch_experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/log/logger.py` & `pydgn-1.4.1/pydgn/log/logger.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/dgn/toy_dgn.py` & `pydgn-1.4.1/pydgn/model/dgn/toy_dgn.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/dgn/toy_mlp.py` & `pydgn-1.4.1/pydgn/model/dgn/toy_mlp.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/interface.py` & `pydgn-1.4.1/pydgn/model/interface.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/readout/graph_readout.py` & `pydgn-1.4.1/pydgn/model/readout/graph_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/readout/link_readout.py` & `pydgn-1.4.1/pydgn/model/readout/link_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/model/readout/node_readout.py` & `pydgn-1.4.1/pydgn/model/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/static.py` & `pydgn-1.4.1/pydgn/static.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/early_stopping.py` & `pydgn-1.4.1/pydgn/training/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/engine_callback.py` & `pydgn-1.4.1/pydgn/training/callback/engine_callback.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/gradient_clipping.py` & `pydgn-1.4.1/pydgn/training/callback/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/metric.py` & `pydgn-1.4.1/pydgn/training/callback/metric.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/optimizer.py` & `pydgn-1.4.1/pydgn/training/callback/optimizer.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/plotter.py` & `pydgn-1.4.1/pydgn/training/callback/plotter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/callback/scheduler.py` & `pydgn-1.4.1/pydgn/training/callback/scheduler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/engine.py` & `pydgn-1.4.1/pydgn/training/engine.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/event/dispatcher.py` & `pydgn-1.4.1/pydgn/training/event/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/event/handler.py` & `pydgn-1.4.1/pydgn/training/event/handler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/event/state.py` & `pydgn-1.4.1/pydgn/training/event/state.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/profiler.py` & `pydgn-1.4.1/pydgn/training/profiler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn/training/util.py` & `pydgn-1.4.1/pydgn/training/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/pydgn.egg-info/PKG-INFO` & `pydgn-1.4.1/pydgn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Python Package for Deep Graph Networks
 Home-page: https://pydgn.readthedocs.io/en/latest/
 Author: Federico Errica
 Author-email: f.errica@protonmail.com
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8,<3.10
+Requires-Python: >=3.8,<=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pydgn-1.4.0/pydgn.egg-info/SOURCES.txt` & `pydgn-1.4.1/pydgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/setup.py` & `pydgn-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 URL = "https://pydgn.readthedocs.io/en/latest/"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
@@ -21,15 +21,15 @@
         "deep-learning-for-graphs",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires=">=3.8,<3.10",
+    python_requires=">=3.8,<=3.11",
     install_requires=[
         "PyYAML == 6.0",
         "requests >= 2.22.0",
         "tensorboard <= 2.11.0",
         "tqdm >= 4.47.0",
         "ogb <= 1.3.3, < 1.4.0",
         "protobuf == 3.20.3",
```

### Comparing `pydgn-1.4.0/tests/data/test_data_provider.py` & `pydgn-1.4.1/tests/data/test_data_provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/data/test_data_splitter.py` & `pydgn-1.4.1/tests/data/test_data_splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/evaluation/test_evaluator.py` & `pydgn-1.4.1/tests/evaluation/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/evaluation/test_search_method.py` & `pydgn-1.4.1/tests/evaluation/test_search_method.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/integration/test_full_experiment.py` & `pydgn-1.4.1/tests/integration/test_full_experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/training/test_early_stopping.py` & `pydgn-1.4.1/tests/training/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.4.0/tests/training/test_metric.py` & `pydgn-1.4.1/tests/training/test_metric.py`

 * *Files identical despite different names*

