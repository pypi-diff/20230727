# Comparing `tmp/autopack_tools-0.4.2.tar.gz` & `tmp/autopack_tools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopack_tools-0.4.2.tar", max compression
+gzip compressed data, was "autopack_tools-0.4.3.tar", max compression
```

## Comparing `autopack_tools-0.4.2.tar` & `autopack_tools-0.4.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.2/LICENSE
--rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.2/README.md
--rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.2/autopack/VERSION
--rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.2/autopack/__init__.py
--rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.2/autopack/__main__.py
--rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.2/autopack/api.py
--rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.2/autopack/cli.py
--rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.2/autopack/errors.py
--rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.2/autopack/filesystem_emulation/__init__.py
--rw-r--r--   0        0        0      950 2023-07-27 03:50:15.932646 autopack_tools-0.4.2/autopack/filesystem_emulation/file_manager.py
--rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.2/autopack/filesystem_emulation/filesystem_file_manager.py
--rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.2/autopack/filesystem_emulation/ram_file_manager.py
--rw-r--r--   0        0        0     4009 2023-07-27 04:24:15.003834 autopack_tools-0.4.2/autopack/filesystem_emulation/workspace_file_manager.py
--rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.2/autopack/get_pack.py
--rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.2/autopack/installation.py
--rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.2/autopack/langchain_wrapper.py
--rw-r--r--   0        0        0     5529 2023-07-27 04:17:12.352396 autopack_tools-0.4.2/autopack/pack.py
--rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.2/autopack/pack_config.py
--rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.2/autopack/pack_response.py
--rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.2/autopack/prompts.py
--rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.2/autopack/search.py
--rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.2/autopack/selection.py
--rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.2/autopack/utils.py
--rw-r--r--   0        0        0     1101 2023-07-27 04:24:25.640424 autopack_tools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-25 23:21:07.938011 autopack_tools-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2050 2023-07-23 21:43:01.334058 autopack_tools-0.4.3/README.md
+-rw-r--r--   0        0        0        6 2023-06-25 23:21:01.956323 autopack_tools-0.4.3/autopack/VERSION
+-rw-r--r--   0        0        0       51 2023-07-22 21:10:26.696185 autopack_tools-0.4.3/autopack/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-25 23:21:01.956609 autopack_tools-0.4.3/autopack/__main__.py
+-rw-r--r--   0        0        0     2796 2023-07-27 03:21:43.783559 autopack_tools-0.4.3/autopack/api.py
+-rw-r--r--   0        0        0     1091 2023-07-22 21:45:58.090041 autopack_tools-0.4.3/autopack/cli.py
+-rw-r--r--   0        0        0      317 2023-07-22 20:36:24.222128 autopack_tools-0.4.3/autopack/errors.py
+-rw-r--r--   0        0        0        0 2023-07-25 02:09:27.676019 autopack_tools-0.4.3/autopack/filesystem_emulation/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-27 03:50:15.932646 autopack_tools-0.4.3/autopack/filesystem_emulation/file_manager.py
+-rw-r--r--   0        0        0     3562 2023-07-25 02:59:38.942285 autopack_tools-0.4.3/autopack/filesystem_emulation/filesystem_file_manager.py
+-rw-r--r--   0        0        0     2985 2023-07-25 03:00:14.263556 autopack_tools-0.4.3/autopack/filesystem_emulation/ram_file_manager.py
+-rw-r--r--   0        0        0     4052 2023-07-27 04:47:20.015891 autopack_tools-0.4.3/autopack/filesystem_emulation/workspace_file_manager.py
+-rw-r--r--   0        0        0     3199 2023-07-27 03:24:17.192602 autopack_tools-0.4.3/autopack/get_pack.py
+-rw-r--r--   0        0        0     4063 2023-07-25 03:31:18.589959 autopack_tools-0.4.3/autopack/installation.py
+-rw-r--r--   0        0        0      746 2023-07-23 22:31:15.553932 autopack_tools-0.4.3/autopack/langchain_wrapper.py
+-rw-r--r--   0        0        0     5529 2023-07-27 04:17:12.352396 autopack_tools-0.4.3/autopack/pack.py
+-rw-r--r--   0        0        0     3159 2023-07-27 03:21:07.242026 autopack_tools-0.4.3/autopack/pack_config.py
+-rw-r--r--   0        0        0      502 2023-07-27 03:28:19.065203 autopack_tools-0.4.3/autopack/pack_response.py
+-rw-r--r--   0        0        0     2217 2023-07-22 21:58:39.610211 autopack_tools-0.4.3/autopack/prompts.py
+-rw-r--r--   0        0        0      394 2023-07-22 23:03:16.870292 autopack_tools-0.4.3/autopack/search.py
+-rw-r--r--   0        0        0     4930 2023-07-27 03:27:48.430037 autopack_tools-0.4.3/autopack/selection.py
+-rw-r--r--   0        0        0     7922 2023-07-25 05:47:59.042910 autopack_tools-0.4.3/autopack/utils.py
+-rw-r--r--   0        0        0     1101 2023-07-27 04:54:38.971302 autopack_tools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 autopack_tools-0.4.3/PKG-INFO
```

### Comparing `autopack_tools-0.4.2/LICENSE` & `autopack_tools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/README.md` & `autopack_tools-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/api.py` & `autopack_tools-0.4.3/autopack/api.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/cli.py` & `autopack_tools-0.4.3/autopack/cli.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/filesystem_emulation/file_manager.py` & `autopack_tools-0.4.3/autopack/filesystem_emulation/file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/filesystem_emulation/filesystem_file_manager.py` & `autopack_tools-0.4.3/autopack/filesystem_emulation/filesystem_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/filesystem_emulation/ram_file_manager.py` & `autopack_tools-0.4.3/autopack/filesystem_emulation/ram_file_manager.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/filesystem_emulation/workspace_file_manager.py` & `autopack_tools-0.4.3/autopack/filesystem_emulation/workspace_file_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 class WorkspaceFileManager(FileManager):
     """
     This class provides file operations restricted to a workspace directory on the local file system.
     """
 
     def __init__(self, config: PackConfig = PackConfig.global_config()):
         super().__init__(config)
-        self.workspace_dir = Path(config.workspace_path)
+
+    @property
+    def workspace_dir(self) -> Path:
+        return Path(self.config.workspace_path)
 
     def read_file(self, file_path: str) -> str:
         """Reads a file from the workspace directory on the local file system.
 
         Args:
             file_path (str): The path to the file to be read, relative to the workspace directory.
```

### Comparing `autopack_tools-0.4.2/autopack/get_pack.py` & `autopack_tools-0.4.3/autopack/get_pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/installation.py` & `autopack_tools-0.4.3/autopack/installation.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/langchain_wrapper.py` & `autopack_tools-0.4.3/autopack/langchain_wrapper.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/pack.py` & `autopack_tools-0.4.3/autopack/pack.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/pack_config.py` & `autopack_tools-0.4.3/autopack/pack_config.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/prompts.py` & `autopack_tools-0.4.3/autopack/prompts.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/selection.py` & `autopack_tools-0.4.3/autopack/selection.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/autopack/utils.py` & `autopack_tools-0.4.3/autopack/utils.py`

 * *Files identical despite different names*

### Comparing `autopack_tools-0.4.2/pyproject.toml` & `autopack_tools-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "autopack-tools"
-version = "0.4.2"
+version = "0.4.3"
 repository = "https://github.com/AutoPackAI/autopack"
 homepage = "https://autopack.ai"
 description = "Package Manager for AI Agent tools"
 authors = ["Erik Peterson <e@eriklp.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "autopack" }]
```

### Comparing `autopack_tools-0.4.2/PKG-INFO` & `autopack_tools-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopack-tools
-Version: 0.4.2
+Version: 0.4.3
 Summary: Package Manager for AI Agent tools
 Home-page: https://autopack.ai
 License: MIT
 Author: Erik Peterson
 Author-email: e@eriklp.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

