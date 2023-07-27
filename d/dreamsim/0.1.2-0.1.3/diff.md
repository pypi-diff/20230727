# Comparing `tmp/dreamsim-0.1.2.tar.gz` & `tmp/dreamsim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamsim-0.1.2.tar", last modified: Thu Jul 20 17:21:35 2023, max compression
+gzip compressed data, was "dreamsim-0.1.3.tar", last modified: Thu Jul 27 14:03:27 2023, max compression
```

## Comparing `dreamsim-0.1.2.tar` & `dreamsim-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.482042 dreamsim-0.1.2/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-06-15 23:35:43.000000 dreamsim-0.1.2/LICENSE
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-20 17:21:35.477307 dreamsim-0.1.2/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     8434 2023-07-20 16:55:30.000000 dreamsim-0.1.2/README.md
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.236991 dreamsim-0.1.2/dreamsim/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1599 2023-07-14 19:18:53.000000 dreamsim-0.1.2/dreamsim/config.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.463767 dreamsim-0.1.2/dreamsim/feature_extraction/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/__init__.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/extractor.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_mae_as_vit.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/load_open_clip_as_dino.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/vision_transformer.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-06-16 01:06:22.000000 dreamsim-0.1.2/dreamsim/feature_extraction/vit_wrapper.py
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    12310 2023-07-14 17:31:28.000000 dreamsim-0.1.2/dreamsim/model.py
-drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-20 17:21:35.305580 dreamsim-0.1.2/dreamsim.egg-info/
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/PKG-INFO
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-07-20 17:21:35.000000 dreamsim-0.1.2/dreamsim.egg-info/SOURCES.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/dependency_links.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/requires.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-07-20 17:21:34.000000 dreamsim-0.1.2/dreamsim.egg-info/top_level.txt
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-07-20 17:21:35.484291 dreamsim-0.1.2/setup.cfg
--rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      976 2023-07-20 17:17:21.000000 dreamsim-0.1.2/setup.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-27 14:03:27.680639 dreamsim-0.1.3/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1118 2023-07-14 19:12:59.000000 dreamsim-0.1.3/LICENSE
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-27 14:03:27.675728 dreamsim-0.1.3/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     8434 2023-07-27 14:00:12.000000 dreamsim-0.1.3/README.md
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-27 14:03:27.485580 dreamsim-0.1.3/dreamsim/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       45 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1599 2023-07-14 19:20:51.000000 dreamsim-0.1.3/dreamsim/config.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-27 14:03:27.662369 dreamsim-0.1.3/dreamsim/feature_extraction/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/__init__.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11551 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/extractor.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     1006 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/load_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     3448 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/load_mae_as_vit.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     2726 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/load_open_clip_as_dino.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    11874 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/vision_transformer.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      444 2023-07-14 19:12:59.000000 dreamsim-0.1.3/dreamsim/feature_extraction/vit_wrapper.py
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)    12310 2023-07-27 13:44:53.000000 dreamsim-0.1.3/dreamsim/model.py
+drwxr-xr-x   0 shobhita (26817) vision-phillipi (24866)        0 2023-07-27 14:03:27.554949 dreamsim-0.1.3/dreamsim.egg-info/
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)     7270 2023-07-27 14:03:27.000000 dreamsim-0.1.3/dreamsim.egg-info/PKG-INFO
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      567 2023-07-27 14:03:27.000000 dreamsim-0.1.3/dreamsim.egg-info/SOURCES.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)        1 2023-07-27 14:03:27.000000 dreamsim-0.1.3/dreamsim.egg-info/dependency_links.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       83 2023-07-27 14:03:27.000000 dreamsim-0.1.3/dreamsim.egg-info/requires.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       37 2023-07-27 14:03:27.000000 dreamsim-0.1.3/dreamsim.egg-info/top_level.txt
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)       38 2023-07-27 14:03:27.682835 dreamsim-0.1.3/setup.cfg
+-rw-r--r--   0 shobhita (26817) vision-phillipi (24866)      976 2023-07-27 14:01:30.000000 dreamsim-0.1.3/setup.py
```

### Comparing `dreamsim-0.1.2/LICENSE` & `dreamsim-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/PKG-INFO` & `dreamsim-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamsim
-Version: 0.1.2
+Version: 0.1.3
 Summary: DreamSim similarity metric
 Home-page: https://github.com/ssundaram21/dreamsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dreamsim-0.1.2/README.md` & `dreamsim-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/config.py` & `dreamsim-0.1.3/dreamsim/config.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/feature_extraction/extractor.py` & `dreamsim-0.1.3/dreamsim/feature_extraction/extractor.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/feature_extraction/load_clip_as_dino.py` & `dreamsim-0.1.3/dreamsim/feature_extraction/load_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/feature_extraction/load_mae_as_vit.py` & `dreamsim-0.1.3/dreamsim/feature_extraction/load_mae_as_vit.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/feature_extraction/load_open_clip_as_dino.py` & `dreamsim-0.1.3/dreamsim/feature_extraction/load_open_clip_as_dino.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/feature_extraction/vision_transformer.py` & `dreamsim-0.1.3/dreamsim/feature_extraction/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/dreamsim/model.py` & `dreamsim-0.1.3/dreamsim/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,16 +160,16 @@
 def download_weights(cache_dir, dreamsim_type):
     """
     Downloads and unzips DreamSim weights.
     """
 
     dreamsim_required_ckpts = {
         "ensemble": ["dino_vitb16_pretrain.pth", "dino_vitb16_lora",
-                     "open_clip_vitb32_pretrain.pth.tar", "open_clip_vitb32_lora",
-                     "clip_vitb32_pretrain.pth.tar", "clip_vitb32_lora"],
+                     "open_clip_vitb16_pretrain.pth.tar", "open_clip_vitb16_lora",
+                     "clip_vitb16_pretrain.pth.tar", "clip_vitb16_lora"],
         "dino_vitb16": ["dino_vitb16_pretrain.pth", "dino_vitb16_single_lora"],
         "open_clip_vitb32": ["open_clip_vitb32_pretrain.pth.tar", "open_clip_vitb32_single_lora"],
         "clip_vitb32": ["clip_vitb32_pretrain.pth.tar", "clip_vitb32_single_lora"]
     }
 
     def check(path):
         for required_ckpt in dreamsim_required_ckpts[dreamsim_type]:
```

### Comparing `dreamsim-0.1.2/dreamsim.egg-info/PKG-INFO` & `dreamsim-0.1.3/dreamsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamsim
-Version: 0.1.2
+Version: 0.1.3
 Summary: DreamSim similarity metric
 Home-page: https://github.com/ssundaram21/dreamsim
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dreamsim-0.1.2/dreamsim.egg-info/SOURCES.txt` & `dreamsim-0.1.3/dreamsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreamsim-0.1.2/setup.py` & `dreamsim-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 long_description = "".join(long_description.split("<!--Experiments-->")[::2])
 long_description = "".join(long_description.split("![teaser](images/figs/teaser.png)"))
 
 setuptools.setup(
     name="dreamsim",
-    version="0.1.2",
+    version="0.1.3",
     description="DreamSim similarity metric",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ssundaram21/dreamsim",
     packages=['dreamsim', 'dreamsim/feature_extraction'],
     install_requires=[
         "numpy",
```

