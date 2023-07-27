# Comparing `tmp/ag_llama_api_s-0.0.4.tar.gz` & `tmp/ag_llama_api_s-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api_s-0.0.4.tar", last modified: Thu Jul 27 11:00:31 2023, max compression
+gzip compressed data, was "dist\ag_llama_api_s-0.0.5.tar", last modified: Thu Jul 27 11:04:06 2023, max compression
```

## Comparing `ag_llama_api_s-0.0.4.tar` & `ag_llama_api_s-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 11:00:31.525259 ag_llama_api_s-0.0.4/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:00:31.524263 ag_llama_api_s-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 11:00:31.502321 ag_llama_api_s-0.0.4/ag_llama_api_s/
--rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.4/ag_llama_api_s/__init__.py
--rw-rw-rw-   0        0        0     9331 2023-07-27 10:59:22.000000 ag_llama_api_s-0.0.4/ag_llama_api_s/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/ag_llama_api_s/choice.py
--rw-rw-rw-   0        0        0     5463 2023-07-27 10:54:26.000000 ag_llama_api_s-0.0.4/ag_llama_api_s/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/ag_llama_api_s/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:00:31.512293 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-27 11:00:31.000000 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      427 2023-07-27 11:00:31.000000 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 11:00:31.000000 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      297 2023-07-27 11:00:31.000000 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 11:00:31.000000 ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 11:00:31.525259 ag_llama_api_s-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:00:31.518307 ag_llama_api_s-0.0.4/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.4/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-27 11:00:31.522268 ag_llama_api_s-0.0.4/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.4/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:04:06.002427 ag_llama_api_s-0.0.5/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:04:06.001421 ag_llama_api_s-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.978482 ag_llama_api_s-0.0.5/ag_llama_api_s/
+-rw-rw-rw-   0        0        0     2187 2023-07-24 22:23:15.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/__init__.py
+-rw-rw-rw-   0        0        0     9118 2023-07-27 11:03:55.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/choice.py
+-rw-rw-rw-   0        0        0     5463 2023-07-27 10:54:26.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/ag_llama_api_s/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.989454 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      297 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-27 11:04:05.000000 ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 11:04:06.003415 ag_llama_api_s-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-07-27 10:19:00.000000 ag_llama_api_s-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.994440 ag_llama_api_s-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api_s-0.0.5/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-27 11:04:05.999425 ag_llama_api_s-0.0.5/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api_s-0.0.5/utils/render.py
```

### Comparing `ag_llama_api_s-0.0.4/PKG-INFO` & `ag_llama_api_s-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api_s
-Version: 0.0.4
+Version: 0.0.5
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s/__init__.py` & `ag_llama_api_s-0.0.5/ag_llama_api_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s/__main__.py` & `ag_llama_api_s-0.0.5/ag_llama_api_s/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,21 +236,16 @@
     logger.error(f"{error.code} {error.description}")
     return jsonify(error={"message": error.description}), error.code
 
 def run_localy(ip,port,model,in8bit=False):
     global stream_model, keep_running_localy
     stream_model = load_model(
         name_or_path=model,
-        revision=MODEL_REVISION,
-        cache_dir=MODEL_CACHE_DIR,
         load_in_8bit=in8bit,
         load_in_4bit=False,
-        local_files_only=MODEL_LOCAL_FILES_ONLY,
-        trust_remote_code=MODEL_TRUST_REMOTE_CODE,
-        half_precision=MODEL_HALF_PRECISION,
     )
     while keep_running_localy:
         try:
             logger.info(f"Starting API...")
             logger.info(f"Start listening on {HOST}:{PORT}")
             waitress.serve(
                 app,
```

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s/choice.py` & `ag_llama_api_s-0.0.5/ag_llama_api_s/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s/model.py` & `ag_llama_api_s-0.0.5/ag_llama_api_s/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s/tokenizer.py` & `ag_llama_api_s-0.0.5/ag_llama_api_s/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/ag_llama_api_s.egg-info/PKG-INFO` & `ag_llama_api_s-0.0.5/ag_llama_api_s.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api-s
-Version: 0.0.4
+Version: 0.0.5
 Summary: ag_llama_api_s Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api_s-0.0.4/setup.py` & `ag_llama_api_s-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/tests/test_choice.py` & `ag_llama_api_s-0.0.5/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/tests/test_model.py` & `ag_llama_api_s-0.0.5/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/tests/test_tokenizer.py` & `ag_llama_api_s-0.0.5/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/utils/download.py` & `ag_llama_api_s-0.0.5/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api_s-0.0.4/utils/render.py` & `ag_llama_api_s-0.0.5/utils/render.py`

 * *Files identical despite different names*

