# Comparing `tmp/log10_io-0.2.2.tar.gz` & `tmp/log10_io-0.2.3.tar.gz`

## Comparing `log10_io-0.2.2.tar` & `log10_io-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.2.2/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.2.2/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.2.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/README.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/biochemist.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/code_optimizer.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/coder.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/cybersecurity_expert.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/email_generator.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/scrape_summarizer.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/agents/translator.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/evals/basic_eval.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/evals/compile.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/evals/fuzzy.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/evals/fuzzy_data.csv
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/evals/match_data.csv
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/anthropic_completion.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/completion_ada.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/get_url.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_babyagi.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_model_logger.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.2.2/examples/logging/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/__init__.py
--rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/anthropic.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/bigquery.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/evals.py
--rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/langchain.py
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/llm.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/load.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/openai.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/tools.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/utils.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/agents/camel.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.2.2/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 log10_io-0.2.2/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.2.2/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.2.2/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.2.3/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.2.3/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/README.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/biochemist.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/code_optimizer.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/coder.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/cybersecurity_expert.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/email_generator.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/agents/translator.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/basic_eval.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/compile.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/fuzzy.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/fuzzy_data.csv
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/evals/match_data.csv
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/anthropic_completion.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/completion_ada.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/get_url.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_babyagi.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_model_logger.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.2.3/examples/logging/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/__init__.py
+-rw-r--r--   0        0        0     4755 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/anthropic.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/bigquery.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/evals.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/langchain.py
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/llm.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/load.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/openai.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/tools.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/utils.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/agents/camel.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.2.3/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 log10_io-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.2.3/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.2.3/PKG-INFO
```

### Comparing `log10_io-0.2.2/.github/workflows/release.yml` & `log10_io-0.2.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/README.md` & `log10_io-0.2.3/examples/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/biochemist.py` & `log10_io-0.2.3/examples/agents/biochemist.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/code_optimizer.py` & `log10_io-0.2.3/examples/agents/code_optimizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/coder.py` & `log10_io-0.2.3/examples/agents/coder.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/cybersecurity_expert.py` & `log10_io-0.2.3/examples/agents/cybersecurity_expert.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/email_generator.py` & `log10_io-0.2.3/examples/agents/email_generator.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/scrape_summarizer.py` & `log10_io-0.2.3/examples/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/agents/translator.py` & `log10_io-0.2.3/examples/agents/translator.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/evals/basic_eval.py` & `log10_io-0.2.3/examples/evals/basic_eval.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/evals/compile.py` & `log10_io-0.2.3/examples/evals/compile.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/evals/fuzzy.py` & `log10_io-0.2.3/examples/evals/fuzzy.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/evals/fuzzy_data.csv` & `log10_io-0.2.3/examples/evals/fuzzy_data.csv`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/evals/match_data.csv` & `log10_io-0.2.3/examples/evals/match_data.csv`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/chatcompletion_async_vs_sync.py` & `log10_io-0.2.3/examples/logging/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/get_url.py` & `log10_io-0.2.3/examples/logging/get_url.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/langchain_babyagi.py` & `log10_io-0.2.3/examples/logging/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/langchain_model_logger.py` & `log10_io-0.2.3/examples/logging/langchain_model_logger.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 
 messages = [
     HumanMessage(content="You are a ping pong machine"),
     HumanMessage(content="Ping?"),
 ]
 
-llm = ChatOpenAI(model_name="gpt-3.5-turbo", callbacks=[log10_callback], temperature=0.5)
-completion = llm.predict_messages(messages)
+llm = ChatOpenAI(model_name="gpt-3.5-turbo", callbacks=[log10_callback], temperature=0.5, tags=["test"])
+completion = llm.predict_messages(messages, tags=["foobar"])
 print(completion)
 
-llm = ChatAnthropic(model="claude-2", callbacks=[log10_callback], temperature=0.7)
+llm = ChatAnthropic(model="claude-2", callbacks=[log10_callback], temperature=0.7, tags=["baz"])
 llm.predict_messages(messages)
 print(completion)
 
 llm = OpenAI(model_name="text-davinci-003", callbacks=[log10_callback], temperature=0.5)
 completion = llm.predict("You are a ping pong machine.\nPing?\n")
 print(completion)
```

### Comparing `log10_io-0.2.2/examples/logging/langchain_multiple_tools.py` & `log10_io-0.2.3/examples/logging/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/langchain_qa.py` & `log10_io-0.2.3/examples/logging/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/langchain_simple_sequential.py` & `log10_io-0.2.3/examples/logging/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/langchain_sqlagent.py` & `log10_io-0.2.3/examples/logging/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/examples/logging/multiple_sessions.py` & `log10_io-0.2.3/examples/logging/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/anthropic.py` & `log10_io-0.2.3/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/bigquery.py` & `log10_io-0.2.3/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/evals.py` & `log10_io-0.2.3/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/langchain.py` & `log10_io-0.2.3/log10/langchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
         """Print out the prompts."""
         logging.debug(
             f"**\n**on_llm_start**\n**\n: serialized:\n {serialized} \n\n prompts:\n {prompts} \n\n rest: {kwargs}"
         )
-
         kwargs = serialized.get("kwargs", {})
         hparams = kwargs_to_hparams(kwargs)
 
         model = kwargs.get("model_name", None)
         if model is None:
             model = kwargs.get("model", None)
         if model is None:
@@ -68,15 +67,15 @@
         if len(prompts) != 1:
             raise BaseException("Only support one prompt at a time")
 
         request = {"model": model, "prompt": prompts[0], **hparams}
 
         logging.debug(f"request: {request}")
 
-        completion_id = self.log_start(request, Kind.text)
+        completion_id = self.log_start(request, Kind.text, tags)
 
         self.runs[run_id] = {
             "kind": Kind.text,
             "completion_id": completion_id,
             "start_time": time.perf_counter(),
             "model": model,
         }
@@ -133,14 +132,15 @@
             **hparams,
         }
         logging.debug(f"request: {request}")
 
         completion_id = self.log_start(
             request,
             Kind.chat,
+            tags,
         )
 
         self.runs[run_id] = {
             "kind": Kind.chat,
             "completion_id": completion_id,
             "start_time": time.perf_counter(),
             "model": model,
```

### Comparing `log10_io-0.2.2/log10/llm.py` & `log10_io-0.2.3/log10/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 import traceback
 
 Role = Enum("Role", ["system", "assistant", "user"])
 Kind = Enum("Kind", ["chat", "text"])
 
-from typing import List
+from typing import List, Optional
 
 import json
 
 import logging
 import requests
 
 
@@ -23,15 +23,22 @@
         token: str = None,
         org_id: str = None,
         tags: List[str] = None,
     ):
         self.url = url if url else os.getenv("LOG10_URL")
         self.token = token if token else os.getenv("LOG10_TOKEN")
         self.org_id = org_id if org_id else os.getenv("LOG10_ORG_ID")
-        self.tags = tags if tags else os.getenv("LOG10_TAGS", "").split(",")
+
+        # Get tags from env, if not set, use empty list
+        if tags:
+            self.tags = tags
+        elif os.getenv("LOG10_TAGS") is not None:
+            self.tags = os.getenv("LOG10_TAGS").split(",")
+        else:
+            self.tags = []
 
 
 class Message(ABC):
     def __init__(
         self, role: Role, content: str, id: str = None, completion: str = None
     ):
         self.id = id
@@ -138,38 +145,44 @@
                 "x-log10-token": self.log10_config.token,
                 "Content-Type": "application/json",
             },
             json=request,
         )
 
     # Save the start of a completion in **openai request format**.
-    def log_start(self, request, kind: Kind):
+    def log_start(self, request, kind: Kind, tags: Optional[List[str]] = None):
         if not self.log10_config:
             return None
 
         res = self.api_request(
             "/api/completions", "POST", {"organization_id": self.log10_config.org_id}
         )
         completion_id = res.json()["completionID"]
 
+        # merge tags
+        if tags:
+            tags = list(set(tags + self.log10_config.tags))
+        else:
+            tags = self.log10_config.tags
+
         res = self.api_request(
             f"/api/completions/{completion_id}",
             "POST",
             {
                 "kind": kind == Kind.text and "completion" or "chat",
                 "organization_id": self.log10_config.org_id,
                 "session_id": self.session_id,
                 "orig_module": "openai.api_resources.completion"
                 if kind == Kind.text
                 else "openai.api_resources.chat_completion",
                 "orig_qualname": "Completion.create"
                 if kind == Kind.text
                 else "ChatCompletion.create",
                 "status": "started",
-                "tags": self.log10_config.tags,
+                "tags": tags,
                 "request": json.dumps(request),
             },
         )
 
         return completion_id
 
     # Save the end of a completion in **openai request format**.
```

### Comparing `log10_io-0.2.2/log10/load.py` & `log10_io-0.2.3/log10/load.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/openai.py` & `log10_io-0.2.3/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/tools.py` & `log10_io-0.2.3/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/utils.py` & `log10_io-0.2.3/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/agents/camel.py` & `log10_io-0.2.3/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/agents/scrape_summarizer.py` & `log10_io-0.2.3/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/log10/schemas/bigquery.json` & `log10_io-0.2.3/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/LICENSE` & `log10_io-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/README.md` & `log10_io-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.2.2/pyproject.toml` & `log10_io-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.2.2"
+version = "0.2.3"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.2.2/PKG-INFO` & `log10_io-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.2.2
+Version: 0.2.3
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

