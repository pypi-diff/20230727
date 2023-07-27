# Comparing `tmp/ml-starter-0.1.39.tar.gz` & `tmp/ml-starter-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.39.tar", last modified: Wed Jul 26 17:41:07 2023, max compression
+gzip compressed data, was "ml-starter-0.1.40.tar", last modified: Thu Jul 27 01:14:42 2023, max compression
```

## Comparing `ml-starter-0.1.39.tar` & `ml-starter-0.1.40.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.264351 ml-starter-0.1.39/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 17:40:55.000000 ml-starter-0.1.39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 17:40:55.000000 ml-starter-0.1.39/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-26 17:41:07.264351 ml-starter-0.1.39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-26 17:40:55.000000 ml-starter-0.1.39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.244350 ml-starter-0.1.39/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.244350 ml-starter-0.1.39/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.244350 ml-starter-0.1.39/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.248350 ml-starter-0.1.39/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.248350 ml-starter-0.1.39/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.248350 ml-starter-0.1.39/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.248350 ml-starter-0.1.39/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.248350 ml-starter-0.1.39/ml/models/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/architectures/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.252351 ml-starter-0.1.39/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.252351 ml-starter-0.1.39/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.252351 ml-starter-0.1.39/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.252351 ml-starter-0.1.39/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.252351 ml-starter-0.1.39/ml/tasks/diffusion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/diffusion/beta_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/diffusion/gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/losses/kl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.256351 ml-starter-0.1.39/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.264351 ml-starter-0.1.39/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.264351 ml-starter-0.1.39/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.264351 ml-starter-0.1.39/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-26 17:40:55.000000 ml-starter-0.1.39/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:41:07.264351 ml-starter-0.1.39/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-26 17:41:07.000000 ml-starter-0.1.39/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-26 17:41:07.000000 ml-starter-0.1.39/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:41:07.000000 ml-starter-0.1.39/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-26 17:41:07.000000 ml-starter-0.1.39/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-26 17:41:07.000000 ml-starter-0.1.39/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-26 17:40:55.000000 ml-starter-0.1.39/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-26 17:41:07.264351 ml-starter-0.1.39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-26 17:40:55.000000 ml-starter-0.1.39/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 01:14:30.000000 ml-starter-0.1.40/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-27 01:14:30.000000 ml-starter-0.1.40/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 01:14:42.993226 ml-starter-0.1.40/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 01:14:30.000000 ml-starter-0.1.40/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.973225 ml-starter-0.1.40/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46173 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.977226 ml-starter-0.1.40/ml/models/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/architectures/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56335 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19251 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.981226 ml-starter-0.1.40/ml/tasks/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/beta_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/diffusion/gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/kl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24976 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.985226 ml-starter-0.1.40/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35281 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-07-27 01:14:30.000000 ml-starter-0.1.40/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:14:42.993226 ml-starter-0.1.40/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-27 01:14:42.000000 ml-starter-0.1.40/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 01:14:30.000000 ml-starter-0.1.40/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-27 01:14:42.993226 ml-starter-0.1.40/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-27 01:14:30.000000 ml-starter-0.1.40/setup.py
```

### Comparing `ml-starter-0.1.39/LICENSE` & `ml-starter-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/PKG-INFO` & `ml-starter-0.1.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.39
+Version: 0.1.40
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.39/README.md` & `ml-starter-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/api.py` & `ml-starter-0.1.40/ml/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,32 +14,36 @@
     "as_cpu_tensor",
     "as_numpy_array",
     "assert_no_nans",
     "AsyncEnvironmentWorker",
     "AsyncIterableDataset",
     "AsyncWorkerPool",
     "atomic_save",
+    "AudioFile",
     "AudioFileDataset",
+    "AudioFolderFilesDataset",
     "AudioFoldersFilesDataset",
     "AudioMagStftConverter",
     "AudioMfccConverter",
+    "AudioProps",
     "AudioPyworldConverter",
     "AudioStftConverter",
     "autocast_all",
     "autocast_tensors",
     "base_device",
     "BaseEnvironmentWorker",
     "BaseLearningTrainer",
     "BaseLearningTrainerConfig",
     "BaseLRScheduler",
     "BaseLRSchedulerConfig",
     "BaseModel",
     "BaseModelConfig",
     "BaseOptimizer",
     "BaseOptimizerConfig",
+    "BaseSpeakerDataset",
     "BaseTask",
     "BaseTaskConfig",
     "BaseTrainer",
     "BaseTrainerConfig",
     "Batch",
     "BiFPN",
     "cached_object",
@@ -54,21 +58,23 @@
     "Clamp",
     "ClippifyDataset",
     "collate_non_null",
     "collate",
     "CollateMode",
     "colorize",
     "ColumnParallelLinear",
+    "ConcatSpeakerDataset",
     "conf_field",
     "configure_logging",
     "detect_device",
     "DictIndex",
     "DiffusionBetaSchedule",
     "ensure_downloaded",
     "Environment",
+    "FolderSpeakerDataset",
     "format_timedelta",
     "freeze_non_lora_",
     "from_args",
     "GaussianDiffusion",
     "GenerativeAdversarialNetworkTask",
     "GenerativeAdversarialNetworkTaskConfig",
     "get_activation",
@@ -299,16 +305,22 @@
 from ml.trainers.rl import ReinforcementLearningTrainer, ReinforcementLearningTrainerConfig
 from ml.trainers.sl import SupervisedLearningTrainer, SupervisedLearningTrainerConfig
 from ml.utils.amp import autocast_all, autocast_tensors
 from ml.utils.argparse import from_args, get_args, get_type_from_string
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.attention import NextTokenDiscriminator
 from ml.utils.audio import (
+    AudioFile,
     AudioFileDataset,
+    AudioFolderFilesDataset,
     AudioFoldersFilesDataset,
+    AudioProps,
+    BaseSpeakerDataset,
+    ConcatSpeakerDataset,
+    FolderSpeakerDataset,
     get_audio_props,
     read_audio,
     read_audio_random_order,
     rechunk_audio,
     set_default_audio_reader,
     set_default_audio_writer,
     write_audio,
```

### Comparing `ml-starter-0.1.39/ml/core/common_types.py` & `ml-starter-0.1.40/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/core/config.py` & `ml-starter-0.1.40/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/core/env.py` & `ml-starter-0.1.40/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/core/registry.py` & `ml-starter-0.1.40/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/core/state.py` & `ml-starter-0.1.40/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/launchers/base.py` & `ml-starter-0.1.40/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/launchers/mp.py` & `ml-starter-0.1.40/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/launchers/sagemaker.py` & `ml-starter-0.1.40/ml/launchers/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/launchers/slurm.py` & `ml-starter-0.1.40/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/launchers/torchrun.py` & `ml-starter-0.1.40/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/loggers/base.py` & `ml-starter-0.1.40/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/loggers/meter.py` & `ml-starter-0.1.40/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/loggers/multi.py` & `ml-starter-0.1.40/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/loggers/stdout.py` & `ml-starter-0.1.40/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/loggers/tensorboard.py` & `ml-starter-0.1.40/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/base.py` & `ml-starter-0.1.40/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/constant.py` & `ml-starter-0.1.40/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.40/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.40/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/gan.py` & `ml-starter-0.1.40/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/linear.py` & `ml-starter-0.1.40/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.40/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.40/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/activations.py` & `ml-starter-0.1.40/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/architectures/bifpn.py` & `ml-starter-0.1.40/ml/models/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/architectures/unet.py` & `ml-starter-0.1.40/ml/models/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/base.py` & `ml-starter-0.1.40/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/codebook.py` & `ml-starter-0.1.40/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/embeddings.py` & `ml-starter-0.1.40/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/gan.py` & `ml-starter-0.1.40/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/init.py` & `ml-starter-0.1.40/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/kmeans.py` & `ml-starter-0.1.40/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/lora.py` & `ml-starter-0.1.40/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/modules.py` & `ml-starter-0.1.40/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/norms.py` & `ml-starter-0.1.40/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/models/parallel.py` & `ml-starter-0.1.40/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/adam.py` & `ml-starter-0.1.40/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/adan.py` & `ml-starter-0.1.40/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/base.py` & `ml-starter-0.1.40/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/common.py` & `ml-starter-0.1.40/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/gan.py` & `ml-starter-0.1.40/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/lion.py` & `ml-starter-0.1.40/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/sgd.py` & `ml-starter-0.1.40/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/optimizers/shampoo.py` & `ml-starter-0.1.40/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/scripts/cli.py` & `ml-starter-0.1.40/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/scripts/stage.py` & `ml-starter-0.1.40/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/scripts/train.py` & `ml-starter-0.1.40/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/base.py` & `ml-starter-0.1.40/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.40/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.40/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/collate.py` & `ml-starter-0.1.40/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.40/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.40/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.40/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.40/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.40/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.40/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/diffusion/beta_schedule.py` & `ml-starter-0.1.40/ml/tasks/diffusion/beta_schedule.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/diffusion/gaussian.py` & `ml-starter-0.1.40/ml/tasks/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/environments/base.py` & `ml-starter-0.1.40/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/environments/utils.py` & `ml-starter-0.1.40/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/environments/worker.py` & `ml-starter-0.1.40/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/gan/base.py` & `ml-starter-0.1.40/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/losses/audio.py` & `ml-starter-0.1.40/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/losses/image.py` & `ml-starter-0.1.40/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/losses/kl.py` & `ml-starter-0.1.40/ml/tasks/losses/kl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/losses/loss.py` & `ml-starter-0.1.40/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/rl/base.py` & `ml-starter-0.1.40/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/rl/replay.py` & `ml-starter-0.1.40/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/tasks/sl/base.py` & `ml-starter-0.1.40/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/base.py` & `ml-starter-0.1.40/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/gan.py` & `ml-starter-0.1.40/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/learning.py` & `ml-starter-0.1.40/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/compile.py` & `ml-starter-0.1.40/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.40/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.40/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.40/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.40/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.40/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.40/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.40/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.40/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/rl.py` & `ml-starter-0.1.40/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/trainers/sl.py` & `ml-starter-0.1.40/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/amp.py` & `ml-starter-0.1.40/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/argparse.py` & `ml-starter-0.1.40/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/atomic.py` & `ml-starter-0.1.40/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/attention.py` & `ml-starter-0.1.40/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/audio.py` & `ml-starter-0.1.40/ml/utils/audio.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
     from ml.utils.audio import read_audio, write_audio
 
 This just uses FFMPEG so it should be rasonably quick.
 """
 
 import fractions
+import itertools
 import logging
 import multiprocessing as mp
 import os
 import random
 import re
 import shutil
 import warnings
-from collections import deque
+from abc import ABC, abstractmethod
+from collections import Counter, deque
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Deque, Iterator, Literal, Sequence, TypeVar
+from typing import Deque, Generic, Iterator, Literal, Sequence, TypeVar
 
 import av
 import numpy as np
 import soundfile as sf
 import torch
 import torchaudio.functional as A
 import tqdm
@@ -618,25 +620,28 @@
     def __init__(
         self,
         audio_file: Path,
         sample_rate: int,
         length_ms: float,
         num_samples_per_clip: int = 1,
         max_iters: int | None = None,
+        channel_idx: int | None = None,
     ) -> None:
         super().__init__()
 
         self.audio_file = audio_file
         self.sample_rate = sample_rate
-        self.current_audio: list[Tensor] | None = None
-        self.chunk_frames = round(sample_rate * length_ms / 1000)
         self.num_samples_per_clip = num_samples_per_clip
         self.max_iters = max_iters
+        self.channel_idx = channel_idx
+
+        self.current_audio: list[Tensor] | None = None
+        self.chunk_frames = round(sample_rate * length_ms / 1000)
+
         self.audio_iter: Iterator[np.ndarray] | None = None
-        self.channel_idx: int | None = None
         self.current_chunk = 0
         self.samples_queue: Deque[Tensor] = deque()
 
     def _get_next_audio(self) -> Tensor:
         assert self.audio_iter is not None, "Must call __iter__ first!"
 
         audio_np = next(self.audio_iter)  # (num_channels, num_frames)
@@ -709,48 +714,53 @@
     Parameters:
         root_dirs: The root directories to search for audio files.
         sample_rate: The sampling rate to resample the audio to.
         length_ms: The length of the audio clips in milliseconds.
         num_samples_per_clip: The number of samples to take from each audio clip.
         num_simultaneous: The number of audio files to load into memory at once.
         max_iters: Maximum number of samples to draw from each clip.
+        channel_idx: The index of the channel to use. If None, will randomly
+            select a channel.
     """
 
     def __init__(
         self,
         root_dirs: Sequence[str | Path],
         sample_rate: int,
         length_ms: float,
         num_simultaneous: int,
         num_samples_per_clip: int = 1,
         max_iters: int | None = None,
+        channel_idx: int | None = None,
     ) -> None:
         super().__init__()
 
         self.files_ds = AudioFoldersFilesDataset(root_dirs)
         self.audio_ds_queue: Deque[tuple[int, Iterator[Tensor]]] = deque()
 
         # Parameters for child dataset.
         self.sample_rate = sample_rate
         self.length_ms = length_ms
         self.num_samples_per_clip = num_samples_per_clip
         self.max_iters = max_iters
+        self.channel_idx = channel_idx
 
         # Keeps track of which indices to sample from.
         self.indices = list(range(len(self.files_ds)))
         self.num_simultaneous = num_simultaneous
 
     def _get_audio_ds(self, index: int) -> tuple[int, Iterator[Tensor]]:
         audio_file, root_dir = self.files_ds[index]
         ds = AudioFileDataset(
             audio_file=root_dir / audio_file.path,
             sample_rate=self.sample_rate,
             length_ms=self.length_ms,
             num_samples_per_clip=self.num_samples_per_clip,
             max_iters=self.max_iters,
+            channel_idx=self.channel_idx,
         )
         return index, iter(ds)
 
     def __iter__(self) -> Iterator[Tensor]:
         winfo = get_worker_info()
         world_size = winfo.num_workers * get_world_size()
 
@@ -778,7 +788,225 @@
             self.audio_ds_queue.append(self._get_audio_ds(next_index))
             return next(self)
         except Exception:
             logger.exception("Error for index %d", index)
             next_index = self.indices.pop()
             self.audio_ds_queue.append(self._get_audio_ds(next_index))
             return next(self)
+
+
+class BaseSpeakerDataset(IterableDataset[tuple[Tensor, int]], ABC):
+    @abstractmethod
+    def num_speakers(self) -> int:
+        """Returns the number of speakers in the dataset.
+
+        Returns:
+            The number of speakers in the dataset.
+        """
+
+    def __iter__(self) -> Iterator[tuple[Tensor, int]]:
+        self.init_worker()
+        return self
+
+    def init_worker(self) -> None:
+        pass
+
+    @abstractmethod
+    def __next__(self) -> tuple[Tensor, int]:
+        """Returns the next item from the dataset.
+
+        Returns:
+            The next item from the dataset.
+        """
+
+
+SpeakerT = TypeVar("SpeakerT", int, str)
+
+
+@dataclass
+class Item:
+    index: int
+    audio_path: Path
+    speaker_id: int
+    iterator: Iterator[Tensor]
+
+
+class FolderSpeakerDataset(BaseSpeakerDataset, Generic[SpeakerT], ABC):
+    """Defines a dataset for iterating through audio samples in a folder.
+
+    This dataset indexes all the audio files in any subdirectory in a folder
+    and returns them in a random order. Child classes should implement the
+    ``get_speaker`` function.
+
+    Parameters:
+        root_dirs: The root directories to search for audio files.
+        length_ms: The length of the audio clips in milliseconds.
+        num_samples_per_clip: The number of samples to take from each audio clip.
+        num_simultaneous: The number of audio files to load into memory at once.
+        max_iters: Maximum number of samples to draw from each clip.
+        specific_speakers: If specified, only loads audio from these speakers.
+        top_n_speakers: If specified, only loads audio from the top N speakers.
+        normalize: If ``True``, normalizes the audio to the range [-1, 1].
+    """
+
+    def __init__(
+        self,
+        root_dir: str | Path,
+        sample_rate: int,
+        length_ms: float,
+        num_samples_per_clip: int,
+        num_simultaneous: int = 1,
+        max_iters: int | None = None,
+        specific_speakers: Sequence[SpeakerT] | None = None,
+        top_n_speakers: int | None = None,
+        normalize: bool = False,
+    ) -> None:
+        super().__init__()
+
+        # Stores the parameters.
+        self.sample_rate = sample_rate
+        self.length_ms = length_ms
+        self.num_samples_per_clip = num_samples_per_clip
+        self.max_iters = max_iters
+        self.specific_speakers: list[SpeakerT] | None = None if specific_speakers is None else list(specific_speakers)
+        self.top_n_speakers = top_n_speakers
+        self.normalize = normalize
+        self.num_simultaneous = num_simultaneous
+
+        # Indexes the files in the root directory.
+        self.files_ds = AudioFolderFilesDataset(root_dir)
+        self.audio_ds_queue: Deque[Item] = deque()
+
+        # Gets the mapping from the speaker ID to the index.
+        speakers = [self.get_speaker(*self.files_ds[i]) for i in range(len(self.files_ds))]
+        speaker_to_id: dict[SpeakerT, int] = {s: i for i, s in enumerate(sorted(set(speakers)))}
+
+        # Filters the file dataset indices to only some subset.
+        all_indices = list(range(len(self.files_ds)))
+        if specific_speakers is not None and top_n_speakers is not None:
+            raise ValueError("Cannot specify both `specific_speakers` and `top_n_speakers`.")
+        if top_n_speakers is not None:
+            speaker_counts = Counter(speakers)
+            specific_speakers = [s for s, _ in speaker_counts.most_common(top_n_speakers)]
+        if specific_speakers is not None:
+            speaker_set = set(specific_speakers)
+            all_indices = [i for i in all_indices if speakers[i] in speaker_set]
+            speaker_to_id = {s: i for i, s in enumerate(sorted(specific_speakers))}
+
+        self.indices = self.all_indices = all_indices
+        self.speaker_to_id: dict[SpeakerT, int] = speaker_to_id
+
+    @abstractmethod
+    def get_speaker(self, audio_file: AudioFile, root_dir: Path) -> SpeakerT:
+        """Returns the speaker for a given audio file.
+
+        Args:
+            audio_file: The audio file relative to the root directory, with
+                its associated properties.
+            root_dir: The root directory of the dataset.
+
+        Returns:
+            The speaker identifier.
+        """
+
+    def num_speakers(self) -> int:
+        return len(self.speaker_to_id)
+
+    def _get_audio_ds(self, index: int) -> Item:
+        audio_file, root_dir = self.files_ds[index]
+
+        ds = AudioFileDataset(
+            audio_file=root_dir / audio_file.path,
+            sample_rate=self.sample_rate,
+            length_ms=self.length_ms,
+            num_samples_per_clip=self.num_samples_per_clip,
+            max_iters=self.max_iters,
+        )
+
+        speaker = self.get_speaker(audio_file, root_dir)
+        speaker_id = self.speaker_to_id[speaker]
+
+        return Item(
+            index=index,
+            audio_path=audio_file.path,
+            speaker_id=speaker_id,
+            iterator=iter(ds),
+        )
+
+    def init_worker(self) -> None:
+        winfo = get_worker_info()
+        world_size = winfo.num_workers * get_world_size()
+
+        # Shuffles the indices and splits them across workers.
+        self.indices = self.all_indices[winfo.worker_id :: world_size]
+        random.shuffle(self.indices)
+
+        # Creates the audio datasets for the first `num_simultaneous` indices.
+        self.audio_ds_queue.clear()
+        self.audio_ds_queue.extend((self._get_audio_ds(i) for i in self.indices[: self.num_simultaneous]))
+        self.indices = self.indices[self.num_simultaneous :]
+
+    def __next__(self) -> tuple[Tensor, int]:
+        item = self.audio_ds_queue.popleft()
+        try:
+            next_sample = next(item.iterator)
+            if self.normalize:
+                next_sample = (next_sample / (next_sample.abs().max() + 1e-6)) * 0.999
+            self.audio_ds_queue.append(item)
+            return next_sample, item.speaker_id
+
+        except StopIteration:
+            if len(self.indices) == 0:
+                raise StopIteration
+            next_index = self.indices.pop()
+            self.audio_ds_queue.append(self._get_audio_ds(next_index))
+            return next(self)
+
+        except Exception:
+            logger.exception("Error for index %d", item.index)
+            next_index = self.indices.pop()
+            self.audio_ds_queue.append(self._get_audio_ds(next_index))
+            return next(self)
+
+
+class ConcatSpeakerDataset(BaseSpeakerDataset):
+    """Defines a dataset to concatenate multiple child speaker datasets.
+
+    This dataset maps the speaker IDs from the child datasets to a global
+    speaker ID.
+
+    Parameters:
+        datasets: The child datasets to concatenate.
+        finish_all: If True, will finish all child datasets before stopping.
+            Otherwise, stops after finishing the first dataset.
+    """
+
+    def __init__(self, datasets: Sequence[BaseSpeakerDataset], finish_all: bool = True) -> None:
+        super().__init__()
+
+        self._datasets = list(datasets)
+        self._num_speakers = [ds.num_speakers() for ds in self._datasets]
+        self._speaker_offset = [0] + list(itertools.accumulate(self._num_speakers))[:-1]
+
+        self.finish_all = finish_all
+
+    def __iter__(self) -> Iterator[tuple[Tensor, int]]:
+        self.iterators = [iter(ds) for ds in self._datasets]
+        return self
+
+    def __next__(self) -> tuple[Tensor, int]:
+        if not self.iterators:
+            raise StopIteration
+
+        try:
+            index = random.randrange(len(self.iterators))
+            audio, speaker_id = next(self.iterators[index])
+            speaker_id += self._speaker_offset[index]
+            return audio, speaker_id
+
+        except StopIteration:
+            if self.finish_all:
+                self.iterators[index], self.iterators[-1] = self.iterators[-1], self.iterators[index]
+                self.iterators.pop()
+                return next(self)
+            else:
+                raise
```

### Comparing `ml-starter-0.1.39/ml/utils/augmentation.py` & `ml-starter-0.1.40/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/caching.py` & `ml-starter-0.1.40/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/checkpoint.py` & `ml-starter-0.1.40/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/cli.py` & `ml-starter-0.1.40/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/colors.py` & `ml-starter-0.1.40/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/containers.py` & `ml-starter-0.1.40/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/data.py` & `ml-starter-0.1.40/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/datetime.py` & `ml-starter-0.1.40/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/device/auto.py` & `ml-starter-0.1.40/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/device/base.py` & `ml-starter-0.1.40/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/device/cpu.py` & `ml-starter-0.1.40/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/device/gpu.py` & `ml-starter-0.1.40/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/device/metal.py` & `ml-starter-0.1.40/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/distributed.py` & `ml-starter-0.1.40/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/exceptions.py` & `ml-starter-0.1.40/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/image.py` & `ml-starter-0.1.40/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/io.py` & `ml-starter-0.1.40/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/large_models.py` & `ml-starter-0.1.40/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/logging.py` & `ml-starter-0.1.40/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/meter.py` & `ml-starter-0.1.40/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/mixed_precision.py` & `ml-starter-0.1.40/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/networking.py` & `ml-starter-0.1.40/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/numpy.py` & `ml-starter-0.1.40/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/parallel.py` & `ml-starter-0.1.40/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/spectrogram.py` & `ml-starter-0.1.40/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/staging.py` & `ml-starter-0.1.40/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/testing.py` & `ml-starter-0.1.40/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/timer.py` & `ml-starter-0.1.40/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/tokens.py` & `ml-starter-0.1.40/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/torch_distributed.py` & `ml-starter-0.1.40/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/triton/kmeans.py` & `ml-starter-0.1.40/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/triton/lion.py` & `ml-starter-0.1.40/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml/utils/video.py` & `ml-starter-0.1.40/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.40/ml_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.39
+Version: 0.1.40
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.39/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.40/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/pyproject.toml` & `ml-starter-0.1.40/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.39/setup.py` & `ml-starter-0.1.40/setup.py`

 * *Files identical despite different names*

