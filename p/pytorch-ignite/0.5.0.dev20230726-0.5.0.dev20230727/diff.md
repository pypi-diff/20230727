# Comparing `tmp/pytorch-ignite-0.5.0.dev20230726.tar.gz` & `tmp/pytorch-ignite-0.5.0.dev20230727.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.5.0.dev20230726.tar", last modified: Wed Jul 26 00:16:28 2023, max compression
+gzip compressed data, was "pytorch-ignite-0.5.0.dev20230727.tar", last modified: Thu Jul 27 00:16:09 2023, max compression
```

## Comparing `pytorch-ignite-0.5.0.dev20230726.tar` & `pytorch-ignite-0.5.0.dev20230727.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.652076 pytorch-ignite-0.5.0.dev20230726/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28359 2023-07-26 00:16:28.652076 pytorch-ignite-0.5.0.dev20230726/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27907 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.636076 pytorch-ignite-0.5.0.dev20230726/ignite/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 00:11:54.000000 pytorch-ignite-0.5.0.dev20230726/ignite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.636076 pytorch-ignite-0.5.0.dev20230726/ignite/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/base/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.636076 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.636076 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/tbptt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.640076 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/clearml_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27453 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/polyaxon_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/tqdm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/visdom_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.640076 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/average_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/cohen_kappa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/gpu_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/precision_recall_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.640076 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/canberra_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/fractional_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/fractional_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/manhattan_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/maximum_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_normalized_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_relative_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/r2_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/wave_hedges_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/roc_auc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.644076 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/auto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.644076 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.644076 pytorch-ignite-0.5.0.dev20230726/ignite/engine/
--rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/engine/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (123)    54999 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/engine/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/engine/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.644076 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44795 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/ema_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    65143 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/state_param_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/time_profilers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/handlers/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.648076 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/classification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/epoch_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/fbeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/frequency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.648076 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/fid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/inception_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_absolute_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_pairwise_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/metrics_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/multilabel_confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.648076 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/rouge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/psnr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/recall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/root_mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/running_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/ssim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/metrics/top_k_categorical_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/ignite/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:16:28.652076 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28359 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:16:28.000000 pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-26 00:16:28.652076 pytorch-ignite-0.5.0.dev20230726/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-26 00:11:12.000000 pytorch-ignite-0.5.0.dev20230726/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27328 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.185761 pytorch-ignite-0.5.0.dev20230727/ignite/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 00:11:11.000000 pytorch-ignite-0.5.0.dev20230727/ignite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.185761 pytorch-ignite-0.5.0.dev20230727/ignite/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/base/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.185761 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.185761 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28619 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/tbptt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.189761 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37618 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/clearml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27453 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/polyaxon_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26517 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/tqdm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/visdom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.189761 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/average_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/cohen_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/gpu_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/precision_recall_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.189761 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/canberra_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/fractional_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/fractional_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/manhattan_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/maximum_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_absolute_relative_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_normalized_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_absolute_percentage_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_relative_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/r2_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/wave_hedges_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/roc_auc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.193762 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/auto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.193762 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26478 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22584 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.193762 pytorch-ignite-0.5.0.dev20230727/ignite/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)    32766 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/engine/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54999 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/engine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.197762 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44795 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/ema_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21756 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65143 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/state_param_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30228 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/time_profilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/handlers/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.197762 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/classification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17638 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/epoch_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/fbeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/frequency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/fid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/inception_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_absolute_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_pairwise_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/metrics_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/multilabel_confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/rouge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9484 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/root_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/running_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/ssim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/metrics/top_k_categorical_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/ignite/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27780 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 00:16:09.000000 pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-27 00:16:09.201762 pytorch-ignite-0.5.0.dev20230727/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-27 00:10:33.000000 pytorch-ignite-0.5.0.dev20230727/setup.py
```

### Comparing `pytorch-ignite-0.5.0.dev20230726/LICENSE` & `pytorch-ignite-0.5.0.dev20230727/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230727/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,33 @@
-Metadata-Version: 2.1
-Name: pytorch-ignite
-Version: 0.5.0.dev20230726
-Summary: A lightweight library to help with training neural networks in PyTorch.
-Home-page: https://github.com/pytorch/ignite
-Author: PyTorch-Ignite Team
-Author-email: contact@pytorch-ignite.ai
-License: BSD
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 <!-- ![Ignite Logo](assets/logo/ignite_logo_mixed.svg) -->
 
-<img src="https://raw.githubusercontent.com/pytorch/ignite/master/assets/logo/ignite_logo_mixed.svg" width=512>
+<img src="assets/logo/ignite_logo_mixed.svg" width=512>
 
 <!-- [![image](https://travis-ci.com/pytorch/ignite.svg?branch=master)](https://travis-ci.com/pytorch/ignite) -->
 
-| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/workflows/Run%20unit%20tests/badge.svg)](https://github.com/pytorch/ignite/actions) [![image](https://img.shields.io/badge/-GPU%20tests-black?style=flat-square)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master)[![image](https://circleci.com/gh/pytorch/ignite.svg?style=svg)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
+| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml) [![image](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml/badge.svg)](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
 |:---
-| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) [![image](https://anaconda.org/pytorch/ignite/badges/downloads.svg)](https://anaconda.org/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) |
+| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) ・ [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) ・ [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) |
 | ![image](https://img.shields.io/badge/-Nightly%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch-nightly/ignite/badges/version.svg)](https://anaconda.org/pytorch-nightly/ignite) [![image](https://img.shields.io/badge/PyPI-pre%20releases-brightgreen)](https://pypi.org/project/pytorch-ignite/#history)|
-| ![image](https://img.shields.io/badge/-Features:-black?style=flat-square) [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) [![image](https://img.shields.io/badge/Optuna-integrated-blue)](https://optuna.org) [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![facebook](https://img.shields.io/badge/news-facebook-blue)](https://www.facebook.com/PyTorch-Ignite-Community-105837321694508) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) |
+| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) |
 | ![image](https://img.shields.io/badge/-Supported_PyTorch/Python_versions:-black?style=flat-square) [![link](https://img.shields.io/badge/-check_here-blue)](https://github.com/pytorch/ignite/actions?query=workflow%3A%22PyTorch+version+tests%22)|
 
 </div>
 
 ## TL;DR
 
 Ignite is a high-level library to help with training and evaluating neural networks in PyTorch flexibly and transparently.
 
 <div align="center">
 
 <a href="https://colab.research.google.com/github/pytorch/ignite/blob/master/assets/tldr/teaser.ipynb">
  <img alt="PyTorch-Ignite teaser"
-      src="https://raw.githubusercontent.com/pytorch/ignite/master/assets/tldr/pytorch-ignite-teaser.gif"
+      src="assets/tldr/pytorch-ignite-teaser.gif"
       width=532>
 </a>
 
 _Click on the image to see complete code_
 
 </div>
```

### Comparing `pytorch-ignite-0.5.0.dev20230726/README.md` & `pytorch-ignite-0.5.0.dev20230727/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,44 @@
+Metadata-Version: 2.1
+Name: pytorch-ignite
+Version: 0.5.0.dev20230727
+Summary: A lightweight library to help with training neural networks in PyTorch.
+Home-page: https://github.com/pytorch/ignite
+Author: PyTorch-Ignite Team
+Author-email: contact@pytorch-ignite.ai
+License: BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 <!-- ![Ignite Logo](assets/logo/ignite_logo_mixed.svg) -->
 
-<img src="assets/logo/ignite_logo_mixed.svg" width=512>
+<img src="https://raw.githubusercontent.com/pytorch/ignite/master/assets/logo/ignite_logo_mixed.svg" width=512>
 
 <!-- [![image](https://travis-ci.com/pytorch/ignite.svg?branch=master)](https://travis-ci.com/pytorch/ignite) -->
 
-| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/workflows/Run%20unit%20tests/badge.svg)](https://github.com/pytorch/ignite/actions) [![image](https://img.shields.io/badge/-GPU%20tests-black?style=flat-square)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master)[![image](https://circleci.com/gh/pytorch/ignite.svg?style=svg)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
+| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml) [![image](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml/badge.svg)](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
 |:---
-| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) [![image](https://anaconda.org/pytorch/ignite/badges/downloads.svg)](https://anaconda.org/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) |
+| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) ・ [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) ・ [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) |
 | ![image](https://img.shields.io/badge/-Nightly%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch-nightly/ignite/badges/version.svg)](https://anaconda.org/pytorch-nightly/ignite) [![image](https://img.shields.io/badge/PyPI-pre%20releases-brightgreen)](https://pypi.org/project/pytorch-ignite/#history)|
-| ![image](https://img.shields.io/badge/-Features:-black?style=flat-square) [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) [![image](https://img.shields.io/badge/Optuna-integrated-blue)](https://optuna.org) [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![facebook](https://img.shields.io/badge/news-facebook-blue)](https://www.facebook.com/PyTorch-Ignite-Community-105837321694508) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) |
+| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) |
 | ![image](https://img.shields.io/badge/-Supported_PyTorch/Python_versions:-black?style=flat-square) [![link](https://img.shields.io/badge/-check_here-blue)](https://github.com/pytorch/ignite/actions?query=workflow%3A%22PyTorch+version+tests%22)|
 
 </div>
 
 ## TL;DR
 
 Ignite is a high-level library to help with training and evaluating neural networks in PyTorch flexibly and transparently.
 
 <div align="center">
 
 <a href="https://colab.research.google.com/github/pytorch/ignite/blob/master/assets/tldr/teaser.ipynb">
  <img alt="PyTorch-Ignite teaser"
-      src="assets/tldr/pytorch-ignite-teaser.gif"
+      src="https://raw.githubusercontent.com/pytorch/ignite/master/assets/tldr/pytorch-ignite-teaser.gif"
       width=532>
 </a>
 
 _Click on the image to see complete code_
 
 </div>
```

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/base/mixins.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/base/mixins.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/common.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/common.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/engines/tbptt.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/engines/tbptt.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/base_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/base_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/clearml_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/clearml_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/mlflow_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/neptune_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/polyaxon_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/polyaxon_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/tensorboard_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/tqdm_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/tqdm_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/visdom_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/visdom_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/handlers/wandb_logger.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/handlers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/average_precision.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/average_precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/cohen_kappa.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/cohen_kappa.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/gpu_info.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/gpu_info.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/precision_recall_curve.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/precision_recall_curve.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/_base.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/_base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/canberra_metric.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/canberra_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/fractional_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/fractional_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/fractional_bias.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/fractional_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/geometric_mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/geometric_mean_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/manhattan_distance.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/maximum_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/maximum_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_absolute_relative_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_absolute_relative_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/mean_normalized_bias.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/mean_normalized_bias.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_absolute_percentage_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_absolute_percentage_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/median_relative_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/median_relative_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/r2_score.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/r2_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/regression/wave_hedges_distance.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/regression/wave_hedges_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/contrib/metrics/roc_auc.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/contrib/metrics/roc_auc.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/auto.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/auto.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/base.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/base.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/horovod.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/horovod.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/native.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/native.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/comp_models/xla.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/comp_models/xla.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/launcher.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/launcher.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/distributed/utils.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/engine/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/engine/deterministic.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/engine/deterministic.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/engine/engine.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/engine/events.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/engine/events.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/engine/utils.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/checkpoint.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/checkpoint.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/early_stopping.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/ema_handler.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/ema_handler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/lr_finder.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/state_param_scheduler.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/state_param_scheduler.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/stores.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/stores.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/terminate_on_nan.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/time_limit.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/time_limit.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/time_profilers.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/time_profilers.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/handlers/timing.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/handlers/timing.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/__init__.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/accumulation.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/accuracy.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/classification_report.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/classification_report.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/epoch_metric.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/epoch_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/fbeta.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/fbeta.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/frequency.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/frequency.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/fid.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/fid.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/inception_score.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/inception_score.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/gan/utils.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/gan/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/loss.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_absolute_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_absolute_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_pairwise_distance.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_pairwise_distance.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/metric.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/metrics_lambda.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/metrics_lambda.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/multilabel_confusion_matrix.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/multilabel_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/bleu.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/bleu.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/rouge.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/rouge.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/nlp/utils.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/precision.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/psnr.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/psnr.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/recall.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/root_mean_squared_error.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/root_mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/running_average.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/running_average.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/ssim.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/ssim.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/metrics/top_k_categorical_accuracy.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/metrics/top_k_categorical_accuracy.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/ignite/utils.py` & `pytorch-ignite-0.5.0.dev20230727/ignite/utils.py`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/pyproject.toml` & `pytorch-ignite-0.5.0.dev20230727/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/PKG-INFO` & `pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-ignite
-Version: 0.5.0.dev20230726
+Version: 0.5.0.dev20230727
 Summary: A lightweight library to help with training neural networks in PyTorch.
 Home-page: https://github.com/pytorch/ignite
 Author: PyTorch-Ignite Team
 Author-email: contact@pytorch-ignite.ai
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,20 +13,19 @@
 
 <!-- ![Ignite Logo](assets/logo/ignite_logo_mixed.svg) -->
 
 <img src="https://raw.githubusercontent.com/pytorch/ignite/master/assets/logo/ignite_logo_mixed.svg" width=512>
 
 <!-- [![image](https://travis-ci.com/pytorch/ignite.svg?branch=master)](https://travis-ci.com/pytorch/ignite) -->
 
-| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/workflows/Run%20unit%20tests/badge.svg)](https://github.com/pytorch/ignite/actions) [![image](https://img.shields.io/badge/-GPU%20tests-black?style=flat-square)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master)[![image](https://circleci.com/gh/pytorch/ignite.svg?style=svg)](https://app.circleci.com/pipelines/github/pytorch/ignite?branch=master) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
+| ![image](https://img.shields.io/badge/-Tests:-black?style=flat-square) [![image](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/pytorch/ignite/actions/workflows/unit-tests.yml) [![image](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml/badge.svg)](https://github.com/pytorch/ignite/actions/workflows/gpu-tests.yml) [![image](https://codecov.io/gh/pytorch/ignite/branch/master/graph/badge.svg)](https://codecov.io/gh/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=docs&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pytorch.org/ignite/index.html) |
 |:---
-| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) [![image](https://anaconda.org/pytorch/ignite/badges/downloads.svg)](https://anaconda.org/pytorch/ignite) [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) |
+| ![image](https://img.shields.io/badge/-Stable%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch/ignite/badges/version.svg)](https://anaconda.org/pytorch/ignite) ・ [![image](https://img.shields.io/badge/dynamic/json.svg?label=PyPI&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fpytorch-ignite%2Fjson&query=%24.info.version&colorB=brightgreen&prefix=v)](https://pypi.org/project/pytorch-ignite/) [![image](https://pepy.tech/badge/pytorch-ignite)](https://pepy.tech/project/pytorch-ignite) ・ [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) |
 | ![image](https://img.shields.io/badge/-Nightly%20Releases:-black?style=flat-square) [![image](https://anaconda.org/pytorch-nightly/ignite/badges/version.svg)](https://anaconda.org/pytorch-nightly/ignite) [![image](https://img.shields.io/badge/PyPI-pre%20releases-brightgreen)](https://pypi.org/project/pytorch-ignite/#history)|
-| ![image](https://img.shields.io/badge/-Features:-black?style=flat-square) [![image](https://img.shields.io/badge/docker-hub-blue)](https://hub.docker.com/u/pytorchignite) [![image](https://img.shields.io/badge/Optuna-integrated-blue)](https://optuna.org) [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) |
-| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![facebook](https://img.shields.io/badge/news-facebook-blue)](https://www.facebook.com/PyTorch-Ignite-Community-105837321694508) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) |
+| ![image](https://img.shields.io/badge/-Community:-black?style=flat-square) [![Twitter](https://img.shields.io/badge/news-twitter-blue)](https://twitter.com/pytorch_ignite) [![discord](https://img.shields.io/badge/chat-discord-blue?logo=discord)](https://discord.gg/djZtm3EmKj) [![numfocus](https://img.shields.io/badge/NumFOCUS-affiliated%20project-green)](https://numfocus.org/sponsored-projects/affiliated-projects) |
 | ![image](https://img.shields.io/badge/-Supported_PyTorch/Python_versions:-black?style=flat-square) [![link](https://img.shields.io/badge/-check_here-blue)](https://github.com/pytorch/ignite/actions?query=workflow%3A%22PyTorch+version+tests%22)|
 
 </div>
 
 ## TL;DR
 
 Ignite is a high-level library to help with training and evaluating neural networks in PyTorch flexibly and transparently.
```

### Comparing `pytorch-ignite-0.5.0.dev20230726/pytorch_ignite.egg-info/SOURCES.txt` & `pytorch-ignite-0.5.0.dev20230727/pytorch_ignite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/setup.cfg` & `pytorch-ignite-0.5.0.dev20230727/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-ignite-0.5.0.dev20230726/setup.py` & `pytorch-ignite-0.5.0.dev20230727/setup.py`

 * *Files identical despite different names*

