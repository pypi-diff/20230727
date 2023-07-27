# Comparing `tmp/ag_llama_api_s-0.0.7.tar.gz` & `tmp/ag_llama_api_s-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api_s-0.0.7.tar", last modified: Thu Jul 27 11:27:00 2023, max compression
+gzip compressed data, was "dist\ag_llama_api_s-0.0.8.tar", last modified: Thu Jul 27 11:43:12 2023, max compression
```

## Comparing `ag_llama_api_s-0.0.7.tar` & `ag_llama_api_s-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.887144 ag_llama_api_s-0.0.7/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:27:00.885150 ag_llama_api_s-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.864206 ag_llama_api_s-0.0.7/ag_llama_api_s/
--rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/__init__.py
--rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/choice.py
--rw-rw-rw-   0        0        0     5192 2023-07-27 11:26:53.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/ag_llama_api_s/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.874178 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 11:27:00.000000 ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:27:00.887144 ag_llama_api_s-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.879166 ag_llama_api_s-0.0.7/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.7/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:27:00.883154 ag_llama_api_s-0.0.7/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.7/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.913389 ag_llama_api_s-0.0.8/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:43:12.912392 ag_llama_api_s-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.891454 ag_llama_api_s-0.0.8/ag_llama_api_s/
+-rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/__init__.py
+-rw-rw-rw-   0        0        0     8785 2023-07-27 11:11:47.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/choice.py
+-rw-rw-rw-   0        0        0     5270 2023-07-27 11:42:39.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/ag_llama_api_s/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.901427 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:43:12.000000 ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:43:12.914386 ag_llama_api_s-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.906407 ag_llama_api_s-0.0.8/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.8/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:43:12.910396 ag_llama_api_s-0.0.8/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.8/utils/render.py
```

### Comparing `ag_llama_api_s-0.0.7/PKG-INFO` & `ag_llama_api_s-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api_s
-Version: 0.0.7
+Version: 0.0.8
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s/__init__.py` & `ag_llama_api_s-0.0.8/ag_llama_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s/__main__.py` & `ag_llama_api_s-0.0.8/ag_llama_api_s/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s/choice.py` & `ag_llama_api_s-0.0.8/ag_llama_api_s/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s/model.py` & `ag_llama_api_s-0.0.8/ag_llama_api_s/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         self,
         prompt,
         max_tokens=16,
         temperature=1.0,
         top_p=1.0,
     ):
         self.wait_and_clear_gpu()
+        logger.info(f"Got number of tokens: {self.get_tokens_count(prompt)}")
         """Create a completion stream for the provided prompt."""
         logger.info(f"Generating pipeline for {self.path}")
         pipe = pipeline(
                 "text-generation",
                 model=self.model,
                 tokenizer=self.tokenizer,
                 max_length=max_tokens,
```

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s/tokenizer.py` & `ag_llama_api_s-0.0.8/ag_llama_api_s/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/ag_llama_api_s.egg-info/PKG-INFO` & `ag_llama_api_s-0.0.8/ag_llama_api_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api-s
-Version: 0.0.7
+Version: 0.0.8
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.7/setup.py` & `ag_llama_api_s-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/tests/test_choice.py` & `ag_llama_api_s-0.0.8/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/tests/test_model.py` & `ag_llama_api_s-0.0.8/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/tests/test_tokenizer.py` & `ag_llama_api_s-0.0.8/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/utils/download.py` & `ag_llama_api_s-0.0.8/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.7/utils/render.py` & `ag_llama_api_s-0.0.8/utils/render.py`

 * *Files identical despite different names*

