# Comparing `tmp/t3w-0.1.0.post1.tar.gz` & `tmp/t3w-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t3w-0.1.0.post1.tar", last modified: Thu Jul 27 08:22:55 2023, max compression
+gzip compressed data, was "t3w-0.1.0.post2.tar", last modified: Thu Jul 27 12:02:05 2023, max compression
```

## Comparing `t3w-0.1.0.post1.tar` & `t3w-0.1.0.post2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 hyuyao    (1000) hyuyao    (1000)        0 2023-07-27 08:22:55.475873 t3w-0.1.0.post1/
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)    11401 2023-07-27 08:07:58.000000 t3w-0.1.0.post1/LICENSE
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)     1698 2023-07-27 08:22:55.475873 t3w-0.1.0.post1/PKG-INFO
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)     1403 2023-07-27 07:59:10.000000 t3w-0.1.0.post1/README.md
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)       38 2023-07-27 08:22:55.475873 t3w-0.1.0.post1/setup.cfg
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)      898 2023-07-27 08:20:37.000000 t3w-0.1.0.post1/setup.py
-drwxr-xr-x   0 hyuyao    (1000) hyuyao    (1000)        0 2023-07-27 08:22:55.475873 t3w-0.1.0.post1/t3w.egg-info/
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)     1698 2023-07-27 08:22:55.000000 t3w-0.1.0.post1/t3w.egg-info/PKG-INFO
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)      167 2023-07-27 08:22:55.000000 t3w-0.1.0.post1/t3w.egg-info/SOURCES.txt
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)        1 2023-07-27 08:22:55.000000 t3w-0.1.0.post1/t3w.egg-info/dependency_links.txt
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)       56 2023-07-27 08:22:55.000000 t3w-0.1.0.post1/t3w.egg-info/requires.txt
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)        4 2023-07-27 08:22:55.000000 t3w-0.1.0.post1/t3w.egg-info/top_level.txt
--rw-r--r--   0 hyuyao    (1000) hyuyao    (1000)    28747 2023-07-27 08:09:51.000000 t3w-0.1.0.post1/t3w.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:05.744051 t3w-0.1.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-27 12:01:53.000000 t3w-0.1.0.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 12:02:05.744051 t3w-0.1.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-27 12:01:53.000000 t3w-0.1.0.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:02:05.744051 t3w-0.1.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-27 12:01:53.000000 t3w-0.1.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:02:05.744051 t3w-0.1.0.post2/t3w.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-27 12:02:05.000000 t3w-0.1.0.post2/t3w.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-27 12:02:05.000000 t3w-0.1.0.post2/t3w.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:02:05.000000 t3w-0.1.0.post2/t3w.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 12:02:05.000000 t3w-0.1.0.post2/t3w.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 12:02:05.000000 t3w-0.1.0.post2/t3w.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28780 2023-07-27 12:01:53.000000 t3w-0.1.0.post2/t3w.py
```

### Comparing `t3w-0.1.0.post1/LICENSE` & `t3w-0.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `t3w-0.1.0.post1/PKG-INFO` & `t3w-0.1.0.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: t3w
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Typed Thin PyTorch Wrapper
 Home-page: https://github.com/tjyuyao/t3w
 Author: Yuyao Huang
 Author-email: huangyuyao@outlook.com
 Description-Content-Type: text/markdown
 Provides-Extra: common
 Provides-Extra: all
 License-File: LICENSE
 
 # `t3w.py` - Typed Thin (Py)Torch Wrapper
 
 T3W is a lightweight framework for training PyTorch models written by Yuyao Huang during his PhD at Tongji University.
-- T3W is "typed". It leverages a stronger and static type compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
+- T3W is "typed". It leverages stronger and static typing compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
 - T3W is "thin". With the philosophy "less is more" in mind, it leverages a minimal codebase in a self-contained single python script that basically only depends on PyTorch to run. The plugin system under interface `ISideEffect` makes T3W not only thin, but also highly extensible.
 - T3W stands with "PyTorch".
 
 See the concise example [mnist_example.py](https://github.com/tjyuyao/t3w/blob/main/mnist_example.py).
 
 If you feel like using `t3w.py`, you can either
 
-- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the latter will install common side effects dependencies like `tqdm` etc. Note that the mnist example requires installing `t3w[common]`.
+- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the `[common]` tag will install dependencies for commonly used side effects (like `tqdm` etc), and `[all]` tag will install dependencies for all supported side effects. Note that the mnist example requires installing `t3w[common]`.
 - just download and integrate the [t3w.py](https://github.com/tjyuyao/t3w/blob/main/t3w.py) source file into your own project if you feel like freezing the version and/or ready to make some of your favorite hacks at low-level.
 
 Detailed documentation will come in the future.
```

### Comparing `t3w-0.1.0.post1/README.md` & `t3w-0.1.0.post2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # `t3w.py` - Typed Thin (Py)Torch Wrapper
 
 T3W is a lightweight framework for training PyTorch models written by Yuyao Huang during his PhD at Tongji University.
-- T3W is "typed". It leverages a stronger and static type compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
+- T3W is "typed". It leverages stronger and static typing compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
 - T3W is "thin". With the philosophy "less is more" in mind, it leverages a minimal codebase in a self-contained single python script that basically only depends on PyTorch to run. The plugin system under interface `ISideEffect` makes T3W not only thin, but also highly extensible.
 - T3W stands with "PyTorch".
 
 See the concise example [mnist_example.py](https://github.com/tjyuyao/t3w/blob/main/mnist_example.py).
 
 If you feel like using `t3w.py`, you can either
 
-- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the latter will install common side effects dependencies like `tqdm` etc. Note that the mnist example requires installing `t3w[common]`.
+- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the `[common]` tag will install dependencies for commonly used side effects (like `tqdm` etc), and `[all]` tag will install dependencies for all supported side effects. Note that the mnist example requires installing `t3w[common]`.
 - just download and integrate the [t3w.py](https://github.com/tjyuyao/t3w/blob/main/t3w.py) source file into your own project if you feel like freezing the version and/or ready to make some of your favorite hacks at low-level.
 
 Detailed documentation will come in the future.
```

### Comparing `t3w-0.1.0.post1/setup.py` & `t3w-0.1.0.post2/setup.py`

 * *Files identical despite different names*

### Comparing `t3w-0.1.0.post1/t3w.egg-info/PKG-INFO` & `t3w-0.1.0.post2/t3w.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: t3w
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Typed Thin PyTorch Wrapper
 Home-page: https://github.com/tjyuyao/t3w
 Author: Yuyao Huang
 Author-email: huangyuyao@outlook.com
 Description-Content-Type: text/markdown
 Provides-Extra: common
 Provides-Extra: all
 License-File: LICENSE
 
 # `t3w.py` - Typed Thin (Py)Torch Wrapper
 
 T3W is a lightweight framework for training PyTorch models written by Yuyao Huang during his PhD at Tongji University.
-- T3W is "typed". It leverages a stronger and static type compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
+- T3W is "typed". It leverages stronger and static typing compared to normal python code for clearer architecture and less bugs. The programming model is object-oriented. Users (you) are required to implement interfaces as subclasses and inject them as dependencies.
 - T3W is "thin". With the philosophy "less is more" in mind, it leverages a minimal codebase in a self-contained single python script that basically only depends on PyTorch to run. The plugin system under interface `ISideEffect` makes T3W not only thin, but also highly extensible.
 - T3W stands with "PyTorch".
 
 See the concise example [mnist_example.py](https://github.com/tjyuyao/t3w/blob/main/mnist_example.py).
 
 If you feel like using `t3w.py`, you can either
 
-- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the latter will install common side effects dependencies like `tqdm` etc. Note that the mnist example requires installing `t3w[common]`.
+- install it with `pip install t3w`, `pip install t3w[common]`, or `pip install t3w[all]`, where the `[common]` tag will install dependencies for commonly used side effects (like `tqdm` etc), and `[all]` tag will install dependencies for all supported side effects. Note that the mnist example requires installing `t3w[common]`.
 - just download and integrate the [t3w.py](https://github.com/tjyuyao/t3w/blob/main/t3w.py) source file into your own project if you feel like freezing the version and/or ready to make some of your favorite hacks at low-level.
 
 Detailed documentation will come in the future.
```

### Comparing `t3w-0.1.0.post1/t3w.py` & `t3w-0.1.0.post2/t3w.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Copyright (C) 2023 Yuyao Huang - All Rights Reserved
-You may use, distribute and modify this code under the
-terms of the Apache 2.0 license, which unfortunately won't be
-written for another century.
-You should have received a copy of the Apache 2.0 license with
-this file. If not, please write to: huangyuyao@outlook.com, or visit https://github.com/tjyuyao/t3w/blob/main/LICENSE:
+
+You may use, distribute and modify this code under the terms of the Apache 2.0
+license, which unfortunately won't be written for another century. You should
+have received a copy of the Apache 2.0 license with this file. If not, please
+write to: huangyuyao@outlook.com, or visit
+https://github.com/tjyuyao/t3w/blob/main/LICENSE:
 """
 
-__version__ = '0.1.0.post1'
+__version__ = '0.1.0.post2'
 
 import torch, gzip, random, numpy, os, math, weakref
 from typing import Any, Sequence, Generic, TypeVar, Optional, Mapping, Type, Hashable, Callable, Dict, Literal, Union, List
 from functools import wraps
 from glob import glob
 from torch.utils.data import DataLoader, Sampler, default_collate, DistributedSampler
 from torch import nn, Tensor
@@ -153,14 +154,15 @@
     def forward(self, mb: IMiniBatch) -> FloatScalarTensor:
         pass
 
 
 class ILoss(IDatumMetric):
     
     loss_reweight: float = 1.
+    higher_better: bool = False
 
 
 class LearningRate(IDatumMetric):
 
     def __init__(self, param_group=0) -> None:
         super().__init__()
         self.pg = param_group
```

