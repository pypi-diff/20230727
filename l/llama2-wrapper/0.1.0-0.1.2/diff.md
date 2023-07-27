# Comparing `tmp/llama2_wrapper-0.1.0.tar.gz` & `tmp/llama2_wrapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama2_wrapper-0.1.0.tar", max compression
+gzip compressed data, was "llama2_wrapper-0.1.2.tar", max compression
```

## Comparing `llama2_wrapper-0.1.0.tar` & `llama2_wrapper-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1060 2023-07-25 10:21:37.826939 llama2_wrapper-0.1.0/LICENSE
--rw-r--r--   0        0        0     8883 2023-07-25 10:21:37.827147 llama2_wrapper-0.1.0/README.md
--rw-r--r--   0        0        0       46 2023-07-27 02:46:01.116569 llama2_wrapper-0.1.0/llama2_wrapper/__init__.py
--rw-r--r--   0        0        0     4793 2023-07-25 10:21:37.827956 llama2_wrapper-0.1.0/llama2_wrapper/model.py
--rw-r--r--   0        0        0      571 2023-07-27 02:20:49.101083 llama2_wrapper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9491 1970-01-01 00:00:00.000000 llama2_wrapper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-25 10:21:37.826939 llama2_wrapper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     9225 2023-07-27 02:49:09.684953 llama2_wrapper-0.1.2/README.md
+-rw-r--r--   0        0        0       46 2023-07-27 02:46:01.116569 llama2_wrapper-0.1.2/llama2_wrapper/__init__.py
+-rw-r--r--   0        0        0     4793 2023-07-25 10:21:37.827956 llama2_wrapper-0.1.2/llama2_wrapper/model.py
+-rw-r--r--   0        0        0     1021 2023-07-27 08:39:09.691513 llama2_wrapper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10350 1970-01-01 00:00:00.000000 llama2_wrapper-0.1.2/PKG-INFO
```

### Comparing `llama2_wrapper-0.1.0/LICENSE` & `llama2_wrapper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama2_wrapper-0.1.0/README.md` & `llama2_wrapper-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # llama2-webui
 
-Running Llama 2 with gradio web UI on GPU or CPU from anywhere (Linux/Windows/Mac). Supporting Llama 2 7B, 13B, 70B with 8-bit, 4-bit mode. Supporting GPU inference with at least 6 GB VRAM, and CPU inference with at least 6 GB RAM.
+Running Llama 2 with gradio web UI on GPU or CPU from anywhere (Linux/Windows/Mac). 
+- Supporting all Llama 2 models (7B, 13B, 70B, GPTQ, GGML) with 8-bit, 4-bit mode. 
+- Supporting GPU inference with at least 6 GB VRAM, and CPU inference.
 
 ![screenshot](./static/screenshot.png)
 
 ## Features
 
 - Supporting models: [Llama-2-7b](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML)/[13b](https://huggingface.co/llamaste/Llama-2-13b-chat-hf)/[70b](https://huggingface.co/llamaste/Llama-2-70b-chat-hf), all [Llama-2-GPTQ](https://huggingface.co/TheBloke/Llama-2-7b-Chat-GPTQ), all [Llama-2-GGML](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML) ...
 - Supporting model backends
@@ -32,23 +34,28 @@
     - [Mac GPU and AMD/Nvidia GPU Acceleration](#mac-gpu-and-amdnvidia-gpu-acceleration)
 - [Contributing](#contributing)
 - [License](#license)
   
 
 
 ## Install
-
 ```
 pip install -r requirements.txt
 ```
 
 `bitsandbytes >= 0.39` may not work on older NVIDIA GPUs. In that case, to use `LOAD_IN_8BIT`, you may have to downgrade like this:
 
 -  `pip install bitsandbytes==0.38.1`
 
+`bitsandbytes` also need a special install for Windows:
+```
+pip uninstall bitsandbytes
+pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.0-py3-none-win_amd64.whl
+```
+
 If run on CPU, install llama.cpp additionally by `pip install llama-cpp-python`.
 
 ## Download Llama-2 Models
 
 Llama 2 is a collection of pre-trained and fine-tuned generative text models ranging in scale from 7 billion to 70 billion parameters.
 
 Llama-2-7b-Chat-GPTQ is the GPTQ model files for [Meta's Llama 2 7b Chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf). GPTQ 4-bit Llama-2 model require less GPU VRAM to run it.
@@ -165,15 +172,17 @@
   <img src="https://contrib.rocks/image?repo=liltom-eth/llama2-webui" />
 </a>
 
 ## License
 
 MIT - see [MIT License](LICENSE)
 
+This project enables users to adapt it freely for proprietary purposes without any restrictions.
+
 ## Credits
 
 - https://huggingface.co/meta-llama/Llama-2-7b-chat-hf
 - https://huggingface.co/spaces/huggingface-projects/llama-2-7b-chat
 - https://huggingface.co/TheBloke/Llama-2-7b-Chat-GPTQ
 - [https://github.com/ggerganov/llama.cpp](https://github.com/ggerganov/llama.cpp)
 - [https://github.com/TimDettmers/bitsandbytes](https://github.com/TimDettmers/bitsandbytes)
-- [https://github.com/PanQiWei/AutoGPTQ](https://github.com/PanQiWei/AutoGPTQ)
+- [https://github.com/PanQiWei/AutoGPTQ](https://github.com/PanQiWei/AutoGPTQ)
```

### Comparing `llama2_wrapper-0.1.0/llama2_wrapper/model.py` & `llama2_wrapper-0.1.2/llama2_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `llama2_wrapper-0.1.0/PKG-INFO` & `llama2_wrapper-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 Metadata-Version: 2.1
 Name: llama2-wrapper
-Version: 0.1.0
-Summary: 
-Author: Tom
+Version: 0.1.2
+Summary: Running Llama 2 on GPU or CPU from anywhere (Linux/Windows/Mac).
+Home-page: https://github.com/liltom-eth/llama2-webui
+License: MIT
+Author: liltom-eth
 Author-email: liltom.eth@gmail.com
 Requires-Python: >=3.10,<3.13
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accelerate (>=0.21.0,<0.22.0)
 Requires-Dist: auto-gptq (==0.3.0)
-Requires-Dist: bitsandbytes (==0.40.2)
+Requires-Dist: bitsandbytes (==0.40.2) ; sys_platform == "darwin"
+Requires-Dist: bitsandbytes (==0.40.2) ; sys_platform == "linux"
+Requires-Dist: bitsandbytes @ https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.0-py3-none-win_amd64.whl ; sys_platform == "win32"
 Requires-Dist: gradio (==3.37.0)
 Requires-Dist: llama-cpp-python (>=0.1.77,<0.2.0)
 Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: scipy (==1.11.1)
 Requires-Dist: sentencepiece (==0.1.99)
 Requires-Dist: torch (==2.0.1)
 Requires-Dist: tqdm (==4.65.0)
 Requires-Dist: transformers (==4.31.0)
+Project-URL: Repository, https://github.com/liltom-eth/llama2-webui
 Description-Content-Type: text/markdown
 
 # llama2-webui
 
-Running Llama 2 with gradio web UI on GPU or CPU from anywhere (Linux/Windows/Mac). Supporting Llama 2 7B, 13B, 70B with 8-bit, 4-bit mode. Supporting GPU inference with at least 6 GB VRAM, and CPU inference with at least 6 GB RAM.
+Running Llama 2 with gradio web UI on GPU or CPU from anywhere (Linux/Windows/Mac). 
+- Supporting all Llama 2 models (7B, 13B, 70B, GPTQ, GGML) with 8-bit, 4-bit mode. 
+- Supporting GPU inference with at least 6 GB VRAM, and CPU inference.
 
 ![screenshot](./static/screenshot.png)
 
 ## Features
 
 - Supporting models: [Llama-2-7b](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML)/[13b](https://huggingface.co/llamaste/Llama-2-13b-chat-hf)/[70b](https://huggingface.co/llamaste/Llama-2-70b-chat-hf), all [Llama-2-GPTQ](https://huggingface.co/TheBloke/Llama-2-7b-Chat-GPTQ), all [Llama-2-GGML](https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML) ...
 - Supporting model backends
@@ -56,23 +64,28 @@
     - [Mac GPU and AMD/Nvidia GPU Acceleration](#mac-gpu-and-amdnvidia-gpu-acceleration)
 - [Contributing](#contributing)
 - [License](#license)
   
 
 
 ## Install
-
 ```
 pip install -r requirements.txt
 ```
 
 `bitsandbytes >= 0.39` may not work on older NVIDIA GPUs. In that case, to use `LOAD_IN_8BIT`, you may have to downgrade like this:
 
 -  `pip install bitsandbytes==0.38.1`
 
+`bitsandbytes` also need a special install for Windows:
+```
+pip uninstall bitsandbytes
+pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.0-py3-none-win_amd64.whl
+```
+
 If run on CPU, install llama.cpp additionally by `pip install llama-cpp-python`.
 
 ## Download Llama-2 Models
 
 Llama 2 is a collection of pre-trained and fine-tuned generative text models ranging in scale from 7 billion to 70 billion parameters.
 
 Llama-2-7b-Chat-GPTQ is the GPTQ model files for [Meta's Llama 2 7b Chat](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf). GPTQ 4-bit Llama-2 model require less GPU VRAM to run it.
@@ -189,15 +202,18 @@
   <img src="https://contrib.rocks/image?repo=liltom-eth/llama2-webui" />
 </a>
 
 ## License
 
 MIT - see [MIT License](LICENSE)
 
+This project enables users to adapt it freely for proprietary purposes without any restrictions.
+
 ## Credits
 
 - https://huggingface.co/meta-llama/Llama-2-7b-chat-hf
 - https://huggingface.co/spaces/huggingface-projects/llama-2-7b-chat
 - https://huggingface.co/TheBloke/Llama-2-7b-Chat-GPTQ
 - [https://github.com/ggerganov/llama.cpp](https://github.com/ggerganov/llama.cpp)
 - [https://github.com/TimDettmers/bitsandbytes](https://github.com/TimDettmers/bitsandbytes)
 - [https://github.com/PanQiWei/AutoGPTQ](https://github.com/PanQiWei/AutoGPTQ)
+
```

