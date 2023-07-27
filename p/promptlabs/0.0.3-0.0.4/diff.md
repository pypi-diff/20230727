# Comparing `tmp/promptlabs-0.0.3.tar.gz` & `tmp/promptlabs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlabs-0.0.3.tar", last modified: Thu Jul 27 06:25:58 2023, max compression
+gzip compressed data, was "promptlabs-0.0.4.tar", last modified: Thu Jul 27 08:52:30 2023, max compression
```

## Comparing `promptlabs-0.0.3.tar` & `promptlabs-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:25:58.757217 promptlabs-0.0.3/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.3/LICENSE
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 06:25:58.757217 promptlabs-0.0.3/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.3/README.md
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:25:58.757217 promptlabs-0.0.3/promptlabs/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       74 2023-07-27 06:25:50.000000 promptlabs-0.0.3/promptlabs/__init__.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:25:58.757217 promptlabs-0.0.3/promptlabs/chain/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.3/promptlabs/chain/__init__.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1816 2023-07-27 05:28:35.000000 promptlabs-0.0.3/promptlabs/chain/base_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4570 2023-07-27 06:01:16.000000 promptlabs-0.0.3/promptlabs/chain/function_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     9607 2023-07-27 05:25:33.000000 promptlabs-0.0.3/promptlabs/chain/llm_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.3/promptlabs/client.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     5401 2023-07-27 05:21:53.000000 promptlabs-0.0.3/promptlabs/pipeline.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:25:58.757217 promptlabs-0.0.3/promptlabs/scheme/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     3660 2023-07-26 10:58:35.000000 promptlabs-0.0.3/promptlabs/scheme/llm.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.3/promptlabs/scheme/template.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 06:25:58.757217 promptlabs-0.0.3/promptlabs.egg-info/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 06:25:58.000000 promptlabs-0.0.3/promptlabs.egg-info/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-27 06:25:58.000000 promptlabs-0.0.3/promptlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-27 06:25:58.000000 promptlabs-0.0.3/promptlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-27 06:25:58.000000 promptlabs-0.0.3/promptlabs.egg-info/requires.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-27 06:25:58.000000 promptlabs-0.0.3/promptlabs.egg-info/top_level.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-27 06:25:58.757217 promptlabs-0.0.3/setup.cfg
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-27 06:25:54.000000 promptlabs-0.0.3/setup.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.069518 promptlabs-0.0.4/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.4/LICENSE
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 08:52:30.065518 promptlabs-0.0.4/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.4/README.md
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       75 2023-07-27 08:51:57.000000 promptlabs-0.0.4/promptlabs/__init__.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/chain/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.4/promptlabs/chain/__init__.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1816 2023-07-27 05:28:35.000000 promptlabs-0.0.4/promptlabs/chain/base_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4455 2023-07-27 08:50:31.000000 promptlabs-0.0.4/promptlabs/chain/function_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     9908 2023-07-27 08:45:47.000000 promptlabs-0.0.4/promptlabs/chain/llm_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.4/promptlabs/client.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     5401 2023-07-27 05:21:53.000000 promptlabs-0.0.4/promptlabs/pipeline.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs/scheme/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     3660 2023-07-26 10:58:35.000000 promptlabs-0.0.4/promptlabs/scheme/llm.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.4/promptlabs/scheme/template.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-27 08:52:30.065518 promptlabs-0.0.4/promptlabs.egg-info/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/requires.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-27 08:52:30.000000 promptlabs-0.0.4/promptlabs.egg-info/top_level.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-27 08:52:30.069518 promptlabs-0.0.4/setup.cfg
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-27 08:51:53.000000 promptlabs-0.0.4/setup.py
```

### Comparing `promptlabs-0.0.3/promptlabs/chain/base_chain.py` & `promptlabs-0.0.4/promptlabs/chain/base_chain.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.3/promptlabs/chain/function_chain.py` & `promptlabs-0.0.4/promptlabs/chain/function_chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 
 from pydantic import Extra, Field, root_validator, PrivateAttr 
 from promptlabs.chain.base_chain import Chain
 from promptlabs.scheme.template import ChainOutput, ChainLog
 
 class FunctionChain(Chain):
     
-    _function: Callable = PrivateAttr(default=None)
+    _function: Callable
     
-    def insert_function(self, function: Callable) -> 'FunctionChain':
+    def with_function(self, function: Callable) -> 'FunctionChain':
         self._function = function
         return self
-
-    def remove_function(self) -> None:
-        self._function = None
-        return
     
     @root_validator(pre=True)
     def set_function(cls, values: Dict) -> Dict:
         if 'function' in values['config']:
             function = values['config']['function']
         else:
             function = None
```

### Comparing `promptlabs-0.0.3/promptlabs/chain/llm_chain.py` & `promptlabs-0.0.4/promptlabs/chain/llm_chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 from promptlabs.scheme.template import ChainOutput, ChainLog
 from promptlabs.scheme.llm import ChatOpenAI, BaseLLM
 
 class LLMChain(Chain):
 
     llm : BaseLLM
     
+    def with_llm(self, llm: BaseLLM) -> 'LLMChain':
+        self.llm = llm
+        return self
+    
+    def insert_llm(self, llm: BaseLLM) -> None:
+        self.llm = llm
+        return
+    
     @root_validator(pre=True)
     def set_llm(cls, values: Dict) -> Dict:
         if "llm_function" not in values['config']:
             chat_openai_config = {
                 "model_name": values['config']['model_name'],
                 "temperature": values['config'].get('temperature', 0.7),
                 "max_tokens": values['config'].get('max_tokens')
@@ -189,14 +197,19 @@
         else:
             return (
                 ChainOutput(chain_success=True, output_variables=llm_result['parsed_output']),
                 ChainLog(logs={"raw_output": llm_result['raw_output']})
             )
 
 class LLMRegexChain(LLMChain):
+    
+    def with_llm(self, llm: BaseLLM) -> 'LLMRegexChain':
+        self.llm = llm
+        return self
+    
     def _call_llm_submodule(
         self,
         inputs: Dict[str, Any]
     ) -> Dict[str, Any]:
         max_retry = 3
         retry_count = 0
         raw_output = None
```

### Comparing `promptlabs-0.0.3/promptlabs/client.py` & `promptlabs-0.0.4/promptlabs/client.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.3/promptlabs/pipeline.py` & `promptlabs-0.0.4/promptlabs/pipeline.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.3/promptlabs/scheme/llm.py` & `promptlabs-0.0.4/promptlabs/scheme/llm.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.3/promptlabs/scheme/template.py` & `promptlabs-0.0.4/promptlabs/scheme/template.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.3/setup.py` & `promptlabs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)
 """
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="promptlabs",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_namespace_packages(),
     description="promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)",
     auther="weavel",
     install_requires=['openai', 'pydantic', 'requests'],
     python_requires='>=3.7.1',
     keywords=['weavel', 'prompt', 'llm', 'promptops', 'promptlabs', 'prompt engineering']
 )
```

