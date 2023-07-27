# Comparing `tmp/michina-0.1.1.tar.gz` & `tmp/michina-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michina-0.1.1.tar", max compression
+gzip compressed data, was "michina-0.2.0.tar", max compression
```

## Comparing `michina-0.1.1.tar` & `michina-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      146 2023-07-25 08:16:01.149793 michina-0.1.1/README.md
--rw-r--r--   0        0        0      122 2023-07-25 00:01:47.195488 michina-0.1.1/michina/checks/__init__.py
--rw-r--r--   0        0        0      238 2023-07-24 23:36:58.809362 michina-0.1.1/michina/checks/base_check.py
--rw-r--r--   0        0        0      175 2023-07-25 00:01:47.195444 michina-0.1.1/michina/checks/consistency/__init__.py
--rw-r--r--   0        0        0     1786 2023-07-25 00:01:47.195414 michina-0.1.1/michina/checks/consistency/check.py
--rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.1.1/michina/checks/consistency/prompt.py
--rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.1.1/michina/checks/tone/__init__.py
--rw-r--r--   0        0        0     1587 2023-07-25 00:01:47.195581 michina-0.1.1/michina/checks/tone/check.py
--rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.1.1/michina/checks/tone/prompt.py
--rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.1.1/michina/exceptions/exceptions.py
--rw-r--r--   0        0        0      469 2023-07-25 08:39:09.246042 michina-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 michina-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      185 2023-07-25 17:25:21.973986 michina-0.2.0/README.md
+-rw-r--r--   0        0        0      122 2023-07-25 00:01:47.195488 michina-0.2.0/michina/checks/__init__.py
+-rw-r--r--   0        0        0      648 2023-07-26 23:54:50.190542 michina-0.2.0/michina/checks/base_check.py
+-rw-r--r--   0        0        0      183 2023-07-26 23:55:55.785232 michina-0.2.0/michina/checks/consistency/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-26 23:56:41.218881 michina-0.2.0/michina/checks/consistency/check.py
+-rw-r--r--   0        0        0     2611 2023-07-24 23:08:42.323294 michina-0.2.0/michina/checks/consistency/prompt.py
+-rw-r--r--   0        0        0      140 2023-07-25 00:01:47.195530 michina-0.2.0/michina/checks/tone/__init__.py
+-rw-r--r--   0        0        0     1419 2023-07-26 23:56:44.395259 michina-0.2.0/michina/checks/tone/check.py
+-rw-r--r--   0        0        0     2397 2023-07-24 23:13:10.018714 michina-0.2.0/michina/checks/tone/prompt.py
+-rw-r--r--   0        0        0      310 2023-07-24 18:35:05.155781 michina-0.2.0/michina/exceptions/exceptions.py
+-rw-r--r--   0        0        0      469 2023-07-27 00:01:25.349664 michina-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 michina-0.2.0/PKG-INFO
```

### Comparing `michina-0.1.1/michina/checks/consistency/check.py` & `michina-0.2.0/michina/checks/consistency/check.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,62 @@
 """
 This is a module for the Michina test suite.
 """
 from michina.checks.base_check import BaseCheck
-from michina.exceptions.exceptions import InvalidTypeException, InvalidXMLException, LanguageModelException
+from michina.exceptions.exceptions import (
+    InvalidTypeException,
+    InvalidXMLException,
+    LanguageModelException,
+)
 from michina.checks.consistency.prompt import CONSISTENCY_CHECK_TEMPLATE
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import LLMChain
 from langchain import PromptTemplate
 from dotenv import load_dotenv
-from os import environ as env
 import xmltodict
 from pydantic import BaseModel
 
 load_dotenv()
 
-class IsConsistentInput(BaseModel):
+
+class ConsistencyCheckInput(BaseModel):
     message: str
     statement: str
 
 
-class IsConsistentResponse(BaseModel):
-    input: IsConsistentInput
+class ConsistencyCheckResponse(BaseModel):
+    input: ConsistencyCheckInput
     reasoning: str
     judgment: float
 
+
 class ConsistencyCheck(BaseCheck):
-    def check(message: str, statement: str) -> IsConsistentResponse:
-        llm = ChatOpenAI(
-            temperature=0,
-            model="gpt-3.5-turbo",
-            openai_api_key=env["OPENAI_API_KEY"],
-        )
+    description: str = "Checks whether the message is consistent with the statement."
 
+    def check(self, message: str, statement: str) -> ConsistencyCheckResponse:
         prompt = PromptTemplate.from_template(CONSISTENCY_CHECK_TEMPLATE)
-        chain = LLMChain(llm=llm, prompt=prompt)
+        chain = LLMChain(llm=self.llm, prompt=prompt)
 
         try:
             string_response = chain.run(message=message, statement=statement)
         except Exception as e:
             raise LanguageModelException(e)
 
         def postprocessor(path, key, value):
             if key == "judgment":
                 return key, float(value)
             else:
                 return key, value
 
         try:
-            dict_response = xmltodict.parse(string_response, postprocessor=postprocessor)
+            dict_response = xmltodict.parse(
+                string_response, postprocessor=postprocessor
+            )
         except Exception as e:
             raise InvalidXMLException(e)
 
         try:
-            response = IsConsistentResponse(**dict_response["response"])
+            response = ConsistencyCheckResponse(**dict_response["response"])
         except Exception as e:
             raise InvalidTypeException(e)
 
         return response
```

### Comparing `michina-0.1.1/michina/checks/consistency/prompt.py` & `michina-0.2.0/michina/checks/consistency/prompt.py`

 * *Files identical despite different names*

### Comparing `michina-0.1.1/michina/checks/tone/check.py` & `michina-0.2.0/michina/checks/tone/check.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 )
 from pydantic import BaseModel
 
 from langchain.chat_models import ChatOpenAI
 from langchain.chains import LLMChain
 from langchain import PromptTemplate
 from dotenv import load_dotenv
-from os import environ as env
 import xmltodict
 
 load_dotenv()
 
 
 class ToneCheckInput(BaseModel):
     message: str
@@ -29,23 +28,17 @@
 
 
 class ToneCheck(BaseCheck):
     description: str = (
         "Checks whether the tone of a given message matches the tone provided."
     )
 
-    def check(message: str, tone: str) -> ToneCheckReponse:
-        llm = ChatOpenAI(
-            temperature=0,
-            model="gpt-3.5-turbo",
-            openai_api_key=env["OPENAI_API_KEY"],
-        )
-
+    def check(self, message: str, tone: str) -> ToneCheckReponse:
         prompt = PromptTemplate.from_template(TONE_CHECK_TEMPLATE)
-        chain = LLMChain(llm=llm, prompt=prompt)
+        chain = LLMChain(llm=self.llm, prompt=prompt)
 
         try:
             string_response = chain.run(message=message, tone=tone)
         except Exception as e:
             raise LanguageModelException(e)
 
         try:
```

### Comparing `michina-0.1.1/michina/checks/tone/prompt.py` & `michina-0.2.0/michina/checks/tone/prompt.py`

 * *Files identical despite different names*

### Comparing `michina-0.1.1/PKG-INFO` & `michina-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: michina
-Version: 0.1.1
+Version: 0.2.0
 Summary: Integ test framework for LLMs.
 Home-page: https://github.com/michina-ai/michina
 Author: bkitano
 Author-email: briankitano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -18,9 +18,12 @@
 Description-Content-Type: text/markdown
 
 # Michina
 From the quechua word for "pasture".
 
 Unit testing and integration testing for LLMs.
 
+## Features
+- [openai] Can run in a Github Actions for workflow
+
 ## Todo
-- make it run on github via github actions
+- Add monitoring
```

