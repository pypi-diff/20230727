# Comparing `tmp/promptlabs-0.0.1.tar.gz` & `tmp/promptlabs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlabs-0.0.1.tar", last modified: Thu Jul 27 05:52:12 2023, max compression
+gzip compressed data, was "promptlabs-0.0.2.tar", last modified: Thu Jul 27 06:15:36 2023, max compression
```

## Comparing `promptlabs-0.0.1.tar` & `promptlabs-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 05:52:12.158431 promptlabs-0.0.1/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.1/LICENSE
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-27 05:52:12.154431 promptlabs-0.0.1/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.1/README.md
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 05:52:12.154431 promptlabs-0.0.1/promptlabs/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       74 2023-07-27 05:47:47.000000 promptlabs-0.0.1/promptlabs/__init__.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 05:52:12.154431 promptlabs-0.0.1/promptlabs/chain/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.1/promptlabs/chain/__init__.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1816 2023-07-27 05:28:35.000000 promptlabs-0.0.1/promptlabs/chain/base_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4611 2023-07-27 05:22:07.000000 promptlabs-0.0.1/promptlabs/chain/function_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     9607 2023-07-27 05:25:33.000000 promptlabs-0.0.1/promptlabs/chain/llm_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.1/promptlabs/client.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     5401 2023-07-27 05:21:53.000000 promptlabs-0.0.1/promptlabs/pipeline.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 05:52:12.154431 promptlabs-0.0.1/promptlabs.egg-info/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-27 05:52:12.000000 promptlabs-0.0.1/promptlabs.egg-info/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      387 2023-07-27 05:52:12.000000 promptlabs-0.0.1/promptlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-27 05:52:12.000000 promptlabs-0.0.1/promptlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-27 05:52:12.000000 promptlabs-0.0.1/promptlabs.egg-info/requires.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-27 05:52:12.000000 promptlabs-0.0.1/promptlabs.egg-info/top_level.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-27 05:52:12.158431 promptlabs-0.0.1/setup.cfg
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      526 2023-07-27 05:50:45.000000 promptlabs-0.0.1/setup.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:15:36.979111 promptlabs-0.0.2/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.2/LICENSE
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-27 06:15:36.979111 promptlabs-0.0.2/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.2/README.md
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:15:36.979111 promptlabs-0.0.2/promptlabs/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       74 2023-07-27 06:15:01.000000 promptlabs-0.0.2/promptlabs/__init__.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:15:36.979111 promptlabs-0.0.2/promptlabs/chain/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.2/promptlabs/chain/__init__.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1816 2023-07-27 05:28:35.000000 promptlabs-0.0.2/promptlabs/chain/base_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4570 2023-07-27 06:01:16.000000 promptlabs-0.0.2/promptlabs/chain/function_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     9607 2023-07-27 05:25:33.000000 promptlabs-0.0.2/promptlabs/chain/llm_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.2/promptlabs/client.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     5401 2023-07-27 05:21:53.000000 promptlabs-0.0.2/promptlabs/pipeline.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:15:36.979111 promptlabs-0.0.2/promptlabs.egg-info/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-27 06:15:36.000000 promptlabs-0.0.2/promptlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      387 2023-07-27 06:15:36.000000 promptlabs-0.0.2/promptlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-27 06:15:36.000000 promptlabs-0.0.2/promptlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-27 06:15:36.000000 promptlabs-0.0.2/promptlabs.egg-info/requires.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-27 06:15:36.000000 promptlabs-0.0.2/promptlabs.egg-info/top_level.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-27 06:15:36.979111 promptlabs-0.0.2/setup.cfg
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      526 2023-07-27 06:14:58.000000 promptlabs-0.0.2/setup.py
```

### Comparing `promptlabs-0.0.1/promptlabs/chain/base_chain.py` & `promptlabs-0.0.2/promptlabs/chain/base_chain.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.1/promptlabs/chain/function_chain.py` & `promptlabs-0.0.2/promptlabs/chain/function_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, Callable
 from abc import ABC, abstractmethod
 
 from pydantic import Extra, Field, root_validator, PrivateAttr 
 from promptlabs.chain.base_chain import Chain
 from promptlabs.scheme.template import ChainOutput, ChainLog
-from promptlabs.chain import FunctionChain
 
 class FunctionChain(Chain):
     
     _function: Callable = PrivateAttr(default=None)
     
-    def insert_function(self, function: Callable) -> FunctionChain:
+    def insert_function(self, function: Callable) -> 'FunctionChain':
         self._function = function
         return self
 
     def remove_function(self) -> None:
         self._function = None
         return
```

### Comparing `promptlabs-0.0.1/promptlabs/chain/llm_chain.py` & `promptlabs-0.0.2/promptlabs/chain/llm_chain.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.1/promptlabs/client.py` & `promptlabs-0.0.2/promptlabs/client.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.1/promptlabs/pipeline.py` & `promptlabs-0.0.2/promptlabs/pipeline.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.1/setup.py` & `promptlabs-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)
 """
 from setuptools import setup, find_packages
 
 setup(
     name="promptlabs",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     description="promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)",
     auther="weavel",
     install_requires=['openai', 'pydantic', 'requests'],
     python_requires='>=3.7.1',
     keywords=['weavel', 'prompt', 'llm', 'promptops', 'promptlabs', 'prompt engineering']
 )
```

