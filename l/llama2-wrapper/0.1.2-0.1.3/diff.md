# Comparing `tmp/llama2_wrapper-0.1.2.tar.gz` & `tmp/llama2_wrapper-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama2_wrapper-0.1.2.tar", max compression
+gzip compressed data, was "llama2_wrapper-0.1.3.tar", max compression
```

## Comparing `llama2_wrapper-0.1.2.tar` & `llama2_wrapper-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1060 2023-07-25 10:21:37.826939 llama2_wrapper-0.1.2/LICENSE
--rw-r--r--   0        0        0     9225 2023-07-27 02:49:09.684953 llama2_wrapper-0.1.2/README.md
--rw-r--r--   0        0        0       46 2023-07-27 02:46:01.116569 llama2_wrapper-0.1.2/llama2_wrapper/__init__.py
--rw-r--r--   0        0        0     4793 2023-07-25 10:21:37.827956 llama2_wrapper-0.1.2/llama2_wrapper/model.py
--rw-r--r--   0        0        0     1021 2023-07-27 08:39:09.691513 llama2_wrapper-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 llama2_wrapper-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-25 10:21:37.826939 llama2_wrapper-0.1.3/LICENSE
+-rw-r--r--   0        0        0       46 2023-07-27 02:46:01.116569 llama2_wrapper-0.1.3/llama2_wrapper/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-25 10:21:37.827956 llama2_wrapper-0.1.3/llama2_wrapper/model.py
+-rw-r--r--   0        0        0      840 2023-07-27 08:55:09.167247 llama2_wrapper-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 llama2_wrapper-0.1.3/PKG-INFO
```

### Comparing `llama2_wrapper-0.1.2/LICENSE` & `llama2_wrapper-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llama2_wrapper-0.1.2/llama2_wrapper/model.py` & `llama2_wrapper-0.1.3/llama2_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `llama2_wrapper-0.1.2/pyproject.toml` & `llama2_wrapper-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [tool.poetry]
 name = "llama2-wrapper"
-version = "0.1.2"
+version = "0.1.3"
 description = "Running Llama 2 on GPU or CPU from anywhere (Linux/Windows/Mac)."
 authors = ["liltom-eth <liltom.eth@gmail.com>"]
 license = "MIT"
-readme = "README.md"
 homepage = "https://github.com/liltom-eth/llama2-webui"
 repository = "https://github.com/liltom-eth/llama2-webui"
 
 packages = [{include = "llama2_wrapper"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
@@ -20,16 +19,15 @@
 sentencepiece = "0.1.99"
 torch = "2.0.1"
 transformers = "4.31.0"
 tqdm = "4.65.0"
 python-dotenv = "1.0.0"
 llama-cpp-python = "^0.1.77"
 bitsandbytes = [
-    {platform = 'win32', url = "https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.0-py3-none-win_amd64.whl"},
     {platform = 'linux', version = "0.40.2"},
     {platform = 'darwin', version = "0.40.2"},
-]   
+]
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

