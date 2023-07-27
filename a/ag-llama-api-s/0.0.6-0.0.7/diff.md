# Comparing `tmp/ag_llama_api_s-0.0.6.tar.gz` & `tmp/ag_llama_api_s-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api_s-0.0.6.tar", last modified: Thu Jul 27 11:07:07 2023, max compression
+gzip compressed data, was "dist\ag_llama_api_s-0.0.7.tar", last modified: Thu Jul 27 11:27:00 2023, max compression
```

## Comparing `ag_llama_api_s-0.0.6.tar` & `ag_llama_api_s-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.358420 ag_llama_api_s-0.0.6/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:07:07.357422 ag_llama_api_s-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.336476 ag_llama_api_s-0.0.6/ag_llama_api_s/
--rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/__init__.py
--rw-rw-rw-   0        0        0     8980 2023-07-27 11:07:02.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/choice.py
--rw-rw-rw-   0        0        0     5463 2023-07-27 11:05:34.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.345453 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:07:07.358420 ag_llama_api_s-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.350440 ag_llama_api_s-0.0.6/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.6/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.354430 ag_llama_api_s-0.0.6/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.887144 ag_llama_api_s-0.0.7/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:27:00.885150 ag_llama_api_s-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.864206 ag_llama_api_s-0.0.7/ag_llama_api_s/
+-rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/__init__.py
+-rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/choice.py
+-rw-rw-rw-   0        0        0     5192 2023-07-27 11:26:53.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.874178 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:27:00.887144 ag_llama_api_s-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.879166 ag_llama_api_s-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.7/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.883154 ag_llama_api_s-0.0.7/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/utils/render.py
```

### Comparing `ag_llama_api_s-0.0.6/PKG-INFO` & `ag_llama_api_s-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api_s
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s/__init__.py` & `ag_llama_api_s-0.0.7/ag_llama_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s/__main__.py` & `ag_llama_api_s-0.0.7/ag_llama_api_s/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,14 @@
                 options[key] = prompts[0]
             elif len(prompts) > 1:
                 abort(400, description="only one prompt is supported")
 
     return options
 
 
-@app.route("/")
-def render_playground():
-    """Render model playground."""
-    if SERVER_NO_PLAYGROUND:
-        abort(404)
-    return render_template("playground.html", model=SERVER_MODEL_NAME)
 
 
 @app.route("/v1/models")
 def list_models():
     """List the currently available models."""
     info = {"id": SERVER_MODEL_NAME, "object": "model"}
     return jsonify(data=[info], object="list")
```

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s/choice.py` & `ag_llama_api_s-0.0.7/ag_llama_api_s/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s/model.py` & `ag_llama_api_s-0.0.7/ag_llama_api_s/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 """
 A text generation model with stream decoding.
 """
 import gc
-import copy
 import pynvml
 import torch
 from sentencepiece import SentencePieceProcessor
-from transformers import (
-    AutoModelForCausalLM,
-    AutoModelForSeq2SeqLM,
-    AutoTokenizer,
-    LogitsProcessorList,
-    MinNewTokensLengthLogitsProcessor,
-    TemperatureLogitsWarper,
-    TopPLogitsWarper,
-)
+
 from transformers import LlamaForCausalLM, LlamaTokenizer, pipeline
 from loguru import logger
-from .choice import map_choice
-from .tokenizer import StreamTokenizer
+
 
 
 class StreamModel:
     """StreamModel wraps around a language model to provide stream decoding."""
 
     def __init__(self, model, tokenizer,**kwargs):
         super().__init__()
@@ -36,15 +26,15 @@
     def __call__(
         self,
         prompt,
         max_tokens=16,
         temperature=1.0,
         top_p=1.0,
     ):
-        
+        self.wait_and_clear_gpu()
         """Create a completion stream for the provided prompt."""
         logger.info(f"Generating pipeline for {self.path}")
         pipe = pipeline(
                 "text-generation",
                 model=self.model,
                 tokenizer=self.tokenizer,
                 max_length=max_tokens,
```

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s/tokenizer.py` & `ag_llama_api_s-0.0.7/ag_llama_api_s/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/PKG-INFO` & `ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api-s
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.6/setup.py` & `ag_llama_api_s-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/tests/test_choice.py` & `ag_llama_api_s-0.0.7/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/tests/test_model.py` & `ag_llama_api_s-0.0.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/tests/test_tokenizer.py` & `ag_llama_api_s-0.0.7/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/utils/download.py` & `ag_llama_api_s-0.0.7/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.6/utils/render.py` & `ag_llama_api_s-0.0.7/utils/render.py`

 * *Files identical despite different names*

