# Comparing `tmp/autopack_tools-0.3.4.tar.gz` & `tmp/autopack_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.3.4.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.0.tar", max compression
```

## Comparing `autopack_tools-0.3.4.tar` & `autopack_tools-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.3.4/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.3.4/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.3.4/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.3.4/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.3.4/autopack/__main__.py
--rw-r--r--   0        0        0     2869 2023-07-23 21:13:30.082198 autopack_tools-0.3.4/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.3.4/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.3.4/autopack/errors.py
--rw-r--r--   0        0        0     2464 2023-07-23 22:09:39.852735 autopack_tools-0.3.4/autopack/get_pack.py
--rw-r--r--   0        0        0     3935 2023-07-23 04:34:40.466812 autopack_tools-0.3.4/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.3.4/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5173 2023-07-23 22:31:30.673220 autopack_tools-0.3.4/autopack/pack.py
--rw-r--r--   0        0        0      276 2023-07-23 21:19:00.939247 autopack_tools-0.3.4/autopack/pack_response.py
--rw-r--r--   0        0        0      393 2023-07-22 23:02:14.133585 autopack_tools-0.3.4/autopack/pack_search_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.3.4/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.3.4/autopack/search.py
--rw-r--r--   0        0        0     3335 2023-07-23 22:12:19.940610 autopack_tools-0.3.4/autopack/selection.py
--rw-r--r--   0        0        0     7904 2023-07-23 05:25:55.315020 autopack_tools-0.3.4/autopack/utils.py
--rw-r--r--   0        0        0     1080 2023-07-23 22:31:44.689747 autopack_tools-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2897 1970-01-01 00:00:00.000000 autopack_tools-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.0/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.0/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.0/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.0/autopack/__main__.py
+-rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.0/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.0/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.0/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.0/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0      846 2023-07-25 03:23:45.618298 autopack_tools-0.4.0/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.0/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.0/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     4007 2023-07-25 02:59:52.529969 autopack_tools-0.4.0/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.0/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.0/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.0/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5246 2023-07-25 05:27:49.353417 autopack_tools-0.4.0/autopack/pack.py
+-rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.0/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.0/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.0/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.0/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.0/autopack/selection.py
+-rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.0/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-07-27 03:29:22.515982 autopack_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.0/PKG-INFO
```

### Comparing `autopack_tools-0.3.4/LICENSE` & `autopack_tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.4/README.md` & `autopack_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.4/autopack/api.py` & `autopack_tools-0.4.0/autopack/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from urllib.parse import urljoin
 
 import requests
 from marshmallow import ValidationError
 
 from autopack.errors import AutoPackFetchError
 from autopack.pack_response import PackResponse
-from autopack.pack_search_response import PackSearchResponse
 from autopack.utils import find_or_create_autopack_dir
 
 API_URL = os.environ.get("AUTOPACK_API_URL", "https://autopack.ai/")
 
 
 def get_pack_details(pack_id: str, remote=False) -> PackResponse:
     if remote:
@@ -60,25 +59,25 @@
 
     elif response.status_code <= 500:
         raise AutoPackFetchError(f"Error: {response.status_code}")
     else:
         raise AutoPackFetchError(f"Error: {response.status_code}")
 
 
-def pack_search(query: str) -> list[PackSearchResponse]:
+def pack_search(query: str) -> list[PackResponse]:
     endpoint = "/api/search"
     url = urljoin(API_URL, endpoint)
     params = {"query": query}
 
     response = requests.get(url, params=params)
     if response.status_code == 200:
         data = response.json()
 
         try:
-            return [PackSearchResponse(**datum) for datum in data["packs"]]
+            return [PackResponse(**datum) for datum in data["packs"]]
         except (ValidationError, TypeError) as e:
             message = f"Pack fetch received invalid data: {e}"
             print(message)
             raise AutoPackFetchError(message)
 
     elif response.status_code <= 500:
         print(f"Error: {response.status_code}")
```

### Comparing `autopack_tools-0.3.4/autopack/cli.py` & `autopack_tools-0.4.0/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.4/autopack/installation.py` & `autopack_tools-0.4.0/autopack/installation.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from git import Repo
 
 from autopack.api import PackResponse, get_pack_details
 from autopack.errors import AutoPackError, AutoPackInstallationError
 from autopack.get_pack import try_get_pack, get_pack
 from autopack.pack import Pack
+from autopack.pack_config import PackConfig
 from autopack.utils import (
     find_or_create_autopack_dir,
     load_metadata_file,
     write_metadata_file,
     extract_unique_directory_name,
 )
 
@@ -78,15 +79,15 @@
 def update_metadata_file(pack_id: str, pack_response: PackResponse):
     metadata = load_metadata_file()
     metadata[pack_id] = pack_response.__dict__
 
     write_metadata_file(metadata)
 
 
-def install_pack(pack_id: str, force_dependencies=False, quiet=True) -> type[Pack]:
+def install_pack(pack_id: str, quiet=True, config: PackConfig = PackConfig.global_config()) -> type[Pack]:
     if not quiet:
         print(f"Installing pack: {pack_id}")
 
     find_or_create_autopack_dir()
 
     pack = try_get_pack(pack_id)
     if pack:
@@ -109,15 +110,17 @@
         git_dir = install_from_git(pack_data, quiet=quiet)
 
         update_metadata_file(pack_id, pack_data)
         pack = get_pack(pack_id)
 
         if pack:
             if pack.dependencies:
-                ask_to_install_dependencies(pack.dependencies, force=force_dependencies, quiet=quiet)
+                ask_to_install_dependencies(
+                    pack.dependencies, force=config.automatically_install_dependencies, quiet=quiet
+                )
             return pack
     except Exception as e:
         raise AutoPackInstallationError(f"Couldn't install pack due to error {e}")
 
     # Clean up bad repo directories to make sure there aren't bad packs in the .autopack dir
     if git_dir and os.path.isdir(git_dir):
         shutil.rmtree(git_dir)
```

### Comparing `autopack_tools-0.3.4/autopack/langchain_wrapper.py` & `autopack_tools-0.4.0/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.4/autopack/pack.py` & `autopack_tools-0.4.0/autopack/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from abc import abstractmethod
 from asyncio import iscoroutinefunction
 from typing import ClassVar, Optional, Callable, Coroutine, Any, Union
 
 from pydantic import BaseModel, ValidationError, Field
 
+from autopack.pack_config import PackConfig
 from autopack.utils import run_args_from_args_schema, acall_llm, call_llm
 
 
 class Pack(BaseModel):
-    arbitrary_types_allowed = True
-
     class Config:
         arbitrary_types_allowed = True
 
     ## Required
 
     # The name of the tool that will be provided to the LLM
     name: ClassVar[str]
@@ -35,14 +34,15 @@
 
     llm: Optional[Callable[[str], str]] = Field(
         None, description="A callable function to call an LLM (string in string out)"
     )
     allm: Union[None, Callable[[str], str], Coroutine[Any, Any, str]] = Field(
         None, description="An asynchronous callable function to call an LLM (string in string out)"
     )
+    config: PackConfig = Field(default=PackConfig.global_config)
 
     def __init__(self, **data):
         super().__init__(**data)
         if self.llm and not callable(self.llm):
             raise TypeError(f"LLM object {self.llm} must be callable")
 
         if self.allm and not iscoroutinefunction(self.allm):
```

### Comparing `autopack_tools-0.3.4/autopack/prompts.py` & `autopack_tools-0.4.0/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.3.4/autopack/selection.py` & `autopack_tools-0.4.0/autopack/selection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,79 @@
 import re
 from typing import Callable, Union, Optional
 
 from langchain.chat_models.base import BaseChatModel
 
 from autopack import Pack
-from autopack.get_pack import get_all_installed_packs
+from autopack.get_pack import get_all_installed_packs, get_all_pack_info
+from autopack.pack_config import PackConfig, InstallerStyle
+from autopack.pack_response import PackResponse
 from autopack.prompts import GET_MORE_TOOLS_TEMPLATE, TOOL_SELECTION_TEMPLATE
-from autopack.utils import functions_bulleted_list, call_llm
+from autopack.utils import call_llm
 
 
-def select_packs_prompt(task_description: str, function_request: Optional[str] = None) -> str:
+def functions_bulleted_list(packs: list[PackResponse]) -> str:
+    functions_string = []
+    grouped_packs: dict[str, list[type[PackResponse]]] = {}
+    for pack in packs:
+        if not pack.categories:
+            continue
+
+        for category in pack.categories:
+            if category not in grouped_packs:
+                grouped_packs[category] = []
+            grouped_packs[category].append(pack)
+
+    for category, category_packs in grouped_packs.items():
+        functions_string.append(f"\n## {category}")
+        sorted_by_name = sorted(category_packs, key=lambda p: p.name)
+        for pack in sorted_by_name:
+            args = pack.run_args
+            args_signature = ", ".join([f"{arg.get('name')}: {arg.get('type')}" for arg in args.values()])
+            args_descriptions = (
+                "; ".join([f"{arg.get('name')} ({arg.get('type')}): {arg.get('description')}" for arg in args.values()])
+                or "None."
+            )
+            functions_string.append(
+                f"- {pack.name}({args_signature}): {pack.description} | Arguments: {args_descriptions}"
+            )
+
+    return "\n".join(functions_string)
+
+
+def select_packs_prompt(
+    packs: list[Union[Pack, PackResponse]], task_description: str, function_request: Optional[str] = None
+) -> str:
     """
     Generate a prompt for the pack selection process based on the task description and an optional function request.
 
     Args:
+        packs: (list[Pack | PackResponse]): Packs to include in selection
         task_description (str): A description of the task to be used when selecting tools.
         function_request (Optional[str]): A specific type of function asked for (e.g. a `get_more_tools` function).
 
     Returns:
         str: A prompt that can be fed to the LLM for pack selection.
     """
 
-    installed_packs = get_all_installed_packs()
-
     if function_request:
-        return TOOL_SELECTION_TEMPLATE.format(task=task_description, functions=functions_bulleted_list(installed_packs))
+        return TOOL_SELECTION_TEMPLATE.format(task=task_description, functions=functions_bulleted_list(packs))
 
     return GET_MORE_TOOLS_TEMPLATE.format(
         task=task_description,
-        functions=functions_bulleted_list(installed_packs),
+        functions=functions_bulleted_list(packs),
         functions_request=function_request,
     )
 
 
 def select_packs(
     task_description: str,
     llm: Union[BaseChatModel, Callable],
     function_request: Optional[str] = None,
+    config: PackConfig = PackConfig.global_config(),
 ) -> list[type[Pack]]:
     """Given a user input describing the task they wish to accomplish, return a list of Pack IDs that the given LLM
     thinks will be suitable for this task.
 
     This is good for a "pre-processing" step after receiving the task but before trying to solve it. This allows you
     to benefit from the wide tool selection while keeping your token usage low.
 
@@ -48,19 +81,26 @@
 
     # TODO: Include user-provided packs into selection
 
     Args:
         task_description (str): A description of the task to be used when selecting tools
         llm (BaseChatModel): An LLM which will be used to evaluate the selection
         function_request (Optional[str]): A specific type of function asked for (e.g. a `get_more_tools` function)
+        config (PackConfig): Custom config to use
 
     Returns:
         list[str]: A list of selected Pack IDs
     """
-    prompt = select_packs_prompt(task_description, function_request)
+
+    if config.installer_style == InstallerStyle.manual:
+        selection_pool = get_all_installed_packs()
+    else:
+        selection_pool = get_all_pack_info()
+
+    prompt = select_packs_prompt(selection_pool, task_description, function_request)
 
     response = call_llm(prompt, llm)
 
     return parse_selection_response(response)
 
 
 def parse_selection_response(response: str) -> list[type[Pack]]:
@@ -72,14 +112,15 @@
     Args:
         response (str): The response from the LLM.
 
     Returns:
         list[str]: A list of parsed pack IDs.
     """
     pack_names = [r.split("(")[0].strip() for r in re.split(r"(?<=\w),|\n", response)]
+
     installed_packs = get_all_installed_packs()
     selected_packs = []
     for pack_name in pack_names:
         try:
             selected_pack = next(pack for pack in installed_packs if pack.name == pack_name)
             selected_packs.append(selected_pack)
         except StopIteration:
```

### Comparing `autopack_tools-0.3.4/autopack/utils.py` & `autopack_tools-0.4.0/autopack/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import json
 import os
 import re
 import sys
 from asyncio import iscoroutinefunction
 from json import JSONDecodeError
 from types import ModuleType
-from typing import TYPE_CHECKING, Any, Callable, Union, Coroutine
+from typing import Callable
+from typing import TYPE_CHECKING, Any, Union, Coroutine
 
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import SystemMessage, BaseMessage
 from pydantic import BaseModel
 
 from autopack.errors import AutoPackLoadError
 from autopack.pack_response import PackResponse
```

### Comparing `autopack_tools-0.3.4/pyproject.toml` & `autopack_tools-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.3.4"
+version = "0.4.0"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
@@ -16,14 +16,15 @@
 python = ">=3.8.1,<4.0"
 requests = "^2.31.0"
 dataclasses-json = "^0.5.8"
 urllib3 = "^1.26.16"
 gitpython = "^3.1.31"
 langchain = ">=0.0.215"
 types-requests = "^2.31.0.2"
+aiofiles = "^23.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.4.0"
 isort = "^5.12.0"
 pytest = "^7.3.2"
```

### Comparing `autopack_tools-0.3.4/PKG-INFO` & `autopack_tools-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.3.4
+Version: 0.4.0
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: dataclasses-json (>=0.5.8,<0.6.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: langchain (>=0.0.215)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: types-requests (>=2.31.0.2,<3.0.0.0)
 Requires-Dist: urllib3 (>=1.26.16,<2.0.0)
 Project-URL: Repository, https://github.com/AutoPackAI/autopack
```

