# Comparing `tmp/bittensor-config-0.0.0.tar.gz` & `tmp/bittensor-config-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-config-0.0.0.tar", last modified: Mon Jun 26 22:42:36 2023, max compression
+gzip compressed data, was "bittensor-config-0.0.1.tar", last modified: Wed Jul 26 22:59:26 2023, max compression
```

## Comparing `bittensor-config-0.0.0.tar` & `bittensor-config-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-26 22:42:36.796168 bittensor-config-0.0.0/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1653 2023-06-26 22:42:36.795996 bittensor-config-0.0.0/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      470 2023-06-26 22:02:34.000000 bittensor-config-0.0.0/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-26 22:42:36.794396 bittensor-config-0.0.0/bittensor_config/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8070 2023-06-26 22:00:48.000000 bittensor-config-0.0.0/bittensor_config/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4218 2023-06-26 22:00:48.000000 bittensor-config-0.0.0/bittensor_config/config_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-26 22:42:36.795428 bittensor-config-0.0.0/bittensor_config.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1653 2023-06-26 22:42:36.000000 bittensor-config-0.0.0/bittensor_config.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      292 2023-06-26 22:42:36.000000 bittensor-config-0.0.0/bittensor_config.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-06-26 22:42:36.000000 bittensor-config-0.0.0/bittensor_config.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       59 2023-06-26 22:42:36.000000 bittensor-config-0.0.0/bittensor_config.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-06-26 22:42:36.000000 bittensor-config-0.0.0/bittensor_config.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-06-26 22:42:36.796269 bittensor-config-0.0.0/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3589 2023-06-26 22:11:08.000000 bittensor-config-0.0.0/setup.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-26 22:42:36.795570 bittensor-config-0.0.0/tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3458 2023-06-26 22:01:37.000000 bittensor-config-0.0.0/tests/test.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:59:26.373654 bittensor-config-0.0.1/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:54.000000 bittensor-config-0.0.1/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1673 2023-07-26 22:59:26.373513 bittensor-config-0.0.1/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      468 2023-07-14 17:36:45.000000 bittensor-config-0.0.1/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:59:26.372629 bittensor-config-0.0.1/bittensor_config/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8070 2023-07-14 17:36:43.000000 bittensor-config-0.0.1/bittensor_config/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4218 2023-06-26 22:00:48.000000 bittensor-config-0.0.1/bittensor_config/config_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-26 22:59:26.373313 bittensor-config-0.0.1/bittensor_config.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1673 2023-07-26 22:59:26.000000 bittensor-config-0.0.1/bittensor_config.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      286 2023-07-26 22:59:26.000000 bittensor-config-0.0.1/bittensor_config.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-26 22:59:26.000000 bittensor-config-0.0.1/bittensor_config.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       71 2023-07-26 22:59:26.000000 bittensor-config-0.0.1/bittensor_config.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-26 22:59:26.000000 bittensor-config-0.0.1/bittensor_config.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-26 22:59:26.373700 bittensor-config-0.0.1/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3589 2023-06-26 22:11:08.000000 bittensor-config-0.0.1/setup.py
```

### Comparing `bittensor-config-0.0.0/PKG-INFO` & `bittensor-config-0.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-config
-Version: 0.0.0
+Version: 0.0.1
 Summary: BittensorConfig is a library for managing the configuration of the Bittensor Python API.
 Home-page: https://github.com/opentensor/bittensor-config
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -20,25 +20,24 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
-# BittensorConfig - v0.0.0
+# BittensorConfig - v0.0.1
 
 BittensorConfig is a library for managing the configuration of the [Bittensor Python API](https://github.com/opentensor/bittensor).
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-config/):
 ```bash
-pip install bittensor-config==0.0.0
+pip install bittensor-config==0.0.1
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-config
 cd bittensor-config
 pip install -e .
 ```
-
-
```

### Comparing `bittensor-config-0.0.0/bittensor_config/__init__.py` & `bittensor-config-0.0.1/bittensor_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 
 import os
 import sys
 import argparse
 from typing import List, Optional
 from copy import deepcopy
```

### Comparing `bittensor-config-0.0.0/bittensor_config/config_impl.py` & `bittensor-config-0.0.1/bittensor_config/config_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-config-0.0.0/bittensor_config.egg-info/PKG-INFO` & `bittensor-config-0.0.1/bittensor_config.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-config
-Version: 0.0.0
+Version: 0.0.1
 Summary: BittensorConfig is a library for managing the configuration of the Bittensor Python API.
 Home-page: https://github.com/opentensor/bittensor-config
 Author: bittensor.com
 Author-email: 
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -20,25 +20,24 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
 
-# BittensorConfig - v0.0.0
+# BittensorConfig - v0.0.1
 
 BittensorConfig is a library for managing the configuration of the [Bittensor Python API](https://github.com/opentensor/bittensor).
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-config/):
 ```bash
-pip install bittensor-config==0.0.0
+pip install bittensor-config==0.0.1
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-config
 cd bittensor-config
 pip install -e .
 ```
-
-
```

### Comparing `bittensor-config-0.0.0/setup.py` & `bittensor-config-0.0.1/setup.py`

 * *Files identical despite different names*

