# Comparing `tmp/neural-amp-modeler-0.7.1.tar.gz` & `tmp/neural-amp-modeler-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-amp-modeler-0.7.1.tar", last modified: Thu Jul 27 06:50:49 2023, max compression
+gzip compressed data, was "neural-amp-modeler-0.7.2.tar", last modified: Thu Jul 27 07:49:17 2023, max compression
```

## Comparing `neural-amp-modeler-0.7.1.tar` & `neural-amp-modeler-0.7.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.126422 neural-amp-modeler-0.7.1/
--rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-27 06:50:49.126146 neural-amp-modeler-0.7.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     5498 2023-07-27 06:27:40.000000 neural-amp-modeler-0.7.1/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.079728 neural-amp-modeler-0.7.1/nam/
--rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.1/nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.1/nam/_core.py
--rw-r--r--   0 steve      (501) staff       (20)       22 2023-07-27 06:33:38.000000 neural-amp-modeler-0.7.1/nam/_version.py
--rw-r--r--   0 steve      (501) staff       (20)    25956 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/nam/data.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.093550 neural-amp-modeler-0.7.1/nam/models/
--rw-r--r--   0 steve      (501) staff       (20)      372 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.1/nam/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.1/nam/models/_activations.py
--rw-r--r--   0 steve      (501) staff       (20)     5964 2023-06-25 16:27:08.000000 neural-amp-modeler-0.7.1/nam/models/_base.py
--rw-r--r--   0 steve      (501) staff       (20)     4816 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/nam/models/_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/nam/models/_names.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.094493 neural-amp-modeler-0.7.1/nam/models/_resources/
--rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.1/nam/models/_resources/loudness_input.wav
--rw-r--r--   0 steve      (501) staff       (20)    13555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.1/nam/models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     9120 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/nam/models/conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1984 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/nam/models/linear.py
--rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.1/nam/models/losses.py
--rw-r--r--   0 steve      (501) staff       (20)     1187 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.1/nam/models/metadata.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.102792 neural-amp-modeler-0.7.1/nam/models/parametric/
--rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.1/nam/models/parametric/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.1/nam/models/parametric/catnets.py
--rw-r--r--   0 steve      (501) staff       (20)    18233 2023-05-20 03:46:31.000000 neural-amp-modeler-0.7.1/nam/models/parametric/hyper_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/nam/models/parametric/params.py
--rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural-amp-modeler-0.7.1/nam/models/recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/nam/models/wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.107817 neural-amp-modeler-0.7.1/nam/train/
--rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/nam/train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      852 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.1/nam/train/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     3911 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.1/nam/train/colab.py
--rw-r--r--   0 steve      (501) staff       (20)    32555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.1/nam/train/core.py
--rw-r--r--   0 steve      (501) staff       (20)    21047 2023-06-22 07:01:43.000000 neural-amp-modeler-0.7.1/nam/train/gui.py
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-29 18:46:19.000000 neural-amp-modeler-0.7.1/nam/util.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.111538 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     1793 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      131 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       10 2023-07-27 06:50:49.000000 neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-07-27 06:50:49.126492 neural-amp-modeler-0.7.1/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)     1406 2023-07-27 06:40:13.000000 neural-amp-modeler-0.7.1/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.112084 neural-amp-modeler-0.7.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.1/tests/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.112711 neural-amp-modeler-0.7.1/tests/resources/
--rw-r--r--   0 steve      (501) staff       (20)      676 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.1/tests/resources/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.114078 neural-amp-modeler-0.7.1/tests/test_bin/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.1/tests/test_bin/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.115130 neural-amp-modeler-0.7.1/tests/test_bin/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.1/tests/test_bin/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6583 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.1/tests/test_bin/test_train/test_main.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_install.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.117048 neural-amp-modeler-0.7.1/tests/test_nam/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    10343 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_data.py
--rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_importable.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.121649 neural-amp-modeler-0.7.1/tests/test_nam/test_models/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     2754 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_base.py
--rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_losses.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.124330 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/
--rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     1218 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/test_catnets.py
--rw-r--r--   0 steve      (501) staff       (20)     2474 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/test_hyper_net.py
--rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 06:50:49.125352 neural-amp-modeler-0.7.1/tests/test_nam/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     4535 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_train/test_core.py
--rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.1/tests/test_nam/test_train/test_version.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.152500 neural-amp-modeler-0.7.2/
+-rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.2/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-27 07:49:17.151904 neural-amp-modeler-0.7.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     5498 2023-07-27 06:27:40.000000 neural-amp-modeler-0.7.2/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.076712 neural-amp-modeler-0.7.2/nam/
+-rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.2/nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.2/nam/_core.py
+-rw-r--r--   0 steve      (501) staff       (20)       22 2023-07-27 07:47:23.000000 neural-amp-modeler-0.7.2/nam/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)    25956 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/nam/data.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.096554 neural-amp-modeler-0.7.2/nam/models/
+-rw-r--r--   0 steve      (501) staff       (20)      372 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.2/nam/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.2/nam/models/_activations.py
+-rw-r--r--   0 steve      (501) staff       (20)     5964 2023-06-25 16:27:08.000000 neural-amp-modeler-0.7.2/nam/models/_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     4816 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/nam/models/_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/nam/models/_names.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.097957 neural-amp-modeler-0.7.2/nam/models/_resources/
+-rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.2/nam/models/_resources/loudness_input.wav
+-rw-r--r--   0 steve      (501) staff       (20)    13555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.2/nam/models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     9120 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/nam/models/conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1984 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/nam/models/linear.py
+-rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.2/nam/models/losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     1187 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.2/nam/models/metadata.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.105975 neural-amp-modeler-0.7.2/nam/models/parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.2/nam/models/parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.2/nam/models/parametric/catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)    18233 2023-05-20 03:46:31.000000 neural-amp-modeler-0.7.2/nam/models/parametric/hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/nam/models/parametric/params.py
+-rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural-amp-modeler-0.7.2/nam/models/recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/nam/models/wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.113463 neural-amp-modeler-0.7.2/nam/train/
+-rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/nam/train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      852 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.2/nam/train/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     3911 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.2/nam/train/colab.py
+-rw-r--r--   0 steve      (501) staff       (20)    32555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.2/nam/train/core.py
+-rw-r--r--   0 steve      (501) staff       (20)    21047 2023-06-22 07:01:43.000000 neural-amp-modeler-0.7.2/nam/train/gui.py
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-29 18:46:19.000000 neural-amp-modeler-0.7.2/nam/util.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.119893 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1793 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      147 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       10 2023-07-27 07:49:17.000000 neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-07-27 07:49:17.152706 neural-amp-modeler-0.7.2/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)     1442 2023-07-27 07:47:23.000000 neural-amp-modeler-0.7.2/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.120880 neural-amp-modeler-0.7.2/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.2/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.122082 neural-amp-modeler-0.7.2/tests/resources/
+-rw-r--r--   0 steve      (501) staff       (20)      676 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.2/tests/resources/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.123263 neural-amp-modeler-0.7.2/tests/test_bin/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.2/tests/test_bin/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.123818 neural-amp-modeler-0.7.2/tests/test_bin/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.2/tests/test_bin/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6583 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.2/tests/test_bin/test_train/test_main.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.129531 neural-amp-modeler-0.7.2/tests/test_nam/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    10343 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_data.py
+-rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_importable.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.142076 neural-amp-modeler-0.7.2/tests/test_nam/test_models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     2754 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_losses.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.147307 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1218 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/test_catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)     2474 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/test_hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-27 07:49:17.150154 neural-amp-modeler-0.7.2/tests/test_nam/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     4535 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_train/test_core.py
+-rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.2/tests/test_nam/test_train/test_version.py
```

### Comparing `neural-amp-modeler-0.7.1/LICENSE` & `neural-amp-modeler-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/README.md` & `neural-amp-modeler-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/__init__.py` & `neural-amp-modeler-0.7.2/nam/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/data.py` & `neural-amp-modeler-0.7.2/nam/data.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/_base.py` & `neural-amp-modeler-0.7.2/nam/models/_base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/_exportable.py` & `neural-amp-modeler-0.7.2/nam/models/_exportable.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/_resources/loudness_input.wav` & `neural-amp-modeler-0.7.2/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/base.py` & `neural-amp-modeler-0.7.2/nam/models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/conv_net.py` & `neural-amp-modeler-0.7.2/nam/models/conv_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/linear.py` & `neural-amp-modeler-0.7.2/nam/models/linear.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/losses.py` & `neural-amp-modeler-0.7.2/nam/models/losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/metadata.py` & `neural-amp-modeler-0.7.2/nam/models/metadata.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/parametric/catnets.py` & `neural-amp-modeler-0.7.2/nam/models/parametric/catnets.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/parametric/hyper_net.py` & `neural-amp-modeler-0.7.2/nam/models/parametric/hyper_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/parametric/params.py` & `neural-amp-modeler-0.7.2/nam/models/parametric/params.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/recurrent.py` & `neural-amp-modeler-0.7.2/nam/models/recurrent.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/models/wavenet.py` & `neural-amp-modeler-0.7.2/nam/models/wavenet.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/train/_version.py` & `neural-amp-modeler-0.7.2/nam/train/_version.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/train/colab.py` & `neural-amp-modeler-0.7.2/nam/train/colab.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/train/core.py` & `neural-amp-modeler-0.7.2/nam/train/core.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/nam/train/gui.py` & `neural-amp-modeler-0.7.2/nam/train/gui.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/neural_amp_modeler.egg-info/SOURCES.txt` & `neural-amp-modeler-0.7.2/neural_amp_modeler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/setup.py` & `neural-amp-modeler-0.7.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "onnxruntime",
     "pydantic",
     "pytorch_lightning",
     "scipy",
     "sounddevice",
     "tensorboard",
     "torch",
+    "transformers>=4",  # Issue-294
     "tqdm",
     "wavio>=0.0.5",  # Breaking change with older versions
 ]
 requirements.extend(get_additional_requirements())
 
 setup(
     name="neural-amp-modeler",
```

### Comparing `neural-amp-modeler-0.7.1/tests/resources/__init__.py` & `neural-amp-modeler-0.7.2/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_bin/test_train/test_main.py` & `neural-amp-modeler-0.7.2/tests/test_bin/test_train/test_main.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_data.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_data.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/base.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_base.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_conv_net.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_conv_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_exportable.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_exportable.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_losses.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/test_catnets.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/test_catnets.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_parametric/test_hyper_net.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_parametric/test_hyper_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_recurrent.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_recurrent.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_models/test_wavenet.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_models/test_wavenet.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_train/test_core.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_train/test_core.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.7.1/tests/test_nam/test_train/test_version.py` & `neural-amp-modeler-0.7.2/tests/test_nam/test_train/test_version.py`

 * *Files identical despite different names*

