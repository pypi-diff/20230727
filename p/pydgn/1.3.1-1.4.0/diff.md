# Comparing `tmp/pydgn-1.3.1.tar.gz` & `tmp/pydgn-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgn-1.3.1.tar", last modified: Thu Mar 23 08:30:09 2023, max compression
+gzip compressed data, was "pydgn-1.4.0.tar", last modified: Thu Jul 27 15:08:04 2023, max compression
```

## Comparing `pydgn-1.3.1.tar` & `pydgn-1.4.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-03-23 08:30:00.000000 pydgn-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-23 08:30:09.803185 pydgn-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-03-23 08:30:00.000000 pydgn-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.795185 pydgn-1.3.1/pydgn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/build_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29522 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    40974 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/provider.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/data/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/random_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/evaluation/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/experiment/semi_supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/experiment/supervised_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/experiment/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/launch_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/log/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/log/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/model/dgn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/dgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/dgn/toy_dgn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/dgn/toy_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.799185 pydgn-1.3.1/pydgn/model/readout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/readout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/readout/graph_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/readout/link_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/model/readout/node_readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/pydgn/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/pydgn/training/callback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/engine_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)    47277 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/callback/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/pydgn/training/event/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/event/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/event/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-23 08:30:00.000000 pydgn-1.3.1/pydgn/training/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.795185 pydgn-1.3.1/pydgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 08:30:09.000000 pydgn-1.3.1/pydgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 08:30:00.000000 pydgn-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-23 08:30:09.803185 pydgn-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-23 08:30:00.000000 pydgn-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/data/test_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/data/test_data_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/evaluation/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/evaluation/test_search_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/integration/test_full_experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:09.803185 pydgn-1.3.1/tests/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/training/test_early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-03-23 08:30:00.000000 pydgn-1.3.1/tests/training/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1520 2023-07-27 15:07:53.000000 pydgn-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 15:08:04.684171 pydgn-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-27 15:07:53.000000 pydgn-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.676171 pydgn-1.4.0/pydgn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/build_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29659 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40974 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/provider.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41773 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/data/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39694 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/random_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/evaluation/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17012 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/semi_supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/supervised_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/experiment/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/launch_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/log/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/log/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1090 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/dgn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/toy_dgn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/dgn/toy_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/model/readout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/graph_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/link_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/model/readout/node_readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.680171 pydgn-1.4.0/pydgn/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/pydgn/training/callback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/engine_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47277 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/callback/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/pydgn/training/event/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/event/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-27 15:07:53.000000 pydgn-1.4.0/pydgn/training/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.676171 pydgn-1.4.0/pydgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:08:04.000000 pydgn-1.4.0/pydgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 15:07:53.000000 pydgn-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-27 15:08:04.684171 pydgn-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-27 15:07:53.000000 pydgn-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/test_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/data/test_data_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/evaluation/test_search_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/integration/test_full_experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:08:04.684171 pydgn-1.4.0/tests/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/test_early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-27 15:07:53.000000 pydgn-1.4.0/tests/training/test_metric.py
```

### Comparing `pydgn-1.3.1/LICENSE` & `pydgn-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/PKG-INFO` & `pydgn-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Python Package for Deep Graph Networks
 Home-page: https://pydgn.readthedocs.io/en/latest/
 Author: Federico Errica
 Author-email: f.errica@protonmail.com
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydgn-1.3.1/README.md` & `pydgn-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/build_dataset.py` & `pydgn-1.4.0/pydgn/build_dataset.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/data/dataset.py` & `pydgn-1.4.0/pydgn/data/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import torch
 import torch_geometric
 from ogb.graphproppred import PygGraphPropPredDataset
 from ogb.utils.url import decide_download, download_url, extract_zip
 from torch_geometric.data import InMemoryDataset, Data, Batch
 from torch_geometric.datasets import TUDataset, Planetoid
-from torch_geometric_temporal import ChickenpoxDatasetLoader
+# from torch_geometric_temporal import ChickenpoxDatasetLoader
 
 
 class ZipDataset(torch.utils.data.Dataset):
     r"""
     This Dataset takes `n` datasets and "zips" them. When asked for the `i`-th
     element, it returns the `i`-th element of all `n` datasets.
 
@@ -861,80 +861,80 @@
                         y=torch.zeros(1, 1),
                         edge_index=torch.zeros(2, 1).long(),
                     )
                 )
             torch.save(fake_graphs, self.processed_paths[i])
 
 
-class ChickenpoxDatasetInterface(TemporalDatasetInterface):
-    r"""
-    Class that acts as wrapper to Pytorch Geometric Temporal Chickenpox dataset
-
-    Args:
-        root (Union[str,Path]): root data folder
-        name (str): name of the dataset
-        lags: (how many original timesteps to aggregate into
-            a single time step)
-        kwargs: optional additional parameters to `ChickenpoxDatasetLoader`
-            (from PyG Temporal)
-    """
-
-    def __init__(self, root, name, lags=4, **kwargs):
-        super().__init__(root, name, **kwargs)
-
-        self.lags = lags
-        self.dataset = ChickenpoxDatasetLoader().get_dataset(lags=lags)
-
-    def get_mask(self, data):
-        """
-        Computes the mask of time steps for which we need to make a prediction.
-        In this case data is a Data object containing a snapshot of a
-        single graph sequence, and the task is node classification
-        at each time step
-
-        Args:
-            data: the data object
-
-        Returns:
-            A tensor indicating the time-steps at which we expect predictions
-        """
-        mask = torch.ones((1, 1))  # time_steps x 1
-        return mask
-
-    @property
-    def dim_node_features(self) -> int:
-        r"""
-        Specifies the number of node features (after pre-processing, but in
-        the end it depends on the model that is implemented).
-        """
-        return self.dataset.features[0].shape[1]
-
-    @property
-    def dim_edge_features(self) -> int:
-        r"""
-        Specifies the number of edge features (after pre-processing, but in
-        the end it depends on the model that is implemented).
-        """
-        return 0
-
-    @property
-    def dim_target(self) -> int:
-        r"""
-        Specifies the dimension of each target vector.
-        """
-        return 1
-
-    def len(self):
-        r"""
-        Returns the number of graphs stored in the dataset.
-        Note: we need to implement both `len` and `__len__` to comply with
-        PyG interface
-        """
-        return len(self)
-
-    def __len__(self):
-        r"""
-        Returns the number of graphs stored in the dataset.
-        Note: we need to implement both `len` and `__len__` to comply with
-        PyG interface
-        """
-        return len(self.dataset.features)  # see DynamicGraphTemporalSignal
+# class ChickenpoxDatasetInterface(TemporalDatasetInterface):
+#     r"""
+#     Class that acts as wrapper to Pytorch Geometric Temporal Chickenpox dataset
+#
+#     Args:
+#         root (Union[str,Path]): root data folder
+#         name (str): name of the dataset
+#         lags: (how many original timesteps to aggregate into
+#             a single time step)
+#         kwargs: optional additional parameters to `ChickenpoxDatasetLoader`
+#             (from PyG Temporal)
+#     """
+#
+#     def __init__(self, root, name, lags=4, **kwargs):
+#         super().__init__(root, name, **kwargs)
+#
+#         self.lags = lags
+#         self.dataset = ChickenpoxDatasetLoader().get_dataset(lags=lags)
+#
+#     def get_mask(self, data):
+#         """
+#         Computes the mask of time steps for which we need to make a prediction.
+#         In this case data is a Data object containing a snapshot of a
+#         single graph sequence, and the task is node classification
+#         at each time step
+#
+#         Args:
+#             data: the data object
+#
+#         Returns:
+#             A tensor indicating the time-steps at which we expect predictions
+#         """
+#         mask = torch.ones((1, 1))  # time_steps x 1
+#         return mask
+#
+#     @property
+#     def dim_node_features(self) -> int:
+#         r"""
+#         Specifies the number of node features (after pre-processing, but in
+#         the end it depends on the model that is implemented).
+#         """
+#         return self.dataset.features[0].shape[1]
+#
+#     @property
+#     def dim_edge_features(self) -> int:
+#         r"""
+#         Specifies the number of edge features (after pre-processing, but in
+#         the end it depends on the model that is implemented).
+#         """
+#         return 0
+#
+#     @property
+#     def dim_target(self) -> int:
+#         r"""
+#         Specifies the dimension of each target vector.
+#         """
+#         return 1
+#
+#     def len(self):
+#         r"""
+#         Returns the number of graphs stored in the dataset.
+#         Note: we need to implement both `len` and `__len__` to comply with
+#         PyG interface
+#         """
+#         return len(self)
+#
+#     def __len__(self):
+#         r"""
+#         Returns the number of graphs stored in the dataset.
+#         Note: we need to implement both `len` and `__len__` to comply with
+#         PyG interface
+#         """
+#         return len(self.dataset.features)  # see DynamicGraphTemporalSignal
```

### Comparing `pydgn-1.3.1/pydgn/data/provider.py` & `pydgn-1.4.0/pydgn/data/provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/data/sampler.py` & `pydgn-1.4.0/pydgn/data/sampler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/data/splitter.py` & `pydgn-1.4.0/pydgn/data/splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/data/transform.py` & `pydgn-1.4.0/pydgn/data/transform.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/data/util.py` & `pydgn-1.4.0/pydgn/data/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/evaluation/config.py` & `pydgn-1.4.0/pydgn/evaluation/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from collections import KeysView, ItemsView
 
 
 class Config:
     r"""
     Simple class to manage the configuration dictionary as a Python object
     with fields.
 
@@ -54,24 +53,24 @@
             default (`object`): the default object
 
         Returns:
             a value from the dictionaryu
         """
         return self.config_dict.get(key, default)
 
-    def keys(self) -> KeysView:
+    def keys(self):
         r"""
         Invokes the `keys()` method of the configuration dictionary
 
         Returns:
             the set of keys in the dictionary
         """
         return self.config_dict.keys()
 
-    def items(self) -> ItemsView:
+    def items(self):
         r"""
         Invokes the `items()` method of the configuration dictionary
 
         Returns:
             a list of (key, value) pairs
         """
         return self.config_dict.items()
```

### Comparing `pydgn-1.3.1/pydgn/evaluation/evaluator.py` & `pydgn-1.4.0/pydgn/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/evaluation/grid.py` & `pydgn-1.4.0/pydgn/evaluation/grid.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/evaluation/random_search.py` & `pydgn-1.4.0/pydgn/evaluation/random_search.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/evaluation/util.py` & `pydgn-1.4.0/pydgn/evaluation/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/experiment/experiment.py` & `pydgn-1.4.0/pydgn/experiment/experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/experiment/semi_supervised_task.py` & `pydgn-1.4.0/pydgn/experiment/semi_supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/experiment/supervised_task.py` & `pydgn-1.4.0/pydgn/experiment/supervised_task.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/launch_experiment.py` & `pydgn-1.4.0/pydgn/launch_experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/log/logger.py` & `pydgn-1.4.0/pydgn/log/logger.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/model/dgn/toy_dgn.py` & `pydgn-1.4.0/pydgn/model/dgn/toy_dgn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional, Tuple, Union
 
 import torch
 from torch import nn
 from torch_geometric.data import Batch, Data
 from torch_geometric.nn import SAGEConv
-from torch_geometric_temporal import DCRNN
+# from torch_geometric_temporal import DCRNN
 
 from pydgn.model.interface import ModelInterface
 
 
 class ToyDGN(ModelInterface):
     """
     A toy Deep Graph Network used to test the library
@@ -77,70 +77,70 @@
             x_all.append(x)
 
         node_embs = torch.cat(x_all, dim=1)
 
         return self.readout(node_embs, batch, **dict(edge_index=edge_index))
 
 
-class ToyDGNTemporal(ModelInterface):
-    """
-    Simple Temporal Deep Graph Network that can be used to test the library
-    """
-
-    def __init__(
-        self,
-        dim_node_features,
-        dim_edge_features,
-        dim_target,
-        readout_class,
-        config,
-    ):
-        super().__init__(
-            dim_node_features,
-            dim_edge_features,
-            dim_target,
-            readout_class,
-            config,
-        )
-
-        self.dim_embedding = 32
-        filter_size = 1
-
-        self.model = DCRNN(dim_node_features, self.dim_embedding, filter_size)
-        self.linear = nn.Linear(self.dim_embedding, self.dim_embedding)
-
-        self.readout = readout_class(
-            dim_node_features=self.dim_embedding,
-            dim_edge_features=dim_edge_features,
-            dim_target=dim_target,
-            config=config,
-        )
-
-    def forward(self, snapshot: Union[Data, Batch], prev_state=None):
-        """
-        Implements an Toy Temporal DGN with some DCRNN graph
-        convolutional layers.
-
-        Args:
-            snapshot (`Union[Data, Batch]`): a graph or batch of graphs
-                at timestep t
-            prev_state (`torch.Tensor`): hidden state of the model
-                (previous time step)
-
-        Returns:
-            the output depends on the readout passed to the model as argument.
-        """
-        # snapshot.x: Tensor of size (num_nodes_t x node_ft_size)
-        # snapshot.edge_index: Adj of size (num_nodes_t x num_nodes_t)
-        x, edge_index, mask = (
-            snapshot.x,
-            snapshot.edge_index,
-            snapshot.time_prediction_mask,
-        )
-
-        h = self.model(x, edge_index, H=prev_state)
-        h = torch.relu(h)
-
-        # Node predictors assume the embedding is in field "x"
-        out, _ = self.readout(h, snapshot.batch)
-
-        return out, h
+# class ToyDGNTemporal(ModelInterface):
+#     """
+#     Simple Temporal Deep Graph Network that can be used to test the library
+#     """
+#
+#     def __init__(
+#         self,
+#         dim_node_features,
+#         dim_edge_features,
+#         dim_target,
+#         readout_class,
+#         config,
+#     ):
+#         super().__init__(
+#             dim_node_features,
+#             dim_edge_features,
+#             dim_target,
+#             readout_class,
+#             config,
+#         )
+#
+#         self.dim_embedding = 32
+#         filter_size = 1
+#
+#         self.model = DCRNN(dim_node_features, self.dim_embedding, filter_size)
+#         self.linear = nn.Linear(self.dim_embedding, self.dim_embedding)
+#
+#         self.readout = readout_class(
+#             dim_node_features=self.dim_embedding,
+#             dim_edge_features=dim_edge_features,
+#             dim_target=dim_target,
+#             config=config,
+#         )
+#
+#     def forward(self, snapshot: Union[Data, Batch], prev_state=None):
+#         """
+#         Implements an Toy Temporal DGN with some DCRNN graph
+#         convolutional layers.
+#
+#         Args:
+#             snapshot (`Union[Data, Batch]`): a graph or batch of graphs
+#                 at timestep t
+#             prev_state (`torch.Tensor`): hidden state of the model
+#                 (previous time step)
+#
+#         Returns:
+#             the output depends on the readout passed to the model as argument.
+#         """
+#         # snapshot.x: Tensor of size (num_nodes_t x node_ft_size)
+#         # snapshot.edge_index: Adj of size (num_nodes_t x num_nodes_t)
+#         x, edge_index, mask = (
+#             snapshot.x,
+#             snapshot.edge_index,
+#             snapshot.time_prediction_mask,
+#         )
+#
+#         h = self.model(x, edge_index, H=prev_state)
+#         h = torch.relu(h)
+#
+#         # Node predictors assume the embedding is in field "x"
+#         out, _ = self.readout(h, snapshot.batch)
+#
+#         return out, h
```

### Comparing `pydgn-1.3.1/pydgn/model/dgn/toy_mlp.py` & `pydgn-1.4.0/pydgn/model/dgn/toy_mlp.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/model/interface.py` & `pydgn-1.4.0/pydgn/model/interface.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/model/readout/graph_readout.py` & `pydgn-1.4.0/pydgn/model/readout/graph_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/model/readout/link_readout.py` & `pydgn-1.4.0/pydgn/model/readout/link_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/model/readout/node_readout.py` & `pydgn-1.4.0/pydgn/model/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/static.py` & `pydgn-1.4.0/pydgn/static.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/early_stopping.py` & `pydgn-1.4.0/pydgn/training/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/engine_callback.py` & `pydgn-1.4.0/pydgn/training/callback/engine_callback.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/gradient_clipping.py` & `pydgn-1.4.0/pydgn/training/callback/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/metric.py` & `pydgn-1.4.0/pydgn/training/callback/metric.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/optimizer.py` & `pydgn-1.4.0/pydgn/training/callback/optimizer.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/plotter.py` & `pydgn-1.4.0/pydgn/training/callback/plotter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/callback/scheduler.py` & `pydgn-1.4.0/pydgn/training/callback/scheduler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/engine.py` & `pydgn-1.4.0/pydgn/training/engine.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/event/dispatcher.py` & `pydgn-1.4.0/pydgn/training/event/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/event/handler.py` & `pydgn-1.4.0/pydgn/training/event/handler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/event/state.py` & `pydgn-1.4.0/pydgn/training/event/state.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/profiler.py` & `pydgn-1.4.0/pydgn/training/profiler.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn/training/util.py` & `pydgn-1.4.0/pydgn/training/util.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/pydgn.egg-info/PKG-INFO` & `pydgn-1.4.0/pydgn.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydgn
-Version: 1.3.1
+Version: 1.4.0
 Summary: A Python Package for Deep Graph Networks
 Home-page: https://pydgn.readthedocs.io/en/latest/
 Author: Federico Errica
 Author-email: f.errica@protonmail.com
 Keywords: deep-graph-networks,evaluation-framework,deep-learning-for-graphs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pydgn-1.3.1/pydgn.egg-info/SOURCES.txt` & `pydgn-1.4.0/pydgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/setup.py` & `pydgn-1.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "1.3.1"
+__version__ = "1.4.0"
 
 URL = "https://pydgn.readthedocs.io/en/latest/"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
@@ -23,23 +23,22 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX :: Linux",
     ],
     python_requires=">=3.8,<3.10",
     install_requires=[
-        "PyYAML >= 5.4",
+        "PyYAML == 6.0",
         "requests >= 2.22.0",
         "tensorboard <= 2.11.0",
         "tqdm >= 4.47.0",
         "ogb <= 1.3.3, < 1.4.0",
         "protobuf == 3.20.3",
         "click <= 8.0.4",
-        "ray == 2.1.0",
+        "ray == 2.6.0",
         "gpustat >= 1.0.0",
         "torch <= 1.13.0",
-        "torch-geometric <= 2.1.0.post1",
-        "torch-geometric-temporal <= 0.54.0",
+        "torch-geometric <= 2.3.0",
         "wandb >= 0.12.15",
     ],
     packages=setuptools.find_packages(),
 )
```

### Comparing `pydgn-1.3.1/tests/data/test_data_provider.py` & `pydgn-1.4.0/tests/data/test_data_provider.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/data/test_data_splitter.py` & `pydgn-1.4.0/tests/data/test_data_splitter.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/evaluation/test_evaluator.py` & `pydgn-1.4.0/tests/evaluation/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/evaluation/test_search_method.py` & `pydgn-1.4.0/tests/evaluation/test_search_method.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/integration/test_full_experiment.py` & `pydgn-1.4.0/tests/integration/test_full_experiment.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/training/test_early_stopping.py` & `pydgn-1.4.0/tests/training/test_early_stopping.py`

 * *Files identical despite different names*

### Comparing `pydgn-1.3.1/tests/training/test_metric.py` & `pydgn-1.4.0/tests/training/test_metric.py`

 * *Files identical despite different names*

