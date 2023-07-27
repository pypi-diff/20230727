# Comparing `tmp/operatorio-0.1.7.tar.gz` & `tmp/operatorio-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.1.7.tar", last modified: Fri Jul 21 19:18:31 2023, max compression
+gzip compressed data, was "operatorio-0.1.8.tar", last modified: Thu Jul 27 19:52:55 2023, max compression
```

## Comparing `operatorio-0.1.7.tar` & `operatorio-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.873286 operatorio-0.1.7/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:18:31.873025 operatorio-0.1.7/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.871976 operatorio-0.1.7/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.7/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     1962 2023-07-21 19:17:57.000000 operatorio-0.1.7/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-21 19:18:31.872789 operatorio-0.1.7/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-07-21 19:18:31.000000 operatorio-0.1.7/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-07-21 19:18:31.873333 operatorio-0.1.7/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-07-21 19:18:04.000000 operatorio-0.1.7/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.485983 operatorio-0.1.8/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-27 19:52:55.485751 operatorio-0.1.8/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.484546 operatorio-0.1.8/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.1.8/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     1914 2023-07-27 19:51:26.000000 operatorio-0.1.8/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-07-27 19:52:55.485506 operatorio-0.1.8/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-07-27 19:52:55.000000 operatorio-0.1.8/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-07-27 19:52:55.486059 operatorio-0.1.8/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-07-27 19:52:44.000000 operatorio-0.1.8/setup.py
```

### Comparing `operatorio-0.1.7/operatorio/main.py` & `operatorio-0.1.8/operatorio/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from dataclasses import dataclass, asdict
 from enum import Enum
 from typing import List, Union, Optional
 from requests.models import PreparedRequest
 
 # Models
 class EntityType(Enum):
-    wallet = "wallet"
     identity = "identity"
-    contract = "contract"
     nft = "nft"
     token = "token"
 
 @dataclass
 class Entity:
     address: str
     description: str
```

### Comparing `operatorio-0.1.7/setup.py` & `operatorio-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.1.7",
+    version="0.1.8",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

