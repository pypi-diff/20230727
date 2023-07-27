# Comparing `tmp/ag_llama_api_s-0.0.5.tar.gz` & `tmp/ag_llama_api_s-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api_s-0.0.5.tar", last modified: Thu Jul 27 11:04:06 2023, max compression
+gzip compressed data, was "dist\ag_llama_api_s-0.0.6.tar", last modified: Thu Jul 27 11:07:07 2023, max compression
```

## Comparing `ag_llama_api_s-0.0.5.tar` & `ag_llama_api_s-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:04:06.002427 ag_llama_api_s-0.0.5/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:04:06.001421 ag_llama_api_s-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.978482 ag_llama_api_s-0.0.5/ag_llama_api_s/
--rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/__init__.py
--rw-rw-rw-   0        0        0     9118 2023-07-27 11:03:55.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/choice.py
--rw-rw-rw-   0        0        0     5463 2023-07-27 10:54:26.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.989454 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:04:06.003415 ag_llama_api_s-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.994440 ag_llama_api_s-0.0.5/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.5/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.999425 ag_llama_api_s-0.0.5/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.358420 ag_llama_api_s-0.0.6/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:07:07.357422 ag_llama_api_s-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.336476 ag_llama_api_s-0.0.6/ag_llama_api_s/
+-rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/__init__.py
+-rw-rw-rw-   0        0        0     8980 2023-07-27 11:07:02.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/choice.py
+-rw-rw-rw-   0        0        0     5463 2023-07-27 11:05:34.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/ag_llama_api_s/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.345453 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:07:07.000000 ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:07:07.358420 ag_llama_api_s-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.350440 ag_llama_api_s-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.6/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:07:07.354430 ag_llama_api_s-0.0.6/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.6/utils/render.py
```

### Comparing `ag_llama_api_s-0.0.5/PKG-INFO` & `ag_llama_api_s-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api_s
-Version: 0.0.5
+Version: 0.0.6
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s/__init__.py` & `ag_llama_api_s-0.0.6/ag_llama_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s/__main__.py` & `ag_llama_api_s-0.0.6/ag_llama_api_s/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,22 +49,18 @@
 keep_running_localy = True
 # Load the language model to be served.
 stream_model = None
 def load_stream_model():
     global stream_model
     stream_model = load_model(
         name_or_path=MODEL,
-        revision=MODEL_REVISION,
-        cache_dir=MODEL_CACHE_DIR,
         load_in_8bit=MODEL_LOAD_IN_8BIT,
         load_in_4bit=MODEL_LOAD_IN_4BIT,
-        local_files_only=MODEL_LOCAL_FILES_ONLY,
-        trust_remote_code=MODEL_TRUST_REMOTE_CODE,
-        half_precision=MODEL_HALF_PRECISION,
     )
+    logger.info(f"Model loaded")
 
 # Create and configure application.
 app = Flask(__name__)
 app.json.ensure_ascii = False
 app.json.sort_keys = False
 app.json.compact = True
 app.url_map.strict_slashes = False
@@ -277,8 +273,9 @@
         ident=SERVER_IDENTITY,
         connection_limit=SERVER_CONNECTION_LIMIT,
         channel_timeout=SERVER_CHANNEL_TIMEOUT,
     )
 
 
 if __name__ == "__main__":
+    logger.info(f"Running from __main__")
     main()
```

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s/choice.py` & `ag_llama_api_s-0.0.6/ag_llama_api_s/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s/model.py` & `ag_llama_api_s-0.0.6/ag_llama_api_s/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s/tokenizer.py` & `ag_llama_api_s-0.0.6/ag_llama_api_s/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/PKG-INFO` & `ag_llama_api_s-0.0.6/ag_llama_api_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api-s
-Version: 0.0.5
+Version: 0.0.6
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.5/setup.py` & `ag_llama_api_s-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/tests/test_choice.py` & `ag_llama_api_s-0.0.6/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/tests/test_model.py` & `ag_llama_api_s-0.0.6/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/tests/test_tokenizer.py` & `ag_llama_api_s-0.0.6/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/utils/download.py` & `ag_llama_api_s-0.0.6/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.5/utils/render.py` & `ag_llama_api_s-0.0.6/utils/render.py`

 * *Files identical despite different names*

