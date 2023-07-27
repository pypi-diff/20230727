# Comparing `tmp/openai_function-0.1.5.tar.gz` & `tmp/openai_function-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.1.5.tar", max compression
+gzip compressed data, was "openai_function-0.1.6.tar", max compression
```

## Comparing `openai_function-0.1.5.tar` & `openai_function-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.5/README.md
--rw-r--r--   0        0        0      464 2023-07-27 02:43:17.922311 openai_function-0.1.5/openai_function/__init__.py
--rw-r--r--   0        0        0     2715 2023-07-27 01:54:52.192346 openai_function-0.1.5/openai_function/chat_completion.py
--rw-r--r--   0        0        0    12285 2023-07-27 03:47:22.555313 openai_function-0.1.5/openai_function/client.py
--rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.5/openai_function/faunadb/__init__.py
--rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.5/openai_function/faunadb/errors.py
--rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.5/openai_function/faunadb/objects.py
--rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.5/openai_function/faunadb/page.py
--rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.5/openai_function/faunadb/query.py
--rw-r--r--   0        0        0      230 2023-07-27 02:40:20.845792 openai_function-0.1.5/openai_function/fields.py
--rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.5/openai_function/json.py
--rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.5/openai_function/logging.py
--rwxr-xr-x   0        0        0    11253 2023-07-27 02:35:12.984719 openai_function-0.1.5/openai_function/odm.py
--rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.5/openai_function/openai_functions.py
--rw-r--r--   0        0        0     9350 2023-07-27 04:52:07.242050 openai_function-0.1.5/openai_function/store.py
--rw-r--r--   0        0        0     1053 2023-07-27 02:35:12.648718 openai_function-0.1.5/openai_function/typedefs.py
--rw-r--r--   0        0        0      502 2023-07-27 04:52:22.830071 openai_function-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 openai_function-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.6/README.md
+-rw-r--r--   0        0        0      464 2023-07-27 02:43:17.922311 openai_function-0.1.6/openai_function/__init__.py
+-rw-r--r--   0        0        0     2715 2023-07-27 01:54:52.192346 openai_function-0.1.6/openai_function/chat_completion.py
+-rw-r--r--   0        0        0    12285 2023-07-27 03:47:22.555313 openai_function-0.1.6/openai_function/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.6/openai_function/faunadb/__init__.py
+-rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.6/openai_function/faunadb/errors.py
+-rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.6/openai_function/faunadb/objects.py
+-rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.6/openai_function/faunadb/page.py
+-rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.6/openai_function/faunadb/query.py
+-rw-r--r--   0        0        0      230 2023-07-27 02:40:20.845792 openai_function-0.1.6/openai_function/fields.py
+-rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.6/openai_function/json.py
+-rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.6/openai_function/logging.py
+-rwxr-xr-x   0        0        0    11253 2023-07-27 02:35:12.984719 openai_function-0.1.6/openai_function/odm.py
+-rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.6/openai_function/openai_functions.py
+-rw-r--r--   0        0        0     9398 2023-07-27 04:54:33.354255 openai_function-0.1.6/openai_function/store.py
+-rw-r--r--   0        0        0     1053 2023-07-27 02:35:12.648718 openai_function-0.1.6/openai_function/typedefs.py
+-rw-r--r--   0        0        0      502 2023-07-27 04:54:39.710264 openai_function-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 openai_function-0.1.6/PKG-INFO
```

### Comparing `openai_function-0.1.5/openai_function/chat_completion.py` & `openai_function-0.1.6/openai_function/chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/client.py` & `openai_function-0.1.6/openai_function/client.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/faunadb/errors.py` & `openai_function-0.1.6/openai_function/faunadb/errors.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/faunadb/objects.py` & `openai_function-0.1.6/openai_function/faunadb/objects.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/faunadb/page.py` & `openai_function-0.1.6/openai_function/faunadb/page.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/faunadb/query.py` & `openai_function-0.1.6/openai_function/faunadb/query.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/json.py` & `openai_function-0.1.6/openai_function/json.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/logging.py` & `openai_function-0.1.6/openai_function/logging.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/odm.py` & `openai_function-0.1.6/openai_function/odm.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/openai_functions.py` & `openai_function-0.1.6/openai_function/openai_functions.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/openai_function/store.py` & `openai_function-0.1.6/openai_function/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,11 +235,11 @@
             logger.exception(exc)
             raise APIException(message=str(exc)) from exc
         
     @handle_errors    
     async def chatgpt(self, text:str, namespace:str="default", context:Optional[str]=None, memory:bool=False, functions:bool=False):
         """ChatGPT4 is a function that allows you to chat with GPT-4, with the option of using memory or functions."""
         if functions:
-            return await self.chat_with_functions(text, context=context)
+            return await self.chat_with_functions(text=text, context=context)
         if memory:
-            return await self.chat_with_memory(text, namespace=namespace)
-        return await self.chat(text)
+            return await self.chat_with_memory(text=text, namespace=namespace, context=context)
+        return await self.chat(text=text,context=context)
```

### Comparing `openai_function-0.1.5/openai_function/typedefs.py` & `openai_function-0.1.6/openai_function/typedefs.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.5/PKG-INFO` & `openai_function-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Oscar Bahamonde
 Author-email: oscarmartinbahamondemunoz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

