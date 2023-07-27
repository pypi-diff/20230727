# Comparing `tmp/tensorneko-0.2.9.tar.gz` & `tmp/tensorneko-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorneko-0.2.9.tar", last modified: Mon Jan 30 22:08:36 2023, max compression
+gzip compressed data, was "tensorneko-0.3.0.tar", last modified: Thu Jul 27 06:17:28 2023, max compression
```

## Comparing `tensorneko-0.2.9.tar` & `tensorneko-0.3.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.785670 tensorneko-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-01-30 22:06:06.000000 tensorneko-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    18081 2023-01-30 22:08:36.785670 tensorneko-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    17035 2023-01-30 22:06:06.000000 tensorneko-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-30 22:08:36.785670 tensorneko-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2023-01-30 22:06:06.000000 tensorneko-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.737670 tensorneko-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko/
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko/arch/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/auto_encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     7194 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/gan.py
--rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/vqvae.py
--rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/arch/wgan.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.749670 tensorneko-0.2.9/src/tensorneko/backend/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/callback/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/display_metrics_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/earlystop_lr.py
--rw-r--r--   0 runner    (1001) docker     (122)      456 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/epoch_num_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      645 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/epoch_time_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/gpu_stats_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      605 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/lr_logger.py
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/nil_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/callback/system_stats_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      942 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/nested_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/dataset/round_robin_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.753670 tensorneko-0.2.9/src/tensorneko/debug/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/debug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.757670 tensorneko-0.2.9/src/tensorneko/evaluation/
--rw-r--r--   0 runner    (1001) docker     (122)      261 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/enum.py
--rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/fid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/iou.py
--rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/psnr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/evaluation/ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.757670 tensorneko-0.2.9/src/tensorneko/io/
--rw-r--r--   0 runner    (1001) docker     (122)      213 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.761670 tensorneko-0.2.9/src/tensorneko/io/mesh/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/mesh_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/mesh/mesh_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.769670 tensorneko-0.2.9/src/tensorneko/layer/
--rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/masked_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/noise.py
--rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/patching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/reshape.py
--rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/stack.py
--rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/layer/vector_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/module/
--rw-r--r--   0 runner    (1001) docker     (122)      403 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/dense.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/gated_conv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/inception.py
--rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/mlp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/residual.py
--rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/module/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9231 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_module.py
--rw-r--r--   0 runner    (1001) docker     (122)     8734 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/neko_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/notebook/
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/notebook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/optim/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/optim/lr_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.773670 tensorneko-0.2.9/src/tensorneko/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/crop.py
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.777670 tensorneko-0.2.9/src/tensorneko/preprocess/face_detector/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/face_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/pad.py
--rw-r--r--   0 runner    (1001) docker     (122)     2262 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/preprocess/resize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/util/
--rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/dispatched_misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4523 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/string_getter.py
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/util/type.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/image_browser/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/image_browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1507 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/log_graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/matplotlib.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.781670 tensorneko-0.2.9/src/tensorneko/visualization/watcher/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-01-30 22:06:06.000000 tensorneko-0.2.9/src/tensorneko/visualization/watcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.745670 tensorneko-0.2.9/src/tensorneko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    18081 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-01-30 22:08:36.000000 tensorneko-0.2.9/src/tensorneko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-30 22:08:36.785670 tensorneko-0.2.9/test/
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-01-30 22:06:06.000000 tensorneko-0.2.9/test/test_library_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-01-30 22:06:06.000000 tensorneko-0.2.9/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-27 06:14:43.000000 tensorneko-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-27 06:17:28.949462 tensorneko-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17201 2023-07-27 06:14:43.000000 tensorneko-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-27 06:17:28.949462 tensorneko-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-07-27 06:14:43.000000 tensorneko-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.905461 tensorneko-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko/
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko/arch/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2137 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/auto_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7205 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/gan.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3730 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/vqvae.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4712 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/arch/wgan.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.913461 tensorneko-0.3.0/src/tensorneko/backend/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/callback/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/display_metrics_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/earlystop_lr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      456 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/epoch_num_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/epoch_time_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1485 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/gpu_stats_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/lr_logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/nil_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      820 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/callback/system_stats_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/nested_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/dataset/round_robin_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.917461 tensorneko-0.3.0/src/tensorneko/debug/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/debug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.921461 tensorneko-0.3.0/src/tensorneko/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      137 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/fid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2914 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/iou.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/psnr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/evaluation/ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.921461 tensorneko-0.3.0/src/tensorneko/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      213 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.925462 tensorneko-0.3.0/src/tensorneko/io/mesh/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/mesh_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/mesh/mesh_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.929462 tensorneko-0.3.0/src/tensorneko/layer/
+-rw-r--r--   0 runner    (1001) docker     (122)     1120 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1177 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6360 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/attention.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1574 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3283 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4796 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/masked_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/noise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6585 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/patching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1481 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/stack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2178 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/layer/vector_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.933462 tensorneko-0.3.0/src/tensorneko/module/
+-rw-r--r--   0 runner    (1001) docker     (122)      403 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/dense.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/gated_conv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/inception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3361 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2958 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/residual.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7602 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/module/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9803 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_module.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10007 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/neko_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/notebook/
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/notebook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/optim/
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.937462 tensorneko-0.3.0/src/tensorneko/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/optim/lr_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.941462 tensorneko-0.3.0/src/tensorneko/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2732 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/crop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.941462 tensorneko-0.3.0/src/tensorneko/preprocess/face_detector/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/face_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3238 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/pad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3469 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/preprocess/resize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     2064 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2455 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/dispatched_misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4565 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2102 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2491 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/string_getter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/util/type.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/visualization/
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.945462 tensorneko-0.3.0/src/tensorneko/visualization/image_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/image_browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/log_graph.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/matplotlib.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/src/tensorneko/visualization/watcher/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-27 06:14:43.000000 tensorneko-0.3.0/src/tensorneko/visualization/watcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.909461 tensorneko-0.3.0/src/tensorneko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    18248 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3060 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-27 06:17:28.000000 tensorneko-0.3.0/src/tensorneko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-27 06:17:28.949462 tensorneko-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-27 06:14:43.000000 tensorneko-0.3.0/test/test_library_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-27 06:14:43.000000 tensorneko-0.3.0/test/test_version.py
```

### Comparing `tensorneko-0.2.9/LICENSE` & `tensorneko-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/PKG-INFO` & `tensorneko-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.2.9
+Version: 0.3.0
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
 Keywords: deep learning,pytorch,AI
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="text-align: center">TensorNeko</h1> 
 
 <div align="center">
     <img src="https://img.shields.io/github/stars/ControlNet/tensorneko?style=flat-square">
@@ -34,20 +34,21 @@
     <a href="https://pypi.org/project/tensorneko/"><img src="https://img.shields.io/pypi/dm/tensorneko?style=flat-square"></a>
     <img src="https://img.shields.io/github/license/ControlNet/tensorneko?style=flat-square">
 </div>
 
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
-    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
+    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Lightning-2.0.*-792EE5?style=flat-square&logo=lightning"></a>
 </div>
 
 <div align="center">
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
+    <a href="https://coveralls.io/github/ControlNet/tensorneko"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/tensorneko?style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -235,15 +236,15 @@
 data_list = ... # a list of data
 def preprocessing(d): ...
 
 # initialize the components
 pb = ProgressBar("Processing", total=len(data_list))
 logger = Logger("Log message")
 var = Variable("Some Value", 0)
-line_chart = LineChart("Line Chart", "x", "y")
+line_chart = LineChart("Line Chart", x_label="x", y_label="y")
 view = View("Data preprocessing").add_all()
 
 t0 = time.time()
 # open server when the code block in running.
 with Server(view, port=8000):
     for i, data in enumerate(data_list):
         preprocessing(data) # do some processing here
@@ -301,15 +302,15 @@
 ```python
 from typing import Optional, Union, Sequence, Dict, List
 
 import torch.nn
 from torch import Tensor
 from torch.optim import Adam
 from torchmetrics import Accuracy
-from pytorch_lightning.callbacks import ModelCheckpoint
+from lightning.pytorch.callbacks import ModelCheckpoint
 
 import tensorneko as neko
 from tensorneko.util import get_activation, get_loss
 
 
 class MnistClassifier(neko.NekoModel):
```

### Comparing `tensorneko-0.2.9/README.md` & `tensorneko-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,21 @@
     <a href="https://pypi.org/project/tensorneko/"><img src="https://img.shields.io/pypi/dm/tensorneko?style=flat-square"></a>
     <img src="https://img.shields.io/github/license/ControlNet/tensorneko?style=flat-square">
 </div>
 
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
-    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
+    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Lightning-2.0.*-792EE5?style=flat-square&logo=lightning"></a>
 </div>
 
 <div align="center">
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
+    <a href="https://coveralls.io/github/ControlNet/tensorneko"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/tensorneko?style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -209,15 +210,15 @@
 data_list = ... # a list of data
 def preprocessing(d): ...
 
 # initialize the components
 pb = ProgressBar("Processing", total=len(data_list))
 logger = Logger("Log message")
 var = Variable("Some Value", 0)
-line_chart = LineChart("Line Chart", "x", "y")
+line_chart = LineChart("Line Chart", x_label="x", y_label="y")
 view = View("Data preprocessing").add_all()
 
 t0 = time.time()
 # open server when the code block in running.
 with Server(view, port=8000):
     for i, data in enumerate(data_list):
         preprocessing(data) # do some processing here
@@ -275,15 +276,15 @@
 ```python
 from typing import Optional, Union, Sequence, Dict, List
 
 import torch.nn
 from torch import Tensor
 from torch.optim import Adam
 from torchmetrics import Accuracy
-from pytorch_lightning.callbacks import ModelCheckpoint
+from lightning.pytorch.callbacks import ModelCheckpoint
 
 import tensorneko as neko
 from tensorneko.util import get_activation, get_loss
 
 
 class MnistClassifier(neko.NekoModel):
```

### Comparing `tensorneko-0.2.9/setup.py` & `tensorneko-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src", include=["tensorneko", "tensorneko.*"]),
     package_data={
         "tensorneko": [
             "version.txt"
         ]
     },
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Utilities"
     ],
 )
```

### Comparing `tensorneko-0.2.9/src/tensorneko/__init__.py` & `tensorneko-0.3.0/src/tensorneko/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/arch/auto_encoder.py` & `tensorneko-0.3.0/src/tensorneko/arch/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/arch/gan.py` & `tensorneko-0.3.0/src/tensorneko/arch/gan.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         return {
             "loss": d_loss + g_loss,
             **{k: v for k, v in d_result.items() if k != "loss"},
             **{k: v for k, v in g_result.items() if k != "loss"},
         }
 
     def on_validation_epoch_end(self) -> None:
-        super().on_epoch_end()
+        super().on_validation_epoch_end()
         if self.sample_z is None:
             self.sample_z = torch.randn(self.num_samples, self.latent_dim, device=self.device)
         sample_generated = self.generator(self.sample_z)
         grid = torchvision.utils.make_grid(sample_generated, nrow=self.grid_cols)
         self.log_image("sample_images", grid)
 
     def configure_optimizers(self):
```

### Comparing `tensorneko-0.2.9/src/tensorneko/arch/vqvae.py` & `tensorneko-0.3.0/src/tensorneko/arch/vqvae.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/arch/wgan.py` & `tensorneko-0.3.0/src/tensorneko/arch/wgan.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/__init__.py` & `tensorneko-0.3.0/src/tensorneko/callback/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/earlystop_lr.py` & `tensorneko-0.3.0/src/tensorneko/callback/earlystop_lr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pytorch_lightning import Trainer, LightningModule
-from pytorch_lightning.callbacks import Callback
+from lightning.pytorch import Trainer, LightningModule
+from lightning.pytorch.callbacks import Callback
 import re
 
 
 class EarlyStoppingLR(Callback):
 
     def __init__(self, lr_threshold: float, mode="all"):
         self.lr_threshold = lr_threshold
```

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/epoch_time_logger.py` & `tensorneko-0.3.0/src/tensorneko/callback/epoch_time_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import time
 
-from pytorch_lightning import Callback, Trainer, LightningModule
+from lightning.pytorch import Callback, Trainer, LightningModule
 
 
 class EpochTimeLogger(Callback):
     """Log spent time for each training epoch"""
     start_time: float
 
     def on_train_epoch_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
```

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/gpu_stats_logger.py` & `tensorneko-0.3.0/src/tensorneko/callback/gpu_stats_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytorch_lightning import Callback, Trainer, LightningModule
+from lightning.pytorch import Callback, Trainer, LightningModule
 
 
 class GpuStatsLogger(Callback):
     """Log GPU stats for each training epoch"""
 
     def __init__(self, delay: float = 0.5):
         try:
```

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/lr_logger.py` & `tensorneko-0.3.0/src/tensorneko/callback/lr_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytorch_lightning import Callback, Trainer, LightningModule
+from lightning.pytorch import Callback, Trainer, LightningModule
 
 
 class LrLogger(Callback):
     """Log learning rate in each epoch start."""
 
     def on_train_epoch_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
         for i, optimizer in enumerate(trainer.optimizers):
```

### Comparing `tensorneko-0.2.9/src/tensorneko/callback/system_stats_logger.py` & `tensorneko-0.3.0/src/tensorneko/callback/system_stats_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pytorch_lightning import Callback, Trainer, LightningModule
+from lightning.pytorch import Callback, Trainer, LightningModule
 
 
 class SystemStatsLogger(Callback):
     """Log system stats for each training epoch"""
 
     def __init__(self):
         try:
```

### Comparing `tensorneko-0.2.9/src/tensorneko/dataset/nested_dataset.py` & `tensorneko-0.3.0/src/tensorneko/dataset/nested_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/dataset/round_robin_dataset.py` & `tensorneko-0.3.0/src/tensorneko/dataset/round_robin_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/evaluation/fid.py` & `tensorneko-0.3.0/src/tensorneko/evaluation/fid.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/evaluation/iou.py` & `tensorneko-0.3.0/src/tensorneko/evaluation/iou.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/evaluation/psnr.py` & `tensorneko-0.3.0/src/tensorneko/evaluation/psnr.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/evaluation/ssim.py` & `tensorneko-0.3.0/src/tensorneko/evaluation/ssim.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/io/reader.py` & `tensorneko-0.3.0/src/tensorneko/io/reader.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/io/writer.py` & `tensorneko-0.3.0/src/tensorneko/io/writer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/__init__.py` & `tensorneko-0.3.0/src/tensorneko/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/aggregation.py` & `tensorneko-0.3.0/src/tensorneko/layer/aggregation.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/attention.py` & `tensorneko-0.3.0/src/tensorneko/layer/attention.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/concatenate.py` & `tensorneko-0.3.0/src/tensorneko/layer/concatenate.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/conv.py` & `tensorneko-0.3.0/src/tensorneko/layer/conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/linear.py` & `tensorneko-0.3.0/src/tensorneko/layer/linear.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/log.py` & `tensorneko-0.3.0/src/tensorneko/layer/log.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/masked_conv2d.py` & `tensorneko-0.3.0/src/tensorneko/layer/masked_conv2d.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/noise.py` & `tensorneko-0.3.0/src/tensorneko/layer/noise.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/patching.py` & `tensorneko-0.3.0/src/tensorneko/layer/patching.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/positional_embedding.py` & `tensorneko-0.3.0/src/tensorneko/layer/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/reshape.py` & `tensorneko-0.3.0/src/tensorneko/layer/reshape.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/stack.py` & `tensorneko-0.3.0/src/tensorneko/layer/stack.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/layer/vector_quantizer.py` & `tensorneko-0.3.0/src/tensorneko/layer/vector_quantizer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/dense.py` & `tensorneko-0.3.0/src/tensorneko/module/dense.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/gated_conv.py` & `tensorneko-0.3.0/src/tensorneko/module/gated_conv.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/inception.py` & `tensorneko-0.3.0/src/tensorneko/module/inception.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/mlp.py` & `tensorneko-0.3.0/src/tensorneko/module/mlp.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/residual.py` & `tensorneko-0.3.0/src/tensorneko/module/residual.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/module/transformer.py` & `tensorneko-0.3.0/src/tensorneko/module/transformer.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/neko_model.py` & `tensorneko-0.3.0/src/tensorneko/neko_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,89 @@
 from abc import abstractmethod
-from typing import Optional, Dict, Union, Sequence, Any
+from typing import Optional, Dict, Union, Sequence, Any, List
 
 import torch
-from pytorch_lightning import LightningModule
-from pytorch_lightning.loggers import LightningLoggerBase
-from pytorch_lightning.utilities.types import EPOCH_OUTPUT, STEP_OUTPUT
+from lightning.pytorch import LightningModule
+from lightning.pytorch.loggers import Logger
+from lightning.pytorch.utilities.types import STEP_OUTPUT
 from torch import Tensor
 
 from .neko_module import NekoModule
 from .neko_trainer import NekoTrainer
 from .util import summarize_dict_by, Shape
 
+EPOCH_OUTPUT = List[STEP_OUTPUT]
+
 
 class NekoModel(LightningModule, NekoModule):
     """
     An abstract class for models. In this module, the loss and other metrics will be automatically logged in
     TensorBoard.
 
     Args:
         name (``str``): Model name
 
         input_shape (:class:`~tensorneko.util.Shape`, optional):
             An optional argument can allow it to plot a graph for TensorBoard
 
-        *args: Other arguments for :class:`~pytorch_lightning.core.lightning.LightningModule`
+        *args: Other arguments for :class:`~lightning.pytorch.core.lightning.LightningModule`
 
-        **kwargs: Other arguments for :class:`~pytorch_lightning.core.lightning.LightningModule`
+        **kwargs: Other arguments for :class:`~lightning.pytorch.core.lightning.LightningModule`
     """
     trainer: NekoTrainer
 
     def __init__(self, name: str,
         input_shape: Optional[Shape] = None, distributed=False, *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
         self.name = name
         self.distributed = distributed
         self.can_plot_graph = input_shape is not None
         if self.can_plot_graph:
             self.input_shape = input_shape
             self.example_input_array = torch.rand([1, *input_shape])
         self.history = []
+        self.training_step_outputs = []
+        self.validation_step_outputs = []
 
     @abstractmethod
     def forward(self, *args, **kwargs):
         ...
 
     @abstractmethod
     def training_step(self,
         batch: Optional[Union[Tensor, Sequence[Tensor]]] = None,
         batch_idx: Optional[int] = None,
         optimizer_idx: Optional[int] = None,
         hiddens: Optional[Tensor] = None
     ) -> Dict[str, Tensor]:
         """
-        The method inherit from :meth:`~pytorch_lightning.core.lightning.LightningModule.training_step`.
+        The method inherit from :meth:`~lightning.pytorch.core.lightning.LightningModule.training_step`.
 
         Here you compute and return the training loss and some additional metrics for e.g.
         the progress bar or logger.
 
         Args:
             batch (:class:`~torch.Tensor` | (:class:`~torch.Tensor`, ...) | [:class:`~torch.Tensor`, ...]):
                 The output of your :class:`~torch.utils.data.DataLoader`. A tensor, tuple or list.
 
             batch_idx (``int``): Integer displaying index of this batch
 
             optimizer_idx (``int``, optional): When using multiple optimizers, this argument will also be present.
 
             hiddens(:class:`~torch.Tensor`, optional): Passed in if
-                :paramref:`~pytorch_lightning.core.lightning.LightningModule.truncated_bptt_steps` > 0.
+                :paramref:`~lightning.pytorch.core.lightning.LightningModule.truncated_bptt_steps` > 0.
 
         Returns:
             ``Dict`` [``str``, :class:`~torch.Tensor`]:
                 A dictionary. Can include any keys, but must include the key ``'loss'``
 
         Notes:
             The return value can be other types, but you need to handle them by override the
-                method :meth:`~pytorch_lightning.TrainingModule.training_step_end`
+                method :meth:`~lightning.pytorch.TrainingModule.training_step_end`
 
         Examples::
 
             def training_step(self, batch, batch_idx):
                 x, y = batch
                 out = self(x)
                 loss = self.loss(out, x)
@@ -90,15 +94,15 @@
     @abstractmethod
     def validation_step(self,
         batch: Optional[Union[Tensor, Sequence[Tensor]]] = None,
         batch_idx: Optional[int] = None,
         dataloader_idx: Optional[int] = None
     ) -> Dict[str, Tensor]:
         """
-        The method inherit from :meth:`~pytorch_lightning.core.lightning.LightningModule.validation_step`.
+        The method inherit from :meth:`~lightning.pytorch.core.lightning.LightningModule.validation_step`.
 
         Operates on a single batch of data from the validation set.
         In this step you'd might generate examples or calculate anything of interest like accuracy.
 
         Args:
             batch (:class:`~torch.Tensor` | (:class:`~torch.Tensor`, ...) | [:class:`~torch.Tensor`, ...]):
                 The output of your :class:`~torch.utils.data.DataLoader`. A tensor, tuple or list.
@@ -121,18 +125,18 @@
                 acc = self.acc(out, x)
                 return {"loss": loss, "acc": acc}
         """
         ...
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: Optional[int] = None) -> Any:
         """
-        Inherit from :meth:`~pytorch_lightning.core.lightning.LightningModule.predict_step`.
+        Inherit from :meth:`~lightning.pytorch.core.lightning.LightningModule.predict_step`.
 
-        Step function called during :meth:`~pytorch_lightning.trainer.trainer.Trainer.predict`.
-        By default, it calls :meth:`~pytorch_lightning.core.lightning.LightningModule.forward`.
+        Step function called during :meth:`~lightning.pytorch.trainer.trainer.Trainer.predict`.
+        By default, it calls :meth:`~lightning.pytorch.core.lightning.LightningModule.forward`.
         Override to add any processing logic.
 
         Args:
             batch (:class:`~torch.Tensor`): Current batch
             batch_idx (``int``): Index of current batch
             dataloader_idx (``int``, optional): Index of the current dataloader
 
@@ -146,46 +150,54 @@
         batch_idx: Optional[int] = None,
         dataloader_idx: Optional[int] = None
     ) -> Dict[str, Tensor]:
         return self.validation_step(batch, batch_idx, dataloader_idx)
 
     @abstractmethod
     def configure_optimizers(self):
-        """Inherit from :meth:`~pytorch_lightning.core.lightning.LightningModule.configure_optimizers`."""
+        """Inherit from :meth:`~lightning.pytorch.core.lightning.LightningModule.configure_optimizers`."""
         ...
 
     @property
-    def logger(self) -> Optional[LightningLoggerBase]:
+    def logger(self) -> Optional[Logger]:
         """
         Returns:
-            :class:`~pytorch_lightning.loggers.LightningLoggerBase` | ``None``:
+            :class:`~lightning.pytorch.loggers.LightningLoggerBase` | ``None``:
                 The training or validation logger for the module.
         """
         if not self.trainer:
             return None
         else:
             return self.trainer.logger
 
-    def training_epoch_end(self, outputs: EPOCH_OUTPUT) -> None:
+    def on_train_batch_end(self, outputs: STEP_OUTPUT, batch: Any, batch_idx: int) -> None:
+        """For each training step end, log the metrics. Append the outputs of training step to the list"""
+        self.training_step_outputs.append(outputs)
+        if self.trainer.log_on_step \
+            and self.logger is not None \
+            and self.trainer.global_step % self.trainer.log_every_n_steps == 0:
+            self.log_on_training_step_end(outputs)
+
+    def on_validation_batch_end(
+        self, outputs: Optional[STEP_OUTPUT], batch: Any, batch_idx: int, dataloader_idx: int = 0
+    ) -> None:
+        """Append the outputs of validation step to the list"""
+        self.validation_step_outputs.append(outputs)
+
+    def on_train_epoch_end(self) -> None:
         """For each training epoch end, log the metrics"""
         if self.trainer.log_on_epoch and self.logger is not None:
-            self.log_on_training_epoch_end(outputs)
+            self.log_on_training_epoch_end(self.training_step_outputs)
+        self.training_step_outputs.clear()
 
-    def validation_epoch_end(self, outputs: EPOCH_OUTPUT) -> None:
+    def on_validation_epoch_end(self) -> None:
         """For each validation epoch end, log the metrics"""
         if self.logger is not None:
-            self.log_on_validation_epoch_end(outputs)
-
-    def training_step_end(self, output: STEP_OUTPUT) -> STEP_OUTPUT:
-        """For each training step end, log the metrics"""
-        if self.trainer.log_on_step \
-            and self.logger is not None \
-            and self.trainer.global_step % self.trainer.log_every_n_steps == 0:
-            self.log_on_training_step_end(output)
-        return output
+            self.log_on_validation_epoch_end(self.validation_step_outputs)
+        self.validation_step_outputs.clear()
 
     def log_on_training_epoch_end(self, outputs: EPOCH_OUTPUT) -> None:
         """Log the training epoch outputs"""
         history_item = {}
         for key in outputs[0].keys():
             getter = summarize_dict_by(key, torch.mean)
             value = getter(outputs)
@@ -202,29 +214,30 @@
         for key in outputs[0].keys():
             getter = summarize_dict_by(key, torch.mean)
             value = getter(outputs)
             self.history[-1]["val_" + key] = value
             self.logger.log_metrics({key: value}, step=self.trainer.global_step)
             self.log(key, value, on_epoch=True, on_step=False, logger=False, sync_dist=self.distributed)
             self.log(f"val_{key}", value, on_epoch=True, on_step=False, logger=False, prog_bar=True,
-                     sync_dist=self.distributed)
+                sync_dist=self.distributed)
 
     def log_on_training_step_end(self, output: STEP_OUTPUT) -> None:
         """Log the training step outputs"""
         history_item = {}
         for key, value in output.items():
             history_item[key] = value
             self.logger.log_metrics({key: value}, step=self.trainer.global_step)
             self.log(key, value, on_epoch=False, on_step=True, logger=False, sync_dist=self.distributed)
         self.history.append(history_item)
 
-    def test_step_end(self, output: STEP_OUTPUT) -> Optional[STEP_OUTPUT]:
+    def on_test_batch_end(
+        self, outputs: Optional[STEP_OUTPUT], batch: Any, batch_idx: int, dataloader_idx: int = 0
+    ) -> None:
         """For each test step end, log the metrics"""
-        self.log_dict(output, sync_dist=self.distributed)
-        return output
+        self.log_dict(outputs, sync_dist=self.distributed)
 
     def log_image(self, name: str, image: torch.Tensor) -> None:
         """Log an image to the logger"""
         if self.logger is None:
             return
 
         self.logger.experiment.add_image(name, torch.clip(image, 0, 1), self.trainer.global_step)
```

### Comparing `tensorneko-0.2.9/src/tensorneko/neko_module.py` & `tensorneko-0.3.0/src/tensorneko/neko_module.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/neko_trainer.py` & `tensorneko-0.3.0/src/tensorneko/neko_trainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,69 @@
 import os
 from datetime import timedelta
-from pathlib import Path
 from time import time
 from typing import Optional, Union, List, Dict
 
-from pytorch_lightning import Trainer, Callback
-from pytorch_lightning.accelerators import Accelerator
-from pytorch_lightning.callbacks import ModelCheckpoint, Checkpoint
-from pytorch_lightning.loggers import Logger, TensorBoardLogger
-from pytorch_lightning.plugins import PLUGIN_INPUT
-from pytorch_lightning.profilers import Profiler
-from pytorch_lightning.strategies import Strategy
-from pytorch_lightning.trainer.connectors.accelerator_connector import _LITERAL_WARN
+from lightning.pytorch import Trainer, Callback
+from lightning.pytorch.accelerators import Accelerator
+from lightning.pytorch.callbacks import ModelCheckpoint, Checkpoint
+from lightning.pytorch.loggers import Logger, TensorBoardLogger
+from lightning.pytorch.plugins import PLUGIN_INPUT
+from lightning.pytorch.profilers import Profiler
+from lightning.pytorch.strategies import Strategy
+from lightning.pytorch.trainer.connectors.accelerator_connector import _LITERAL_WARN
+from lightning.fabric.plugins.precision.precision import _PRECISION_INPUT
+from lightning.fabric.utilities.types import _PATH
 
 from .callback import NilCallback, LrLogger, EpochNumLogger, EpochTimeLogger, GpuStatsLogger, SystemStatsLogger
 
 
 class NekoTrainer(Trainer):
 
     def __init__(self,
         logger: Optional[str],
         enable_checkpointing: bool = True,
         callbacks: Optional[Union[List[Callback], Callback]] = None,
         log_every_n_steps: int = 50,
-        gpus: int = 0,
-        precision: Union[int, str] = 32,
-        default_root_dir: Optional[str] = None,
-        gradient_clip_val: float = 0.0,
-        gradient_clip_algorithm: str = 'norm',
+        precision: _PRECISION_INPUT = "32-true",
+        accelerator: Union[str, Accelerator] = "auto",
+        strategy: Union[str, Strategy] = "auto",
+        devices: Union[List[int], str, int] = "auto",
         num_nodes: int = 1,
-        num_processes: Optional[int] = None,  # TODO: Remove in 2.0
-        tpu_cores: Optional[Union[List[int], str, int]] = None,  # TODO: Remove in 2.0
-        ipus: Optional[int] = None,  # TODO: Remove in 2.0
-        devices: Optional[Union[List[int], str, int]] = None,
-        auto_select_gpus: bool = False,
-        enable_progress_bar: bool = True,
-        overfit_batches: Union[int, float] = 0.0,
-        track_grad_norm: Union[int, float, str] = -1,
-        check_val_every_n_epoch: Optional[int] = 1,
         fast_dev_run: Union[int, bool] = False,
-        accumulate_grad_batches: Optional[Union[int, Dict[int, int]]] = None,
         max_epochs: Optional[int] = None,
         min_epochs: Optional[int] = None,
         max_steps: int = -1,
         min_steps: Optional[int] = None,
         max_time: Optional[Union[str, timedelta, Dict[str, int]]] = None,
         limit_train_batches: Optional[Union[int, float]] = None,
         limit_val_batches: Optional[Union[int, float]] = None,
         limit_test_batches: Optional[Union[int, float]] = None,
         limit_predict_batches: Optional[Union[int, float]] = None,
+        overfit_batches: Union[int, float] = 0.0,
         val_check_interval: Optional[Union[int, float]] = None,
-        accelerator: Optional[Union[str, Accelerator]] = None,
-        strategy: Optional[Union[str, Strategy]] = None,
-        sync_batchnorm: bool = False,
-        enable_model_summary: bool = True,
-        weights_save_path: Optional[str] = None,  # TODO: Remove in 1.8
-        num_sanity_val_steps: int = 2,
-        resume_from_checkpoint: Optional[Union[Path, str]] = None,
-        profiler: Optional[Union[Profiler, str]] = None,
-        benchmark: Optional[bool] = None,
+        check_val_every_n_epoch: Optional[int] = 1,
+        num_sanity_val_steps: Optional[int] = None,
+        enable_progress_bar: Optional[bool] = None,
+        enable_model_summary: Optional[bool] = None,
+        accumulate_grad_batches: int = 1,
+        gradient_clip_val: Optional[Union[int, float]] = None,
+        gradient_clip_algorithm: Optional[str] = None,
         deterministic: Optional[Union[bool, _LITERAL_WARN]] = None,
-        reload_dataloaders_every_n_epochs: int = 0,
-        auto_lr_find: Union[bool, str] = False,
-        replace_sampler_ddp: bool = True,
+        benchmark: Optional[bool] = True,
+        inference_mode: bool = True,
+        use_distributed_sampler: bool = True,
+        profiler: Optional[Union[Profiler, str]] = None,
         detect_anomaly: bool = False,
-        auto_scale_batch_size: Union[str, bool] = False,
+        barebones: bool = False,
         plugins: Optional[Union[PLUGIN_INPUT, List[PLUGIN_INPUT]]] = None,
-        amp_backend: str = "native",
-        amp_level: Optional[str] = None,
-        move_metrics_to_cpu: bool = False,
-        multiple_trainloader_mode: str = "max_size_cycle",
+        sync_batchnorm: bool = False,
+        reload_dataloaders_every_n_epochs: int = 0,
+        default_root_dir: Optional[_PATH] = None,
     ):
-        super().__init__()
-
         # define a random logger name
         self.log_name = f"{logger}_{int(time())}"
         if callbacks is None:
             callbacks = []
         # build checkpoint callback or from user defined
         if enable_checkpointing and len([c for c in callbacks if isinstance(c, Checkpoint)]) == 0:
             # use default checkpoint callback
@@ -129,63 +116,105 @@
         if self.log_on_epoch:
             log_every_n_steps = 10000000
 
         super().__init__(
             logger=logger is not None,
             enable_checkpointing=enable_checkpointing,
             callbacks=cbs,
-            default_root_dir=default_root_dir,
-            gradient_clip_val=gradient_clip_val,
-            gradient_clip_algorithm=gradient_clip_algorithm,
-            num_nodes=num_nodes,
-            num_processes=num_processes,
+            accelerator=accelerator,
+            strategy=strategy,
             devices=devices,
-            gpus=gpus,
-            auto_select_gpus=auto_select_gpus,
-            tpu_cores=tpu_cores,
-            ipus=ipus,
-            enable_progress_bar=enable_progress_bar,
-            overfit_batches=overfit_batches,
-            track_grad_norm=track_grad_norm,
-            check_val_every_n_epoch=check_val_every_n_epoch,
+            num_nodes=num_nodes,
+            precision=precision,
             fast_dev_run=fast_dev_run,
-            accumulate_grad_batches=accumulate_grad_batches,
             max_epochs=max_epochs,
             min_epochs=min_epochs,
             max_steps=max_steps,
             min_steps=min_steps,
             max_time=max_time,
             limit_train_batches=limit_train_batches,
             limit_val_batches=limit_val_batches,
             limit_test_batches=limit_test_batches,
             limit_predict_batches=limit_predict_batches,
+            overfit_batches=overfit_batches,
             val_check_interval=val_check_interval,
+            check_val_every_n_epoch=check_val_every_n_epoch,
+            num_sanity_val_steps=num_sanity_val_steps,
             log_every_n_steps=log_every_n_steps,
-            accelerator=accelerator,
-            strategy=strategy,
-            sync_batchnorm=sync_batchnorm,
-            precision=precision,
+            enable_progress_bar=enable_progress_bar,
             enable_model_summary=enable_model_summary,
-            weights_save_path=weights_save_path,
-            num_sanity_val_steps=num_sanity_val_steps,
-            resume_from_checkpoint=resume_from_checkpoint,
-            profiler=profiler,
-            benchmark=benchmark,
+            accumulate_grad_batches=accumulate_grad_batches,
+            gradient_clip_val=gradient_clip_val,
+            gradient_clip_algorithm=gradient_clip_algorithm,
             deterministic=deterministic,
-            reload_dataloaders_every_n_epochs=reload_dataloaders_every_n_epochs,
-            auto_lr_find=auto_lr_find,
-            replace_sampler_ddp=replace_sampler_ddp,
+            benchmark=benchmark,
+            inference_mode=inference_mode,
+            use_distributed_sampler=use_distributed_sampler,
+            profiler=profiler,
             detect_anomaly=detect_anomaly,
-            auto_scale_batch_size=auto_scale_batch_size,
+            barebones=barebones,
             plugins=plugins,
-            amp_backend=amp_backend,
-            amp_level=amp_level,
-            move_metrics_to_cpu=move_metrics_to_cpu,
-            multiple_trainloader_mode=multiple_trainloader_mode
+            sync_batchnorm=sync_batchnorm,
+            reload_dataloaders_every_n_epochs=reload_dataloaders_every_n_epochs,
+            default_root_dir=default_root_dir,
         )
+
+        # super().__init__(
+        #     logger=logger is not None,
+        #     enable_checkpointing=enable_checkpointing,
+        #     callbacks=cbs,
+        #     default_root_dir=default_root_dir,
+        #     gradient_clip_val=gradient_clip_val,
+        #     gradient_clip_algorithm=gradient_clip_algorithm,
+        #     num_nodes=num_nodes,
+        #     num_processes=num_processes,
+        #     devices=devices,
+        #     gpus=gpus,
+        #     auto_select_gpus=auto_select_gpus,
+        #     tpu_cores=tpu_cores,
+        #     ipus=ipus,
+        #     enable_progress_bar=enable_progress_bar,
+        #     overfit_batches=overfit_batches,
+        #     track_grad_norm=track_grad_norm,
+        #     check_val_every_n_epoch=check_val_every_n_epoch,
+        #     fast_dev_run=fast_dev_run,
+        #     accumulate_grad_batches=accumulate_grad_batches,
+        #     max_epochs=max_epochs,
+        #     min_epochs=min_epochs,
+        #     max_steps=max_steps,
+        #     min_steps=min_steps,
+        #     max_time=max_time,
+        #     limit_train_batches=limit_train_batches,
+        #     limit_val_batches=limit_val_batches,
+        #     limit_test_batches=limit_test_batches,
+        #     limit_predict_batches=limit_predict_batches,
+        #     val_check_interval=val_check_interval,
+        #     log_every_n_steps=log_every_n_steps,
+        #     accelerator=accelerator,
+        #     strategy=strategy,
+        #     sync_batchnorm=sync_batchnorm,
+        #     precision=precision,
+        #     enable_model_summary=enable_model_summary,
+        #     weights_save_path=weights_save_path,
+        #     num_sanity_val_steps=num_sanity_val_steps,
+        #     resume_from_checkpoint=resume_from_checkpoint,
+        #     profiler=profiler,
+        #     benchmark=benchmark,
+        #     deterministic=deterministic,
+        #     reload_dataloaders_every_n_epochs=reload_dataloaders_every_n_epochs,
+        #     auto_lr_find=auto_lr_find,
+        #     replace_sampler_ddp=replace_sampler_ddp,
+        #     detect_anomaly=detect_anomaly,
+        #     auto_scale_batch_size=auto_scale_batch_size,
+        #     plugins=plugins,
+        #     amp_backend=amp_backend,
+        #     amp_level=amp_level,
+        #     move_metrics_to_cpu=move_metrics_to_cpu,
+        #     multiple_trainloader_mode=multiple_trainloader_mode
+        # )
         # init loggers for training and validation
         self.has_no_logger = logger is None
 
         self.logger_train = TensorBoardLogger(save_dir=self.default_root_dir, name="logs",
             version=os.path.join(self.log_name, "train"), log_graph=False
             # TODO: Fix log_Graph
         ) if self.has_no_logger is not None else None
```

### Comparing `tensorneko-0.2.9/src/tensorneko/preprocess/__init__.py` & `tensorneko-0.3.0/src/tensorneko/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/preprocess/crop.py` & `tensorneko-0.3.0/src/tensorneko/preprocess/crop.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/preprocess/enum.py` & `tensorneko-0.3.0/src/tensorneko/preprocess/enum.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/preprocess/pad.py` & `tensorneko-0.3.0/src/tensorneko/preprocess/pad.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/__init__.py` & `tensorneko-0.3.0/src/tensorneko/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/configuration.py` & `tensorneko-0.3.0/src/tensorneko/util/configuration.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/dispatched_misc.py` & `tensorneko-0.3.0/src/tensorneko/util/dispatched_misc.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/misc.py` & `tensorneko-0.3.0/src/tensorneko/util/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import numpy
 import numpy as np
 import torch
 from torch import Tensor
 from torch.nn import Module
 
-from tensorneko_util.util import F, _
 from tensorneko_util.util.misc import generate_inf_seq, listdir, with_printed, ifelse, dict_add, as_list, \
     identity, list_to_dict, compose, circular_pad
 from .type import T, A
 
 
 def reduce_dict_by(key: str, op: Callable[[T, T], T]) -> Callable[[List[Dict[str, T]]], T]:
     """
@@ -36,15 +35,18 @@
         6.3
         >>> reduce_dict_by("b", lambda x1, x2: x1 - x2)(x)
         -1
         >>> reduce_dict_by("c", lambda x1, x2: 10 * x1 + x2)(x)
         tensor([350.])
 
     """
-    return F() >> (map, _[key]) >> list >> F(reduce, op)
+    def wrapper(x: List[Dict[str, T]]) -> T:
+        values = [d[key] for d in x]
+        return reduce(op, values)
+    return wrapper
 
 
 def summarize_dict_by(key: str, op: Callable[[Union[Sequence[T], T]], T]
 ) -> Callable[[List[Dict[str, T]]], T]:
     """
     Apply summarizer function to a list of dictionaries.
 
@@ -75,23 +77,22 @@
         >>>     return x
         >>> summarize_dict_by("c", some_func)(x)
         350
         >>> summarize_dict_by("d", lambda x: np.sum(x, axis=0))(x)
         array([3.])
 
     """
-    return F() >> (map, _[key]) >> list >> ifelse(
-        lambda xs: type(xs[0]) is Tensor,
-        func_true=torch.vstack,
-        func_false=ifelse(
-            lambda xs: type(xs[0]) is np.ndarray,
-            func_true=numpy.vstack,
-            func_false=_
-        )
-    ) >> op
+    def wrapper(x: List[Dict[str, T]]) -> T:
+        values = [d[key] for d in x]
+        if type(values[0]) is Tensor:
+            values = torch.vstack(values)
+        elif type(values[0]) is np.ndarray:
+            values = np.vstack(values)
+        return op(values)
+    return wrapper
 
 
 def with_printed_shape(x: A) -> A:
     """
     An identity function but with shape printed .
 
     Args:
@@ -104,15 +105,15 @@
 
         >>> x = torch.tensor([1.5, 2.5, 3.5])
         >>> y = with_printed_shape(x)
         torch.Size([3])
         >>> x == y
         tensor([True, True, True])
     """
-    return F(with_printed, func=lambda tensor: tensor.shape)(x)
+    return with_printed(x, func=lambda tensor: tensor.shape)
 
 
 def is_bad_num(x: Tensor) -> Tensor:
     """
     Checking the element in input tensor is bad number (NaN or Inf).
 
     Args:
```

### Comparing `tensorneko-0.2.9/src/tensorneko/util/reproducibility.py` & `tensorneko-0.3.0/src/tensorneko/util/reproducibility.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/string_getter.py` & `tensorneko-0.3.0/src/tensorneko/util/string_getter.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/util/type.py` & `tensorneko-0.3.0/src/tensorneko/util/type.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/visualization/__init__.py` & `tensorneko-0.3.0/src/tensorneko/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko/visualization/log_graph.py` & `tensorneko-0.3.0/src/tensorneko/visualization/log_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Iterable
 
 import torch
 from torch import randn
 from torch.nn import Module
-from torch.utils.tensorboard import SummaryWriter
 
 from ..util import Shape
 
 
 def log_graph(module: Module, input_shape_list: Iterable[Shape], log_dir: str = None) -> None:
     """
     Plot a graph of model for TensorBoard.
@@ -36,14 +35,15 @@
 
         .. code-block:: bash
 
             tensorboard --logdir="graphs"
 
     """
 
+    from torch.utils.tensorboard import SummaryWriter
     writer = SummaryWriter(log_dir=log_dir)
     xs = list(map(lambda shape: randn(torch.Size((1, *shape))), input_shape_list))
     if len(xs) == 1:
         writer.add_graph(module, xs[0])
     else:
         writer.add_graph(module, xs)
     writer.close()
```

### Comparing `tensorneko-0.2.9/src/tensorneko/visualization/matplotlib.py` & `tensorneko-0.3.0/src/tensorneko/visualization/matplotlib.py`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/src/tensorneko.egg-info/PKG-INFO` & `tensorneko-0.3.0/src/tensorneko.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: tensorneko
-Version: 0.2.9
+Version: 0.3.0
 Summary: Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 Home-page: https://github.com/ControlNet/tensorneko
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/tensorneko/issues
 Project-URL: Source Code, https://github.com/ControlNet/tensorneko
 Keywords: deep learning,pytorch,AI
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 style="text-align: center">TensorNeko</h1> 
 
 <div align="center">
     <img src="https://img.shields.io/github/stars/ControlNet/tensorneko?style=flat-square">
@@ -34,20 +34,21 @@
     <a href="https://pypi.org/project/tensorneko/"><img src="https://img.shields.io/pypi/dm/tensorneko?style=flat-square"></a>
     <img src="https://img.shields.io/github/license/ControlNet/tensorneko?style=flat-square">
 </div>
 
 <div align="center">    
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/tensorneko?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.9.0-EE4C2C?style=flat-square&logo=pytorch"></a>
-    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Pytorch%20Lightning-1.7.*-792EE5?style=flat-square&logo=pytorch-lightning"></a>
+    <a href="https://www.pytorchlightning.ai/"><img src="https://img.shields.io/badge/Lightning-2.0.*-792EE5?style=flat-square&logo=lightning"></a>
 </div>
 
 <div align="center">
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/unittest.yml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/tensorneko/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/tensorneko/release.yml?branch=master&label=release&style=flat-square"></a>
+    <a href="https://coveralls.io/github/ControlNet/tensorneko"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/tensorneko?style=flat-square"></a>
 </div>
 
 Tensor Neural Engine Kompanion. An util library based on PyTorch and PyTorch Lightning.
 
 ## Install
 
 ```shell
@@ -235,15 +236,15 @@
 data_list = ... # a list of data
 def preprocessing(d): ...
 
 # initialize the components
 pb = ProgressBar("Processing", total=len(data_list))
 logger = Logger("Log message")
 var = Variable("Some Value", 0)
-line_chart = LineChart("Line Chart", "x", "y")
+line_chart = LineChart("Line Chart", x_label="x", y_label="y")
 view = View("Data preprocessing").add_all()
 
 t0 = time.time()
 # open server when the code block in running.
 with Server(view, port=8000):
     for i, data in enumerate(data_list):
         preprocessing(data) # do some processing here
@@ -301,15 +302,15 @@
 ```python
 from typing import Optional, Union, Sequence, Dict, List
 
 import torch.nn
 from torch import Tensor
 from torch.optim import Adam
 from torchmetrics import Accuracy
-from pytorch_lightning.callbacks import ModelCheckpoint
+from lightning.pytorch.callbacks import ModelCheckpoint
 
 import tensorneko as neko
 from tensorneko.util import get_activation, get_loss
 
 
 class MnistClassifier(neko.NekoModel):
```

### Comparing `tensorneko-0.2.9/src/tensorneko.egg-info/SOURCES.txt` & `tensorneko-0.3.0/src/tensorneko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorneko-0.2.9/test/test_version.py` & `tensorneko-0.3.0/test/test_version.py`

 * *Files identical despite different names*

