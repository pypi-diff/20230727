# Comparing `tmp/bayesian-torch-0.3.0.tar.gz` & `tmp/bayesian-torch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bayesian-torch-0.3.0.tar", last modified: Tue Dec 13 22:11:47 2022, max compression
+gzip compressed data, was "/srv/data2/bayesian-torch/dist/.tmp-uobq9167/bayesian-torch-0.4.0.tar", last modified: Thu Jul 27 07:31:10 2023, max compression
```

## Comparing `bayesian-torch-0.3.0.tar` & `bayesian-torch-0.4.0.tar`

### file list

```diff
@@ -1,86 +1,114 @@
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1891 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/.gitignore
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1518 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/LICENSE
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11446 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/PKG-INFO
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    10594 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/README.md
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/assets/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    31054 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/assets/bayesian-torch.png
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/__init__.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/examples/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    19395 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_cifar.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    17165 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_cifar_dnn2bnn.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    17576 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_flipout_cifar.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    26797 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_flipout_imagenet.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    26630 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_imagenet.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     8831 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_mnist.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    15198 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_cifar.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    20770 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_imagenet.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7802 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_mnist.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/layers/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      170 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2914 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/base_variational_layer.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7672 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/batchnorm.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      703 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/dropout.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       85 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    45002 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/conv_flipout.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7601 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/linear_flipout.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6456 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/rnn_flipout.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      508 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/relu.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       97 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    42425 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/conv_variational.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7859 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/linear_variational.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6241 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/rnn_variational.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/models/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/__init__.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     5618 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_flipout.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    10349 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_flipout_large.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6184 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_variational.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9864 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_variational_large.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2246 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/bayesian/simple_cnn_variational.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/models/deterministic/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/deterministic/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     4587 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/deterministic/resnet.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7104 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/deterministic/resnet_large.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      836 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/deterministic/simple_cnn.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6350 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/dnn_to_bnn.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/models/flipout/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/flipout/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/flipout/resnet.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2267 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/models/flipout/simple_cnn.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      202 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_bayesian_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      209 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_bayesian_flipout_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      238 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_bayesian_flipout_imagenet.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      230 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_bayesian_imagenet.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      244 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_bayesian_mnist.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      153 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_deterministic_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      181 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_deterministic_imagenet.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      243 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/test_deterministic_mnist.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      166 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_bayesian_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      174 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_bayesian_flipout_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      245 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_bayesian_flipout_imagenet.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      237 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_bayesian_imagenet.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      217 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_bayesian_mnist.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      153 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_deterministic_cifar.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      227 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_deterministic_mnist.sh
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      195 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/scripts/train_flipout_mnist.sh
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch/utils/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/utils/__init__.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    18234 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/utils/avuc_loss.py
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6111 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/bayesian_torch/utils/util.py
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11446 2022-12-13 22:11:46.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/PKG-INFO
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     3041 2022-12-13 22:11:46.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        1 2022-12-13 22:11:46.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       73 2022-12-13 22:11:46.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/requires.txt
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       15 2022-12-13 22:11:46.000000 bayesian-torch-0.3.0/bayesian_torch.egg-info/top_level.txt
-drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/doc/
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    59529 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/doc/bayesian_torch.layers.md
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       73 2022-12-13 22:07:06.000000 bayesian-torch-0.3.0/requirements.txt
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       38 2022-12-13 22:11:47.000000 bayesian-torch-0.3.0/setup.cfg
--rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1427 2022-12-13 22:10:11.000000 bayesian-torch-0.3.0/setup.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1891 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/.gitignore
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1518 2023-07-27 07:13:40.000000 bayesian-torch-0.4.0/LICENSE
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11947 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/PKG-INFO
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11132 2023-07-27 07:15:29.000000 bayesian-torch-0.4.0/README.md
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/assets/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    31054 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/assets/bayesian-torch.png
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       55 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/__init__.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/ao/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/ao/__init__.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/__init__.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/__init__.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/modules/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    58114 2023-07-27 07:09:26.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/modules/quantize_conv_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     8011 2023-07-27 07:09:14.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/modules/quantize_linear_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    52514 2023-07-27 07:09:00.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/modules/quantized_conv_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     8183 2023-07-27 07:09:46.000000 bayesian-torch-0.4.0/bayesian_torch/ao/nn/quantized/modules/quantized_linear_flipout.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/ao/quantization/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      101 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/ao/quantization/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     5149 2023-07-27 07:08:47.000000 bayesian-torch-0.4.0/bayesian_torch/ao/quantization/quantize.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/examples/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    19395 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_cifar.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    20472 2023-07-27 06:16:10.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_cifar_dnn2bnn.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    17576 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_flipout_cifar.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    26797 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_flipout_imagenet.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    26630 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_imagenet.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    10900 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_imagenet_bnn2qbnn.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    18383 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_imagenet_dnn2bnn.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     8831 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_mnist.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    15198 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_cifar.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    20770 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_imagenet.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7802 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_mnist.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      924 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/examples/quantization_test.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/layers/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      170 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2914 2023-07-27 07:06:44.000000 bayesian-torch-0.4.0/bayesian_torch/layers/base_variational_layer.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     8036 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/batchnorm.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      703 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/dropout.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      200 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    48151 2023-07-27 07:06:16.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/conv_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9493 2023-07-27 07:05:46.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/linear_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    56072 2023-07-27 07:05:34.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/quantized_conv_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11826 2023-07-27 07:06:28.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/quantized_linear_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6456 2023-07-27 07:06:03.000000 bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/rnn_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      508 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/relu.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      222 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    43902 2023-07-27 07:07:55.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/conv_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9335 2023-07-27 07:07:03.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/linear_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    63003 2023-07-27 07:08:09.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/quantize_conv_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9644 2023-07-27 07:07:36.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/quantize_linear_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6241 2023-07-27 07:07:21.000000 bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/rnn_variational.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/models/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/__init__.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9072 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/quantized_resnet_flipout_large.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9193 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/quantized_resnet_variational_large.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     5618 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_flipout.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    10349 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_flipout_large.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6184 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     9892 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_variational_large.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2246 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/bayesian/simple_cnn_variational.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    10823 2023-07-27 07:10:01.000000 bayesian-torch-0.4.0/bayesian_torch/models/bnn_to_qbnn.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/models/deterministic/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/deterministic/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     4978 2023-07-27 05:56:15.000000 bayesian-torch-0.4.0/bayesian_torch/models/deterministic/resnet.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     7104 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/deterministic/resnet_large.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      836 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/deterministic/simple_cnn.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6350 2023-07-27 07:10:13.000000 bayesian-torch-0.4.0/bayesian_torch/models/dnn_to_bnn.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/models/flipout/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/flipout/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/flipout/resnet.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     2267 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/models/flipout/simple_cnn.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/quantization/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       60 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/quantization/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      119 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/quantization/quantize.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      311 2023-07-27 06:40:04.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/quantize_bayesian_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      202 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_bayesian_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      209 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_bayesian_flipout_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      238 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_bayesian_flipout_imagenet.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      230 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_bayesian_imagenet.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      244 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_bayesian_mnist.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      153 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_deterministic_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      181 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_deterministic_imagenet.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      243 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/test_deterministic_mnist.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      166 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_bayesian_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      174 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_bayesian_flipout_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      245 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_bayesian_flipout_imagenet.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      237 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_bayesian_imagenet.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      217 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_bayesian_mnist.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      153 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_deterministic_cifar.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      227 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_deterministic_mnist.sh
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)      195 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/scripts/train_flipout_mnist.sh
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch/utils/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/bayesian_torch/utils/__init__.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    18234 2023-07-27 07:05:10.000000 bayesian-torch-0.4.0/bayesian_torch/utils/avuc_loss.py
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     6111 2023-07-27 07:05:22.000000 bayesian-torch-0.4.0/bayesian_torch/utils/util.py
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    11947 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     4236 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)        1 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       73 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/requires.txt
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       15 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/bayesian_torch.egg-info/top_level.txt
+drwxrwxr-x   0 ranganath  (1001) ranganath  (1001)        0 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/doc/
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)    59529 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/doc/bayesian_torch.layers.md
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       73 2023-07-27 05:39:27.000000 bayesian-torch-0.4.0/requirements.txt
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)       38 2023-07-27 07:31:10.000000 bayesian-torch-0.4.0/setup.cfg
+-rw-rw-r--   0 ranganath  (1001) ranganath  (1001)     1427 2023-07-27 07:16:35.000000 bayesian-torch-0.4.0/setup.py
```

### Comparing `bayesian-torch-0.3.0/.gitignore` & `bayesian-torch-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/LICENSE` & `bayesian-torch-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Intel Labs
+Copyright (c) 2023, Intel Labs
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/PKG-INFO` & `bayesian-torch-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bayesian-torch
-Version: 0.3.0
+Version: 0.4.0
 Summary: A library for Bayesian neural network layers and uncertainty estimation in Deep Learning
 Home-page: https://github.com/IntelLabs/bayesian-torch
 Author: Intel Labs
 Author-email: ranganath.krishnan@intel.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -24,17 +22,17 @@
 <img src="https://raw.githubusercontent.com/IntelLabs/bayesian-torch/5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png" width="500px">
 <h2 >
 A library for Bayesian neural network layers and uncertainty estimation in Deep Learning </a>
 </h2>
 
 [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://github.com/IntelLabs/bayesian-torch)
 [![pytorch](https://img.shields.io/badge/pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch)
-[![version](https://img.shields.io/badge/release-0.2.1-green)](https://github.com/IntelLabs/bayesian-torch/releases)
+[![version](https://img.shields.io/badge/release-0.4.0-green)](https://github.com/IntelLabs/bayesian-torch/releases)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/IntelLabs/bayesian-torch/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/bayesian-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)](https://pepy.tech/project/bayesian-torch)
+[![Downloads](https://static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-torch)
 <h4 align="center">
   <a href="https://github.com/IntelLabs/bayesian-torch#installing-bayesian-torch">Get Started</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#usage">Example usage</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch/blob/main/doc/bayesian_torch.layers.md">Documentation</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#citing">Citing</a>   
 </h4>
 
@@ -61,16 +59,17 @@
       LinearFlipout 
       Conv1dFlipout, Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout, ConvTranspose3dFlipout
       LSTMFlipout
 
 
 
 **Key features:**
-* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
+* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
 * [MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72): Specifying weight priors and variational posteriors in Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/AAAI/article/view/5875)]
+* [Quantization](https://github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of Bayesian deep neural network models with simple API's [enable_prepare()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L160)
 * [AvUC](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)]
 
 ## Installing Bayesian-Torch
 
 **To install core library using `pip`:**
 ```
 pip install bayesian-torch
@@ -215,14 +214,21 @@
 To evaluate deterministic ResNet on CIFAR10, run this command:
 
 **Vanilla**
 ```test
 sh scripts/test_deterministic_cifar.sh
 ```
 
+### Post Training Quantization (PTQ)
+
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this command:
+```test
+sh scripts/quantize_bayesian_cifar.sh
+```
+
 ## Citing
 
 If you use this code, please cite as:
 ```sh
 @software{krishnan2022bayesiantorch,
   author       = {Ranganath Krishnan and Pi Esposito and Mahesh Subedar},               
   title        = {Bayesian-Torch: Bayesian neural network layers for uncertainty estimation},
@@ -258,9 +264,7 @@
   year={2020},
   url = {https://ojs.aaai.org/index.php/AAAI/article/view/5875}
 }
 ```
 
 This library and code is intended for researchers and developers, enables to quantify principled uncertainty estimates from deep learning model predictions using stochastic variational inference in Bayesian neural networks. 
 Feedbacks, issues and contributions are welcome. Email to <ranganath.krishnan@intel.com> for any questions.
-
-
```

#### html2text {}

```diff
@@ -1,32 +1,31 @@
-Metadata-Version: 2.1 Name: bayesian-torch Version: 0.3.0 Summary: A library
+Metadata-Version: 2.1 Name: bayesian-torch Version: 0.4.0 Summary: A library
 for Bayesian neural network layers and uncertainty estimation in Deep Learning
 Home-page: https://github.com/IntelLabs/bayesian-torch Author: Intel Labs
-Author-email: ranganath.krishnan@intel.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
+Author-email: ranganath.krishnan@intel.com Classifier: Development Status :: 3
+- Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE
          [https://raw.githubusercontent.com/IntelLabs/bayesian-torch/
       5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png]
  ***** A library for Bayesian neural network layers and uncertainty estimation
                             in Deep Learning *****
      [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://
 github.com/IntelLabs/bayesian-torch) [![pytorch](https://img.shields.io/badge/
    pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch) [!
-     [version](https://img.shields.io/badge/release-0.2.1-green)](https://
+     [version](https://img.shields.io/badge/release-0.4.0-green)](https://
       github.com/IntelLabs/bayesian-torch/releases) [![license](https://
     img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/
       IntelLabs/bayesian-torch/blob/main/LICENSE) [![Downloads](https://
-                 static.pepy.tech/personalized-badge/bayesian-
-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)]
-                  (https://pepy.tech/project/bayesian-torch)
+  static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-
+                                    torch)
          *** Get_Started | Example_usage | Documentation | Citing ***
 ___ Bayesian-Torch is a library of neural network layers and utilities
 extending the core of PyTorch to enable Bayesian inference in deep learning
 models to quantify principled uncertainty estimates in model predictions. ##
 Overview Bayesian-Torch is designed to be flexible and enables seamless
 extension of deterministic deep neural network model to corresponding Bayesian
 form by simply replacing the deterministic layers with Bayesian layers. It
@@ -40,45 +39,51 @@
 ConvTranspose3dReparameterization LSTMReparameterization * **[Variational
 layers with Flipout Monte Carlo estimators](https://github.com/IntelLabs/
 bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)** [[Wen et al.
 2018](https://arxiv.org/abs/1803.04386)] LinearFlipout Conv1dFlipout,
 Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout,
 ConvTranspose3dFlipout LSTMFlipout **Key features:** * [dnn_to_bnn()](https://
 github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/
-dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn)
-model of any architecture to Bayesian deep neural network (bnn) model,
-simplifying the model definition i.e. drop-in replacements of Convolutional,
-Linear and LSTM layers to corresponding Bayesian layers. This will enable
-seamless conversion of existing topology of larger models to Bayesian deep
-neural network models for extending towards uncertainty-aware applications. *
-[MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/
-utils/util.py#L72): Specifying weight priors and variational posteriors in
-Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://
-ojs.aaai.org/index.php/AAAI/article/view/5875)] * [AvUC](https://github.com/
-IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy
-versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://
-proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
-Paper.pdf)] ## Installing Bayesian-Torch **To install core library using `pip`:
-** ``` pip install bayesian-torch ``` **To install latest development version
-from source:** ```sh git clone https://github.com/IntelLabs/bayesian-torch cd
-bayesian-torch pip install . ```  ## Usage There are two ways to build Bayesian
-deep neural networks using Bayesian-Torch: 1. Convert an existing deterministic
-deep neural network (dnn) model to Bayesian deep neural network (bnn) model
-with dnn_to_bnn() API 2. Define your custom model using the Bayesian layers (
-[Reparameterization](https://github.com/IntelLabs/bayesian-torch/tree/main/
-bayesian_torch/layers/variational_layers) or [Flipout](https://github.com/
-IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)) (1)
-For instance, building Bayesian-ResNet18 from torchvision deterministic
-ResNet18 model is as simple as: ``` import torch import torchvision from
-bayesian_torch.models.dnn_to_bnn import dnn_to_bnn, get_kl_loss
-const_bnn_prior_parameters = { "prior_mu": 0.0, "prior_sigma": 1.0,
-"posterior_mu_init": 0.0, "posterior_rho_init": -3.0, "type":
-"Reparameterization", # Flipout or Reparameterization "moped_enable": False, #
-True to initialize mu/sigma from the pretrained dnn weights "moped_delta": 0.5,
-} model = torchvision.models.resnet18() dnn_to_bnn(model,
+dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An
+API to convert deterministic deep neural network (dnn) model of any
+architecture to Bayesian deep neural network (bnn) model, simplifying the model
+definition i.e. drop-in replacements of Convolutional, Linear and LSTM layers
+to corresponding Bayesian layers. This will enable seamless conversion of
+existing topology of larger models to Bayesian deep neural network models for
+extending towards uncertainty-aware applications. * [MOPED](https://github.com/
+IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72):
+Specifying weight priors and variational posteriors in Bayesian neural networks
+with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/
+AAAI/article/view/5875)] * [Quantization](https://github.com/IntelLabs/
+bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of
+Bayesian deep neural network models with simple API's [enable_prepare()](https:
+//github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/
+quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/
+blob/main/bayesian_torch/ao/quantization/quantize.py#L160) * [AvUC](https://
+github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/
+avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and
+Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/
+d3d9446802a44259755d38e6d163e820-Paper.pdf)] ## Installing Bayesian-Torch **To
+install core library using `pip`:** ``` pip install bayesian-torch ``` **To
+install latest development version from source:** ```sh git clone https://
+github.com/IntelLabs/bayesian-torch cd bayesian-torch pip install . ```  ##
+Usage There are two ways to build Bayesian deep neural networks using Bayesian-
+Torch: 1. Convert an existing deterministic deep neural network (dnn) model to
+Bayesian deep neural network (bnn) model with dnn_to_bnn() API 2. Define your
+custom model using the Bayesian layers ([Reparameterization](https://
+github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/
+variational_layers) or [Flipout](https://github.com/IntelLabs/bayesian-torch/
+tree/main/bayesian_torch/layers/flipout_layers)) (1) For instance, building
+Bayesian-ResNet18 from torchvision deterministic ResNet18 model is as simple
+as: ``` import torch import torchvision from bayesian_torch.models.dnn_to_bnn
+import dnn_to_bnn, get_kl_loss const_bnn_prior_parameters = { "prior_mu": 0.0,
+"prior_sigma": 1.0, "posterior_mu_init": 0.0, "posterior_rho_init": -3.0,
+"type": "Reparameterization", # Flipout or Reparameterization "moped_enable":
+False, # True to initialize mu/sigma from the pretrained dnn weights
+"moped_delta": 0.5, } model = torchvision.models.resnet18() dnn_to_bnn(model,
 const_bnn_prior_parameters) ``` To use MOPED method i.e. setting the prior and
 initializing variational parameters from a pretrained deterministic model
 (helps training convergence of larger models): ``` const_bnn_prior_parameters =
 { "prior_mu": 0.0, "prior_sigma": 1.0, "posterior_mu_init": 0.0,
 "posterior_rho_init": -3.0, "type": "Reparameterization", # Flipout or
 Reparameterization "moped_enable": True, # True to initialize mu/sigma from the
 pretrained dnn weights "moped_delta": 0.5, } model =
@@ -111,25 +116,27 @@
 train deterministic ResNet on CIFAR10, run this command: **Vanilla** ```train
 sh scripts/train_deterministic_cifar.sh ``` ### Evaluation To evaluate Bayesian
 ResNet on CIFAR10, run this command: **Mean-field variational inference
 (Reparameterized Monte Carlo estimator)** ```test sh scripts/
 test_bayesian_cifar.sh ``` **Mean-field variational inference (Flipout Monte
 Carlo estimator)** ```test sh scripts/test_bayesian_flipout_cifar.sh ``` To
 evaluate deterministic ResNet on CIFAR10, run this command: **Vanilla** ```test
-sh scripts/test_deterministic_cifar.sh ``` ## Citing If you use this code,
-please cite as: ```sh @software{krishnan2022bayesiantorch, author = {Ranganath
-Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-Torch: Bayesian
-neural network layers for uncertainty estimation}, month = jan, year = 2022,
-doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/zenodo.5908307}
-howpublished = {\url{https://github.com/IntelLabs/bayesian-torch}} } ```
-Accuracy versus Uncertainty Calibration (AvUC) loss ```sh @inproceedings
-{NEURIPS2020_d3d94468, title = {Improving model calibration with accuracy
-versus uncertainty optimization}, author = {Krishnan, Ranganath and Tickoo,
-Omesh}, booktitle = {Advances in Neural Information Processing Systems}, volume
-= {33}, pages = {18237--18248}, year = {2020}, url = {https://
+sh scripts/test_deterministic_cifar.sh ``` ### Post Training Quantization (PTQ)
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this
+command: ```test sh scripts/quantize_bayesian_cifar.sh ``` ## Citing If you use
+this code, please cite as: ```sh @software{krishnan2022bayesiantorch, author =
+{Ranganath Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-
+Torch: Bayesian neural network layers for uncertainty estimation}, month = jan,
+year = 2022, doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/
+zenodo.5908307} howpublished = {\url{https://github.com/IntelLabs/bayesian-
+torch}} } ``` Accuracy versus Uncertainty Calibration (AvUC) loss ```sh
+@inproceedings{NEURIPS2020_d3d94468, title = {Improving model calibration with
+accuracy versus uncertainty optimization}, author = {Krishnan, Ranganath and
+Tickoo, Omesh}, booktitle = {Advances in Neural Information Processing
+Systems}, volume = {33}, pages = {18237--18248}, year = {2020}, url = {https://
 proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
 Paper.pdf} } ``` MOdel Priors with Empirical Bayes using DNN (MOPED) ```sh
 @inproceedings{krishnan2020specifying, title={Specifying weight priors in
 bayesian deep neural networks with empirical bayes}, author={Krishnan,
 Ranganath and Subedar, Mahesh and Tickoo, Omesh}, booktitle={Proceedings of the
 AAAI Conference on Artificial Intelligence}, volume={34}, number={04}, pages=
 {4477--4484}, year={2020}, url = {https://ojs.aaai.org/index.php/AAAI/article/
```

### Comparing `bayesian-torch-0.3.0/README.md` & `bayesian-torch-0.4.0/bayesian_torch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,38 @@
+Metadata-Version: 2.1
+Name: bayesian-torch
+Version: 0.4.0
+Summary: A library for Bayesian neural network layers and uncertainty estimation in Deep Learning
+Home-page: https://github.com/IntelLabs/bayesian-torch
+Author: Intel Labs
+Author-email: ranganath.krishnan@intel.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/IntelLabs/bayesian-torch/5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png" width="500px">
 <h2 >
 A library for Bayesian neural network layers and uncertainty estimation in Deep Learning </a>
 </h2>
 
 [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://github.com/IntelLabs/bayesian-torch)
 [![pytorch](https://img.shields.io/badge/pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch)
-[![version](https://img.shields.io/badge/release-0.2.1-green)](https://github.com/IntelLabs/bayesian-torch/releases)
+[![version](https://img.shields.io/badge/release-0.4.0-green)](https://github.com/IntelLabs/bayesian-torch/releases)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/IntelLabs/bayesian-torch/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/bayesian-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)](https://pepy.tech/project/bayesian-torch)
+[![Downloads](https://static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-torch)
 <h4 align="center">
   <a href="https://github.com/IntelLabs/bayesian-torch#installing-bayesian-torch">Get Started</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#usage">Example usage</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch/blob/main/doc/bayesian_torch.layers.md">Documentation</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#citing">Citing</a>   
 </h4>
 
@@ -40,16 +59,17 @@
       LinearFlipout 
       Conv1dFlipout, Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout, ConvTranspose3dFlipout
       LSTMFlipout
 
 
 
 **Key features:**
-* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
+* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
 * [MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72): Specifying weight priors and variational posteriors in Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/AAAI/article/view/5875)]
+* [Quantization](https://github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of Bayesian deep neural network models with simple API's [enable_prepare()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L160)
 * [AvUC](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)]
 
 ## Installing Bayesian-Torch
 
 **To install core library using `pip`:**
 ```
 pip install bayesian-torch
@@ -194,14 +214,21 @@
 To evaluate deterministic ResNet on CIFAR10, run this command:
 
 **Vanilla**
 ```test
 sh scripts/test_deterministic_cifar.sh
 ```
 
+### Post Training Quantization (PTQ)
+
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this command:
+```test
+sh scripts/quantize_bayesian_cifar.sh
+```
+
 ## Citing
 
 If you use this code, please cite as:
 ```sh
 @software{krishnan2022bayesiantorch,
   author       = {Ranganath Krishnan and Pi Esposito and Mahesh Subedar},               
   title        = {Bayesian-Torch: Bayesian neural network layers for uncertainty estimation},
```

#### html2text {}

```diff
@@ -1,21 +1,31 @@
+Metadata-Version: 2.1 Name: bayesian-torch Version: 0.4.0 Summary: A library
+for Bayesian neural network layers and uncertainty estimation in Deep Learning
+Home-page: https://github.com/IntelLabs/bayesian-torch Author: Intel Labs
+Author-email: ranganath.krishnan@intel.com Classifier: Development Status :: 3
+- Alpha Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE
          [https://raw.githubusercontent.com/IntelLabs/bayesian-torch/
       5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png]
  ***** A library for Bayesian neural network layers and uncertainty estimation
                             in Deep Learning *****
      [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://
 github.com/IntelLabs/bayesian-torch) [![pytorch](https://img.shields.io/badge/
    pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch) [!
-     [version](https://img.shields.io/badge/release-0.2.1-green)](https://
+     [version](https://img.shields.io/badge/release-0.4.0-green)](https://
       github.com/IntelLabs/bayesian-torch/releases) [![license](https://
     img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/
       IntelLabs/bayesian-torch/blob/main/LICENSE) [![Downloads](https://
-                 static.pepy.tech/personalized-badge/bayesian-
-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)]
-                  (https://pepy.tech/project/bayesian-torch)
+  static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-
+                                    torch)
          *** Get_Started | Example_usage | Documentation | Citing ***
 ___ Bayesian-Torch is a library of neural network layers and utilities
 extending the core of PyTorch to enable Bayesian inference in deep learning
 models to quantify principled uncertainty estimates in model predictions. ##
 Overview Bayesian-Torch is designed to be flexible and enables seamless
 extension of deterministic deep neural network model to corresponding Bayesian
 form by simply replacing the deterministic layers with Bayesian layers. It
@@ -29,45 +39,51 @@
 ConvTranspose3dReparameterization LSTMReparameterization * **[Variational
 layers with Flipout Monte Carlo estimators](https://github.com/IntelLabs/
 bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)** [[Wen et al.
 2018](https://arxiv.org/abs/1803.04386)] LinearFlipout Conv1dFlipout,
 Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout,
 ConvTranspose3dFlipout LSTMFlipout **Key features:** * [dnn_to_bnn()](https://
 github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/
-dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn)
-model of any architecture to Bayesian deep neural network (bnn) model,
-simplifying the model definition i.e. drop-in replacements of Convolutional,
-Linear and LSTM layers to corresponding Bayesian layers. This will enable
-seamless conversion of existing topology of larger models to Bayesian deep
-neural network models for extending towards uncertainty-aware applications. *
-[MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/
-utils/util.py#L72): Specifying weight priors and variational posteriors in
-Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://
-ojs.aaai.org/index.php/AAAI/article/view/5875)] * [AvUC](https://github.com/
-IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy
-versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://
-proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
-Paper.pdf)] ## Installing Bayesian-Torch **To install core library using `pip`:
-** ``` pip install bayesian-torch ``` **To install latest development version
-from source:** ```sh git clone https://github.com/IntelLabs/bayesian-torch cd
-bayesian-torch pip install . ```  ## Usage There are two ways to build Bayesian
-deep neural networks using Bayesian-Torch: 1. Convert an existing deterministic
-deep neural network (dnn) model to Bayesian deep neural network (bnn) model
-with dnn_to_bnn() API 2. Define your custom model using the Bayesian layers (
-[Reparameterization](https://github.com/IntelLabs/bayesian-torch/tree/main/
-bayesian_torch/layers/variational_layers) or [Flipout](https://github.com/
-IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)) (1)
-For instance, building Bayesian-ResNet18 from torchvision deterministic
-ResNet18 model is as simple as: ``` import torch import torchvision from
-bayesian_torch.models.dnn_to_bnn import dnn_to_bnn, get_kl_loss
-const_bnn_prior_parameters = { "prior_mu": 0.0, "prior_sigma": 1.0,
-"posterior_mu_init": 0.0, "posterior_rho_init": -3.0, "type":
-"Reparameterization", # Flipout or Reparameterization "moped_enable": False, #
-True to initialize mu/sigma from the pretrained dnn weights "moped_delta": 0.5,
-} model = torchvision.models.resnet18() dnn_to_bnn(model,
+dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An
+API to convert deterministic deep neural network (dnn) model of any
+architecture to Bayesian deep neural network (bnn) model, simplifying the model
+definition i.e. drop-in replacements of Convolutional, Linear and LSTM layers
+to corresponding Bayesian layers. This will enable seamless conversion of
+existing topology of larger models to Bayesian deep neural network models for
+extending towards uncertainty-aware applications. * [MOPED](https://github.com/
+IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72):
+Specifying weight priors and variational posteriors in Bayesian neural networks
+with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/
+AAAI/article/view/5875)] * [Quantization](https://github.com/IntelLabs/
+bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of
+Bayesian deep neural network models with simple API's [enable_prepare()](https:
+//github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/
+quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/
+blob/main/bayesian_torch/ao/quantization/quantize.py#L160) * [AvUC](https://
+github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/
+avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and
+Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/
+d3d9446802a44259755d38e6d163e820-Paper.pdf)] ## Installing Bayesian-Torch **To
+install core library using `pip`:** ``` pip install bayesian-torch ``` **To
+install latest development version from source:** ```sh git clone https://
+github.com/IntelLabs/bayesian-torch cd bayesian-torch pip install . ```  ##
+Usage There are two ways to build Bayesian deep neural networks using Bayesian-
+Torch: 1. Convert an existing deterministic deep neural network (dnn) model to
+Bayesian deep neural network (bnn) model with dnn_to_bnn() API 2. Define your
+custom model using the Bayesian layers ([Reparameterization](https://
+github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/
+variational_layers) or [Flipout](https://github.com/IntelLabs/bayesian-torch/
+tree/main/bayesian_torch/layers/flipout_layers)) (1) For instance, building
+Bayesian-ResNet18 from torchvision deterministic ResNet18 model is as simple
+as: ``` import torch import torchvision from bayesian_torch.models.dnn_to_bnn
+import dnn_to_bnn, get_kl_loss const_bnn_prior_parameters = { "prior_mu": 0.0,
+"prior_sigma": 1.0, "posterior_mu_init": 0.0, "posterior_rho_init": -3.0,
+"type": "Reparameterization", # Flipout or Reparameterization "moped_enable":
+False, # True to initialize mu/sigma from the pretrained dnn weights
+"moped_delta": 0.5, } model = torchvision.models.resnet18() dnn_to_bnn(model,
 const_bnn_prior_parameters) ``` To use MOPED method i.e. setting the prior and
 initializing variational parameters from a pretrained deterministic model
 (helps training convergence of larger models): ``` const_bnn_prior_parameters =
 { "prior_mu": 0.0, "prior_sigma": 1.0, "posterior_mu_init": 0.0,
 "posterior_rho_init": -3.0, "type": "Reparameterization", # Flipout or
 Reparameterization "moped_enable": True, # True to initialize mu/sigma from the
 pretrained dnn weights "moped_delta": 0.5, } model =
@@ -100,25 +116,27 @@
 train deterministic ResNet on CIFAR10, run this command: **Vanilla** ```train
 sh scripts/train_deterministic_cifar.sh ``` ### Evaluation To evaluate Bayesian
 ResNet on CIFAR10, run this command: **Mean-field variational inference
 (Reparameterized Monte Carlo estimator)** ```test sh scripts/
 test_bayesian_cifar.sh ``` **Mean-field variational inference (Flipout Monte
 Carlo estimator)** ```test sh scripts/test_bayesian_flipout_cifar.sh ``` To
 evaluate deterministic ResNet on CIFAR10, run this command: **Vanilla** ```test
-sh scripts/test_deterministic_cifar.sh ``` ## Citing If you use this code,
-please cite as: ```sh @software{krishnan2022bayesiantorch, author = {Ranganath
-Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-Torch: Bayesian
-neural network layers for uncertainty estimation}, month = jan, year = 2022,
-doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/zenodo.5908307}
-howpublished = {\url{https://github.com/IntelLabs/bayesian-torch}} } ```
-Accuracy versus Uncertainty Calibration (AvUC) loss ```sh @inproceedings
-{NEURIPS2020_d3d94468, title = {Improving model calibration with accuracy
-versus uncertainty optimization}, author = {Krishnan, Ranganath and Tickoo,
-Omesh}, booktitle = {Advances in Neural Information Processing Systems}, volume
-= {33}, pages = {18237--18248}, year = {2020}, url = {https://
+sh scripts/test_deterministic_cifar.sh ``` ### Post Training Quantization (PTQ)
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this
+command: ```test sh scripts/quantize_bayesian_cifar.sh ``` ## Citing If you use
+this code, please cite as: ```sh @software{krishnan2022bayesiantorch, author =
+{Ranganath Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-
+Torch: Bayesian neural network layers for uncertainty estimation}, month = jan,
+year = 2022, doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/
+zenodo.5908307} howpublished = {\url{https://github.com/IntelLabs/bayesian-
+torch}} } ``` Accuracy versus Uncertainty Calibration (AvUC) loss ```sh
+@inproceedings{NEURIPS2020_d3d94468, title = {Improving model calibration with
+accuracy versus uncertainty optimization}, author = {Krishnan, Ranganath and
+Tickoo, Omesh}, booktitle = {Advances in Neural Information Processing
+Systems}, volume = {33}, pages = {18237--18248}, year = {2020}, url = {https://
 proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
 Paper.pdf} } ``` MOdel Priors with Empirical Bayes using DNN (MOPED) ```sh
 @inproceedings{krishnan2020specifying, title={Specifying weight priors in
 bayesian deep neural networks with empirical bayes}, author={Krishnan,
 Ranganath and Subedar, Mahesh and Tickoo, Omesh}, booktitle={Proceedings of the
 AAAI Conference on Artificial Intelligence}, volume={34}, number={04}, pages=
 {4477--4484}, year={2020}, url = {https://ojs.aaai.org/index.php/AAAI/article/
```

### Comparing `bayesian-torch-0.3.0/assets/bayesian-torch.png` & `bayesian-torch-0.4.0/assets/bayesian-torch.png`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_cifar.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_cifar.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_cifar_dnn2bnn.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_imagenet_dnn2bnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,43 +9,50 @@
 import torch.backends.cudnn as cudnn
 import torch.optim
 import torch.utils.data
 from torch.utils.tensorboard import SummaryWriter
 import torchvision.transforms as transforms
 import torchvision.datasets as datasets
 
-import bayesian_torch.models.deterministic.resnet as resnet
+import bayesian_torch.models.deterministic.resnet_large as resnet
 import numpy as np
 from bayesian_torch.models.dnn_to_bnn import dnn_to_bnn, get_kl_loss
 
 model_names = sorted(
     name
     for name in resnet.__dict__
     if name.islower() and not name.startswith("__") and name.startswith("resnet") and callable(resnet.__dict__[name])
 )
 
 print(model_names)
-len_trainset = 50000
-len_testset = 10000
+best_acc1 = 0
+len_trainset = 1281167
+len_valset = 50000
 
-parser = argparse.ArgumentParser(description="CIFAR10")
+
+parser = argparse.ArgumentParser(description="ImageNet")
+parser.add_argument('data',
+                    metavar='DIR',
+                    default='data/imagenet',
+                    help='path to dataset')
 parser.add_argument(
     "--arch",
     "-a",
     metavar="ARCH",
-    default="resnet20",
+    default="resnet50",
     choices=model_names,
-    help="model architecture: " + " | ".join(model_names) + " (default: resnet20)",
+    help="model architecture: " + " | ".join(model_names) + " (default: resnet50)",
 )
 parser.add_argument(
     "-j", "--workers", default=8, type=int, metavar="N", help="number of data loading workers (default: 8)"
 )
-parser.add_argument("--epochs", default=200, type=int, metavar="N", help="number of total epochs to run")
+parser.add_argument("--epochs", default=90, type=int, metavar="N", help="number of total epochs to run")
 parser.add_argument("--start-epoch", default=0, type=int, metavar="N", help="manual epoch number (useful on restarts)")
-parser.add_argument("-b", "--batch-size", default=128, type=int, metavar="N", help="mini-batch size (default: 512)")
+parser.add_argument("-b", "--batch-size", default=128, type=int, metavar="N", help="mini-batch size (default: 128)")
+parser.add_argument('--val_batch_size', default=1000, type=int)
 parser.add_argument("--lr", "--learning-rate", default=0.001, type=float, metavar="LR", help="initial learning rate")
 parser.add_argument("--momentum", default=0.9, type=float, metavar="M", help="momentum")
 parser.add_argument(
     "--weight-decay", "--wd", default=1e-4, type=float, metavar="W", help="weight decay (default: 5e-4)"
 )
 parser.add_argument("--print-freq", "-p", default=50, type=int, metavar="N", help="print frequency (default: 20)")
 parser.add_argument("--resume", default="", type=str, metavar="PATH", help="path to latest checkpoint (default: none)")
@@ -66,23 +73,23 @@
     default="",
     type=str,
 )
 parser.add_argument(
     "--moped-delta-factor",
     dest="moped_delta_factor",
     help="MOPED delta scale factor",
-    default=0.2,
+    default=0.001,
     type=float,
 )
 
 parser.add_argument(
     "--bnn-rho-init",
     dest="bnn_rho_init",
     help="rho init for bnn layers",
-    default=-3.0,
+    default=-10.0,
     type=float,
 )
 
 parser.add_argument(
     "--use-flipout-layers",
     type=bool,
     default=False,
@@ -113,15 +120,15 @@
     default=True,
     metavar="N",
     help="use tensorboard for logging and visualization of training progress",
 )
 parser.add_argument(
     "--log_dir",
     type=str,
-    default="./logs/cifar/bayesian",
+    default="./logs/imagenet/bayesian",
     metavar="N",
     help="use tensorboard for logging and visualization of training progress",
 )
 
 best_prec1 = 0
 
 
@@ -142,24 +149,36 @@
         "moped_delta": args.moped_delta_factor,
     }
 
     # Check the save_dir exists or not
     if not os.path.exists(args.save_dir):
         os.makedirs(args.save_dir)
 
-    model = torch.nn.DataParallel(resnet.__dict__[args.arch]())
+    model = torch.nn.DataParallel(resnet.__dict__[args.arch](pretrained=True))
     model.cuda() if torch.cuda.is_available() else model.cpu()
     if moped_enable:
         checkpoint = torch.load(args.moped_init_model)
         if "state_dict" in checkpoint.keys():
             model.load_state_dict(checkpoint["state_dict"])
         else:
             model.load_state_dict(checkpoint)
 
+    const_bnn_prior_parameters["moped_enable"]=True
     dnn_to_bnn(model, const_bnn_prior_parameters)  # only replaces linear and conv layers
+
+    save_checkpoint(
+                    {
+                        "epoch": 0,
+                        "state_dict": model.state_dict(),
+                        "best_prec1": best_prec1,
+                    },
+                    False,
+                    filename=os.path.join(args.save_dir, "bayesian_{}_imagenet.pth".format(args.arch)),
+                )
+
     if torch.cuda.is_available():
         model.cuda()
     else:
         model.cpu()
 
     # optionally resume from a checkpoint
     if args.resume:
@@ -178,52 +197,53 @@
     tb_writer = None
     if args.tensorboard:
         logger_dir = os.path.join(args.log_dir, "tb_logger")
         if not os.path.exists(logger_dir):
             os.makedirs(logger_dir)
         tb_writer = SummaryWriter(logger_dir)
 
-    normalize = transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
+    valdir = os.path.join(args.data, 'val') #Imagenet_2012Val
+    normalize = transforms.Normalize(mean=[0.485, 0.456, 0.406],
+                                     std=[0.229, 0.224, 0.225])
+
+    # train_loader = torch.utils.data.DataLoader(
+    #     datasets.CIFAR10(
+    #         root="./data",
+    #         train=True,
+    #         transform=transforms.Compose(
+    #             [
+    #                 transforms.RandomHorizontalFlip(),
+    #                 transforms.RandomCrop(32, 4),
+    #                 transforms.ToTensor(),
+    #                 normalize,
+    #             ]
+    #         ),
+    #         download=True,
+    #     ),
+    #     batch_size=args.batch_size,
+    #     shuffle=True,
+    #     num_workers=args.workers,
+    #     pin_memory=True,
+    # )
+
+    val_dataset = datasets.ImageFolder(
+        valdir,
+        transforms.Compose([
+            transforms.Resize(256),
+            transforms.CenterCrop(224),
+            transforms.ToTensor(),
+            normalize,
+        ]))
+    val_loader = torch.utils.data.DataLoader(val_dataset,
+                                             batch_size=args.val_batch_size,
+                                             shuffle=False,
+                                             num_workers=args.workers,
+                                             pin_memory=True)
 
-    train_loader = torch.utils.data.DataLoader(
-        datasets.CIFAR10(
-            root="./data",
-            train=True,
-            transform=transforms.Compose(
-                [
-                    transforms.RandomHorizontalFlip(),
-                    transforms.RandomCrop(32, 4),
-                    transforms.ToTensor(),
-                    normalize,
-                ]
-            ),
-            download=True,
-        ),
-        batch_size=args.batch_size,
-        shuffle=True,
-        num_workers=args.workers,
-        pin_memory=True,
-    )
-
-    val_loader = torch.utils.data.DataLoader(
-        datasets.CIFAR10(
-            root="./data",
-            train=False,
-            transform=transforms.Compose(
-                [
-                    transforms.ToTensor(),
-                    normalize,
-                ]
-            ),
-        ),
-        batch_size=args.batch_size,
-        shuffle=False,
-        num_workers=args.workers,
-        pin_memory=True,
-    )
+    print('len valset: ', len(val_dataset))
 
     if not os.path.exists(args.save_dir):
         os.makedirs(args.save_dir)
 
     if torch.cuda.is_available():
         criterion = nn.CrossEntropyLoss().cuda()
     else:
@@ -238,14 +258,15 @@
             param_group["lr"] = args.lr * 0.1
 
     if args.evaluate:
         validate(val_loader, model, criterion)
         return
 
     if args.mode == "train":
+        pass
 
         for epoch in range(args.start_epoch, args.epochs):
 
             lr = args.lr
             if epoch >= 80 and epoch < 120:
                 lr = 0.1 * args.lr
             elif epoch >= 120 and epoch < 160:
@@ -270,19 +291,19 @@
                 save_checkpoint(
                     {
                         "epoch": epoch + 1,
                         "state_dict": model.state_dict(),
                         "best_prec1": best_prec1,
                     },
                     is_best,
-                    filename=os.path.join(args.save_dir, "bayesian_{}_cifar.pth".format(args.arch)),
+                    filename=os.path.join(args.save_dir, "bayesian_{}_imagenet.pth".format(args.arch)),
                 )
 
     elif args.mode == "test":
-        checkpoint_file = args.save_dir + "/bayesian_{}_cifar.pth".format(args.arch)
+        checkpoint_file = args.save_dir + "/bayesian_{}_imagenet.pth".format(args.arch)
         if torch.cuda.is_available():
             checkpoint = torch.load(checkpoint_file)
         else:
             checkpoint = torch.load(checkpoint_file, map_location=torch.device("cpu"))
         model.load_state_dict(checkpoint["state_dict"])
         evaluate(args, model, val_loader)
 
@@ -445,39 +466,47 @@
     test_loss = 0
     correct = 0
     output_list = []
     labels_list = []
     model.eval()
     with torch.no_grad():
         begin = time.time()
+        i=0
         for data, target in val_loader:
             if torch.cuda.is_available():
                 data, target = data.cuda(), target.cuda()
             else:
                 data, target = data.cpu(), target.cpu()
             output_mc = []
             for mc_run in range(args.num_monte_carlo):
                 output = model.forward(data)
                 output_mc.append(output)
             output_ = torch.stack(output_mc)
             output_list.append(output_)
             labels_list.append(target)
+            i+=1
+            # if i==10:
+            #     break
         end = time.time()
-        print("inference throughput: ", len_testset / (end - begin), " images/s")
+        print("inference throughput: ", 50000 / (end - begin), " images/s")
 
-        output = torch.stack(output_list)
-        output = output.permute(1, 0, 2, 3)
-        output = output.contiguous().view(args.num_monte_carlo, len_testset, -1)
+        # output = torch.stack(output_list)
+        # output = output.permute(1, 0, 2, 3)
+        # output = output.contiguous().view(args.num_monte_carlo, len_valset, -1)
+        output = torch.cat(output_list, 1)
         output = torch.nn.functional.softmax(output, dim=2)
         labels = torch.cat(labels_list)
         pred_mean = output.mean(dim=0)
         Y_pred = torch.argmax(pred_mean, axis=1)
-        print("Test accuracy:", (Y_pred.data.cpu().numpy() == labels.data.cpu().numpy()).mean() * 100)
+        
         np.save("./probs_cifar_mc.npy", output.data.cpu().numpy())
         np.save("./cifar_test_labels_mc.npy", labels.data.cpu().numpy())
+        print(Y_pred.shape, labels.shape)
+        print(Y_pred[:100], labels[:100])
+        print("Test accuracy:", (Y_pred.data.cpu().numpy() == labels.data.cpu().numpy()).mean() * 100)
 
 
 def save_checkpoint(state, is_best, filename="checkpoint.pth.tar"):
     """
     Save the training model
     """
     torch.save(state, filename)
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_flipout_cifar.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_flipout_cifar.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_flipout_imagenet.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_flipout_imagenet.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_imagenet.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_imagenet.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_bayesian_mnist.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_bayesian_mnist.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_cifar.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_cifar.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_imagenet.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_imagenet.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/examples/main_deterministic_mnist.py` & `bayesian-torch-0.4.0/bayesian_torch/examples/main_deterministic_mnist.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/base_variational_layer.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/base_variational_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/batchnorm.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/batchnorm.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,30 +50,37 @@
 
     def _check_input_dim(self, input):
         if input.dim() != 4:
             raise ValueError('expected 4D input (got {}D input)'.format(
                 input.dim()))
 
     def forward(self, input):
-        self._check_input_dim(input[0])
         exponential_average_factor = 0.0
         if self.training and self.track_running_stats:
             self.num_batches_tracked += 1
         if self.momentum is None:  # use cumulative moving average
             exponential_average_factor = 1.0 / self.num_batches_tracked.item()
         else:  # use exponential moving average
             exponential_average_factor = self.momentum
 
-        out = F.batch_norm(input[0], self.running_mean, self.running_var,
-                           self.weight, self.bias, self.training
-                           or not self.track_running_stats,
-                           exponential_average_factor, self.eps)
-        kl = 0
-        return out, kl
-
+        if len(input) == 2:
+            self._check_input_dim(input[0])
+            out = F.batch_norm(input[0], self.running_mean, self.running_var,
+                            self.weight, self.bias, self.training
+                            or not self.track_running_stats,
+                            exponential_average_factor, self.eps)
+            kl = 0
+            return out, kl
+        else:
+            out = F.batch_norm(input, self.running_mean, self.running_var,
+                            self.weight, self.bias, self.training
+                            or not self.track_running_stats,
+                            exponential_average_factor, self.eps)
+            return out
+            
 
 class BatchNorm1dLayer(nn.Module):
     def __init__(self,
                  num_features,
                  eps=1e-5,
                  momentum=0.1,
                  affine=True,
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/dropout.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/conv_flipout.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/conv_flipout.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -33,14 +33,17 @@
 # @authors: Ranganath Krishnan, Piero Esposito
 #
 # ======================================================================================
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base_variational_layer import BaseVariationalLayer_, get_kernel_size
+from torch.quantization.observer import HistogramObserver, PerChannelMinMaxObserver, MinMaxObserver
+from torch.quantization.qconfig import QConfig
+
 
 from torch.distributions.normal import Normal
 from torch.distributions.uniform import Uniform
 
 __all__ = [
     'Conv1dFlipout',
     'Conv2dFlipout',
@@ -132,14 +135,23 @@
             self.register_parameter('mu_bias', None)
             self.register_parameter('rho_bias', None)
             self.register_buffer('eps_bias', None, persistent=False)
             self.register_buffer('prior_bias_mu', None, persistent=False)
             self.register_buffer('prior_bias_sigma', None, persistent=False)
 
         self.init_parameters()
+        self.quant_prepare=False
+    
+    def prepare(self):
+        self.qint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.qint8, qscheme=torch.per_tensor_symmetric), activation=MinMaxObserver.with_args(dtype=torch.qint8,qscheme=torch.per_tensor_symmetric))) for _ in range(4)])
+        self.quint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.quint8), activation=MinMaxObserver.with_args(dtype=torch.quint8))) for _ in range(8)])
+        self.dequant = torch.quantization.DeQuantStub()
+        self.quant_prepare=True
 
     def init_parameters(self):
         # prior values
         self.prior_weight_mu.data.fill_(self.prior_mean)
         self.prior_weight_sigma.data.fill_(self.prior_variance)
 
         # init our weights for the deterministic and perturbated weights
@@ -299,14 +311,23 @@
             self.register_parameter('mu_bias', None)
             self.register_parameter('rho_bias', None)
             self.register_buffer('eps_bias', None, persistent=False)
             self.register_buffer('prior_bias_mu', None, persistent=False)
             self.register_buffer('prior_bias_sigma', None, persistent=False)
 
         self.init_parameters()
+        self.quant_prepare=False
+    
+    def prepare(self):
+        self.qint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.qint8, qscheme=torch.per_tensor_symmetric), activation=MinMaxObserver.with_args(dtype=torch.qint8,qscheme=torch.per_tensor_symmetric))) for _ in range(4)])
+        self.quint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.quint8), activation=MinMaxObserver.with_args(dtype=torch.quint8))) for _ in range(8)])
+        self.dequant = torch.quantization.DeQuantStub()
+        self.quant_prepare=True
 
     def init_parameters(self):
         # prior values
         self.prior_weight_mu.data.fill_(self.prior_mean)
         self.prior_weight_sigma.data.fill_(self.prior_variance)
 
         # init our weights for the deterministic and perturbated weights
@@ -361,26 +382,47 @@
             eps_bias = self.eps_bias.data.normal_()
             bias = (sigma_bias * eps_bias)
             if return_kl:
                 kl = kl + self.kl_div(self.mu_bias, sigma_bias, self.prior_bias_mu,
                                       self.prior_bias_sigma)
 
         # perturbed feedforward
-        perturbed_outputs = F.conv2d(x * sign_input,
+        x_tmp = x * sign_input
+        perturbed_outputs_tmp = F.conv2d(x * sign_input,
                                      weight=delta_kernel,
                                      bias=bias,
                                      stride=self.stride,
                                      padding=self.padding,
                                      dilation=self.dilation,
-                                     groups=self.groups) * sign_output
+                                     groups=self.groups)
+        perturbed_outputs = perturbed_outputs_tmp * sign_output
+        out = outputs + perturbed_outputs
+
+        if self.quant_prepare:
+            # quint8 quantstub
+            x = self.quint_quant[0](x) # input
+            outputs = self.quint_quant[1](outputs) # output
+            sign_input = self.quint_quant[2](sign_input)
+            sign_output = self.quint_quant[3](sign_output)
+            x_tmp = self.quint_quant[4](x_tmp)
+            perturbed_outputs_tmp = self.quint_quant[5](perturbed_outputs_tmp) # output
+            perturbed_outputs = self.quint_quant[6](perturbed_outputs) # output
+            out = self.quint_quant[7](out) # output
+
+            # qint8 quantstub
+            sigma_weight = self.qint_quant[0](sigma_weight) # weight
+            mu_kernel = self.qint_quant[1](self.mu_kernel) # weight
+            eps_kernel = self.qint_quant[2](eps_kernel) # random variable
+            delta_kernel =self.qint_quant[3](delta_kernel) # multiply activation
 
         # returning outputs + perturbations
         if return_kl:
-            return outputs + perturbed_outputs, kl
-        return outputs + perturbed_outputs
+            return out, kl
+        return out
+
 
 
 class Conv3dFlipout(BaseVariationalLayer_):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
@@ -553,14 +595,15 @@
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride=1,
                  padding=0,
                  dilation=1,
                  groups=1,
+                 output_padding=0,
                  prior_mean=0,
                  prior_variance=1,
                  posterior_mu_init=0,
                  posterior_rho_init=-3.0,
                  bias=True):
         """
         Implements ConvTranspose1d layer with Flipout reparameterization trick.
@@ -584,14 +627,15 @@
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
+        self.output_padding = output_padding
         self.dilation = dilation
         self.groups = groups
         self.bias = bias
 
         self.kl = 0
 
         self.prior_mean = prior_mean
@@ -665,14 +709,15 @@
 
         # linear outputs
         outputs = F.conv_transpose1d(x,
                                      weight=self.mu_kernel,
                                      bias=self.mu_bias,
                                      stride=self.stride,
                                      padding=self.padding,
+                                     output_padding=self.output_padding,
                                      dilation=self.dilation,
                                      groups=self.groups)
 
         # sampling perturbation signs
         sign_input = x.clone().uniform_(-1, 1).sign()
         sign_output = outputs.clone().uniform_(-1, 1).sign()
 
@@ -698,14 +743,15 @@
         # perturbed feedforward
         perturbed_outputs = F.conv_transpose1d(
             x * sign_input,
             weight=delta_kernel,
             bias=bias,
             stride=self.stride,
             padding=self.padding,
+            output_padding=self.output_padding,
             dilation=self.dilation,
             groups=self.groups) * sign_output
 
         self.kl = kl
         # returning outputs + perturbations
         if return_kl:
             return outputs + perturbed_outputs, kl
@@ -715,14 +761,15 @@
 class ConvTranspose2dFlipout(BaseVariationalLayer_):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride=1,
                  padding=0,
+                 output_padding=0,
                  dilation=1,
                  groups=1,
                  prior_mean=0,
                  prior_variance=1,
                  posterior_mu_init=0,
                  posterior_rho_init=-3.0,
                  bias=True):
@@ -748,14 +795,15 @@
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
+        self.output_padding = output_padding
         self.dilation = dilation
         self.groups = groups
         self.bias = bias
 
         self.kl = 0
 
         self.prior_mean = prior_mean
@@ -833,14 +881,15 @@
 
         # linear outputs
         outputs = F.conv_transpose2d(x,
                                      bias=self.mu_bias,
                                      weight=self.mu_kernel,
                                      stride=self.stride,
                                      padding=self.padding,
+                                     output_padding=self.output_padding,
                                      dilation=self.dilation,
                                      groups=self.groups)
 
         # sampling perturbation signs
         sign_input = x.clone().uniform_(-1, 1).sign()
         sign_output = outputs.clone().uniform_(-1, 1).sign()
 
@@ -866,14 +915,15 @@
         # perturbed feedforward
         perturbed_outputs = F.conv_transpose2d(
             x * sign_input,
             bias=bias,
             weight=delta_kernel,
             stride=self.stride,
             padding=self.padding,
+            output_padding=self.output_padding,
             dilation=self.dilation,
             groups=self.groups) * sign_output
 
         self.kl = kl
         # returning outputs + perturbations
         if return_kl:
             return outputs + perturbed_outputs, kl
@@ -883,14 +933,15 @@
 class ConvTranspose3dFlipout(BaseVariationalLayer_):
     def __init__(self,
                  in_channels,
                  out_channels,
                  kernel_size,
                  stride=1,
                  padding=0,
+                 output_padding=0,
                  dilation=1,
                  groups=1,
                  prior_mean=0,
                  prior_variance=1,
                  posterior_mu_init=0,
                  posterior_rho_init=-3.0,
                  bias=True):
@@ -916,14 +967,15 @@
         super().__init__()
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
+        self.output_padding = output_padding
         self.dilation = dilation
         self.groups = groups
 
         self.prior_mean = prior_mean
         self.prior_variance = prior_variance
         self.posterior_mu_init = posterior_mu_init
         self.posterior_rho_init = posterior_rho_init
@@ -1001,14 +1053,15 @@
 
         # linear outputs
         outputs = F.conv_transpose3d(x,
                                      weight=self.mu_kernel,
                                      bias=self.mu_bias,
                                      stride=self.stride,
                                      padding=self.padding,
+                                     output_padding=self.output_padding,
                                      dilation=self.dilation,
                                      groups=self.groups)
 
         # sampling perturbation signs
         sign_input = x.clone().uniform_(-1, 1).sign()
         sign_output = outputs.clone().uniform_(-1, 1).sign()
 
@@ -1033,14 +1086,15 @@
         # perturbed feedforward
         perturbed_outputs = F.conv_transpose3d(
             x * sign_input,
             weight=delta_kernel,
             bias=bias,
             stride=self.stride,
             padding=self.padding,
+            output_padding=self.output_padding,
             dilation=self.dilation,
             groups=self.groups) * sign_output
 
         self.kl = kl
         # returning outputs + perturbations
         if return_kl:
             return outputs + perturbed_outputs, kl
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/linear_flipout.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/linear_flipout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -36,14 +36,16 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch.distributions.normal import Normal
 from torch.distributions.uniform import Uniform
 from ..base_variational_layer import BaseVariationalLayer_
+from torch.quantization.observer import HistogramObserver, PerChannelMinMaxObserver, MinMaxObserver
+from torch.quantization.qconfig import QConfig
 
 __all__ = ["LinearFlipout"]
 
 
 class LinearFlipout(BaseVariationalLayer_):
     def __init__(self,
                  in_features,
@@ -103,14 +105,23 @@
             self.register_buffer('prior_bias_mu', None, persistent=False)
             self.register_buffer('prior_bias_sigma', None, persistent=False)
             self.register_parameter('mu_bias', None)
             self.register_parameter('rho_bias', None)
             self.register_buffer('eps_bias', None, persistent=False)
 
         self.init_parameters()
+        self.quant_prepare=False
+    
+    def prepare(self):
+        self.qint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.qint8, qscheme=torch.per_tensor_symmetric), activation=MinMaxObserver.with_args(dtype=torch.qint8,qscheme=torch.per_tensor_symmetric))) for _ in range(4)])
+        self.quint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.quint8), activation=MinMaxObserver.with_args(dtype=torch.quint8))) for _ in range(8)])
+        self.dequant = torch.quantization.DeQuantStub()
+        self.quant_prepare=True
 
     def init_parameters(self):
         # init prior mu
         self.prior_weight_mu.fill_(self.prior_mean)
         self.prior_weight_sigma.fill_(self.prior_variance)
 
         # init weight and base perturbation weights
@@ -132,15 +143,17 @@
         return kl
 
     def forward(self, x, return_kl=True):
         if self.dnn_to_bnn_flag:
             return_kl = False
         # sampling delta_W
         sigma_weight = torch.log1p(torch.exp(self.rho_weight))
-        delta_weight = (sigma_weight * self.eps_weight.data.normal_())
+        eps_weight = self.eps_weight.data.normal_()
+        delta_weight = sigma_weight * eps_weight
+        # delta_weight = (sigma_weight * self.eps_weight.data.normal_())
 
         # get kl divergence
         if return_kl:
             kl = self.kl_div(self.mu_weight, sigma_weight, self.prior_weight_mu,
                              self.prior_weight_sigma)
 
         bias = None
@@ -149,18 +162,37 @@
             bias = (sigma_bias * self.eps_bias.data.normal_())
             if return_kl:
                 kl = kl + self.kl_div(self.mu_bias, sigma_bias, self.prior_bias_mu,
                                       self.prior_bias_sigma)
 
         # linear outputs
         outputs = F.linear(x, self.mu_weight, self.mu_bias)
-
         sign_input = x.clone().uniform_(-1, 1).sign()
         sign_output = outputs.clone().uniform_(-1, 1).sign()
-
-        perturbed_outputs = F.linear(x * sign_input, delta_weight,
-                                     bias) * sign_output
+        x_tmp = x * sign_input
+        perturbed_outputs_tmp = F.linear(x_tmp, delta_weight, bias)
+        perturbed_outputs = perturbed_outputs_tmp * sign_output
+        out = outputs + perturbed_outputs
+
+        if self.quant_prepare:
+            # quint8 quantstub
+            x = self.quint_quant[0](x) # input
+            outputs = self.quint_quant[1](outputs) # output
+            sign_input = self.quint_quant[2](sign_input)
+            sign_output = self.quint_quant[3](sign_output)
+            x_tmp = self.quint_quant[4](x_tmp)
+            perturbed_outputs_tmp = self.quint_quant[5](perturbed_outputs_tmp) # output
+            perturbed_outputs = self.quint_quant[6](perturbed_outputs) # output
+            out = self.quint_quant[7](out) # output
+
+            # qint8 quantstub
+            sigma_weight = self.qint_quant[0](sigma_weight) # weight
+            mu_weight = self.qint_quant[1](self.mu_weight) # weight
+            eps_weight = self.qint_quant[2](eps_weight) # random variable
+            delta_weight =self.qint_quant[3](delta_weight) # multiply activation
+            
 
         # returning outputs + perturbations
         if return_kl:
-            return outputs + perturbed_outputs, kl
-        return outputs + perturbed_outputs
+            return out, kl
+        return out
+
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/flipout_layers/rnn_flipout.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/flipout_layers/rnn_flipout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/conv_variational.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/conv_variational.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -44,14 +44,16 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import Parameter
 from ..base_variational_layer import BaseVariationalLayer_, get_kernel_size
 import math
+from torch.quantization.observer import HistogramObserver, PerChannelMinMaxObserver, MinMaxObserver
+from torch.quantization.qconfig import QConfig
 
 __all__ = [
     'Conv1dReparameterization',
     'Conv2dReparameterization',
     'Conv3dReparameterization',
     'ConvTranspose1dReparameterization',
     'ConvTranspose2dReparameterization',
@@ -291,14 +293,23 @@
             self.register_parameter('mu_bias', None)
             self.register_parameter('rho_bias', None)
             self.register_buffer('eps_bias', None, persistent=False)
             self.register_buffer('prior_bias_mu', None, persistent=False)
             self.register_buffer('prior_bias_sigma', None, persistent=False)
 
         self.init_parameters()
+        self.quant_prepare=False
+
+    def prepare(self):
+        self.qint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.qint8, qscheme=torch.per_tensor_symmetric), activation=MinMaxObserver.with_args(dtype=torch.qint8,qscheme=torch.per_tensor_symmetric))) for _ in range(5)])
+        self.quint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.quint8), activation=MinMaxObserver.with_args(dtype=torch.quint8))) for _ in range(2)])
+        self.dequant = torch.quantization.DeQuantStub()
+        self.quant_prepare=True
 
     def init_parameters(self):
         self.prior_weight_mu.fill_(self.prior_mean)
         self.prior_weight_sigma.fill_(self.prior_variance)
 
         self.mu_kernel.data.normal_(mean=self.posterior_mu_init[0], std=0.1)
         self.rho_kernel.data.normal_(mean=self.posterior_rho_init[0], std=0.1)
@@ -321,15 +332,16 @@
 
     def forward(self, input, return_kl=True):
         if self.dnn_to_bnn_flag:
             return_kl = False
 
         sigma_weight = torch.log1p(torch.exp(self.rho_kernel))
         eps_kernel = self.eps_kernel.data.normal_()
-        weight = self.mu_kernel + (sigma_weight * eps_kernel)
+        tmp_result = sigma_weight * eps_kernel
+        weight = self.mu_kernel + tmp_result
 
         if return_kl:
             kl_weight = self.kl_div(self.mu_kernel, sigma_weight,
                                     self.prior_weight_mu, self.prior_weight_sigma)
         bias = None
 
         if self.bias:
@@ -338,21 +350,35 @@
             bias = self.mu_bias + (sigma_bias * eps_bias)
             if return_kl:
                 kl_bias = self.kl_div(self.mu_bias, sigma_bias, self.prior_bias_mu,
                                       self.prior_bias_sigma)
 
         out = F.conv2d(input, weight, bias, self.stride, self.padding,
                        self.dilation, self.groups)
+
+        if self.quant_prepare:
+            # quint8 quantstub
+            input = self.quint_quant[0](input) # input
+            out = self.quint_quant[1](out) # output
+
+            # qint8 quantstub
+            sigma_weight = self.qint_quant[0](sigma_weight) # weight
+            mu_kernel = self.qint_quant[1](self.mu_kernel) # weight
+            eps_kernel = self.qint_quant[2](eps_kernel) # random variable
+            tmp_result =self.qint_quant[3](tmp_result) # multiply activation
+            weight = self.qint_quant[4](weight) # add activatation
+            
+
         if return_kl:
             if self.bias:
                 kl = kl_weight + kl_bias
             else:
                 kl = kl_weight
             return out, kl
-
+            
         return out
 
 
 class Conv3dReparameterization(BaseVariationalLayer_):
     def __init__(self,
                  in_channels,
                  out_channels,
@@ -942,7 +968,8 @@
             if self.bias:
                 kl = kl_weight + kl_bias
             else:
                 kl = kl_weight
             return out, kl
 
         return out
+
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/linear_variational.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/linear_variational.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -43,14 +43,16 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import Module, Parameter
 from ..base_variational_layer import BaseVariationalLayer_
 import math
+from torch.quantization.observer import HistogramObserver, PerChannelMinMaxObserver, MinMaxObserver
+from torch.quantization.qconfig import QConfig
 
 
 class LinearReparameterization(BaseVariationalLayer_):
     def __init__(self,
                  in_features,
                  out_features,
                  prior_mean=0,
@@ -112,14 +114,23 @@
             self.register_buffer('prior_bias_mu', None, persistent=False)
             self.register_buffer('prior_bias_sigma', None, persistent=False)
             self.register_parameter('mu_bias', None)
             self.register_parameter('rho_bias', None)
             self.register_buffer('eps_bias', None, persistent=False)
 
         self.init_parameters()
+        self.quant_prepare=False
+    
+    def prepare(self):
+        self.qint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.qint8, qscheme=torch.per_tensor_symmetric), activation=MinMaxObserver.with_args(dtype=torch.qint8,qscheme=torch.per_tensor_symmetric))) for _ in range(5)])
+        self.quint_quant = nn.ModuleList([torch.quantization.QuantStub(
+                                         QConfig(weight=MinMaxObserver.with_args(dtype=torch.quint8), activation=MinMaxObserver.with_args(dtype=torch.quint8))) for _ in range(2)])
+        self.dequant = torch.quantization.DeQuantStub()
+        self.quant_prepare=True
 
     def init_parameters(self):
         self.prior_weight_mu.fill_(self.prior_mean)
         self.prior_weight_sigma.fill_(self.prior_variance)
 
         self.mu_weight.data.normal_(mean=self.posterior_mu_init[0], std=0.1)
         self.rho_weight.data.normal_(mean=self.posterior_rho_init[0], std=0.1)
@@ -143,29 +154,46 @@
                               self.prior_bias_mu, self.prior_bias_sigma)
         return kl
 
     def forward(self, input, return_kl=True):
         if self.dnn_to_bnn_flag:
             return_kl = False
         sigma_weight = torch.log1p(torch.exp(self.rho_weight))
-        weight = self.mu_weight + \
-            (sigma_weight * self.eps_weight.data.normal_())
+        eps_weight = self.eps_weight.data.normal_()
+        tmp_result = sigma_weight * eps_weight
+        weight = self.mu_weight + tmp_result
+
+
         if return_kl:
             kl_weight = self.kl_div(self.mu_weight, sigma_weight,
                                     self.prior_weight_mu, self.prior_weight_sigma)
         bias = None
 
         if self.mu_bias is not None:
             sigma_bias = torch.log1p(torch.exp(self.rho_bias))
             bias = self.mu_bias + (sigma_bias * self.eps_bias.data.normal_())
             if return_kl:
                 kl_bias = self.kl_div(self.mu_bias, sigma_bias, self.prior_bias_mu,
                                       self.prior_bias_sigma)
 
         out = F.linear(input, weight, bias)
+
+        if self.quant_prepare:
+            # quint8 quantstub
+            input = self.quint_quant[0](input) # input
+            out = self.quint_quant[1](out) # output
+
+            # qint8 quantstub
+            sigma_weight = self.qint_quant[0](sigma_weight) # weight
+            mu_weight = self.qint_quant[1](self.mu_weight) # weight
+            eps_weight = self.qint_quant[2](eps_weight) # random variable
+            tmp_result =self.qint_quant[3](tmp_result) # multiply activation
+            weight = self.qint_quant[4](weight) # add activatation
+
+
         if return_kl:
             if self.mu_bias is not None:
                 kl = kl_weight + kl_bias
             else:
                 kl = kl_weight
 
             return out, kl
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/layers/variational_layers/rnn_variational.py` & `bayesian-torch-0.4.0/bayesian_torch/layers/variational_layers/rnn_variational.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_flipout.py` & `bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_flipout.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_flipout_large.py` & `bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_flipout_large.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_variational.py` & `bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_variational.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/bayesian/resnet_variational_large.py` & `bayesian-torch-0.4.0/bayesian_torch/models/bayesian/resnet_variational_large.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import torch.nn.functional as F
 import torch.nn.init as init
 from bayesian_torch.layers import Conv2dReparameterization
 from bayesian_torch.layers import LinearReparameterization
 from bayesian_torch.layers import BatchNorm2dLayer
 
 __all__ = [
-    'ResNet', 'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152'
+    'ResNet', 'resnet18', 'resnet34', 'resnet50', 'resnet101', 'resnet152', 'BasicBlock', 'Bottleneck'
 ]
 
 prior_mu = 0.0
 prior_sigma = 0.1
 posterior_mu_init = 0.0
 posterior_rho_init = -9.0
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/bayesian/simple_cnn_variational.py` & `bayesian-torch-0.4.0/bayesian_torch/models/bayesian/simple_cnn_variational.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/deterministic/resnet.py` & `bayesian-torch-0.4.0/bayesian_torch/models/deterministic/resnet.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,57 +39,67 @@
         self.conv1 = nn.Conv2d(in_planes,
                                planes,
                                kernel_size=3,
                                stride=stride,
                                padding=1,
                                bias=False)
         self.bn1 = nn.BatchNorm2d(planes)
+        self.relu1 = nn.ReLU(inplace=True)
         self.conv2 = nn.Conv2d(planes,
                                planes,
                                kernel_size=3,
                                stride=1,
                                padding=1,
                                bias=False)
         self.bn2 = nn.BatchNorm2d(planes)
-
+        self.skip_add = nn.quantized.FloatFunctional()
         self.shortcut = nn.Sequential()
+        self.relu2 = nn.ReLU(inplace=True)
+
         if stride != 1 or in_planes != planes:
             if option == 'A':
                 self.shortcut = LambdaLayer(lambda x: F.pad(
-                    x[:, :, ::2, ::2],
+                    x[:, :, ::2, ::2].contiguous(),
                     (0, 0, 0, 0, planes // 4, planes // 4), "constant", 0))
             elif option == 'B':
                 self.shortcut = nn.Sequential(
                     nn.Conv2d(in_planes,
                               self.expansion * planes,
                               kernel_size=1,
                               stride=stride,
                               bias=False),
                     nn.BatchNorm2d(self.expansion * planes))
 
     def forward(self, x):
-        out = F.relu(self.bn1(self.conv1(x)))
-        out = self.bn2(self.conv2(out))
-        out += self.shortcut(x)
-        out = F.relu(out)
+        identity = self.shortcut(x)
+        out = self.conv1(x)
+        out = self.bn1(out)
+        out = self.relu1(out)
+
+        out = self.conv2(out)
+        out = self.bn2(out)
+        out = self.skip_add.add(out, identity)
+        #out += self.shortcut(x)
+        out = self.relu2(out)
         return out
-
+        
 
 class ResNet(nn.Module):
     def __init__(self, block, num_blocks, num_classes=10):
         super(ResNet, self).__init__()
         self.in_planes = 16
 
         self.conv1 = nn.Conv2d(3,
                                16,
                                kernel_size=3,
                                stride=1,
                                padding=1,
                                bias=False)
         self.bn1 = nn.BatchNorm2d(16)
+        self.relu1 = nn.ReLU(inplace=True)
         self.layer1 = self._make_layer(block, 16, num_blocks[0], stride=1)
         self.layer2 = self._make_layer(block, 32, num_blocks[1], stride=2)
         self.layer3 = self._make_layer(block, 64, num_blocks[2], stride=2)
         self.linear = nn.Linear(64, num_classes)
 
         self.apply(_weights_init)
 
@@ -99,24 +109,25 @@
         for stride in strides:
             layers.append(block(self.in_planes, planes, stride))
             self.in_planes = planes * block.expansion
 
         return nn.Sequential(*layers)
 
     def forward(self, x):
-        out = F.relu(self.bn1(self.conv1(x)))
+        out = self.conv1(x)
+        out = self.bn1(out)
+        out = self.relu1(out)
         out = self.layer1(out)
         out = self.layer2(out)
         out = self.layer3(out)
         out = F.avg_pool2d(out, out.size()[3])
         out = out.view(out.size(0), -1)
         out = self.linear(out)
         return out
 
-
 def resnet20():
     return ResNet(BasicBlock, [3, 3, 3])
 
 
 def resnet32():
     return ResNet(BasicBlock, [5, 5, 5])
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/deterministic/resnet_large.py` & `bayesian-torch-0.4.0/bayesian_torch/models/deterministic/resnet_large.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/deterministic/simple_cnn.py` & `bayesian-torch-0.4.0/bayesian_torch/models/deterministic/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/dnn_to_bnn.py` & `bayesian-torch-0.4.0/bayesian_torch/models/dnn_to_bnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs
+# Copyright (C) 2023 Intel Labs
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/models/flipout/simple_cnn.py` & `bayesian-torch-0.4.0/bayesian_torch/models/flipout/simple_cnn.py`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/bayesian_torch/utils/avuc_loss.py` & `bayesian-torch-0.4.0/bayesian_torch/utils/avuc_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch/utils/util.py` & `bayesian-torch-0.4.0/bayesian_torch/utils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Intel Labs 
+# Copyright (C) 2023 Intel Labs 
 #
 # BSD-3-Clause License
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch.egg-info/PKG-INFO` & `bayesian-torch-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,19 @@
-Metadata-Version: 2.1
-Name: bayesian-torch
-Version: 0.3.0
-Summary: A library for Bayesian neural network layers and uncertainty estimation in Deep Learning
-Home-page: https://github.com/IntelLabs/bayesian-torch
-Author: Intel Labs
-Author-email: ranganath.krishnan@intel.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/IntelLabs/bayesian-torch/5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png" width="500px">
 <h2 >
 A library for Bayesian neural network layers and uncertainty estimation in Deep Learning </a>
 </h2>
 
 [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://github.com/IntelLabs/bayesian-torch)
 [![pytorch](https://img.shields.io/badge/pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch)
-[![version](https://img.shields.io/badge/release-0.2.1-green)](https://github.com/IntelLabs/bayesian-torch/releases)
+[![version](https://img.shields.io/badge/release-0.4.0-green)](https://github.com/IntelLabs/bayesian-torch/releases)
 [![license](https://img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/IntelLabs/bayesian-torch/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/bayesian-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)](https://pepy.tech/project/bayesian-torch)
+[![Downloads](https://static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-torch)
 <h4 align="center">
   <a href="https://github.com/IntelLabs/bayesian-torch#installing-bayesian-torch">Get Started</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#usage">Example usage</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch/blob/main/doc/bayesian_torch.layers.md">Documentation</a> |
   <a href="https://github.com/IntelLabs/bayesian-torch#citing">Citing</a>   
 </h4>
 
@@ -61,16 +40,17 @@
       LinearFlipout 
       Conv1dFlipout, Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout, ConvTranspose3dFlipout
       LSTMFlipout
 
 
 
 **Key features:**
-* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
+* [dnn_to_bnn()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An API to convert deterministic deep neural network (dnn) model of any architecture to Bayesian deep neural network (bnn) model, simplifying the model definition i.e. drop-in replacements  of Convolutional, Linear and LSTM layers to corresponding Bayesian layers. This will enable seamless conversion of existing topology of larger models to Bayesian deep neural network models for extending towards uncertainty-aware applications. 
 * [MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72): Specifying weight priors and variational posteriors in Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/AAAI/article/view/5875)]
+* [Quantization](https://github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of Bayesian deep neural network models with simple API's [enable_prepare()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/quantize.py#L160)
 * [AvUC](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-Paper.pdf)]
 
 ## Installing Bayesian-Torch
 
 **To install core library using `pip`:**
 ```
 pip install bayesian-torch
@@ -215,14 +195,21 @@
 To evaluate deterministic ResNet on CIFAR10, run this command:
 
 **Vanilla**
 ```test
 sh scripts/test_deterministic_cifar.sh
 ```
 
+### Post Training Quantization (PTQ)
+
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this command:
+```test
+sh scripts/quantize_bayesian_cifar.sh
+```
+
 ## Citing
 
 If you use this code, please cite as:
 ```sh
 @software{krishnan2022bayesiantorch,
   author       = {Ranganath Krishnan and Pi Esposito and Mahesh Subedar},               
   title        = {Bayesian-Torch: Bayesian neural network layers for uncertainty estimation},
@@ -258,9 +245,7 @@
   year={2020},
   url = {https://ojs.aaai.org/index.php/AAAI/article/view/5875}
 }
 ```
 
 This library and code is intended for researchers and developers, enables to quantify principled uncertainty estimates from deep learning model predictions using stochastic variational inference in Bayesian neural networks. 
 Feedbacks, issues and contributions are welcome. Email to <ranganath.krishnan@intel.com> for any questions.
-
-
```

#### html2text {}

```diff
@@ -1,32 +1,20 @@
-Metadata-Version: 2.1 Name: bayesian-torch Version: 0.3.0 Summary: A library
-for Bayesian neural network layers and uncertainty estimation in Deep Learning
-Home-page: https://github.com/IntelLabs/bayesian-torch Author: Intel Labs
-Author-email: ranganath.krishnan@intel.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Description-Content-Type: text/markdown License-File: LICENSE
          [https://raw.githubusercontent.com/IntelLabs/bayesian-torch/
       5a4793ba0a54660c891df8af0d5729e840340a88/assets/bayesian-torch.png]
  ***** A library for Bayesian neural network layers and uncertainty estimation
                             in Deep Learning *****
      [![python](https://img.shields.io/badge/python-3.7%2B-blue)](https://
 github.com/IntelLabs/bayesian-torch) [![pytorch](https://img.shields.io/badge/
    pytorch-1.7.0%2B-orange)](https://github.com/IntelLabs/bayesian-torch) [!
-     [version](https://img.shields.io/badge/release-0.2.1-green)](https://
+     [version](https://img.shields.io/badge/release-0.4.0-green)](https://
       github.com/IntelLabs/bayesian-torch/releases) [![license](https://
     img.shields.io/badge/license-BSD%203--Clause-blue)](https://github.com/
       IntelLabs/bayesian-torch/blob/main/LICENSE) [![Downloads](https://
-                 static.pepy.tech/personalized-badge/bayesian-
-torch?period=total&units=international_system&left_color=grey&right_color=darkblue&left_text=downloads)]
-                  (https://pepy.tech/project/bayesian-torch)
+  static.pepy.tech/badge/bayesian-torch)](https://pepy.tech/project/bayesian-
+                                    torch)
          *** Get_Started | Example_usage | Documentation | Citing ***
 ___ Bayesian-Torch is a library of neural network layers and utilities
 extending the core of PyTorch to enable Bayesian inference in deep learning
 models to quantify principled uncertainty estimates in model predictions. ##
 Overview Bayesian-Torch is designed to be flexible and enables seamless
 extension of deterministic deep neural network model to corresponding Bayesian
 form by simply replacing the deterministic layers with Bayesian layers. It
@@ -40,45 +28,51 @@
 ConvTranspose3dReparameterization LSTMReparameterization * **[Variational
 layers with Flipout Monte Carlo estimators](https://github.com/IntelLabs/
 bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)** [[Wen et al.
 2018](https://arxiv.org/abs/1803.04386)] LinearFlipout Conv1dFlipout,
 Conv2dFlipout, Conv3dFlipout, ConvTranspose1dFlipout, ConvTranspose2dFlipout,
 ConvTranspose3dFlipout LSTMFlipout **Key features:** * [dnn_to_bnn()](https://
 github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/models/
-dnn_to_bnn.py#L127): An API to convert deterministic deep neural network (dnn)
-model of any architecture to Bayesian deep neural network (bnn) model,
-simplifying the model definition i.e. drop-in replacements of Convolutional,
-Linear and LSTM layers to corresponding Bayesian layers. This will enable
-seamless conversion of existing topology of larger models to Bayesian deep
-neural network models for extending towards uncertainty-aware applications. *
-[MOPED](https://github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/
-utils/util.py#L72): Specifying weight priors and variational posteriors in
-Bayesian neural networks with Empirical Bayes [[Krishnan et al. 2020](https://
-ojs.aaai.org/index.php/AAAI/article/view/5875)] * [AvUC](https://github.com/
-IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/avuc_loss.py): Accuracy
-versus Uncertainty Calibration loss [[Krishnan and Tickoo 2020](https://
-proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
-Paper.pdf)] ## Installing Bayesian-Torch **To install core library using `pip`:
-** ``` pip install bayesian-torch ``` **To install latest development version
-from source:** ```sh git clone https://github.com/IntelLabs/bayesian-torch cd
-bayesian-torch pip install . ```  ## Usage There are two ways to build Bayesian
-deep neural networks using Bayesian-Torch: 1. Convert an existing deterministic
-deep neural network (dnn) model to Bayesian deep neural network (bnn) model
-with dnn_to_bnn() API 2. Define your custom model using the Bayesian layers (
-[Reparameterization](https://github.com/IntelLabs/bayesian-torch/tree/main/
-bayesian_torch/layers/variational_layers) or [Flipout](https://github.com/
-IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/flipout_layers)) (1)
-For instance, building Bayesian-ResNet18 from torchvision deterministic
-ResNet18 model is as simple as: ``` import torch import torchvision from
-bayesian_torch.models.dnn_to_bnn import dnn_to_bnn, get_kl_loss
-const_bnn_prior_parameters = { "prior_mu": 0.0, "prior_sigma": 1.0,
-"posterior_mu_init": 0.0, "posterior_rho_init": -3.0, "type":
-"Reparameterization", # Flipout or Reparameterization "moped_enable": False, #
-True to initialize mu/sigma from the pretrained dnn weights "moped_delta": 0.5,
-} model = torchvision.models.resnet18() dnn_to_bnn(model,
+dnn_to_bnn.py#L127): Seamless conversion of model to be Uncertainty-aware. An
+API to convert deterministic deep neural network (dnn) model of any
+architecture to Bayesian deep neural network (bnn) model, simplifying the model
+definition i.e. drop-in replacements of Convolutional, Linear and LSTM layers
+to corresponding Bayesian layers. This will enable seamless conversion of
+existing topology of larger models to Bayesian deep neural network models for
+extending towards uncertainty-aware applications. * [MOPED](https://github.com/
+IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/util.py#L72):
+Specifying weight priors and variational posteriors in Bayesian neural networks
+with Empirical Bayes [[Krishnan et al. 2020](https://ojs.aaai.org/index.php/
+AAAI/article/view/5875)] * [Quantization](https://github.com/IntelLabs/
+bayesian-torch/tree/main/bayesian_torch/ao): Post Training Quantization of
+Bayesian deep neural network models with simple API's [enable_prepare()](https:
+//github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/ao/quantization/
+quantize.py#L134) and [convert()](https://github.com/IntelLabs/bayesian-torch/
+blob/main/bayesian_torch/ao/quantization/quantize.py#L160) * [AvUC](https://
+github.com/IntelLabs/bayesian-torch/blob/main/bayesian_torch/utils/
+avuc_loss.py): Accuracy versus Uncertainty Calibration loss [[Krishnan and
+Tickoo 2020](https://proceedings.neurips.cc/paper/2020/file/
+d3d9446802a44259755d38e6d163e820-Paper.pdf)] ## Installing Bayesian-Torch **To
+install core library using `pip`:** ``` pip install bayesian-torch ``` **To
+install latest development version from source:** ```sh git clone https://
+github.com/IntelLabs/bayesian-torch cd bayesian-torch pip install . ```  ##
+Usage There are two ways to build Bayesian deep neural networks using Bayesian-
+Torch: 1. Convert an existing deterministic deep neural network (dnn) model to
+Bayesian deep neural network (bnn) model with dnn_to_bnn() API 2. Define your
+custom model using the Bayesian layers ([Reparameterization](https://
+github.com/IntelLabs/bayesian-torch/tree/main/bayesian_torch/layers/
+variational_layers) or [Flipout](https://github.com/IntelLabs/bayesian-torch/
+tree/main/bayesian_torch/layers/flipout_layers)) (1) For instance, building
+Bayesian-ResNet18 from torchvision deterministic ResNet18 model is as simple
+as: ``` import torch import torchvision from bayesian_torch.models.dnn_to_bnn
+import dnn_to_bnn, get_kl_loss const_bnn_prior_parameters = { "prior_mu": 0.0,
+"prior_sigma": 1.0, "posterior_mu_init": 0.0, "posterior_rho_init": -3.0,
+"type": "Reparameterization", # Flipout or Reparameterization "moped_enable":
+False, # True to initialize mu/sigma from the pretrained dnn weights
+"moped_delta": 0.5, } model = torchvision.models.resnet18() dnn_to_bnn(model,
 const_bnn_prior_parameters) ``` To use MOPED method i.e. setting the prior and
 initializing variational parameters from a pretrained deterministic model
 (helps training convergence of larger models): ``` const_bnn_prior_parameters =
 { "prior_mu": 0.0, "prior_sigma": 1.0, "posterior_mu_init": 0.0,
 "posterior_rho_init": -3.0, "type": "Reparameterization", # Flipout or
 Reparameterization "moped_enable": True, # True to initialize mu/sigma from the
 pretrained dnn weights "moped_delta": 0.5, } model =
@@ -111,25 +105,27 @@
 train deterministic ResNet on CIFAR10, run this command: **Vanilla** ```train
 sh scripts/train_deterministic_cifar.sh ``` ### Evaluation To evaluate Bayesian
 ResNet on CIFAR10, run this command: **Mean-field variational inference
 (Reparameterized Monte Carlo estimator)** ```test sh scripts/
 test_bayesian_cifar.sh ``` **Mean-field variational inference (Flipout Monte
 Carlo estimator)** ```test sh scripts/test_bayesian_flipout_cifar.sh ``` To
 evaluate deterministic ResNet on CIFAR10, run this command: **Vanilla** ```test
-sh scripts/test_deterministic_cifar.sh ``` ## Citing If you use this code,
-please cite as: ```sh @software{krishnan2022bayesiantorch, author = {Ranganath
-Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-Torch: Bayesian
-neural network layers for uncertainty estimation}, month = jan, year = 2022,
-doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/zenodo.5908307}
-howpublished = {\url{https://github.com/IntelLabs/bayesian-torch}} } ```
-Accuracy versus Uncertainty Calibration (AvUC) loss ```sh @inproceedings
-{NEURIPS2020_d3d94468, title = {Improving model calibration with accuracy
-versus uncertainty optimization}, author = {Krishnan, Ranganath and Tickoo,
-Omesh}, booktitle = {Advances in Neural Information Processing Systems}, volume
-= {33}, pages = {18237--18248}, year = {2020}, url = {https://
+sh scripts/test_deterministic_cifar.sh ``` ### Post Training Quantization (PTQ)
+To quantize Bayesian ResNet (convert to INT8) and evaluate on CIFAR10, run this
+command: ```test sh scripts/quantize_bayesian_cifar.sh ``` ## Citing If you use
+this code, please cite as: ```sh @software{krishnan2022bayesiantorch, author =
+{Ranganath Krishnan and Pi Esposito and Mahesh Subedar}, title = {Bayesian-
+Torch: Bayesian neural network layers for uncertainty estimation}, month = jan,
+year = 2022, doi = {10.5281/zenodo.5908307}, url = {https://doi.org/10.5281/
+zenodo.5908307} howpublished = {\url{https://github.com/IntelLabs/bayesian-
+torch}} } ``` Accuracy versus Uncertainty Calibration (AvUC) loss ```sh
+@inproceedings{NEURIPS2020_d3d94468, title = {Improving model calibration with
+accuracy versus uncertainty optimization}, author = {Krishnan, Ranganath and
+Tickoo, Omesh}, booktitle = {Advances in Neural Information Processing
+Systems}, volume = {33}, pages = {18237--18248}, year = {2020}, url = {https://
 proceedings.neurips.cc/paper/2020/file/d3d9446802a44259755d38e6d163e820-
 Paper.pdf} } ``` MOdel Priors with Empirical Bayes using DNN (MOPED) ```sh
 @inproceedings{krishnan2020specifying, title={Specifying weight priors in
 bayesian deep neural networks with empirical bayes}, author={Krishnan,
 Ranganath and Subedar, Mahesh and Tickoo, Omesh}, booktitle={Proceedings of the
 AAAI Conference on Artificial Intelligence}, volume={34}, number={04}, pages=
 {4477--4484}, year={2020}, url = {https://ojs.aaai.org/index.php/AAAI/article/
```

### Comparing `bayesian-torch-0.3.0/bayesian_torch.egg-info/SOURCES.txt` & `bayesian-torch-0.4.0/bayesian_torch.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,51 +6,73 @@
 assets/bayesian-torch.png
 bayesian_torch/__init__.py
 bayesian_torch.egg-info/PKG-INFO
 bayesian_torch.egg-info/SOURCES.txt
 bayesian_torch.egg-info/dependency_links.txt
 bayesian_torch.egg-info/requires.txt
 bayesian_torch.egg-info/top_level.txt
+bayesian_torch/ao/__init__.py
+bayesian_torch/ao/nn/__init__.py
+bayesian_torch/ao/nn/quantized/__init__.py
+bayesian_torch/ao/nn/quantized/modules/quantize_conv_variational.py
+bayesian_torch/ao/nn/quantized/modules/quantize_linear_variational.py
+bayesian_torch/ao/nn/quantized/modules/quantized_conv_flipout.py
+bayesian_torch/ao/nn/quantized/modules/quantized_linear_flipout.py
+bayesian_torch/ao/quantization/__init__.py
+bayesian_torch/ao/quantization/quantize.py
 bayesian_torch/examples/main_bayesian_cifar.py
 bayesian_torch/examples/main_bayesian_cifar_dnn2bnn.py
 bayesian_torch/examples/main_bayesian_flipout_cifar.py
 bayesian_torch/examples/main_bayesian_flipout_imagenet.py
 bayesian_torch/examples/main_bayesian_imagenet.py
+bayesian_torch/examples/main_bayesian_imagenet_bnn2qbnn.py
+bayesian_torch/examples/main_bayesian_imagenet_dnn2bnn.py
 bayesian_torch/examples/main_bayesian_mnist.py
 bayesian_torch/examples/main_deterministic_cifar.py
 bayesian_torch/examples/main_deterministic_imagenet.py
 bayesian_torch/examples/main_deterministic_mnist.py
+bayesian_torch/examples/quantization_test.py
 bayesian_torch/layers/__init__.py
 bayesian_torch/layers/base_variational_layer.py
 bayesian_torch/layers/batchnorm.py
 bayesian_torch/layers/dropout.py
 bayesian_torch/layers/relu.py
 bayesian_torch/layers/flipout_layers/__init__.py
 bayesian_torch/layers/flipout_layers/conv_flipout.py
 bayesian_torch/layers/flipout_layers/linear_flipout.py
+bayesian_torch/layers/flipout_layers/quantized_conv_flipout.py
+bayesian_torch/layers/flipout_layers/quantized_linear_flipout.py
 bayesian_torch/layers/flipout_layers/rnn_flipout.py
 bayesian_torch/layers/variational_layers/__init__.py
 bayesian_torch/layers/variational_layers/conv_variational.py
 bayesian_torch/layers/variational_layers/linear_variational.py
+bayesian_torch/layers/variational_layers/quantize_conv_variational.py
+bayesian_torch/layers/variational_layers/quantize_linear_variational.py
 bayesian_torch/layers/variational_layers/rnn_variational.py
 bayesian_torch/models/__init__.py
+bayesian_torch/models/bnn_to_qbnn.py
 bayesian_torch/models/dnn_to_bnn.py
 bayesian_torch/models/bayesian/__init__.py
+bayesian_torch/models/bayesian/quantized_resnet_flipout_large.py
+bayesian_torch/models/bayesian/quantized_resnet_variational_large.py
 bayesian_torch/models/bayesian/resnet_flipout.py
 bayesian_torch/models/bayesian/resnet_flipout_large.py
 bayesian_torch/models/bayesian/resnet_variational.py
 bayesian_torch/models/bayesian/resnet_variational_large.py
 bayesian_torch/models/bayesian/simple_cnn_variational.py
 bayesian_torch/models/deterministic/__init__.py
 bayesian_torch/models/deterministic/resnet.py
 bayesian_torch/models/deterministic/resnet_large.py
 bayesian_torch/models/deterministic/simple_cnn.py
 bayesian_torch/models/flipout/__init__.py
 bayesian_torch/models/flipout/resnet.py
 bayesian_torch/models/flipout/simple_cnn.py
+bayesian_torch/quantization/__init__.py
+bayesian_torch/quantization/quantize.py
+bayesian_torch/scripts/quantize_bayesian_cifar.sh
 bayesian_torch/scripts/test_bayesian_cifar.sh
 bayesian_torch/scripts/test_bayesian_flipout_cifar.sh
 bayesian_torch/scripts/test_bayesian_flipout_imagenet.sh
 bayesian_torch/scripts/test_bayesian_imagenet.sh
 bayesian_torch/scripts/test_bayesian_mnist.sh
 bayesian_torch/scripts/test_deterministic_cifar.sh
 bayesian_torch/scripts/test_deterministic_imagenet.sh
```

### Comparing `bayesian-torch-0.3.0/doc/bayesian_torch.layers.md` & `bayesian-torch-0.4.0/doc/bayesian_torch.layers.md`

 * *Files identical despite different names*

### Comparing `bayesian-torch-0.3.0/setup.py` & `bayesian-torch-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open(path.join(this_directory, 'requirements.txt'), encoding='utf-8') as f:
     install_requires = f.read()
 
 setup(
     name = "bayesian-torch",
     packages = find_packages(),
-    version = "0.3.0",
+    version = "0.4.0",
     description = "A library for Bayesian neural network layers and uncertainty estimation in Deep Learning",
     author = "Intel Labs",
     author_email = "ranganath.krishnan@intel.com",
     url = "https://github.com/IntelLabs/bayesian-torch",
     long_description = long_desc,
     long_description_content_type = "text/markdown",
     install_requires = install_requires,
```

