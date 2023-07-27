# Comparing `tmp/autopack_tools-0.4.0.tar.gz` & `tmp/autopack_tools-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.4.0.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.1.tar", max compression
```

## Comparing `autopack_tools-0.4.0.tar` & `autopack_tools-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.0/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.0/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.0/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.0/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.0/autopack/__main__.py
--rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.0/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.0/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.0/autopack/errors.py
--rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.0/autopack/filesystem_emulation/__init__.py
--rw-r--r--   0        0        0      846 2023-07-25 03:23:45.618298 autopack_tools-0.4.0/autopack/filesystem_emulation/file_manager.py
--rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.0/autopack/filesystem_emulation/filesystem_file_manager.py
--rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.0/autopack/filesystem_emulation/ram_file_manager.py
--rw-r--r--   0        0        0     4007 2023-07-25 02:59:52.529969 autopack_tools-0.4.0/autopack/filesystem_emulation/workspace_file_manager.py
--rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.0/autopack/get_pack.py
--rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.0/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.0/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5246 2023-07-25 05:27:49.353417 autopack_tools-0.4.0/autopack/pack.py
--rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.0/autopack/pack_config.py
--rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.0/autopack/pack_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.0/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.0/autopack/search.py
--rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.0/autopack/selection.py
--rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.0/autopack/utils.py
--rw-r--r--   0        0        0     1101 2023-07-27 03:29:22.515982 autopack_tools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.1/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.1/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.1/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.1/autopack/__main__.py
+-rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.1/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.1/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.1/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.1/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-27 03:50:15.932646 autopack_tools-0.4.1/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.1/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.1/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     4007 2023-07-25 02:59:52.529969 autopack_tools-0.4.1/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.1/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.1/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.1/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5529 2023-07-27 04:17:12.352396 autopack_tools-0.4.1/autopack/pack.py
+-rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.1/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.1/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.1/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.1/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.1/autopack/selection.py
+-rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.1/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-07-27 04:17:31.593863 autopack_tools-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.1/PKG-INFO
```

### Comparing `autopack_tools-0.4.0/LICENSE` & `autopack_tools-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/README.md` & `autopack_tools-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/api.py` & `autopack_tools-0.4.1/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/cli.py` & `autopack_tools-0.4.1/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/filesystem_emulation/file_manager.py` & `autopack_tools-0.4.1/autopack/filesystem_emulation/file_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,13 +19,17 @@
         pass
 
     @abstractmethod
     def write_file(self, file_path: str, content: str) -> str:
         pass
 
     @abstractmethod
+    async def awrite_file(self, file_path: str, content: str) -> str:
+        pass
+
+    @abstractmethod
     def delete_file(self, file_path: str) -> str:
         pass
 
     @abstractmethod
     def list_files(self, dir_path: str) -> str:
         pass
```

### Comparing `autopack_tools-0.4.0/autopack/filesystem_emulation/filesystem_file_manager.py` & `autopack_tools-0.4.1/autopack/filesystem_emulation/filesystem_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/filesystem_emulation/ram_file_manager.py` & `autopack_tools-0.4.1/autopack/filesystem_emulation/ram_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/filesystem_emulation/workspace_file_manager.py` & `autopack_tools-0.4.1/autopack/filesystem_emulation/workspace_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/get_pack.py` & `autopack_tools-0.4.1/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/installation.py` & `autopack_tools-0.4.1/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/langchain_wrapper.py` & `autopack_tools-0.4.1/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/pack.py` & `autopack_tools-0.4.1/autopack/pack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
 from asyncio import iscoroutinefunction
 from typing import ClassVar, Optional, Callable, Coroutine, Any, Union
 
 from pydantic import BaseModel, ValidationError, Field
 
+from autopack.filesystem_emulation.file_manager import FileManager
 from autopack.pack_config import PackConfig
 from autopack.utils import run_args_from_args_schema, acall_llm, call_llm
 
 
 class Pack(BaseModel):
     class Config:
         arbitrary_types_allowed = True
@@ -34,18 +35,21 @@
 
     llm: Optional[Callable[[str], str]] = Field(
         None, description="A callable function to call an LLM (string in string out)"
     )
     allm: Union[None, Callable[[str], str], Coroutine[Any, Any, str]] = Field(
         None, description="An asynchronous callable function to call an LLM (string in string out)"
     )
-    config: PackConfig = Field(default=PackConfig.global_config)
+    config: PackConfig = Field(default_factory=PackConfig.global_config)
 
     def __init__(self, **data):
         super().__init__(**data)
+        if not self.config.filesystem_manager:
+            self.config.init_filesystem_manager()
+
         if self.llm and not callable(self.llm):
             raise TypeError(f"LLM object {self.llm} must be callable")
 
         if self.allm and not iscoroutinefunction(self.allm):
             raise TypeError(f"Async LLM object {self.llm} must be async and callable")
 
         if self.name is None:
@@ -114,14 +118,18 @@
         return call_llm(prompt, self.llm)
 
     async def acall_llm(self, prompt: str) -> str:
         if self.allm is None:
             return self.call_llm(prompt)
         return await acall_llm(prompt, self.allm)
 
+    @property
+    def filesystem_manager(self) -> FileManager:
+        return self.config.filesystem_manager
+
     def validate_tool_args(self, **kwargs):
         """Validate the arguments against the args_schema model.
 
         Args:
             kwargs (dict[str, Any]): The arguments to validate.
         Returns:
             True if the arguments are valid.
```

### Comparing `autopack_tools-0.4.0/autopack/pack_config.py` & `autopack_tools-0.4.1/autopack/pack_config.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/prompts.py` & `autopack_tools-0.4.1/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/selection.py` & `autopack_tools-0.4.1/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/autopack/utils.py` & `autopack_tools-0.4.1/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.0/pyproject.toml` & `autopack_tools-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.4.0"
+version = "0.4.1"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.4.0/PKG-INFO` & `autopack_tools-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.4.0
+Version: 0.4.1
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

