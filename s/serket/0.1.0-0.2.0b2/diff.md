# Comparing `tmp/serket-0.1.0.tar.gz` & `tmp/serket-0.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serket-0.1.0.tar", last modified: Thu Jul 27 06:38:26 2023, max compression
+gzip compressed data, was "serket-0.2.0b2.tar", last modified: Thu Apr 20 00:19:56 2023, max compression
```

## Comparing `serket-0.1.0.tar` & `serket-0.2.0b2.tar`

### file list

```diff
@@ -1,22 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:38:26.879925 serket-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 06:38:06.000000 serket-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 06:38:26.879925 serket-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-27 06:38:06.000000 serket-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:38:26.875925 serket-0.1.0/finitediffx/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-27 06:38:06.000000 serket-0.1.0/finitediffx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:38:26.879925 serket-0.1.0/finitediffx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-27 06:38:06.000000 serket-0.1.0/finitediffx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18661 2023-07-27 06:38:06.000000 serket-0.1.0/finitediffx/_src/fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    24729 2023-07-27 06:38:06.000000 serket-0.1.0/finitediffx/_src/finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-27 06:38:06.000000 serket-0.1.0/finitediffx/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 06:38:06.000000 serket-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:38:26.879925 serket-0.1.0/serket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 06:38:26.000000 serket-0.1.0/serket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 06:38:26.000000 serket-0.1.0/serket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 06:38:26.000000 serket-0.1.0/serket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 06:38:26.000000 serket-0.1.0/serket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 06:38:26.000000 serket-0.1.0/serket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 06:38:26.879925 serket-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 06:38:26.879925 serket-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-27 06:38:06.000000 serket-0.1.0/tests/test_fgrad.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-07-27 06:38:06.000000 serket-0.1.0/tests/test_finite_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:56.003651 serket-0.2.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-20 00:19:45.000000 serket-0.2.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-20 00:19:56.003651 serket-0.2.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-04-20 00:19:45.000000 serket-0.2.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/lazy_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/experimental/test_lazy_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.999651 serket-0.2.0b2/serket/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13148 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/activation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.999651 serket-0.2.0b2/serket/nn/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12172 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blocks/vgg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47883 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40972 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/fft_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/fully_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/random_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37417 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/recurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/nn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-20 00:19:45.000000 serket-0.2.0b2/serket/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:55.995651 serket-0.2.0b2/serket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36824 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 00:19:55.000000 serket-0.2.0b2/serket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:19:56.003651 serket-0.2.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-20 00:19:45.000000 serket-0.2.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:56.003651 serket-0.2.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33451 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_fft_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_fully_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_laplace2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30469 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_random_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-20 00:19:45.000000 serket-0.2.0b2/tests/test_utils.py
```

### Comparing `serket-0.1.0/LICENSE` & `serket-0.2.0b2/LICENSE`

 * *Files identical despite different names*

