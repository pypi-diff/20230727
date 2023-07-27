# Comparing `tmp/openai_wrapper-0.6.2.tar.gz` & `tmp/openai_wrapper-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_wrapper-0.6.2.tar", max compression
+gzip compressed data, was "openai_wrapper-0.6.3.tar", max compression
```

## Comparing `openai_wrapper-0.6.2.tar` & `openai_wrapper-0.6.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      134 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/openai_wrapper/__init__.py
--rw-r--r--   0        0        0     5585 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/openai_wrapper/chat_completion.py
--rw-r--r--   0        0        0    18790 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/openai_wrapper/completion.py
--rw-r--r--   0        0        0     2053 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/openai_wrapper/config.py
--rw-r--r--   0        0        0     4367 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/openai_wrapper/embeddings.py
--rw-r--r--   0        0        0      729 2023-07-25 10:50:05.301129 openai_wrapper-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      134 2023-07-27 07:06:17.473784 openai_wrapper-0.6.3/openai_wrapper/__init__.py
+-rw-r--r--   0        0        0     5973 2023-07-27 07:06:17.473784 openai_wrapper-0.6.3/openai_wrapper/chat_completion.py
+-rw-r--r--   0        0        0    19182 2023-07-27 07:06:17.477784 openai_wrapper-0.6.3/openai_wrapper/completion.py
+-rw-r--r--   0        0        0     2053 2023-07-27 07:06:17.477784 openai_wrapper-0.6.3/openai_wrapper/config.py
+-rw-r--r--   0        0        0     4367 2023-07-27 07:06:17.477784 openai_wrapper-0.6.3/openai_wrapper/embeddings.py
+-rw-r--r--   0        0        0      729 2023-07-27 07:06:17.477784 openai_wrapper-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 openai_wrapper-0.6.3/PKG-INFO
```

### Comparing `openai_wrapper-0.6.2/openai_wrapper/chat_completion.py` & `openai_wrapper-0.6.3/openai_wrapper/chat_completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         logging.info(f"ChatGPT Model: {model}")
 
         self.use_case_name = use_case_name
         self.config = config
         self.mongo_client = config.mongo_client
         self.async_mongo_client = config.async_mongo_client
         self.openai_client = config.openai_client
+        self.wrapper_initiated = datetime.utcnow()
 
         self.model_params = {
             "model": model,
             "messages": [],
             "temperature": 0.7,
             "top_p": 1,
             "max_tokens": 256,
@@ -115,16 +116,17 @@
             process_response_args = {}
 
         preprocessed_messages = preprocess_messages(messages, **preprocess_messages_args)
         self.model_params["messages"] = preprocessed_messages
 
         if functions is not None:
             self.model_params["functions"] = functions
-
+        self.openai_started = datetime.utcnow()
         response = self.openai_client.ChatCompletion.create(**self.model_params)
+        self.openai_ended = datetime.utcnow()
 
         if process_response is not None:
             response = process_response(response, **process_response_args)
 
         is_function_call = 'function_call' in response.choices[0].message
 
         document = {
@@ -133,14 +135,19 @@
             "response": response.choices[0].message["content"] if not is_function_call else None,
             "function_to_call": dict(response.choices[0].message["function_call"]) if is_function_call else None,
             "openai_response": response.__dict__['_previous'],
             "model_params": self.model_params,
             "created_at": str(datetime.utcnow()),
             "experiment_metadata": self.experiment_metadata,
             "project_metadata": self.project_metadata,
+            "timestamps": {
+                            "wrapper_initiated": self.wrapper_initiated,
+                            "openai_started": self.openai_started,
+                            "openai_ended": self.openai_ended
+            }
         }
 
         if self.extra_params is not None:
             document.update(self.extra_params)
 
         mongo_db = self.mongo_client[self.config.mongo_db_name]
         mongo_collection = mongo_db[self.use_case_name]
```

### Comparing `openai_wrapper-0.6.2/openai_wrapper/completion.py` & `openai_wrapper-0.6.3/openai_wrapper/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         logging.info(f"GPT-3 Model: {model}")
 
         self.use_case_name = use_case_name
         self.config = config
         self.mongo_client = config.mongo_client
         self.async_mongo_client = config.async_mongo_client
         self.openai_client = config.openai_client
+        self.wrapper_initiated = datetime.utcnow()
+
         if datetime.utcnow() < datetime(2022, 9, 1):
             self.TEXT_MODELS_COST_PER_1K_TOKENS = {
                 "text-ada-001": 0.0008,
                 "text-babbage-001": 0.0012,
                 "text-curie-001": 0.0060,
                 "text-davinci-002": 0.0600
             }
@@ -165,15 +167,17 @@
 
         if preprocess_prompt_args is None:
             preprocess_prompt_args = {}
         if process_response_args is None:
             process_response_args = {}
 
         preprocessed_prompt = preprocess_prompt(prompt, **preprocess_prompt_args)
+        self.openai_started = datetime.utcnow()
         response = self.openai_client.Completion.create(**self.model_params, prompt=preprocessed_prompt)
+        self.openai_ended = datetime.utcnow()
 
         all_logprobs = {'tokens': [], 'token_logprobs': [], 'top_logprobs': [], 'text_offset': []}
         completion_text = ""
         token_number = 0
 
         for resp in response:                
             logprobs = resp['choices'][0]['logprobs']                
@@ -198,15 +202,20 @@
             "prompt_version_description": prompt_version_description,
             "completion_text":  completion_text,
             "openai_response": openai_response,
             "model_params": self.model_params,
             "created_at": str(datetime.utcnow()),
             "experiment_metadata": self.experiment_metadata,
             "project_metadata": self.project_metadata,
-            "request_cost_in_usd": request_costs
+            "request_cost_in_usd": request_costs,
+            "timestamps" : {
+                            "wrapper_initiated": self.wrapper_initiated,
+                            "openai_started": self.openai_started,
+                            "openai_ended": self.openai_ended
+            }
         }
 
         if self.extra_params is not None:
             document.update(self.extra_params)
 
         mongo_db = self.mongo_client[self.config.mongo_db_name]
         mongo_collection = mongo_db[self.use_case_name]
```

### Comparing `openai_wrapper-0.6.2/openai_wrapper/config.py` & `openai_wrapper-0.6.3/openai_wrapper/config.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.6.2/openai_wrapper/embeddings.py` & `openai_wrapper-0.6.3/openai_wrapper/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_wrapper-0.6.2/pyproject.toml` & `openai_wrapper-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-wrapper"
-version = "0.6.2"
+version = "0.6.3"
 description = "A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models."
 authors = ["AI Team <datascience@prosus.com>"]
 license = "MIT License"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 openai = "^0.27.2"
```

### Comparing `openai_wrapper-0.6.2/PKG-INFO` & `openai_wrapper-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-wrapper
-Version: 0.6.2
+Version: 0.6.3
 Summary: A wrapper for OpenAI's python API which wraps around the openAI functions and stores the request, response and metadata to MongoDB. The stored data can be used to fine tune GPT-3 models or HuggingFace models.
 License: MIT
 Author: AI Team
 Author-email: datascience@prosus.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

