# Comparing `tmp/codeinterpreterapi-0.0.6.tar.gz` & `tmp/codeinterpreterapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.6.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.7.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.6.tar` & `codeinterpreterapi-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.6/LICENSE
--rw-r--r--   0        0        0     3513 2023-07-17 11:19:56.497686 codeinterpreterapi-0.0.6/README.md
--rw-r--r--   0        0        0      104 2023-07-16 13:21:57.042269 codeinterpreterapi-0.0.6/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.6/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     1578 2023-07-17 13:27:01.999997 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0      977 2023-07-17 11:28:50.790393 codeinterpreterapi-0.0.6/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      370 2023-07-17 13:25:52.072577 codeinterpreterapi-0.0.6/codeinterpreterapi/config.py
--rw-r--r--   0        0        0      225 2023-07-17 11:27:36.915415 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1379 2023-07-17 11:23:07.801403 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/modifications_check.py
--rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/remove_dl_link.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     2308 2023-07-16 23:45:20.639555 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.6/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     8129 2023-07-17 13:26:32.320429 codeinterpreterapi-0.0.6/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      629 2023-07-17 13:28:21.645307 codeinterpreterapi-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4288 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4364 2023-07-27 12:56:18.816462 codeinterpreterapi-0.0.7/README.md
+-rw-r--r--   0        0        0      104 2023-07-27 17:09:11.503788 codeinterpreterapi-0.0.7/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-27 17:09:11.504081 codeinterpreterapi-0.0.7/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-27 17:09:11.504186 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     1578 2023-07-27 17:09:11.504417 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0      977 2023-07-27 17:09:11.504941 codeinterpreterapi-0.0.7/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      390 2023-07-17 19:38:21.218647 codeinterpreterapi-0.0.7/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0      225 2023-07-17 11:27:36.915415 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1379 2023-07-17 11:23:07.801403 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/modifications_check.py
+-rw-r--r--   0        0        0      959 2023-07-17 11:26:26.313924 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/remove_dl_link.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2385 2023-07-27 12:56:18.814797 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.7/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     8266 2023-07-27 17:11:47.122779 codeinterpreterapi-0.0.7/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      686 2023-07-27 17:16:10.970203 codeinterpreterapi-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5259 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.7/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.6/LICENSE` & `codeinterpreterapi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/README.md` & `codeinterpreterapi-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 async def main():
     # create a session
     session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
-    output = await session.generate_response(
+    response = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
 
-    # ouput the response (text + image)
+    # output the response (text + image)
     print("AI: ", response.content)
     for file in response.files:
         file.show_image()
 
     # terminate the session
     await session.astop()
-    
+
 
 if __name__ == "__main__":
     import asyncio
     # run the async function
     asyncio.run(main())
 
 ```
@@ -69,15 +69,15 @@
     # context manager for auto start/stop of the session
     async with CodeInterpreterSession() as session:
         # define the user request
         user_request = "Analyze this dataset and plot something interesting about it."
         files = [
             File.from_path("examples/assets/iris.csv"),
         ]
-        
+
         # generate the response
         response = await session.generate_response(
             user_request, files=files
         )
 
         # output to the user
         print("AI: ", response.content)
@@ -92,32 +92,54 @@
 ```
 
 ![Iris Dataset Analysis](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/iris_analysis.png?raw=true)  
 Iris Dataset Analysis Output
 
 ## Production
 
-In case you want to deploy to production you can use the CodeBox API for easy scaling.
+In case you want to deploy to production, you can utilize the CodeBox API for seamless scalability.
 
-Please contact me if you interested in this, because it's still in early development.
+Please contact me if you are interested in this, as it is still in the early stages of development.
 
 ## Contributing
 
-There are some TODOs left in the code
-so if you want to contribute feel free to do so.
+There are some remaining TODOs in the code.
+So, if you want to contribute, feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue or pull request and I will review it.
 
-Also please submit any bugs you find as an issue
-with a minimal code example or screenshot.
-This helps me a lot to improve the code.
+Please also submit any bugs you find as an issue with a minimal code example or screenshot.
+This helps me a lot in improving the code.
 
 Thanks!
 
+## Streamlit WebApp
+
+To start the web application created with streamlit:
+
+```bash
+streamlit run frontend/app.py
+```
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
 But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
+
+## Support this project
+
+If you would like to help this project with a donation, you can [click here](https://ko-fi.com/shroominic).
+Thanks, this helps a lot! ❤️
+
+## Star History
+
+<a href="https://star-history.com/#shroominic/codeinterpreter-api&Date">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date" />
+    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date" />
+  </picture>
+</a>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/chains/remove_download_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/modifications_check.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/remove_dl_link.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/remove_dl_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/schema/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def save(self, path: str):
         with open(path, "wb") as f:
             f.write(self.content)
 
     async def asave(self, path: str):
         await asyncio.to_thread(self.save, path)
 
-    def show_image(self):
+    def get_image(self):
         try:
             from PIL import Image  # type: ignore
         except ImportError:
             print(
                 "Please install it with `pip install codeinterpreterapi[image_support]` to display images."
             )
             exit(1)
@@ -52,14 +52,19 @@
         img_io = BytesIO(self.content)
         img = Image.open(img_io)
 
         # Convert image to RGB if it's not
         if img.mode not in ('RGB', 'L'):  # L is for greyscale images
             img = img.convert('RGB')
 
+        return img
+
+    def show_image(self):
+        img = self.get_image()
+
         # Display the image
         try:
             # Try to get the IPython shell if available.
             shell = get_ipython().__class__.__name__  # type: ignore
 
             # If the shell is ZMQInteractiveShell, it means we're in a Jupyter notebook or similar.
             if shell == 'ZMQInteractiveShell':
```

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/schema/response.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.6/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.7/codeinterpreterapi/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import uuid, base64, re
 from io import BytesIO
 from typing import Optional
 from codeboxapi import CodeBox  # type: ignore
 from codeboxapi.schema import CodeBoxOutput  # type: ignore
-from langchain.tools import StructuredTool
+from langchain.tools import StructuredTool, BaseTool
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.prompts.chat import MessagesPlaceholder
 from langchain.agents import AgentExecutor, BaseSingleActionAgent
 from langchain.memory import ConversationBufferMemory
 
 from codeinterpreterapi.schema import CodeInterpreterResponse, CodeInput, File, UserRequest
@@ -16,49 +16,59 @@
 from codeinterpreterapi.prompts import code_interpreter_system_message
 from codeinterpreterapi.callbacks import CodeCallbackHandler
 from codeinterpreterapi.chains.modifications_check import get_file_modifications
 from codeinterpreterapi.chains.remove_download_link import remove_download_link
 
 
 class CodeInterpreterSession:
-    def __init__(self, model=None, openai_api_key=None) -> None:
+    def __init__(
+        self,
+        model="gpt-4",
+        openai_api_key=settings.OPENAI_API_KEY,
+        verbose=settings.VERBOSE,
+        tools: list[BaseTool] = [],
+    ) -> None:
         self.codebox = CodeBox()
-        self.tools: list[StructuredTool] = self._tools()
+        self.verbose = verbose
+        self.tools: list[BaseTool] = self._tools(tools)
         self.llm: BaseChatModel = self._llm(model, openai_api_key)
         self.agent_executor: AgentExecutor = self._agent_executor()
         self.input_files: list[File] = []
         self.output_files: list[File] = []
-    
+
     async def astart(self) -> None:
         await self.codebox.astart()
 
-    def _tools(self) -> list[StructuredTool]:
-        return [
+    def _tools(
+        self, 
+        additional_tools: list[BaseTool]
+    ) -> list[BaseTool]:
+        return additional_tools + [
             StructuredTool(
                 name="python",
                 description=
                 # TODO: variables as context to the agent
                 # TODO: current files as context to the agent
                 "Input a string of code to a python interpreter (jupyter kernel). "
                 "Variables are preserved between runs. ",
                 func=self.run_handler,
                 coroutine=self.arun_handler,
                 args_schema=CodeInput,
             ),
         ]
 
-    def _llm(self, model: Optional[str] = None, openai_api_key: Optional[str] = None) -> BaseChatModel:
-        if model is None:
-            model = "gpt-4"
-
+    def _llm(
+        self, 
+        model: str, 
+        openai_api_key: Optional[str] = None
+    ) -> BaseChatModel:
         if openai_api_key is None:
-            if settings.OPENAI_API_KEY is None:
-                raise ValueError("OpenAI API key missing.")
-            else:
-                openai_api_key = settings.OPENAI_API_KEY
+            raise ValueError(
+                "OpenAI API key missing. Set OPENAI_API_KEY env variable or pass `openai_api_key` to session."
+            )
 
         return ChatOpenAI(
             temperature=0.03,
             model=model,
             openai_api_key=openai_api_key,
             max_retries=3,
             request_timeout=60 * 3,
@@ -74,21 +84,21 @@
 
     def _agent_executor(self) -> AgentExecutor:
         return AgentExecutor.from_agent_and_tools(
             agent=self._agent(),
             callbacks=[CodeCallbackHandler(self)],
             max_iterations=9,
             tools=self.tools,
-            verbose=settings.VERBOSE,
+            verbose=self.verbose,
             memory=ConversationBufferMemory(memory_key="memory", return_messages=True),
         )
 
     async def show_code(self, code: str) -> None:
         """Callback function to show code to the user."""
-        if settings.VERBOSE:
+        if self.verbose:
             print(code)
 
     def run_handler(self, code: str):
         raise NotImplementedError("Use arun_handler for now.")
 
     async def arun_handler(self, code: str):
         """Run code in container and send the output to the user"""
@@ -109,15 +119,15 @@
                 if package := re.search(
                     r"ModuleNotFoundError: No module named '(.*)'", output.content
                 ):
                     await self.codebox.ainstall(package.group(1))
                     return f"{package.group(1)} was missing but got installed now. Please try again."
             else: pass
                 # TODO: preanalyze error to optimize next code generation
-            if settings.VERBOSE:
+            if self.verbose:
                 print("Error:", output.content)
 
         elif modifications := await get_file_modifications(code, self.llm):
             for filename in modifications:
                 if filename in [file.name for file in self.input_files]:
                     continue
                 fileb = await self.codebox.adownload(filename)
@@ -166,15 +176,15 @@
         """Generate a Code Interpreter response based on the user's input."""
         user_request = UserRequest(content=user_msg, files=files)
         try:
             await self.input_handler(user_request)
             response = await self.agent_executor.arun(input=user_request.content)
             return await self.output_handler(response)
         except Exception as e:
-            if settings.VERBOSE:
+            if self.verbose:
                 import traceback
 
                 traceback.print_exc()
             if detailed_error:
                 return CodeInterpreterResponse(
                     content=f"Error in CodeInterpreterSession: {e.__class__.__name__}  - {e}"
                 )
@@ -182,17 +192,17 @@
                 return CodeInterpreterResponse(
                     content="Sorry, something went while generating your response."
                     "Please try again or restart the session."
                 )
 
     async def is_running(self) -> bool:
         return await self.codebox.astatus() == "running"
-    
+
     async def astop(self) -> None:
         await self.codebox.astop()
-    
+
     async def __aenter__(self) -> "CodeInterpreterSession":
         await self.astart()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self.astop()
```

### Comparing `codeinterpreterapi-0.0.6/PKG-INFO` & `codeinterpreterapi-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.6
+Version: 0.0.7
 Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
-Requires-Dist: codeboxapi (>=0.0.8,<0.0.9)
+Provides-Extra: streamlit-support
+Requires-Dist: codeboxapi (>=0.0.9,<0.0.10)
 Requires-Dist: langchain (>=0.0.232,<0.0.233)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
@@ -52,26 +53,26 @@
 
 async def main():
     # create a session
     session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
-    output = await session.generate_response(
+    response = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
 
-    # ouput the response (text + image)
+    # output the response (text + image)
     print("AI: ", response.content)
     for file in response.files:
         file.show_image()
 
     # terminate the session
     await session.astop()
-    
+
 
 if __name__ == "__main__":
     import asyncio
     # run the async function
     asyncio.run(main())
 
 ```
@@ -89,15 +90,15 @@
     # context manager for auto start/stop of the session
     async with CodeInterpreterSession() as session:
         # define the user request
         user_request = "Analyze this dataset and plot something interesting about it."
         files = [
             File.from_path("examples/assets/iris.csv"),
         ]
-        
+
         # generate the response
         response = await session.generate_response(
             user_request, files=files
         )
 
         # output to the user
         print("AI: ", response.content)
@@ -112,33 +113,55 @@
 ```
 
 ![Iris Dataset Analysis](https://github.com/shroominic/codeinterpreter-api/blob/main/examples/assets/iris_analysis.png?raw=true)  
 Iris Dataset Analysis Output
 
 ## Production
 
-In case you want to deploy to production you can use the CodeBox API for easy scaling.
+In case you want to deploy to production, you can utilize the CodeBox API for seamless scalability.
 
-Please contact me if you interested in this, because it's still in early development.
+Please contact me if you are interested in this, as it is still in the early stages of development.
 
 ## Contributing
 
-There are some TODOs left in the code
-so if you want to contribute feel free to do so.
+There are some remaining TODOs in the code.
+So, if you want to contribute, feel free to do so.
 You can also suggest new features. Code refactoring is also welcome.
 Just open an issue or pull request and I will review it.
 
-Also please submit any bugs you find as an issue
-with a minimal code example or screenshot.
-This helps me a lot to improve the code.
+Please also submit any bugs you find as an issue with a minimal code example or screenshot.
+This helps me a lot in improving the code.
 
 Thanks!
 
+## Streamlit WebApp
+
+To start the web application created with streamlit:
+
+```bash
+streamlit run frontend/app.py
+```
+
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Contact
 
 You can contact me at [contact@shroominic.com](mailto:contact@shroominic.com).
 But I prefer to use [Twitter](https://twitter.com/shroominic) or [Discord](https://gptassistant.app/community) DMs.
 
+## Support this project
+
+If you would like to help this project with a donation, you can [click here](https://ko-fi.com/shroominic).
+Thanks, this helps a lot! ❤️
+
+## Star History
+
+<a href="https://star-history.com/#shroominic/codeinterpreter-api&Date">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date&theme=dark" />
+    <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date" />
+    <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=shroominic/codeinterpreter-api&type=Date" />
+  </picture>
+</a>
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

