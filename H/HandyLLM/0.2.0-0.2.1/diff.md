# Comparing `tmp/HandyLLM-0.2.0.tar.gz` & `tmp/HandyLLM-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.2.0.tar", last modified: Thu Jul 27 03:54:14 2023, max compression
+gzip compressed data, was "HandyLLM-0.2.1.tar", last modified: Thu Jul 27 13:37:04 2023, max compression
```

## Comparing `HandyLLM-0.2.0.tar` & `HandyLLM-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 03:54:14.000000 HandyLLM-0.2.0/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/src/handyllm/prompt_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:54:14.178492 HandyLLM-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 03:54:04.000000 HandyLLM-0.2.0/tests/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 13:37:04.000000 HandyLLM-0.2.1/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10156 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/src/handyllm/prompt_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:37:04.198620 HandyLLM-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-27 13:36:54.000000 HandyLLM-0.2.1/tests/test_stream.py
```

### Comparing `HandyLLM-0.2.0/PKG-INFO` & `HandyLLM-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.2.0
+Version: 0.2.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.2.0/README.md` & `HandyLLM-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.0/pyproject.toml` & `HandyLLM-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `HandyLLM-0.2.0/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.2.1/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.2.0
+Version: 0.2.1
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.2.0/src/handyllm/endpoint_manager.py` & `HandyLLM-0.2.1/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.0/src/handyllm/openai_api.py` & `HandyLLM-0.2.1/src/handyllm/openai_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,52 +54,47 @@
         headers = {
             'Authorization': 'Bearer ' + api_key,
             'Content-Type': 'application/json'
             }
         if organization is not None:
             headers['OpenAI-Organization'] = organization
         
+        stream = kwargs.get('stream', False)
         response = requests.post(
             url, 
             headers=headers, 
             # data=json.dumps(request_data),
             json=request_data,
-            timeout=timeout
+            stream=stream,
+            timeout=timeout,
             )
         if response.status_code != 200:
             # report both status code and error message
             try:
                 message = response.json()['error']['message']
             except:
                 message = response.text
             err_msg = f"OpenAI API error ({url} {response.status_code} {response.reason}): {message}"
             module_logger.error(err_msg)
             raise Exception(err_msg)
 
-        stream = kwargs.get('stream', False)
         if stream:
             return OpenAIAPI._gen_stream_response(response)
         else:
             return response.json()
 
     @staticmethod
     def _gen_stream_response(response):
-        data_buffer = ''
-        for chunk in response.iter_content(decode_unicode=True):
-            data_buffer += chunk
-            while '\n' in data_buffer:  # when '\n' is in the buffer, there is a complete message to process
-                line, data_buffer = data_buffer.split('\n', 1)
-                line = line.strip()
-                if line.startswith('data:'):
-                    line = line[len('data:'):].strip()
-                    if line == '[DONE]':  # end the function when '[DONE]' message is received
-                        return
-                    else:
-                        data = json.loads(line)
-                        yield data
+        for byte_line in response.iter_lines():  # do not auto decode
+            if byte_line:
+                if byte_line.strip() == b"data: [DONE]":
+                    return
+                if byte_line.startswith(b"data: "):
+                    line = byte_line[len(b"data: "):].decode("utf-8")
+                    yield json.loads(line)
 
     @staticmethod
     def stream_chat(response):
         for data in response:
             if 'content' in data['choices'][0]['delta']:
                 yield data['choices'][0]['delta']['content']
     
@@ -142,17 +137,30 @@
                 end_time = time.time()
                 ## log this on result
                 log_strs = []
                 log_strs.append(f"Chat request result ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
 
                 log_strs.append(" OUTPUT START ".center(50, '-'))
-                log_strs.append(response['choices'][0]['message']['content'])
-                log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
-                logger.info('\n'.join(log_strs))
+                stream = kwargs.get('stream', False)
+                if stream:
+                    def wrapper(response):
+                        text = ''
+                        for data in response:
+                            if 'content' in data['choices'][0]['delta']:
+                                text += data['choices'][0]['delta']['content']
+                            yield data
+                        log_strs.append(text)
+                        log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
+                        logger.info('\n'.join(log_strs))
+                    response = wrapper(response)
+                else:
+                    log_strs.append(response['choices'][0]['message']['content'])
+                    log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
+                    logger.info('\n'.join(log_strs))
         except Exception as e:
             if logger is not None:
                 end_time = time.time()
                 log_strs = []
                 log_strs.append(f"Chat request error ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
                 log_strs.append(str(e))
@@ -183,17 +191,29 @@
                 end_time = time.time()
                 ## log this on result
                 log_strs = []
                 log_strs.append(f"Completions request result ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
 
                 log_strs.append(" OUTPUT START ".center(50, '-'))
-                log_strs.append(response['choices'][0]['text'])
-                log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
-                logger.info('\n'.join(log_strs))
+                stream = kwargs.get('stream', False)
+                if stream:
+                    def wrapper(response):
+                        text = ''
+                        for data in response:
+                            text += data['choices'][0]['text']
+                            yield data
+                        log_strs.append(text)
+                        log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
+                        logger.info('\n'.join(log_strs))
+                    response = wrapper(response)
+                else:
+                    log_strs.append(response['choices'][0]['text'])
+                    log_strs.append(" OUTPUT END ".center(50, '-')+"\n")
+                    logger.info('\n'.join(log_strs))
         except Exception as e:
             if logger is not None:
                 end_time = time.time()
                 log_strs = []
                 log_strs.append(f"Completions request error ({end_time-start_time:.2f}s)")
                 log_strs.append(input_str)
                 log_strs.append(str(e))
```

### Comparing `HandyLLM-0.2.0/src/handyllm/prompt_converter.py` & `HandyLLM-0.2.1/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.0/tests/test_api.py` & `HandyLLM-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.0/tests/test_prompt.py` & `HandyLLM-0.2.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.2.0/tests/test_stream.py` & `HandyLLM-0.2.1/tests/test_stream.py`

 * *Files identical despite different names*

