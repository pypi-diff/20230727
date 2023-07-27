# Comparing `tmp/torchaug-0.2.0.tar.gz` & `tmp/torchaug-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchaug-0.2.0.tar", last modified: Wed Jul 26 22:50:00 2023, max compression
+gzip compressed data, was "torchaug-0.2.1.tar", last modified: Thu Jul 27 17:59:15 2023, max compression
```

## Comparing `torchaug-0.2.0.tar` & `torchaug-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:50:00.467944 torchaug-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-07-26 22:49:50.000000 torchaug-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-26 22:50:00.467944 torchaug-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-26 22:49:50.000000 torchaug-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-26 22:49:50.000000 torchaug-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 22:49:50.000000 torchaug-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:50:00.467944 torchaug-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:50:00.467944 torchaug-0.2.0/torchaug/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 22:49:50.000000 torchaug-0.2.0/torchaug/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:50:00.467944 torchaug-0.2.0/torchaug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-26 22:50:00.000000 torchaug-0.2.0/torchaug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-26 22:50:00.000000 torchaug-0.2.0/torchaug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:50:00.000000 torchaug-0.2.0/torchaug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 22:50:00.000000 torchaug-0.2.0/torchaug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 22:50:00.000000 torchaug-0.2.0/torchaug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    21777 2023-07-27 17:59:05.000000 torchaug-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-27 17:59:15.460238 torchaug-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-27 17:59:05.000000 torchaug-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-27 17:59:05.000000 torchaug-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 17:59:05.000000 torchaug-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:59:15.460238 torchaug-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/torchaug/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 17:59:05.000000 torchaug-0.2.1/torchaug/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:59:15.460238 torchaug-0.2.1/torchaug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 17:59:15.000000 torchaug-0.2.1/torchaug.egg-info/top_level.txt
```

### Comparing `torchaug-0.2.0/LICENSE` & `torchaug-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchaug-0.2.0/PKG-INFO` & `torchaug-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.2.0
+Version: 0.2.1
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@hotmail.fr>
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -52,26 +52,23 @@
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
 See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
 
 ## How to use
 
-0. Install a Pytorch >= 2.0 environment and Python >= 3.8.
+0. Install a Pytorch >= 2.0 environment.
 
-1. Clone the repo.
-
-2. Install Torchaug
+1. Install Torchaug.
 
 ```bash
-cd torchaug
-pip3 install .
+pip3 install torchaug
 ```
 
-3. Import data augmentations just as Torchvision
+2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
 
 transform = RandomColorJitter(...)
 batch_transform = BatchRandomColorJitter(...)
```

### Comparing `torchaug-0.2.0/README.md` & `torchaug-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,26 +20,23 @@
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
 See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
 
 ## How to use
 
-0. Install a Pytorch >= 2.0 environment and Python >= 3.8.
+0. Install a Pytorch >= 2.0 environment.
 
-1. Clone the repo.
-
-2. Install Torchaug
+1. Install Torchaug.
 
 ```bash
-cd torchaug
-pip3 install .
+pip3 install torchaug
 ```
 
-3. Import data augmentations just as Torchvision
+2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
 
 transform = RandomColorJitter(...)
 batch_transform = BatchRandomColorJitter(...)
```

### Comparing `torchaug-0.2.0/pyproject.toml` & `torchaug-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchaug-0.2.0/torchaug.egg-info/PKG-INFO` & `torchaug-0.2.1/torchaug.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchaug
-Version: 0.2.0
+Version: 0.2.1
 Summary: Torchvision Complementary tool to perform batch and GPU data augmentations.
 Author-email: Julien Denize <julien.denize@hotmail.fr>
 Project-URL: Homepage, https://github.com/juliendenize/torchaug
 Project-URL: Bug Tracker, https://github.com/juliendenize/torchaug/issues
 Project-URL: Download, https://github.com/juliendenize/torchaug
 Project-URL: Source Code, https://github.com/juliendenize/torchaug
 Keywords: computer vision,deep learning,pytorch
@@ -52,26 +52,23 @@
 
 To be sure to retrieve the same data augmentations as Torchvision, it has been tested on each of its augmentations.
 
 See [here](augmentations.md) the implemented data augmentations and [here](speed_comparison.md) the speed comparison with Torchvision.
 
 ## How to use
 
-0. Install a Pytorch >= 2.0 environment and Python >= 3.8.
+0. Install a Pytorch >= 2.0 environment.
 
-1. Clone the repo.
-
-2. Install Torchaug
+1. Install Torchaug.
 
 ```bash
-cd torchaug
-pip3 install .
+pip3 install torchaug
 ```
 
-3. Import data augmentations just as Torchvision
+2. Import data augmentations either from `torchaug.transforms` or `torchaug.batch_transforms` packages.
 
 ```python
 from torchaug.transforms import RandomColorJitter
 from torchaug.batch_transforms import BatchRandomColorJitter
 
 transform = RandomColorJitter(...)
 batch_transform = BatchRandomColorJitter(...)
```

