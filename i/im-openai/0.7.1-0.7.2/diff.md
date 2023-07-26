# Comparing `tmp/im_openai-0.7.1.tar.gz` & `tmp/im_openai-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.7.1.tar", last modified: Thu Jul 20 01:11:49 2023, max compression
+gzip compressed data, was "im_openai-0.7.2.tar", last modified: Wed Jul 26 22:08:36 2023, max compression
```

## Comparing `im_openai-0.7.1.tar` & `im_openai-0.7.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:49.049346 im_openai-0.7.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.7.1/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.7.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.7.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-20 01:11:49.049911 im_openai-0.7.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.7.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:48.982871 im_openai-0.7.1/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.7.1/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.7.1/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.7.1/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:49.002091 im_openai-0.7.1/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-20 01:11:24.000000 im_openai-0.7.1/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5456 2023-07-20 00:33:04.000000 im_openai-0.7.1/im_openai/client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:49.041556 im_openai-0.7.1/im_openai/langchain/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.7.1/im_openai/langchain/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    18494 2023-07-20 01:09:06.000000 im_openai-0.7.1/im_openai/langchain/callbacks.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.7.1/im_openai/langchain/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4533 2023-07-20 00:23:59.000000 im_openai-0.7.1/im_openai/langchain/util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3668 2023-07-20 00:32:40.000000 im_openai-0.7.1/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.7.1/im_openai/template.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9375 2023-07-20 01:08:51.000000 im_openai-0.7.1/im_openai/test_langchain_util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:49.021229 im_openai-0.7.1/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-20 01:11:48.000000 im_openai-0.7.1/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      701 2023-07-20 01:11:48.000000 im_openai-0.7.1/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-20 01:11:48.000000 im_openai-0.7.1/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-20 01:11:48.000000 im_openai-0.7.1/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-20 01:11:48.000000 im_openai-0.7.1/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.7.1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-20 01:11:49.052267 im_openai-0.7.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-20 01:11:24.000000 im_openai-0.7.1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-20 01:11:49.047410 im_openai-0.7.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.7.1/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.7.1/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.322852 im_openai-0.7.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.7.2/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.7.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.7.2/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-26 22:08:36.323721 im_openai-0.7.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.7.2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.246557 im_openai-0.7.2/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4934 2023-07-20 00:09:46.000000 im_openai-0.7.2/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.7.2/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.7.2/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.263656 im_openai-0.7.2/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-26 22:07:56.000000 im_openai-0.7.2/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5456 2023-07-21 22:04:26.000000 im_openai-0.7.2/im_openai/client.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.297186 im_openai-0.7.2/im_openai/langchain/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      210 2023-07-20 00:23:59.000000 im_openai-0.7.2/im_openai/langchain/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17290 2023-07-25 00:41:12.000000 im_openai-0.7.2/im_openai/langchain/callbacks.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3039 2023-07-18 23:10:42.000000 im_openai-0.7.2/im_openai/langchain/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7888 2023-07-25 03:35:20.000000 im_openai-0.7.2/im_openai/langchain/util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3834 2023-07-21 22:37:56.000000 im_openai-0.7.2/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.7.2/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.283445 im_openai-0.7.2/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3774 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      741 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-26 22:08:36.000000 im_openai-0.7.2/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-07-20 00:25:03.000000 im_openai-0.7.2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-26 22:08:36.326246 im_openai-0.7.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-26 22:07:53.000000 im_openai-0.7.2/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-26 22:08:36.318875 im_openai-0.7.2/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.7.2/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-07-20 00:09:46.000000 im_openai-0.7.2/tests/test_im_openai.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9375 2023-07-20 01:08:51.000000 im_openai-0.7.2/tests/test_langchain.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13484 2023-07-25 03:36:46.000000 im_openai-0.7.2/tests/test_langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2961 2023-07-21 22:42:02.000000 im_openai-0.7.2/tests/test_patch.py
```

### Comparing `im_openai-0.7.1/CONTRIBUTING.rst` & `im_openai-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/LICENSE` & `im_openai-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/PKG-INFO` & `im_openai-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.7.1
+Version: 0.7.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `im_openai-0.7.1/README.md` & `im_openai-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/docs/Makefile` & `im_openai-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/docs/conf.py` & `im_openai-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/docs/installation.rst` & `im_openai-0.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/docs/make.bat` & `im_openai-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/im_openai/client.py` & `im_openai-0.7.2/im_openai/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,19 +83,19 @@
 
 @asynccontextmanager
 async def event_session(
     project_key: str,
     api_name: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
+    model_params: Dict | None = None,
     chat_id: str | None = None,
     prompt_template_params: dict | None = None,
     prompt_event_id: str | None = None,
     parent_event_id: str | None = None,
-    model_params: Dict | None = None,
 ):
     """Context manager for sending an event to Imaginary Dev.
 
     Usage::
 
         with event_session(project_key, api_name, prompt_text, prompt_event_id) as complete_event:
             # do something
```

### Comparing `im_openai-0.7.1/im_openai/langchain/callbacks.py` & `im_openai-0.7.2/im_openai/langchain/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     StringPromptTemplate,
 )
 from langchain.prompts.chat import BaseChatPromptTemplate, BaseMessagePromptTemplate
 from langchain.schema import AgentAction, AgentFinish, BaseMessage, LLMResult
 
 from im_openai import client
 
+from . import util
 from .patch import loads
-from .util import format_chat_template, format_langchain_value, make_stub_inputs
 
 logger = logging.getLogger(__name__)
 
 from functools import wraps
 
 
 class PromptWatchCallbacks(BaseCallbackHandler):
@@ -69,15 +69,15 @@
             raise ValueError("project_key must be provided")
         self.valid_namespaces = valid_namespaces
         self.runs = {}
         self.api_name = api_name
         if template_text is not None:
             self.template_text = template_text
         elif template_chat is not None:
-            self.template_chat = format_chat_template(template_chat)
+            self.template_chat = util.format_chat_template(template_chat)
         else:
             self.template_chat = None
         self.parent_run_ids = {}
 
     def _get_run(self, run_id: UUID):
         if run_id in self.runs:
             return self.runs[run_id]
@@ -229,16 +229,16 @@
         run = self._get_run(run_id)
         if not run:
             return
         model_params = _extract_openai_params(serialized)
         run["messages"] = messages
         run["now"] = time.time()
         run["model_params"] = model_params
-
         template_chat = self._resolve_chat_template(run_id)
+
         asyncio.run(
             self._async_send_chat(
                 run_id,
                 template_chat,
                 run["inputs"],
                 messages,
                 parent_event_id=parent_run_id,
@@ -343,20 +343,22 @@
         model_params: Dict | None = None,
         is_chat: bool = False,
     ):
         async with aiohttp.ClientSession() as session:
             generations_lists = result.generations if result else []
             for iteration, generations in zip_longest(iterations, generations_lists):
                 response_text = "".join(g.text for g in generations) if generations else None
-                json_inputs = {key: format_langchain_value(value) for key, value in inputs.items()}
+                json_inputs = {
+                    key: util.format_langchain_value(value) for key, value in inputs.items()
+                }
                 model_params = model_params.copy() if model_params else {}
                 if is_chat:
                     model_params["modelType"] = "chat"
                     prompt = (
-                        {"chat": format_chat_template(iteration)}  # type: ignore
+                        {"chat": util.format_chat_template(iteration)}  # type: ignore
                         if not template
                         else None
                     )
                     prompt_template_text = None
                     prompt_template_chat = template
                 else:
                     model_params["modelType"] = "completion"
@@ -439,47 +441,26 @@
 
     def _resolve_chat_template(self, run_id: UUID):
         """Resolve the template_chat into a list of dicts"""
         template: Optional[BasePromptTemplate] = self._get_run_info(run_id, "prompt_template")
         inputs: Optional[Dict[str, Any]] = self._get_run_info(run_id, "inputs")
         template_chat = None
         if template and inputs:
-            stub_inputs = make_stub_inputs(inputs)
-            # Some of the templat formatters get upset if you pass in extra keys
-            filtered_stub_inputs = {
-                k: v for k, v in stub_inputs.items() if k in template.input_variables
-            }
-            if isinstance(template, (BaseMessagePromptTemplate, BaseChatPromptTemplate)):
-                # We can't go through format_prompt because it doesn't like formatting the wrong types
-                template_chat = template.format_messages(**filtered_stub_inputs)
-
-            elif isinstance(template, StringPromptTemplate):
-                template_chat = template.format_prompt(**filtered_stub_inputs).to_messages()
-            else:
-                raise ValueError(f"Unknown template type {type(template)}")
-            template_chat = format_chat_template(template_chat)  # type: ignore
+            messages = util.format_chat_template_with_inputs(template, inputs)
+            json_messages = util.format_chat_template(messages)  # type: ignore
+            template_chat = util.replace_array_variables_with_placeholders(json_messages, inputs)
         return template_chat
 
     def _resolve_completion_template(self, run_id: UUID):
         """Resolve the template_chat into a list of dicts"""
         template = self._get_run_info(run_id, "prompt_template")
         inputs = self._get_run_info(run_id, "inputs")
         template_text: str | None = None
         if template and inputs:
-            stub_inputs = make_stub_inputs(inputs)
-            filtered_stub_inputs = {
-                k: v for k, v in stub_inputs.items() if k in template.input_variables
-            }
-            if isinstance(template, BaseChatPromptTemplate):
-                # We can't go through format_prompt because it doesn't like formatting the wrong types
-                template_text = template.format(**filtered_stub_inputs)
-            elif isinstance(template, StringPromptTemplate):
-                template_text = template.format_prompt(**filtered_stub_inputs).to_string()
-            else:
-                raise ValueError(f"Unknown template type {type(template)}")
+            template_text = util.format_completion_template_with_inputs(template, inputs)
             # template_text = format_chat_template(template_text)  # type: ignore
         return template_text
 
 
 def _extract_openai_params(serialized: Dict):
     return {k: v for k, v in serialized["kwargs"].items() if isinstance(v, (int, float, str, bool))}
```

### Comparing `im_openai-0.7.1/im_openai/langchain/patch.py` & `im_openai-0.7.2/im_openai/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/im_openai/patch.py` & `im_openai-0.7.2/im_openai/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import os
 from typing import Callable, List
 
-from openai import ChatCompletion, Completion
+import openai
 
 from .client import event_session
 
 
 def patch_openai_class(cls, get_prompt_template: Callable, get_result: Callable):
     oldcreate = cls.create
 
@@ -16,14 +16,15 @@
         ip_project_key=None,
         ip_api_name: str | None = None,
         ip_event_id: str | None = None,
         ip_template_text: str | None = None,
         ip_template_chat: List | None = None,
         ip_template_params=None,
         ip_chat_id: str | None = None,
+        ip_parent_event_id: str | None = None,
         **kwargs,
     ):
         if ip_project_key is None:
             ip_project_key = os.environ.get("PROMPT_PROJECT_KEY")
         if ip_project_key is None:
             return oldcreate(*args, **kwargs)
 
@@ -32,35 +33,38 @@
         if "messages" in kwargs:
             template_params = {}
             del model_params["messages"]
             model_params["modelType"] = "chat"
             for message in kwargs["messages"]:
                 if hasattr(message["content"], "template_args"):
                     template_params.update(message["content"].template_args)
-            ip_template_params = template_params
+            if ip_template_params is None:
+                ip_template_params = {}
+            ip_template_params.update(template_params)
         if "prompt" in kwargs:
             del model_params["prompt"]
             model_params["modelType"] = "completion"
 
         if ip_template_text is None and ip_template_chat is None:
             ip_template = get_prompt_template(*args, **kwargs)
             if isinstance(ip_template, str):
                 ip_template_text = ip_template
             elif isinstance(ip_template, list):
                 ip_template_chat = ip_template
 
         async with event_session(
             project_key=ip_project_key,
             api_name=ip_api_name,
+            model_params=model_params,
             prompt_template_text=ip_template_text,
             prompt_template_chat=ip_template_chat,
             chat_id=ip_chat_id,
             prompt_template_params=ip_template_params,
             prompt_event_id=ip_event_id,
-            model_params=model_params,
+            parent_event_id=ip_parent_event_id,
         ) as complete_event:
             response = oldcreate(*args, **kwargs)
             await complete_event(get_result(response))
         return response
 
     oldacreate = cls.acreate
 
@@ -91,24 +95,24 @@
 
     Returns a function which may be called to "unpatch" the APIs."""
 
     def get_completion_prompt(*args, prompt=None, **kwargs):
         return prompt
 
     unpatch_completion = patch_openai_class(
-        Completion, get_completion_prompt, lambda x: x["choices"][0]["text"]
+        openai.Completion, get_completion_prompt, lambda x: x["choices"][0]["text"]
     )
 
     def get_chat_prompt(*args, messages=None, **kwargs):
         # TODO: What should we be sending? For now we'll just send the last message
         prompt_text = messages
         return prompt_text
 
     unpatch_chat = patch_openai_class(
-        ChatCompletion,
+        openai.ChatCompletion,
         get_chat_prompt,
         lambda x: x["choices"][0]["message"]["content"],
     )
 
     def unpatch():
         unpatch_chat()
         unpatch_completion()
```

### Comparing `im_openai-0.7.1/im_openai/test_langchain_util.py` & `im_openai-0.7.2/tests/test_langchain.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.7.1/im_openai.egg-info/PKG-INFO` & `im_openai-0.7.2/im_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.7.1
+Version: 0.7.2
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `im_openai-0.7.1/im_openai.egg-info/SOURCES.txt` & `im_openai-0.7.2/im_openai.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,21 @@
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 im_openai/__init__.py
 im_openai/client.py
 im_openai/patch.py
 im_openai/template.py
-im_openai/test_langchain_util.py
 im_openai.egg-info/PKG-INFO
 im_openai.egg-info/SOURCES.txt
 im_openai.egg-info/dependency_links.txt
 im_openai.egg-info/not-zip-safe
 im_openai.egg-info/top_level.txt
 im_openai/langchain/__init__.py
 im_openai/langchain/callbacks.py
 im_openai/langchain/patch.py
 im_openai/langchain/util.py
 tests/__init__.py
-tests/test_im_openai.py
+tests/test_im_openai.py
+tests/test_langchain.py
+tests/test_langchain_util.py
+tests/test_patch.py
```

### Comparing `im_openai-0.7.1/setup.py` & `im_openai-0.7.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.7.1",
+    version="0.7.2",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.7.1/tests/test_im_openai.py` & `im_openai-0.7.2/tests/test_im_openai.py`

 * *Files identical despite different names*

