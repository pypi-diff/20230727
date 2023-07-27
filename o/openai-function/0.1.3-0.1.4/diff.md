# Comparing `tmp/openai_function-0.1.3.tar.gz` & `tmp/openai_function-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.1.3.tar", max compression
+gzip compressed data, was "openai_function-0.1.4.tar", max compression
```

## Comparing `openai_function-0.1.3.tar` & `openai_function-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.3/README.md
--rw-r--r--   0        0        0      464 2023-07-27 02:43:17.922311 openai_function-0.1.3/openai_function/__init__.py
--rw-r--r--   0        0        0     2715 2023-07-27 01:54:52.192346 openai_function-0.1.3/openai_function/chat_completion.py
--rw-r--r--   0        0        0    12278 2023-07-27 02:35:12.968719 openai_function-0.1.3/openai_function/client.py
--rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.3/openai_function/faunadb/__init__.py
--rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/errors.py
--rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/objects.py
--rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/page.py
--rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.3/openai_function/faunadb/query.py
--rw-r--r--   0        0        0      230 2023-07-27 02:40:20.845792 openai_function-0.1.3/openai_function/fields.py
--rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.3/openai_function/json.py
--rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.3/openai_function/logging.py
--rwxr-xr-x   0        0        0    11253 2023-07-27 02:35:12.984719 openai_function-0.1.3/openai_function/odm.py
--rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.3/openai_function/openai_functions.py
--rw-r--r--   0        0        0     8670 2023-07-27 02:59:40.216643 openai_function-0.1.3/openai_function/store.py
--rw-r--r--   0        0        0     1053 2023-07-27 02:35:12.648718 openai_function-0.1.3/openai_function/typedefs.py
--rw-r--r--   0        0        0      464 2023-07-27 02:58:49.164533 openai_function-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 openai_function-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.4/README.md
+-rw-r--r--   0        0        0      464 2023-07-27 02:43:17.922311 openai_function-0.1.4/openai_function/__init__.py
+-rw-r--r--   0        0        0     2715 2023-07-27 01:54:52.192346 openai_function-0.1.4/openai_function/chat_completion.py
+-rw-r--r--   0        0        0    12285 2023-07-27 03:47:22.555313 openai_function-0.1.4/openai_function/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.4/openai_function/faunadb/__init__.py
+-rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.4/openai_function/faunadb/errors.py
+-rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.4/openai_function/faunadb/objects.py
+-rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.4/openai_function/faunadb/page.py
+-rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.4/openai_function/faunadb/query.py
+-rw-r--r--   0        0        0      230 2023-07-27 02:40:20.845792 openai_function-0.1.4/openai_function/fields.py
+-rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.4/openai_function/json.py
+-rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.4/openai_function/logging.py
+-rwxr-xr-x   0        0        0    11253 2023-07-27 02:35:12.984719 openai_function-0.1.4/openai_function/odm.py
+-rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.4/openai_function/openai_functions.py
+-rw-r--r--   0        0        0     8783 2023-07-27 03:55:42.528046 openai_function-0.1.4/openai_function/store.py
+-rw-r--r--   0        0        0     1053 2023-07-27 02:35:12.648718 openai_function-0.1.4/openai_function/typedefs.py
+-rw-r--r--   0        0        0      502 2023-07-27 04:03:43.068773 openai_function-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 openai_function-0.1.4/PKG-INFO
```

### Comparing `openai_function-0.1.3/openai_function/chat_completion.py` & `openai_function-0.1.4/openai_function/chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/client.py` & `openai_function-0.1.4/openai_function/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,20 @@
 import logging
 import os
 import typing
 from dataclasses import dataclass, field
 from functools import wraps
 from re import T
 from threading import Lock
-from typing import (
-    Any,
-    AsyncGenerator,
-    Dict,
-    List,
-    Literal,
-    NamedTuple,
-    Optional,
-    Type,
-    Union,
-)
-
-from aiohttp import (
-    ClientConnectionError,
-    ClientConnectorSSLError,
-    ClientResponse,
-    ClientSession,
-    ClientTimeout,
-    TCPConnector,
-)
+from typing import (Any, AsyncGenerator, Dict, List, Literal, NamedTuple,
+                    Optional, Type, Union)
+
+from aiohttp import (ClientConnectionError, ClientConnectorSSLError,
+                     ClientResponse, ClientSession, ClientTimeout,
+                     TCPConnector)
 from aiohttp.web_exceptions import HTTPException
 from dotenv import load_dotenv
 from multidict import CIMultiDict
 from pydantic import BaseModel
 
 from .faunadb.errors import FaunaException
 from .faunadb.objects import Expr
@@ -284,15 +270,15 @@
         self,
         url: str,
         method: Method = "GET",
         json: MaybeJson = None,
     ):
         session = await self.__load__()
         async with session.request(
-            method, url, headers=self.config.headers, json=json
+            method=method, url=url, headers=self.config.headers, json=json
         ) as response:
             self.config.logger.info("Fetching JSON from %s with method %s", url, method)
             try:
                 return await response.json()
             except (
                 HTTPException,
                 FaunaException,
```

### Comparing `openai_function-0.1.3/openai_function/faunadb/errors.py` & `openai_function-0.1.4/openai_function/faunadb/errors.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/faunadb/objects.py` & `openai_function-0.1.4/openai_function/faunadb/objects.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/faunadb/page.py` & `openai_function-0.1.4/openai_function/faunadb/page.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/faunadb/query.py` & `openai_function-0.1.4/openai_function/faunadb/query.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/json.py` & `openai_function-0.1.4/openai_function/json.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/logging.py` & `openai_function-0.1.4/openai_function/logging.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/odm.py` & `openai_function-0.1.4/openai_function/odm.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/openai_functions.py` & `openai_function-0.1.4/openai_function/openai_functions.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/openai_function/store.py` & `openai_function-0.1.4/openai_function/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         return response["choices"][0]["message"]["content"]
 
     @handle_errors
     async def chat_with_memory(self, text: str, namespace: str = "default") -> str:
         """Chat completion with similarity search retrieval from pinecone"""
         try:
             embedding = await self.create_embeddings(text)
+            print(embedding)
             query_request = QueryRequest(vector=embedding, namespace=namespace)
             query_response: QueryResponse = await self.query_vectors(query_request)
             logger.info("# of matches: %s", len(query_response.matches))  # type: ignore
             similar_text_chunks = [
                 i.metadata.get("text", "") for i in query_response.matches
             ]
             similar_text = "Previous Similar results:" + "\n".join(similar_text_chunks)
@@ -163,18 +164,20 @@
         """Chat completion with functions."""
         return await function_call(text, context=context, functions=functions)
 
     @handle_errors
     async def create_embeddings(self, text: str) -> Vector:
         """Creates embeddings for the given texts."""
         response = await openai.Embedding.acreate(
-            engine="text-embedding-ada-002",
+            model="text-embedding-ada-002",
             input=text,
         )
+        logger.info(response)
         assert isinstance(response, dict)
+        logger.info("Embedding created for: %s", text)
         return response["data"][0]["embedding"]
 
     async def chat_stream(self, text: str) -> AsyncGenerator[str, None]:
         """Chat completion stream with no functions."""
         response = openai.ChatCompletion.acreate(
             model="gpt-4-0613",
             messages=[{"role": "user", "content": text}],
```

### Comparing `openai_function-0.1.3/openai_function/typedefs.py` & `openai_function-0.1.4/openai_function/typedefs.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.3/PKG-INFO` & `openai_function-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: openai-function
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Oscar Bahamonde
 Author-email: oscarmartinbahamondemunoz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: iso8601 (>=2.0.0,<3.0.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pydantic[dotenv] (==1.10.11)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
```

