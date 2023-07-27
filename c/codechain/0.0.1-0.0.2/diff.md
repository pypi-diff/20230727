# Comparing `tmp/codechain-0.0.1.tar.gz` & `tmp/codechain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codechain-0.0.1.tar", last modified: Thu Jul 27 12:16:28 2023, max compression
+gzip compressed data, was "codechain-0.0.2.tar", last modified: Thu Jul 27 12:28:08 2023, max compression
```

## Comparing `codechain-0.0.1.tar` & `codechain-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:16:28.163189 codechain-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:16:28.162933 codechain-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1011 2023-07-27 11:41:19.000000 codechain-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:16:28.160450 codechain-0.0.1/codechain/
--rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.1/codechain/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      861 2023-07-27 01:45:31.000000 codechain-0.0.1/codechain/evaluation.py
--rw-r--r--   0 james      (501) staff       (20)     3415 2023-07-27 11:22:00.000000 codechain-0.0.1/codechain/generation.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:16:28.162482 codechain-0.0.1/codechain.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:16:28.000000 codechain-0.0.1/codechain.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      252 2023-07-27 12:16:28.000000 codechain-0.0.1/codechain.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-07-27 12:16:28.000000 codechain-0.0.1/codechain.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:16:28.000000 codechain-0.0.1/codechain.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:16:28.000000 codechain-0.0.1/codechain.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-07-27 12:16:28.163401 codechain-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1066 2023-07-27 12:15:29.000000 codechain-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:28:08.389360 codechain-0.0.2/
+-rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:28:08.389226 codechain-0.0.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1011 2023-07-27 11:41:19.000000 codechain-0.0.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:28:08.388263 codechain-0.0.2/codechain/
+-rw-r--r--   0 james      (501) staff       (20)       69 2023-07-27 01:45:29.000000 codechain-0.0.2/codechain/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      861 2023-07-27 01:45:31.000000 codechain-0.0.2/codechain/evaluation.py
+-rw-r--r--   0 james      (501) staff       (20)     3407 2023-07-27 12:25:27.000000 codechain-0.0.2/codechain/generation.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-27 12:28:08.389053 codechain-0.0.2/codechain.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     1587 2023-07-27 12:28:08.000000 codechain-0.0.2/codechain.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      252 2023-07-27 12:28:08.000000 codechain-0.0.2/codechain.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-27 12:28:08.000000 codechain-0.0.2/codechain.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:28:08.000000 codechain-0.0.2/codechain.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       10 2023-07-27 12:28:08.000000 codechain-0.0.2/codechain.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-27 12:28:08.389394 codechain-0.0.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1066 2023-07-27 12:26:33.000000 codechain-0.0.2/setup.py
```

### Comparing `codechain-0.0.1/PKG-INFO` & `codechain-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `codechain-0.0.1/README.md` & `codechain-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `codechain-0.0.1/codechain/evaluation.py` & `codechain-0.0.2/codechain/evaluation.py`

 * *Files identical despite different names*

### Comparing `codechain-0.0.1/codechain/generation.py` & `codechain-0.0.2/codechain/generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,9 +92,9 @@
        CompleteCodeChain.from_instruction(instruction=instruction, llm=llm)
     )
   
   @classmethod
   def from_llm(cls, llm: BaseLanguageModel) -> "HumanEvalChain":
 
     return cls.from_llm(
-        CompleteCodeChain.from_instruction(llm=llm)
+        CompleteCodeChain.from_llm(llm=llm)
     )
```

### Comparing `codechain-0.0.1/codechain.egg-info/PKG-INFO` & `codechain-0.0.2/codechain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codechain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Code generation with LLMs
 Author: James Murdza
 Author-email: <james@jamesmurdza.com>
 Project-URL: Source, https://github.com/jamesmurdza/codechain
 Keywords: python,llms,codegen,code generation
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `codechain-0.0.1/setup.py` & `codechain-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Code generation with LLMs'
 
 # Setting up
 setup(
     name="codechain",
     version=VERSION,
     author="James Murdza",
```

