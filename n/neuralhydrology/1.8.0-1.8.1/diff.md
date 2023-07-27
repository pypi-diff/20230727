# Comparing `tmp/neuralhydrology-1.8.0.tar.gz` & `tmp/neuralhydrology-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralhydrology-1.8.0.tar", last modified: Fri Jul  7 11:06:08 2023, max compression
+gzip compressed data, was "neuralhydrology-1.8.1.tar", last modified: Thu Jul 27 20:17:35 2023, max compression
```

## Comparing `neuralhydrology-1.8.0.tar` & `neuralhydrology-1.8.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.938261 neuralhydrology-1.8.0/neuralhydrology/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45263 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/basedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsaus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelscl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/genericdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/hourlycamelsus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/lamah.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datasetzoo/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/datautils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/climateindices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/dischargeinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/pet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/datautils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.942261 neuralhydrology-1.8.0/neuralhydrology/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    28418 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/modelzoo/
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/arlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/cudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/customlstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/ealstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/embcudalstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/fc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/gru.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10145 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/handoff_forecast_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/head.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/inputlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/mclstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/mtslstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/multihead_forecast_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/odelstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/sequential_forecast_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/stacked_forecast_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/modelzoo/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/nh_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/nh_run_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/training/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/basetrainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/training/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/neuralhydrology/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29390 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/configutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/nh_results_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/ratingcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    32397 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/neuralhydrology/utils/samplingutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.938261 neuralhydrology-1.8.0/neuralhydrology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 11:06:08.000000 neuralhydrology-1.8.0/neuralhydrology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:06:08.946261 neuralhydrology-1.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_config_runs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_custom_lstm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-07 11:05:59.000000 neuralhydrology-1.8.0/test/test_mclstm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.592443 neuralhydrology-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-27 20:17:35.588443 neuralhydrology-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.580443 neuralhydrology-1.8.1/neuralhydrology/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.584443 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45263 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/basedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsaus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelscl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/genericdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/hourlycamelsus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13428 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datasetzoo/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.584443 neuralhydrology-1.8.1/neuralhydrology/datautils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datautils/climateindices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datautils/dischargeinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datautils/pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/datautils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.584443 neuralhydrology-1.8.1/neuralhydrology/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.588443 neuralhydrology-1.8.1/neuralhydrology/modelzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/arlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/cudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/customlstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/ealstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/embcudalstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/gru.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10145 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/handoff_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/inputlayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/mclstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/mtslstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/multihead_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/odelstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/sequential_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/stacked_forecast_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/modelzoo/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/nh_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/nh_run_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.588443 neuralhydrology-1.8.1/neuralhydrology/training/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/basetrainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17483 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/training/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.588443 neuralhydrology-1.8.1/neuralhydrology/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29390 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/configutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/nh_results_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/ratingcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34129 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/neuralhydrology/utils/samplingutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.580443 neuralhydrology-1.8.1/neuralhydrology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 20:17:35.000000 neuralhydrology-1.8.1/neuralhydrology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 20:17:35.592443 neuralhydrology-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 20:17:35.588443 neuralhydrology-1.8.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/test/test_config_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/test/test_custom_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/test/test_datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 20:17:27.000000 neuralhydrology-1.8.1/test/test_mclstm.py
```

### Comparing `neuralhydrology-1.8.0/LICENSE` & `neuralhydrology-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/PKG-INFO` & `neuralhydrology-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.8.0
+Version: 1.8.1
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.8.0/README.md` & `neuralhydrology-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/__init__.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/basedataset.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/basedataset.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsaus.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsaus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsbr.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsbr.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelscl.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelscl.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsgb.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsgb.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/camelsus.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/camelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/caravan.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/caravan.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/genericdataset.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/genericdataset.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/hourlycamelsus.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/hourlycamelsus.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/lamah.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/lamah.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datasetzoo/template.py` & `neuralhydrology-1.8.1/neuralhydrology/datasetzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datautils/climateindices.py` & `neuralhydrology-1.8.1/neuralhydrology/datautils/climateindices.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datautils/dischargeinput.py` & `neuralhydrology-1.8.1/neuralhydrology/datautils/dischargeinput.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datautils/pet.py` & `neuralhydrology-1.8.1/neuralhydrology/datautils/pet.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/datautils/utils.py` & `neuralhydrology-1.8.1/neuralhydrology/datautils/utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/__init__.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/evaluate.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/metrics.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/plots.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/plots.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/signatures.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/signatures.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/evaluation/tester.py` & `neuralhydrology-1.8.1/neuralhydrology/evaluation/tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 import sys
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from pandas.tseries.frequencies import to_offset
 import torch
 import xarray
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from neuralhydrology.datasetzoo import get_dataset
 from neuralhydrology.datasetzoo.basedataset import BaseDataset
 from neuralhydrology.datautils.utils import get_frequency_factor, load_basin_file, sort_frequencies
 from neuralhydrology.evaluation import plots
 from neuralhydrology.evaluation.metrics import calculate_metrics, get_available_metrics
-from neuralhydrology.evaluation.utils import load_scaler, load_basin_id_encoding
+from neuralhydrology.evaluation.utils import load_scaler, load_basin_id_encoding, metrics_to_dataframe
 from neuralhydrology.modelzoo import get_model
 from neuralhydrology.modelzoo.basemodel import BaseModel
 from neuralhydrology.training import get_loss_obj, get_regularization_obj
 from neuralhydrology.training.logger import Logger
 from neuralhydrology.utils.config import Config
 from neuralhydrology.utils.errors import AllNaNError, NoEvaluationDataError
 
@@ -210,15 +209,16 @@
                     # skip basin
                     continue
                 if self.cfg.cache_validation_data and self.period == "validation":
                     self.cached_datasets[basin] = ds
 
             loader = DataLoader(ds, batch_size=self.cfg.batch_size, num_workers=0, collate_fn=ds.collate_fn)
 
-            y_hat, y, dates, all_losses, all_output[basin] = self._evaluate(model, loader, ds.frequencies, save_all_output)
+            y_hat, y, dates, all_losses, all_output[basin] = self._evaluate(model, loader, ds.frequencies,
+                                                                            save_all_output)
 
             # log loss of this basin plus number of samples in the logger to compute epoch aggregates later
             if experiment_logger is not None:
                 experiment_logger.log_step(**{k: (v, len(loader)) for k, v in all_losses.items()})
 
             predict_last_n = self.cfg.predict_last_n
             seq_length = self.cfg.seq_length
@@ -342,19 +342,15 @@
         results_to_save = None
         states_to_save = None
         if save_results:
             results_to_save = results
         if save_all_output:
             states_to_save = all_output
         if save_results or save_all_output:
-            self._save_results(
-                results=results_to_save, 
-                states=states_to_save,
-                epoch=epoch
-            )
+            self._save_results(results=results_to_save, states=states_to_save, epoch=epoch)
 
         return results
 
     def _create_and_log_figures(self, results: dict, experiment_logger: Logger, epoch: int):
         basins = list(results.keys())
         random.shuffle(basins)
         for target_var in self.cfg.target_variables:
@@ -386,15 +382,15 @@
 
         # make sure the parent directory exists
         parent_directory = self.run_dir / self.period / weight_file.stem
         parent_directory.mkdir(parents=True, exist_ok=True)
 
         # save metrics any time this funciton is called, as long as they exist
         if self.cfg.metrics:
-            df = self._metrics_to_dataframe(results)
+            df = metrics_to_dataframe(results, self.cfg.metrics)
             metrics_file = parent_directory / f"{self.period}_metrics.csv"
             df.to_csv(metrics_file)
             LOGGER.info(f"Stored metrics at {metrics_file}")
 
         # store all results packed as pickle file
         if results is not None:
             result_file = parent_directory / f"{self.period}_results.p"
@@ -405,43 +401,14 @@
         # store all model output packed as pickle file
         if states is not None:
             result_file = parent_directory / f"{self.period}_all_output.p"
             with result_file.open("wb") as fp:
                 pickle.dump(states, fp)
             LOGGER.info(f"Stored states at {result_file}")
 
-
-    def _metrics_to_dataframe(self, results: dict) -> pd.DataFrame:
-        """Extract all metric values from result dictionary and convert to pandas.DataFrame
-
-        Parameters
-        ----------
-        results: dict
-            Dictionary, containing the results of the model evaluation as returned by the `Tester.evaluate()`.
-
-        Returns
-        -------
-        A basin indexed DataFrame with one column per metric. In case of multi-frequency runs, the metric names contain
-        the corresponding frequency as a suffix.
-        """
-        metrics_dict = defaultdict(dict)
-        for basin, basin_data in results.items():
-            for freq_results in basin_data.values():
-                for metric in self.cfg.metrics:
-                    if metric in freq_results.keys():
-                        metrics_dict[basin][metric] = freq_results[metric]
-                    else:
-                        # in case the current period has no valid samples, the result dict has no metric-key
-                        metrics_dict[basin][metric] = np.nan
-
-        df = pd.DataFrame.from_dict(metrics_dict, orient="index")
-        df.index.name = "basin"
-
-        return df
-
     def _evaluate(self, model: BaseModel, loader: DataLoader, frequencies: List[str], save_all_output: bool = False):
         """Evaluate model"""
         predict_last_n = self.cfg.predict_last_n
         if isinstance(predict_last_n, int):
             predict_last_n = {frequencies[0]: predict_last_n}  # if predict_last_n is int, there's only one frequency
 
         preds, obs, dates, all_output = {}, {}, {}, {}
@@ -454,17 +421,21 @@
                         data[key] = data[key].to(self.device)
                 data = model.pre_model_hook(data, is_train=False)
                 predictions, loss = self._get_predictions_and_loss(model, data)
 
                 if all_output:
                     for key, value in predictions.items():
                         if value is not None and type(value) != dict:
-                            all_output[key].append(value.detach().cpu().numpy()) 
+                            all_output[key].append(value.detach().cpu().numpy())
                 elif save_all_output:
-                    all_output = {key: [value.detach().cpu().numpy()] for key, value in predictions.items() if value is not None and type(value) != dict}
+                    all_output = {
+                        key: [value.detach().cpu().numpy()]
+                        for key, value in predictions.items()
+                        if value is not None and type(value) != dict
+                    }
 
                 for freq in frequencies:
                     if predict_last_n[freq] == 0:
                         continue  # no predictions for this frequency
                     freq_key = '' if len(frequencies) == 1 else f'_{freq}'
                     y_hat_sub, y_sub = self._subset_targets(model, data, predictions, predict_last_n[freq], freq_key)
                     # Date subsetting is universal across all models and thus happens here.
@@ -484,24 +455,24 @@
             for freq in preds.keys():
                 preds[freq] = preds[freq].numpy()
                 obs[freq] = obs[freq].numpy()
 
         # concatenate all output variables (currently a dict-of-dicts) into a single-level dict
         for key, list_of_data in all_output.items():
             all_output[key] = np.concatenate(list_of_data, 0)
-            
+
         # set to NaN explicitly if all losses are NaN to avoid RuntimeWarning
         mean_losses = {}
         if len(losses) == 0:
             mean_losses['loss'] = np.nan
         else:
             for loss_name in losses[0].keys():
                 loss_values = [loss[loss_name] for loss in losses]
                 mean_losses[loss_name] = np.nanmean(loss_values) if not np.all(np.isnan(loss_values)) else np.nan
-        
+
         return preds, obs, dates, mean_losses, all_output
 
     def _get_predictions_and_loss(self, model: BaseModel, data: Dict[str, torch.Tensor]) -> Tuple[torch.Tensor, float]:
         predictions = model(data)
         _, all_losses = self.loss_obj(predictions, data)
         return predictions, {k: v.item() for k, v in all_losses.items()}
 
@@ -595,8 +566,7 @@
         for i, var in enumerate(self.cfg.target_variables):
             data[f"{var}_obs"] = (('date', 'time_step'), y[:, :, i])
             data[f"{var}_sim"] = (('date', 'time_step', 'samples'), y_hat[:, :, i, :])
         return data
 
     def _get_plots(self, qobs: np.ndarray, qsim: np.ndarray, title: str):
         return plots.uncertainty_plot(qobs, qsim, title)
-
```

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/__init__.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/arlstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/arlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/basemodel.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/basemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Dict, Optional, Callable
+from typing import Dict
 
 import torch
 import torch.nn as nn
 
+from neuralhydrology.evaluation.utils import load_scaler
 from neuralhydrology.utils.config import Config
 from neuralhydrology.utils.samplingutils import sample_pointpredictions, umal_extend_batch
 
 
 class BaseModel(nn.Module):
     """Abstract base model class, don't use this class for model training.
 
@@ -49,15 +50,16 @@
             Number of point predictions that ought ot be sampled form the model. 
 
         Returns
         -------
         Dict[str, torch.Tensor]
             Sampled point predictions 
         """
-        return sample_pointpredictions(self, data, n_samples)
+        scaler = load_scaler(self.cfg.run_dir)
+        return sample_pointpredictions(self, data, n_samples, scaler)
 
     def forward(self, data: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """Perform a forward pass.
 
         Parameters
         ----------
         data : Dict[str, torch.Tensor]
@@ -65,15 +67,15 @@
 
         Returns
         -------
         Dict[str, torch.Tensor]
             Model output and potentially any intermediate states and activations as a dictionary.
         """
         raise NotImplementedError
-    
+
     def pre_model_hook(self, data: Dict[str, torch.Tensor], is_train: bool) -> Dict[str, torch.Tensor]:
         """A function to execute before the model in training, validaton and test. 
         The beahvior can be adapted depending on the run configuration and the provided arguments.
 
         Parameters
         ----------
         data : Dict[str, torch.Tensor]
@@ -86,10 +88,10 @@
         data : Dict[str, torch.Tensor]
             The modified (or unmodified) data that are used for the training or evaluation.
         """
         if self.cfg.head.lower() == "umal":
             data = umal_extend_batch(data, self.cfg, n_taus=self.cfg.n_taus, extend_y=True)
         else:
             # here one can implement additional pre model hooks
-            pass 
+            pass
 
         return data
```

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/cudalstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/cudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/customlstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/customlstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/ealstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/ealstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/embcudalstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/embcudalstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/fc.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/fc.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/gru.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/gru.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/handoff_forecast_lstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/handoff_forecast_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/head.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/head.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/inputlayer.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/inputlayer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/mclstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/mclstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/mtslstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/mtslstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/multihead_forecast_lstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/multihead_forecast_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/odelstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/odelstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/sequential_forecast_lstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/sequential_forecast_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/stacked_forecast_lstm.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/stacked_forecast_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/template.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/template.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/modelzoo/transformer.py` & `neuralhydrology-1.8.1/neuralhydrology/modelzoo/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/nh_run.py` & `neuralhydrology-1.8.1/neuralhydrology/nh_run.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/nh_run_scheduler.py` & `neuralhydrology-1.8.1/neuralhydrology/nh_run_scheduler.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/__init__.py` & `neuralhydrology-1.8.1/neuralhydrology/training/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/basetrainer.py` & `neuralhydrology-1.8.1/neuralhydrology/training/basetrainer.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/logger.py` & `neuralhydrology-1.8.1/neuralhydrology/training/logger.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/loss.py` & `neuralhydrology-1.8.1/neuralhydrology/training/loss.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/regularization.py` & `neuralhydrology-1.8.1/neuralhydrology/training/regularization.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/training/train.py` & `neuralhydrology-1.8.1/neuralhydrology/training/train.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/config.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/config.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/configutils.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/configutils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/logging_utils.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/nh_results_ensemble.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/nh_results_ensemble.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import pandas as pd
 import xarray as xr
 from tqdm import tqdm
 
 sys.path.append(str(Path(__file__).parent.parent.parent))
 from neuralhydrology.datautils.utils import get_frequency_factor, sort_frequencies
 from neuralhydrology.evaluation.metrics import calculate_metrics, get_available_metrics
-from neuralhydrology.evaluation.tester import BaseTester
+from neuralhydrology.evaluation.utils import metrics_to_dataframe
 from neuralhydrology.utils.config import Config
 from neuralhydrology.utils.errors import AllNaNError
 
 
 def create_results_ensemble(run_dirs: List[Path],
                             best_k: int = None,
                             metrics: List[str] = None,
@@ -109,16 +109,17 @@
                                             end=ensemble_xr.coords['date'].values[-1] \
                                                 + pd.Timedelta(days=1, seconds=-1),
                                             freq=freq)
             mask = np.ones(frequency_factor).astype(bool)
             mask[:-len(ensemble_xr.coords['time_step'])] = False
             freq_date_range = freq_date_range[np.tile(mask, len(ensemble_xr.coords['date']))]
 
-            ensemble_xr = ensemble_xr.isel(time_step=slice(-frequency_factor, None)).stack(
-                datetime=['date', 'time_step'])
+            ensemble_xr = ensemble_xr.isel(time_step=slice(-frequency_factor, None)) \
+                .stack(datetime=['date', 'time_step']) \
+                .drop_vars({'datetime', 'date', 'time_step'})
             ensemble_xr['datetime'] = freq_date_range
             for target_var in target_vars:
                 # average predictions
                 ensemble_xr[f'{target_var}_sim'] = ensemble_xr[f'{target_var}_sim'] / len(results_files)
 
                 # clip predictions to zero
                 sim = ensemble_xr[f'{target_var}_sim']
@@ -141,31 +142,32 @@
                         + str(err)
                     print(msg)
                     ensemble_metrics = {metric: np.nan for metric in metrics}
 
                 # add variable identifier to metrics if needed
                 if len(target_vars) > 1:
                     ensemble_metrics = {f'{target_var}_{key}': val for key, val in ensemble_metrics.items()}
+                # add frequency identifier to metrics if needed
+                if len(frequencies) > 1:
+                    ensemble_metrics = {f'{key}_{freq}': val for key, val in ensemble_metrics.items()}
                 for metric, val in ensemble_metrics.items():
-                    ensemble[basin][freq][f'{metric}_{freq}'] = val
+                    ensemble[basin][freq][metric] = val
 
             ensemble[basin][freq]['xr'] = ensemble_xr
 
     return dict(ensemble)
 
 
 def _get_medians(results: dict, metric='NSE') -> dict:
     """Calculates median metric across all basins. """
     medians = {}
     key = metric
     frequencies = list(results[list(results.keys())[0]].keys())
     for freq in frequencies:
-        # if the one freq was resampled, there still is a freq suffix
-        if len(frequencies) > 1 or (len(frequencies) == 1 and
-                                    f'{metric}_{freq}' in results[list(results.keys())[0]][freq]):
+        if len(frequencies) > 1:
             key = f'{metric}_{freq}'
         metric_values = [v[freq][key] for v in results.values() if freq in v.keys() and key in v[freq].keys()]
         medians[freq] = np.nanmedian(metric_values)
 
     return medians
 
 
@@ -213,29 +215,33 @@
                         help='If provided, will only use the k results files with the best median validation NSEs.')
     parser.add_argument('--epoch',
                         type=int,
                         required=False,
                         help='If provided, will return results of this specific epoch otherwise of the last epoch')
     args = vars(parser.parse_args())
 
-    ensemble_results = create_results_ensemble([Path(f) for f in args['run_dirs']],
+    run_dirs = [Path(f) for f in args['run_dirs']]
+    ensemble_results = create_results_ensemble(run_dirs,
                                                args['best_k'],
                                                metrics=args['metrics'],
                                                period=args['period'],
                                                epoch=args['epoch'])
     output_dir = Path(args['output_dir']).absolute()
 
+    metrics = args['metrics']
+    if metrics is None:
+        metrics = Config(run_dirs[0] / 'config.yml').metrics
     try:
-        df = BaseTester.metrics_to_dataframe(ensemble_results)
+        df = metrics_to_dataframe(ensemble_results, metrics)
         file_name = output_dir / f"{args['period']}_ensemble_metrics.csv"
         df.to_csv(file_name)
         print(f"Stored metrics of ensemble run to {file_name}")
     except RuntimeError as err:
         # in case no metrics were computed
-        pass                                               
+        pass
 
     file_name = output_dir / f"{args['period']}_ensemble_results.p"
     pickle.dump(ensemble_results, open(file_name, 'wb'))
     print(f'Successfully written results to {file_name}')
 
 
 if __name__ == '__main__':
```

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/ratingcurve.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/ratingcurve.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/neuralhydrology/utils/samplingutils.py` & `neuralhydrology-1.8.1/neuralhydrology/utils/samplingutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import List, Dict, Callable
+from typing import Callable, Dict, List, Union
 
 import numpy as np
-from numba import njit
+import pandas as pd
 import torch
-from torch.distributions import Categorical, Uniform
+import xarray
+from numba import njit
+from torch.distributions import Categorical
 
 from neuralhydrology.utils.config import Config
 
 
-def sample_pointpredictions(model: 'BaseModel', data: Dict[str, torch.Tensor],
-                            n_samples: int) -> Dict[str, torch.Tensor]:
+def sample_pointpredictions(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int,
+                            scaler: Dict[str, Union[pd.Series, xarray.Dataset]]) -> Dict[str, torch.Tensor]:
     """Point prediction samplers for the different uncertainty estimation approaches.
     
     This function provides different point sampling functions for the different uncertainty estimation approaches 
     (i.e. Gaussian Mixture Models (GMM), Countable Mixtures of Asymmetric Laplacians (CMAL), Uncountable Mixtures of 
     Asymmetric Laplacians (UMAL), and Monte-Carlo Dropout (MCD); note: MCD can be combined with the others, by setting 
     `mc_dropout` to `True` in the configuration file). 
     
@@ -25,30 +27,32 @@
     ----------
     model : BaseModel
         The neuralhydrology model from which to sample from.
     data : Dict[str, torch.Tensor]
         Dictionary, containing input features as key-value pairs.
     n_samples : int
         The number of point prediction samples that should be created.
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
 
     Returns
     -------
     Dict[str, torch.Tensor]
         Dictionary, containing the sampled model outputs for the `predict_last_n` (config argument) time steps of 
         each frequency.
     """
 
     if model.cfg.head.lower() == "gmm":
-        samples = sample_gmm(model, data, n_samples)
+        samples = sample_gmm(model, data, n_samples, scaler)
     elif model.cfg.head.lower() == "cmal":
-        samples = sample_cmal(model, data, n_samples)
+        samples = sample_cmal(model, data, n_samples, scaler)
     elif model.cfg.head.lower() == "umal":
-        samples = sample_umal(model, data, n_samples)
+        samples = sample_umal(model, data, n_samples, scaler)
     elif model.cfg.head.lower() == "regression":
-        samples = sample_mcd(model, data, n_samples)  # regression head assumes mcd
+        samples = sample_mcd(model, data, n_samples, scaler)  # regression head assumes mcd
     else:
         raise NotImplementedError(f"Sampling mode not supported for head {model.cfg.head.lower()}!")
 
     return samples
 
 
 def _subset_target(parameter: Dict[str, torch.Tensor], n_target: int, steps: int) -> Dict[str, torch.Tensor]:
@@ -56,42 +60,50 @@
     start = n_target * steps
     end = (n_target + 1) * steps
     parameter_sub = parameter[:, :, start:end]
 
     return parameter_sub
 
 
-def _handle_negative_values(cfg: Config, values: torch.Tensor, sample_values: Callable) -> torch.Tensor:
+def _handle_negative_values(cfg: Config, values: torch.Tensor, sample_values: Callable,
+                            scaler: Dict[str, Union[pd.Series, xarray.Dataset]], nth_target: int) -> torch.Tensor:
     """Handle negative samples that arise while sampling from the uncertainty estimates.
 
     Currently supports (a) 'clip' for directly clipping values at zero and (b) 'truncate' for resampling values 
     that are below zero. 
 
     Parameters
     ----------
     cfg : Config
         The run configuration.
     values : torch.Tensor
         Tensor with the sampled values.
     sample_values : Callable
         Sampling function to allow for repeated sampling in the case of truncation-handling. 
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
+    nth_target : int
+        Index of the sampled target variable in cfg.target_variables.
 
     Returns
     -------
     torch.Tensor
         Bound values according to user specifications.  
     """
+    center = scaler["xarray_feature_center"][cfg.target_variables[nth_target]]
+    scale = scaler["xarray_feature_scale"][cfg.target_variables[nth_target]]
+    normalized_zero = -torch.from_numpy((center / scale).values).to(values)
     if cfg.negative_sample_handling.lower() == 'clip':
-        values = torch.relu(values)
+        values = torch.clamp(values, min=normalized_zero)
     elif cfg.negative_sample_handling.lower() == 'truncate':
-        values_smaller_zero = values < 0
+        values_smaller_zero = values < normalized_zero
         try_count = 0
-        while any(values_smaller_zero.flatten()):
+        while torch.any(values_smaller_zero.flatten()):
             values[values_smaller_zero] = sample_values(values_smaller_zero)
-            values_smaller_zero = values < 0
+            values_smaller_zero = values < normalized_zero
             try_count += 1
             if try_count >= cfg.negative_sample_max_retries:
                 break
     elif cfg.negative_sample_handling is None or cfg.negative_sample_handling.lower() == 'none':
         pass
     else:
         raise NotImplementedError(
@@ -207,15 +219,16 @@
         if isinstance(self.predict_last_n, int):
             frequency_last_n = self.predict_last_n
         else:
             frequency_last_n = self.predict_last_n[freq_suffix[1:]]
         return frequency_last_n
 
 
-def sample_mcd(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int) -> Dict[str, torch.Tensor]:
+def sample_mcd(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int,
+               scaler: Dict[str, Union[pd.Series, xarray.Dataset]]) -> Dict[str, torch.Tensor]:
     """MC-Dropout based point predictions sampling.
 
     Naive sampling. This function does `n_samples` forward passes for each sample in the batch. Currently it is 
     only useful for models with dropout, to perform MC-Dropout sampling. 
     Note: Calling this function will force the model to train mode (`model.train()`) and not set it back to its original
     state. 
 
@@ -227,14 +240,16 @@
     ----------
     model : BaseModel
         A model with a non-probabilistic head.
     data : Dict[str, torch.Tensor]
         Dictionary, containing input features as key-value pairs.
     n_samples : int
         Number of samples to generate for each input sample.
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
 
     Returns
     -------
     Dict[str, torch.Tensor]
         Dictionary, containing the sampled model outputs for the `predict_last_n` (config argument) time steps of 
         each frequency.
     """
@@ -261,25 +276,26 @@
                     target_values[ids, -frequency_last_n:, i] = value_buffer.detach().cpu()
                 return target_values
 
             ids = list(range(data[f'x_d{freq_suffix}'].shape[0]))
             values = _sample_values(ids)
 
             # bind values and add to sample_points:
-            values = _handle_negative_values(setup.cfg, values, _sample_values)
+            values = _handle_negative_values(setup.cfg, values, _sample_values, scaler, nth_target)
             sample_points.append(values)
 
         # add sample_points to dictionary of samples:
         freq_key = f'y_hat{freq_suffix}'
         samples.update({freq_key: torch.stack(sample_points, 2)})
 
     return samples
 
 
-def sample_gmm(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int) -> Dict[str, torch.Tensor]:
+def sample_gmm(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int,
+               scaler: Dict[str, Union[pd.Series, xarray.Dataset]]) -> Dict[str, torch.Tensor]:
     """Sample point predictions with the Gaussian Mixture (GMM) head.
 
     This function generates `n_samples` GMM sample points for each entry in the batch. Concretely, the model is 
     executed once (forward pass) and then the sample points are generated by sampling from the resulting mixtures. 
     Good references for learning about GMMs are [#]_ and [#]_. 
 
     The negative sample handling currently supports (a) 'clip' for directly clipping sample_points at zero and 
@@ -293,14 +309,16 @@
     ----------
     model : BaseModel
         A model with a GMM head.
     data : Dict[str, torch.Tensor]
         Dictionary, containing input features as key-value pairs.
     n_samples : int
         Number of samples to generate for each input sample.
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
 
     Returns
     -------
     Dict[str, torch.Tensor]
         Dictionary, containing the sampled model outputs for the `predict_last_n` (config argument) time steps of 
         each frequency. 
 
@@ -344,26 +362,31 @@
                 m_sub = torch.repeat_interleave(m_target[mask_nan, :, :], n_samples, dim=0)
                 s_sub = torch.repeat_interleave(s_target[mask_nan, :, :], n_samples, dim=0)
                 p_sub = torch.repeat_interleave(p_target[mask_nan, :, :], n_samples, dim=0)
 
                 # sample values, handle negatives and add to sample points:
                 values = _sample_gaussian_mixtures(np.ones(s_sub.shape, dtype=bool), m_sub, s_sub, p_sub)
                 values = _handle_negative_values(
-                    setup.cfg, values, sample_values=lambda ids: _sample_gaussian_mixtures(ids, m_sub, s_sub, p_sub))
-                values = values.view(-1, frequency_last_n, n_samples)
+                    setup.cfg,
+                    values,
+                    sample_values=lambda ids: _sample_gaussian_mixtures(ids, m_sub, s_sub, p_sub),
+                    scaler=scaler,
+                    nth_target=nth_target)
+                values = values.view(-1, n_samples, frequency_last_n).permute(0, 2, 1)
 
                 sample_points[mask_nan, :, nth_target, :] = values.detach().cpu()
 
         # add sample_points to dictionary of samples:
         freq_key = f'y_hat{freq_suffix}'
         samples.update({freq_key: sample_points})
     return samples
 
 
-def sample_cmal(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int) -> Dict[str, torch.Tensor]:
+def sample_cmal(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int,
+                scaler: Dict[str, Union[pd.Series, xarray.Dataset]]) -> Dict[str, torch.Tensor]:
     """Sample point predictions with the Countable Mixture of Asymmetric Laplacians (CMAL) head.
 
     This function generates `n_samples` CMAL sample points for each entry in the batch. Concretely, the model is 
     executed once (forward pass) and then the sample points are generated by sampling from the resulting mixtures. 
     General information about CMAL can be found in [#]_.
 
     The negative sample handling currently supports (a) 'clip' for directly clipping sample_points at zero and (b) 
@@ -377,14 +400,16 @@
     ----------
     model : BaseModel
         A model with a CMAL head.
     data : Dict[str, torch.Tensor]
         Dictionary, containing input features as key-value pairs.
     n_samples : int
         Number of samples to generate for each input sample.
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
 
     Returns
     -------
     Dict[str, torch.Tensor]
         Dictionary, containing the sampled model outputs for the `predict_last_n` (config argument) time steps of 
         each frequency. The shape of the output tensor for each frequency is 
         ``[batch size, predict_last_n, n_samples]``.
@@ -442,28 +467,31 @@
                     b_sub = b_target[mask_nan, nth_timestep, :].gather(1, sub_choices)
 
                     ids = np.ones(b_sub.shape, dtype=bool)
                     values_unbound = _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub)
                     values[mask_nan, nth_timestep] = _handle_negative_values(
                         setup.cfg,
                         values_unbound,
-                        sample_values=lambda ids: _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub))
+                        sample_values=lambda ids: _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub),
+                        scaler=scaler,
+                        nth_target=nth_target)
 
             # add the values to the sample_points:
-            values = values.reshape(-1, frequency_last_n, n_samples)
+            values = values.permute(1, 0).reshape(frequency_last_n, -1, n_samples).permute(1, 0, 2)
             values = values.detach().cpu()
             sample_points.append(values)
 
         # add sample_points to dictionary of samples:
         freq_key = f'y_hat{freq_suffix}'
         samples.update({freq_key: torch.stack(sample_points, 2)})
     return samples
 
 
-def sample_umal(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int) -> Dict[str, torch.Tensor]:
+def sample_umal(model: 'BaseModel', data: Dict[str, torch.Tensor], n_samples: int,
+                scaler: Dict[str, Union[pd.Series, xarray.Dataset]]) -> Dict[str, torch.Tensor]:
     """Sample point predictions with the Uncountable Mixture of Asymmetric Laplacians (UMAL) head.
 
     This function generates `n_samples` UMAL sample points for each entry in the batch. Concretely, the model is 
     executed once (forward pass) and then the sample points are generated by sampling from the resulting mixtures. 
     Details about the UMAL approach can be found in [#]_.
 
     The negative sample handling currently supports (a) 'clip' for directly clipping sample_points at zero and (b) 
@@ -477,14 +505,16 @@
     ----------
     model : BaseModel
         A model with an UMAL head.
     data : Dict[str, torch.Tensor]
         Dictionary, containing input features as key-value pairs.
     n_samples : int
         Number of samples to generate for each input sample.
+    scaler : Dict[str, Union[pd.Series, xarray.Dataset]]
+        Scaler of the run.
 
     Returns
     -------
     Dict[str, torch.Tensor]
         Dictionary containing the sampled model outputs for the `predict_last_n` (config argument) time steps of 
         each frequency.
 
@@ -544,15 +574,17 @@
                     t_sub = t_target[mask_nan, :, sub_choice]
 
                     ids = np.ones(b_sub.shape, dtype=bool)
                     values_unbound = _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub)
                     values = _handle_negative_values(
                         setup.cfg,
                         values_unbound,
-                        sample_values=lambda ids: _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub))
+                        sample_values=lambda ids: _sample_asymmetric_laplacians(ids, m_sub, b_sub, t_sub),
+                        scaler=scaler,
+                        nth_target=nth_target)
 
                     # add values to sample_points:
                     values = values.detach().cpu().unsqueeze(1)
                     sample_points[mask_nan, -frequency_last_n:, nth_target, nth_sample] = values
 
         # add sample_points to dictionary of samples:
         freq_key = f'y_hat{freq_suffix}'
@@ -618,16 +650,16 @@
             data[f'x_one_hot{freq_suffix}'] = data[f'x_one_hot{freq_suffix}'].repeat(n_taus, 1)
 
     return data
 
 
 @njit
 def bernoulli_subseries_sampler(
-    data: np.ndarray, 
-    missing_fraction: float, 
+    data: np.ndarray,
+    missing_fraction: float,
     mean_missing_length: float,
     start_sampling_on: bool = True,
 ) -> np.ndarray:
     """Samples a timeseries according to a pair of Bernoulli processes.
 
     The objective is to sample subsequences of a given timeseries under two criteria:
         1)  Expected long-term sample ratio (i.e., the total fraction of points in a time series 
@@ -664,40 +696,40 @@
         return np.full(data.shape, np.nan)
 
     # Check that the input data is a 1-d timeseries.
     if not (data.ndim == 1 or (data.ndim == 2 and data.shape[-1] == 1)):
         raise ValueError('Shape of timeseries data must be N or (N, 1).')
 
     # Check that the distribution parameters make sense.
-    if mean_missing_length < missing_fraction / (1-missing_fraction):
+    if mean_missing_length < missing_fraction / (1 - missing_fraction):
         raise ValueError('Incompatible distribution parameters in timeseries sampling. Must be: ',
                          'mean_missing_length >= missing_fraction / (1-missing_fraction).')
     if missing_fraction < 0 or missing_fraction > 1:
         raise ValueError('Missing fraction must be in [0,1]')
-    
+
     if mean_missing_length <= 0:
         raise ValueError('Mean missing length must be > 0.')
 
     # Derive Bernoulli rate parameters.
     on_shift_rate = 1 / mean_missing_length
-    off_shift_rate = on_shift_rate * missing_fraction / (1-missing_fraction)
+    off_shift_rate = on_shift_rate * missing_fraction / (1 - missing_fraction)
 
     # Initialize storage for the samples.
     sampled_data = np.full(data.shape, np.nan)
     sampled_data[0] = data[0]
     if not start_sampling_on:
-      sampled_data[0] = np.nan
+        sampled_data[0] = np.nan
 
     # Bernoulli sampling.
     up_switches = np.random.binomial(n=1, p=on_shift_rate, size=data.shape)
     down_switches = np.random.binomial(n=1, p=off_shift_rate, size=data.shape)
 
     # Sampling -> stochastic process.
     for n in range(1, len(data)):
-        if np.isnan(sampled_data[n-1]):
+        if np.isnan(sampled_data[n - 1]):
             if up_switches[n]:
                 sampled_data[n] = data[n]
         else:
             if not down_switches[n]:
                 sampled_data[n] = data[n]
 
     return sampled_data
```

### Comparing `neuralhydrology-1.8.0/neuralhydrology.egg-info/PKG-INFO` & `neuralhydrology-1.8.1/neuralhydrology.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralhydrology
-Version: 1.8.0
+Version: 1.8.1
 Summary: Library for training deep learning models with environmental focus
 Home-page: https://neuralhydrology.readthedocs.io
 Author: Frederik Kratzert, Daniel Klotz, Martin Gauch
 Author-email: neuralhydrology@googlegroups.com
 Project-URL: Documentation, https://neuralhydrology.readthedocs.io
 Project-URL: Source, https://github.com/neuralhydrology/neuralhydrology
 Project-URL: Research Blog, https://neuralhydrology.github.io/
```

### Comparing `neuralhydrology-1.8.0/neuralhydrology.egg-info/SOURCES.txt` & `neuralhydrology-1.8.1/neuralhydrology.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/setup.py` & `neuralhydrology-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/test/test_config_runs.py` & `neuralhydrology-1.8.1/test/test_config_runs.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/test/test_custom_lstm.py` & `neuralhydrology-1.8.1/test/test_custom_lstm.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/test/test_datautils.py` & `neuralhydrology-1.8.1/test/test_datautils.py`

 * *Files identical despite different names*

### Comparing `neuralhydrology-1.8.0/test/test_mclstm.py` & `neuralhydrology-1.8.1/test/test_mclstm.py`

 * *Files identical despite different names*

