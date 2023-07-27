# Comparing `tmp/lycoris_lora-1.8.1.dev3.tar.gz` & `tmp/lycoris_lora-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.1.dev3.tar", last modified: Sun Jul 23 05:44:50 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.2.tar", last modified: Thu Jul 27 09:34:23 2023, max compression
```

## Comparing `lycoris_lora-1.8.1.dev3.tar` & `lycoris_lora-1.8.2.tar`

### file list

```diff
@@ -1,60 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.267795 lycoris_lora-1.8.1.dev3/
--rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.1.dev3/Algo.md
--rw-rw-rw-   0        0        0     1111 2023-07-22 06:17:56.000000 lycoris_lora-1.8.1.dev3/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.1.dev3/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.1.dev3/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-23 05:44:50.267795 lycoris_lora-1.8.1.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     7451 2023-07-22 06:17:56.000000 lycoris_lora-1.8.1.dev3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.241794 lycoris_lora-1.8.1.dev3/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.1.dev3/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.1.dev3/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/experiments/compare_norm.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.1.dev3/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.1.dev3/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.1.dev3/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/experiments/loha_svd.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.1.dev3/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.1.dev3/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.1.dev3/experiments/time_test.py
--rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.1.dev3/experiments/weakre_speed.py
--rw-rw-rw-   0        0        0     4116 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/hyperdream_gen_weight.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.242794 lycoris_lora-1.8.1.dev3/lycoris/
--rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-07-23 03:48:18.000000 lycoris_lora-1.8.1.dev3/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.244796 lycoris_lora-1.8.1.dev3/lycoris/kohya/
--rw-rw-rw-   0        0        0    39941 2023-07-23 04:02:52.000000 lycoris_lora-1.8.1.dev3/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    48868 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/kohya/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/kohya/kohya_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.249795 lycoris_lora-1.8.1.dev3/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     7334 2023-07-22 06:17:56.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/hyperlycoris.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.251295 lycoris_lora-1.8.1.dev3/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8229 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    10342 2023-07-22 06:17:56.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    10065 2023-07-22 06:17:56.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    12654 2023-07-23 05:44:15.000000 lycoris_lora-1.8.1.dev3/lycoris/modules/lokr.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.252794 lycoris_lora-1.8.1.dev3/lycoris/utils/
--rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-23 03:53:39.000000 lycoris_lora-1.8.1.dev3/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/lycoris/utils/xformers_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.266295 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-23 05:44:50.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1256 2023-07-23 05:44:50.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 05:44:50.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-23 05:44:50.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 05:44:50.000000 lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 05:44:50.268294 lycoris_lora-1.8.1.dev3/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-23 05:44:38.000000 lycoris_lora-1.8.1.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:44:50.267295 lycoris_lora-1.8.1.dev3/tools/
--rw-rw-rw-   0        0        0     4093 2023-07-23 03:43:26.000000 lycoris_lora-1.8.1.dev3/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2299 2023-07-23 03:43:55.000000 lycoris_lora-1.8.1.dev3/tools/merge.py
--rw-rw-rw-   0        0        0    55333 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev3/train_hyperdream.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.446088 lycoris_lora-1.8.2/
+-rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.2/Algo.md
+-rw-rw-rw-   0        0        0     1277 2023-07-27 09:31:21.000000 lycoris_lora-1.8.2/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.2/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.2/LICENSE.md
+-rw-rw-rw-   0        0        0      348 2023-07-27 09:34:23.445588 lycoris_lora-1.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7531 2023-07-27 09:30:40.000000 lycoris_lora-1.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.422509 lycoris_lora-1.8.2/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.2/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.2/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/experiments/compare_norm.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.2/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.2/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.2/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/experiments/loha_svd.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.2/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.2/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.2/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.2/experiments/weakre_speed.py
+-rw-rw-rw-   0        0        0     4110 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/hyperdream_gen_weight.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.423513 lycoris_lora-1.8.2/lycoris/
+-rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-07-27 02:52:33.000000 lycoris_lora-1.8.2/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.426020 lycoris_lora-1.8.2/lycoris/kohya/
+-rw-rw-rw-   0        0        0    42380 2023-07-27 02:15:26.000000 lycoris_lora-1.8.2/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    56362 2023-07-27 09:26:55.000000 lycoris_lora-1.8.2/lycoris/kohya/model_utils.py
+-rw-rw-rw-   0        0        0    58870 2023-07-27 09:27:06.000000 lycoris_lora-1.8.2/lycoris/kohya/original_unet.py
+-rw-rw-rw-   0        0        0    20779 2023-07-27 09:28:08.000000 lycoris_lora-1.8.2/lycoris/kohya/sdxl_model_util.py
+-rw-rw-rw-   0        0        0    41085 2023-07-27 03:12:49.000000 lycoris_lora-1.8.2/lycoris/kohya/sdxl_original_unet.py
+-rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/kohya/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.430020 lycoris_lora-1.8.2/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     7334 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/hyperlycoris.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.431019 lycoris_lora-1.8.2/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8228 2023-07-25 10:04:24.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     8111 2023-07-25 10:04:17.000000 lycoris_lora-1.8.2/lycoris/modules/hypernet/text_encoder.py
+-rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    10342 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    10065 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    12654 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/modules/lokr.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.432019 lycoris_lora-1.8.2/lycoris/utils/
+-rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-25 09:54:09.000000 lycoris_lora-1.8.2/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/lycoris/utils/xformers_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.443585 lycoris_lora-1.8.2/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-27 09:34:23.000000 lycoris_lora-1.8.2/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:34:23.446088 lycoris_lora-1.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-07-27 09:34:17.000000 lycoris_lora-1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:34:23.444589 lycoris_lora-1.8.2/tools/
+-rw-rw-rw-   0        0        0     4087 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-07-27 02:15:19.000000 lycoris_lora-1.8.2/tools/merge.py
+-rw-rw-rw-   0        0        0    55484 2023-07-25 09:54:11.000000 lycoris_lora-1.8.2/train_hyperdream.py
```

### Comparing `lycoris_lora-1.8.1.dev3/.gitignore` & `lycoris_lora-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/Algo.md` & `lycoris_lora-1.8.2/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/Change.md` & `lycoris_lora-1.8.2/Change.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change Log
 
+## 2023/07/27 update to 1.8.2
+* Update utils in kohya-ss/sd-scripts
+
+## 2023/07/27 update to 1.8.1
+* Add config/preset system
+* Improve the project structure
+
 ## 2023/07/19 update to 1.8.0
 * reimplement weight init method
 * implement HyperDreamBooth into LyCORIS
 * better file structure
 
 ## 2023/06/28 update to 1.7.1
 * **rearrange the version format, previous 0.1.7 should be 1.7.0**
```

### Comparing `lycoris_lora-1.8.1.dev3/Demo.md` & `lycoris_lora-1.8.2/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/LICENSE.md` & `lycoris_lora-1.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/README.md` & `lycoris_lora-1.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -107,18 +107,17 @@
 
 * Tips:
   * Use network_dim=0 or conv_dim=0 to disable linear/conv layer
   * LoHa/LoKr/(IA)^3 doesn't support dropout yet.
 
 
 ### For a1111's sd-webui
+**After sd-webui 1.5.0, you can directly use any LyCORIS model with built-in lora system**
 download [Extension](https://github.com/KohakuBlueleaf/a1111-sd-webui-lycoris) into sd-webui, and then use LyCORIS model in the extra netowrks tabs.
 
-**Not For Kohya-ss' Additional Network**
-
 
 ### Extract LoCon
 You can extract LoCon from a dreambooth model with its base model.
 ```bash
 python3 extract_locon.py <settings> <base_model> <db_model> <output>
 ```
 Use --help to get more info
@@ -134,18 +133,20 @@
 ## Example and Comparing for different algo
 see [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) and [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md)
 
 
 ## Change Log
 For full log, please see [Change.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Change.md)
 
-## 2023/07/19 update to 1.8.0
-* reimplement weight init method
-* implement HyperDreamBooth into LyCORIS
-* better file structure
+## 2023/07/27 update to 1.8.2
+* Update utils in kohya-ss/sd-scripts
+
+## 2023/07/27 update to 1.8.1
+* Add config/preset system
+* Improve the project structure
 
 
 ## Todo list
 - [ ] Module and Document for using LyCORIS in any other model, Not only SD.
 - [x] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
   * also need custom backward to save the vram
 - [ ] Low rank + sparse representation
```

### Comparing `lycoris_lora-1.8.1.dev3/experiments/better_conv.py` & `lycoris_lora-1.8.2/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/better_conv_extract.py` & `lycoris_lora-1.8.2/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/compare_norm.py` & `lycoris_lora-1.8.2/experiments/compare_norm.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/concept_neuron.py` & `lycoris_lora-1.8.2/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/locon_extract_test.py` & `lycoris_lora-1.8.2/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/locon_merge_test.py` & `lycoris_lora-1.8.2/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/loha_svd.py` & `lycoris_lora-1.8.2/experiments/loha_svd.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/singular_value_test.py` & `lycoris_lora-1.8.2/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/sparse_bias_test.py` & `lycoris_lora-1.8.2/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/experiments/time_test.py` & `lycoris_lora-1.8.2/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/hyperdream_gen_weight.py` & `lycoris_lora-1.8.2/hyperdream_gen_weight.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         "--weight", help='weight for the lyco model to merge',
         default='1.0', type=float
     )
     return parser.parse_args()
 ARGS = get_args()
 
 
-from lycoris.kohya.kohya_model_utils import (
+from lycoris.kohya.model_utils import (
     load_file
 )
 from library.model_util import load_models_from_stable_diffusion_checkpoint
 from lycoris.kohya import create_hypernetwork
 
 import torch
 import torch.nn as nn
```

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/config.py` & `lycoris_lora-1.8.2/lycoris/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         ],
         'text_encoder_target_name': [],
     },
     'unet-only':{
         'enable_conv': True,
         'unet_target_module':[
             "Transformer2DModel", 
-            "Attention", 
             "ResnetBlock2D", 
             "Downsample2D", 
             "Upsample2D"
         ],
         'unet_target_name':[
             "conv_in",
             "conv_out",
```

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.2/lycoris/kohya/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import math
 from warnings import warn
 import os
 from typing import List
 import torch
 import torch.utils.checkpoint as checkpoint
 
-from .kohya_utils import *
+from .utils import *
 from ..modules.locon import LoConModule
 from ..modules.loha import LohaModule
 from ..modules.ia3 import IA3Module
 from ..modules.lokr import LokrModule
 from ..modules.dylora import DyLoraModule
 from ..modules.glora import GLoRAModule
-from ..modules.hypernet import ImgWeightGenerator
+from ..modules.hypernet import ImgWeightGenerator, TextWeightGenerator
 
 from ..config import PRESET
 from ..utils.preset import read_preset
 
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
@@ -93,15 +93,15 @@
     if algo=='dylora':
         #dylora didn't support scale weight norm yet
         delattr(network, 'apply_max_norm_regularization')
     
     return network
 
 
-def create_hypernetwork(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
+def create_hypernetwork(multiplier, network_dim, network_alpha, vae, text_encoder, unet, vocab_size, **kwargs):
     if network_dim is None:
         network_dim = 4
     dropout = float(kwargs.get('dropout', 0.) or 0.)
     rank_dropout = float(kwargs.get("rank_dropout", 0.) or 0.)
     module_dropout = float(kwargs.get("module_dropout", 0.) or 0.)
     algo = (kwargs.get('algo', 'lora') or 'lora').lower()
     use_cp = (not kwargs.get('disable_conv_cp', True)
@@ -121,15 +121,16 @@
     return HyperDreamNetwork(
         text_encoder, unet, 
         multiplier=multiplier, 
         lora_dim=network_dim, alpha=network_alpha,
         use_cp=use_cp,
         dropout=dropout, rank_dropout=rank_dropout, module_dropout=module_dropout,
         network_module=network_module,
-        down_dim=down_dim, up_dim=up_dim, delta_iters=delta_iters, decoder_blocks=decoder_blocks,
+        down_dim=down_dim, up_dim=up_dim, delta_iters=delta_iters, 
+        decoder_blocks=decoder_blocks, vocab_size=vocab_size,
         decompose_both=kwargs.get('decompose_both', False),
         factor=kwargs.get('factor', -1),
         block_size = block_size
     )
 
 
 class LycorisNetwork(torch.nn.Module):
@@ -509,15 +510,15 @@
         self, 
         text_encoder, unet, 
         multiplier=1.0, 
         lora_dim=4, alpha=1,
         use_cp = False,
         dropout = 0, rank_dropout = 0, module_dropout = 0,
         network_module = LoConModule,
-        down_dim = 100, up_dim = 50, delta_iters = 5, decoder_blocks = 4,
+        down_dim = 100, up_dim = 50, delta_iters = 5, decoder_blocks = 4, vocab_size = 49408,
         **kwargs,
     ) -> None:
         super().__init__()
         self.gradient_ckpt = False
         self.multiplier = multiplier
         self.lora_dim = lora_dim
         self.alpha = alpha
@@ -615,17 +616,23 @@
             ))
         print(f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules.")
 
         self.unet_loras = create_modules(LycorisNetwork.LORA_PREFIX_UNET, unet, LycorisNetwork.UNET_TARGET_REPLACE_MODULE)
         print(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
         
         self.loras: list[LoConModule] = self.text_encoder_loras + self.unet_loras
-        self.weight_generater = ImgWeightGenerator(
+        self.img_weight_generater = ImgWeightGenerator(
             weight_dim=(down_dim+up_dim)*lora_dim,
-            weight_num=len(self.loras),
+            weight_num=len(self.unet_loras),
+            sample_iters=delta_iters,
+            decoder_blocks=decoder_blocks,
+        )
+        self.text_weight_generater = TextWeightGenerator(
+            weight_dim=(down_dim+up_dim)*lora_dim,
+            weight_num=len(self.text_encoder_loras),
             sample_iters=delta_iters,
             decoder_blocks=decoder_blocks,
         )
         self.split = (down_dim* lora_dim, up_dim  * lora_dim)
         self.lora_dim = lora_dim
 
         self.weights_sd = None
@@ -635,31 +642,49 @@
         for lora in self.text_encoder_loras + self.unet_loras:
             assert lora.lora_name not in names, f"duplicated lora name: {lora.lora_name}"
             names.add(lora.lora_name)
         
         self.checkpoint = torch.nn.Parameter(torch.tensor(0.0))
         
         with torch.no_grad():
-            self.update_reference(torch.randn(1, 3, *self.weight_generater.ref_size))
+            self.update_reference(
+                torch.randn(1, 3, *self.img_weight_generater.ref_size),
+                ["test"]
+            )
         
         # for lora in self.loras:
         #     assert torch.all(lora.data[0]==0)
 
-    def gen_weight(self, ref_img, iter=None):
-        weights = self.weight_generater(ref_img, iter)
-        weights = weights + self.checkpoint
-        return [i.split(self.split, dim=-1) for i in weights.split(1, dim=1)]
+    def gen_weight(self, ref_img, caption, iter=None, ensure_grad=0):
+        unet_weights = self.img_weight_generater(ref_img, iter, ensure_grad=ensure_grad)
+        unet_weights = unet_weights + self.checkpoint
+        unet_weights =  [i.split(self.split, dim=-1) for i in unet_weights.split(1, dim=1)]
+        text_weights = self.text_weight_generater(caption, iter, ensure_grad=ensure_grad)
+        text_weights = text_weights + self.checkpoint
+        text_weights =  [i.split(self.split, dim=-1) for i in text_weights.split(1, dim=1)]
+        return unet_weights, text_weights
 
-    def update_reference(self, ref_img, iter=None):
+    def update_reference(self, ref_img, caption, iter=None):
         # use idx for aux weight seed
         if self.gradient_ckpt and self.training:
-            weights_list = checkpoint.checkpoint(self.gen_weight, ref_img, iter)
-        else:
-            weights_list = self.gen_weight(ref_img, iter)
-        for idx, (lora, weight) in enumerate(zip(self.loras, weights_list)):
+            ensure_grad = torch.zeros(1, device=ref_img.device, requires_grad=True)
+            unet_weights_list, text_weights_list = checkpoint.checkpoint(
+                self.gen_weight, ref_img, caption, iter, ensure_grad
+            )
+        else:
+            unet_weights_list, text_weights_list = self.gen_weight(ref_img, caption, iter)
+            
+        for idx, (lora, weight) in enumerate(zip(self.unet_loras, unet_weights_list)):
+            assert lora.multiplier > 0, f"multiplier must be positive: {lora.multiplier}"
+            # weight: [batch, 1, weight_dim]
+            # if weight.dim()==3:
+            #     weight = weight.squeeze(1)
+            lora.update_weights(*weight, idx)
+            
+        for idx, (lora, weight) in enumerate(zip(self.text_encoder_loras, text_weights_list)):
             assert lora.multiplier > 0, f"multiplier must be positive: {lora.multiplier}"
             # weight: [batch, 1, weight_dim]
             # if weight.dim()==3:
             #     weight = weight.squeeze(1)
             lora.update_weights(*weight, idx)
 
     def set_multiplier(self, multiplier):
@@ -710,24 +735,37 @@
 
     def enable_gradient_checkpointing(self):
         self.gradient_ckpt = True
 
     def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
         self.requires_grad_(True)
         all_params = []
-        all_params.append({
-            'params': (
-                [p for p in self.weight_generater.decoder_model.parameters()]
-                + [p for p in self.weight_generater.pos_emb_proj.parameters()]
-                + [p for p in self.weight_generater.feature_proj.parameters()]
-                + ([p for p in self.weight_generater.encoder_model.parameters()] 
-                   if self.weight_generater.train_encoder else [])
-            ), 
-            'lr': learning_rate
-        })
+        
+        if self.text_encoder_loras:
+            all_params.append({
+                'params': (
+                    [p for p in self.text_weight_generater.decoder_model.parameters()]
+                    + [p for p in self.text_weight_generater.pos_emb_proj.parameters()]
+                    + [p for p in self.text_weight_generater.feature_proj.parameters()]
+                    + ([p for p in self.text_weight_generater.encoder_model.parameters()] 
+                    if self.text_weight_generater.train_encoder else [])
+                ), 
+                'lr': text_encoder_lr
+            })
+        if self.unet_loras:
+            all_params.append({
+                'params': (
+                    [p for p in self.img_weight_generater.decoder_model.parameters()]
+                    + [p for p in self.img_weight_generater.pos_emb_proj.parameters()]
+                    + [p for p in self.img_weight_generater.feature_proj.parameters()]
+                    + ([p for p in self.img_weight_generater.encoder_model.parameters()] 
+                    if self.img_weight_generater.train_encoder else [])
+                ), 
+                'lr': unet_lr
+            })
         return all_params
 
     def prepare_grad_etc(self, text_encoder, unet):
         self.requires_grad_(True)
 
     def on_epoch_start(self, text_encoder, unet):
         self.train()
@@ -735,19 +773,25 @@
     def get_trainable_params(self):
         return self.parameters()
 
     def save_weights(self, file, dtype, metadata):
         if metadata is not None and len(metadata) == 0:
             metadata = None
 
-        state_dict = self.weight_generater.state_dict()
-        if not self.weight_generater.train_encoder:
-            for k in self.weight_generater.encoder_model.state_dict().keys():
+        state_dict = self.img_weight_generater.state_dict()
+        if not self.img_weight_generater.train_encoder:
+            for k in self.img_weight_generater.encoder_model.state_dict().keys():
+                state_dict.pop(f'encoder_model.{k}')
+        state_dict = {f'img_weight_generater.{i}': v for i, v in state_dict.items()}
+
+        state_dict = self.text_weight_generater.state_dict()
+        if not self.text_weight_generater.train_encoder:
+            for k in self.text_weight_generater.encoder_model.state_dict().keys():
                 state_dict.pop(f'encoder_model.{k}')
-        state_dict = {f'weight_generater.{i}': v for i, v in state_dict.items()}
+        state_dict = {f'text_weight_generater.{i}': v for i, v in state_dict.items()}
 
         if dtype is not None:
             for key in list(state_dict.keys()):
                 v = state_dict[key]
                 v = v.detach().clone().to("cpu").to(dtype)
                 state_dict[key] = v
```

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/kohya/kohya_model_utils.py` & `lycoris_lora-1.8.2/lycoris/kohya/model_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# https://github.com/kohya-ss/sd-scripts/blob/b78c0e2a69e52ce6c79abc6c8c82d1a9cabcf05c/library/model_util.py
 # v1: split from train_db_fixed.py.
 # v2: support safetensors
 
 import math
 import os
 import torch
+import diffusers
 from transformers import CLIPTextModel, CLIPTokenizer, CLIPTextConfig, logging
-from diffusers import AutoencoderKL, DDIMScheduler, StableDiffusionPipeline, UNet2DConditionModel
+from diffusers import AutoencoderKL, DDIMScheduler, StableDiffusionPipeline  # , UNet2DConditionModel
 from safetensors.torch import load_file, save_file
+from .original_unet import UNet2DConditionModel
 
 # DiffUsers版StableDiffusionのモデルパラメータ
 NUM_TRAIN_TIMESTEPS = 1000
 BETA_START = 0.00085
 BETA_END = 0.0120
 
 UNET_PARAMS_MODEL_CHANNELS = 320
@@ -18,26 +21,28 @@
 UNET_PARAMS_ATTENTION_RESOLUTIONS = [4, 2, 1]
 UNET_PARAMS_IMAGE_SIZE = 64  # fixed from old invalid value `32`
 UNET_PARAMS_IN_CHANNELS = 4
 UNET_PARAMS_OUT_CHANNELS = 4
 UNET_PARAMS_NUM_RES_BLOCKS = 2
 UNET_PARAMS_CONTEXT_DIM = 768
 UNET_PARAMS_NUM_HEADS = 8
+# UNET_PARAMS_USE_LINEAR_PROJECTION = False
 
 VAE_PARAMS_Z_CHANNELS = 4
 VAE_PARAMS_RESOLUTION = 256
 VAE_PARAMS_IN_CHANNELS = 3
 VAE_PARAMS_OUT_CH = 3
 VAE_PARAMS_CH = 128
 VAE_PARAMS_CH_MULT = [1, 2, 4, 4]
 VAE_PARAMS_NUM_RES_BLOCKS = 2
 
 # V2
 V2_UNET_PARAMS_ATTENTION_HEAD_DIM = [5, 10, 20, 20]
 V2_UNET_PARAMS_CONTEXT_DIM = 1024
+# V2_UNET_PARAMS_USE_LINEAR_PROJECTION = True
 
 # Diffusersの設定を読み込むための参照モデル
 DIFFUSERS_REF_MODEL_ID_V1 = "runwayml/stable-diffusion-v1-5"
 DIFFUSERS_REF_MODEL_ID_V2 = "stabilityai/stable-diffusion-2-1"
 
 
 # region StableDiffusion->Diffusersの変換コード
@@ -120,25 +125,38 @@
     mapping = []
     for old_item in old_list:
         new_item = old_item
 
         new_item = new_item.replace("norm.weight", "group_norm.weight")
         new_item = new_item.replace("norm.bias", "group_norm.bias")
 
-        new_item = new_item.replace("q.weight", "query.weight")
-        new_item = new_item.replace("q.bias", "query.bias")
+        if diffusers.__version__ < "0.17.0":
+            new_item = new_item.replace("q.weight", "query.weight")
+            new_item = new_item.replace("q.bias", "query.bias")
 
-        new_item = new_item.replace("k.weight", "key.weight")
-        new_item = new_item.replace("k.bias", "key.bias")
+            new_item = new_item.replace("k.weight", "key.weight")
+            new_item = new_item.replace("k.bias", "key.bias")
 
-        new_item = new_item.replace("v.weight", "value.weight")
-        new_item = new_item.replace("v.bias", "value.bias")
+            new_item = new_item.replace("v.weight", "value.weight")
+            new_item = new_item.replace("v.bias", "value.bias")
 
-        new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
-        new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
+            new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
+            new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
+        else:
+            new_item = new_item.replace("q.weight", "to_q.weight")
+            new_item = new_item.replace("q.bias", "to_q.bias")
+
+            new_item = new_item.replace("k.weight", "to_k.weight")
+            new_item = new_item.replace("k.bias", "to_k.bias")
+
+            new_item = new_item.replace("v.weight", "to_v.weight")
+            new_item = new_item.replace("v.bias", "to_v.bias")
+
+            new_item = new_item.replace("proj_out.weight", "to_out.0.weight")
+            new_item = new_item.replace("proj_out.bias", "to_out.0.bias")
 
         new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
 
         mapping.append({"old": old_item, "new": new_item})
 
     return mapping
 
@@ -185,16 +203,24 @@
         new_path = new_path.replace("middle_block.2", "mid_block.resnets.1")
 
         if additional_replacements is not None:
             for replacement in additional_replacements:
                 new_path = new_path.replace(replacement["old"], replacement["new"])
 
         # proj_attn.weight has to be converted from conv 1D to linear
-        if "proj_attn.weight" in new_path:
-            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0]
+        reshaping = False
+        if diffusers.__version__ < "0.17.0":
+            if "proj_attn.weight" in new_path:
+                reshaping = True
+        else:
+            if ".attentions." in new_path and ".0.to_" in new_path and old_checkpoint[path["old"]].ndim > 2:
+                reshaping = True
+
+        if reshaping:
+            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0, 0]
         else:
             checkpoint[new_path] = old_checkpoint[path["old"]]
 
 
 def conv_attn_to_linear(checkpoint):
     keys = list(checkpoint.keys())
     attn_keys = ["query.weight", "key.weight", "value.weight"]
@@ -353,16 +379,17 @@
             resnet_0_paths = renew_resnet_paths(output_block_layers, n_shave_prefix_segments=1)
             for path in resnet_0_paths:
                 old_path = ".".join(["output_blocks", str(i), path["old"]])
                 new_path = ".".join(["up_blocks", str(block_id), "resnets", str(layer_in_block_id), path["new"]])
 
                 new_checkpoint[new_path] = unet_state_dict[old_path]
 
-    # SDのv2では1*1のconv2dがlinearに変わっているので、linear->convに変換する
-    if v2:
+    # SDのv2では1*1のconv2dがlinearに変わっている
+    # 誤って Diffusers 側を conv2d のままにしてしまったので、変換必要
+    if v2 and not config.get("use_linear_projection", False):
         linear_transformer_to_conv(new_checkpoint)
 
     return new_checkpoint
 
 
 def convert_ldm_vae_checkpoint(checkpoint, config):
     # extract state dict for VAE
@@ -464,15 +491,15 @@
     paths = renew_vae_attention_paths(mid_attentions)
     meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
     assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
     conv_attn_to_linear(new_checkpoint)
     return new_checkpoint
 
 
-def create_unet_diffusers_config(v2):
+def create_unet_diffusers_config(v2, use_linear_projection_in_v2=False):
     """
     Creates a config for the diffusers based on the config of the LDM model.
     """
     # unet_params = original_config.model.params.unet_config.params
 
     block_out_channels = [UNET_PARAMS_MODEL_CHANNELS * mult for mult in UNET_PARAMS_CHANNEL_MULT]
 
@@ -496,15 +523,18 @@
         out_channels=UNET_PARAMS_OUT_CHANNELS,
         down_block_types=tuple(down_block_types),
         up_block_types=tuple(up_block_types),
         block_out_channels=tuple(block_out_channels),
         layers_per_block=UNET_PARAMS_NUM_RES_BLOCKS,
         cross_attention_dim=UNET_PARAMS_CONTEXT_DIM if not v2 else V2_UNET_PARAMS_CONTEXT_DIM,
         attention_head_dim=UNET_PARAMS_NUM_HEADS if not v2 else V2_UNET_PARAMS_ATTENTION_HEAD_DIM,
+        # use_linear_projection=UNET_PARAMS_USE_LINEAR_PROJECTION if not v2 else V2_UNET_PARAMS_USE_LINEAR_PROJECTION,
     )
+    if v2 and use_linear_projection_in_v2:
+        config["use_linear_projection"] = True
 
     return config
 
 
 def create_vae_diffusers_config():
     """
     Creates a config for the diffusers based on the config of the LDM model.
@@ -721,14 +751,112 @@
     new_state_dict = {v: unet_state_dict[k] for k, v in mapping.items()}
 
     if v2:
         conv_transformer_to_linear(new_state_dict)
 
     return new_state_dict
 
+def controlnet_conversion_map():
+    unet_conversion_map = [
+        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
+        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
+        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
+        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
+        ("input_blocks.0.0.weight", "conv_in.weight"),
+        ("input_blocks.0.0.bias", "conv_in.bias"),
+        ("middle_block_out.0.weight", "controlnet_mid_block.weight"),
+        ("middle_block_out.0.bias", "controlnet_mid_block.bias"),
+    ]
+
+    unet_conversion_map_resnet = [
+        ("in_layers.0", "norm1"),
+        ("in_layers.2", "conv1"),
+        ("out_layers.0", "norm2"),
+        ("out_layers.3", "conv2"),
+        ("emb_layers.1", "time_emb_proj"),
+        ("skip_connection", "conv_shortcut"),
+    ]
+
+    unet_conversion_map_layer = []
+    for i in range(4):
+        for j in range(2):
+            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
+            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
+            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
+
+            if i < 3:
+                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
+                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
+                unet_conversion_map_layer.append((sd_down_atn_prefix, hf_down_atn_prefix))
+
+        if i < 3:
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
+            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
+            unet_conversion_map_layer.append((sd_downsample_prefix, hf_downsample_prefix))
+
+    hf_mid_atn_prefix = "mid_block.attentions.0."
+    sd_mid_atn_prefix = "middle_block.1."
+    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
+
+    for j in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{j}."
+        sd_mid_res_prefix = f"middle_block.{2*j}."
+        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    controlnet_cond_embedding_names = (
+        ["conv_in"] + [f"blocks.{i}" for i in range(6)] + ["conv_out"]
+    )
+    for i, hf_prefix in enumerate(controlnet_cond_embedding_names):
+        hf_prefix = f"controlnet_cond_embedding.{hf_prefix}."
+        sd_prefix = f"input_hint_block.{i*2}."
+        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
+
+    for i in range(12):
+        hf_prefix = f"controlnet_down_blocks.{i}."
+        sd_prefix = f"zero_convs.{i}.0."
+        unet_conversion_map_layer.append((sd_prefix, hf_prefix))
+
+    return unet_conversion_map, unet_conversion_map_resnet, unet_conversion_map_layer
+
+
+def convert_controlnet_state_dict_to_sd(controlnet_state_dict):
+    unet_conversion_map, unet_conversion_map_resnet, unet_conversion_map_layer = controlnet_conversion_map()
+
+    mapping = {k: k for k in controlnet_state_dict.keys()}
+    for sd_name, diffusers_name in unet_conversion_map:
+        mapping[diffusers_name] = sd_name
+    for k, v in mapping.items():
+        if "resnets" in k:
+            for sd_part, diffusers_part in unet_conversion_map_resnet:
+                v = v.replace(diffusers_part, sd_part)
+            mapping[k] = v
+    for k, v in mapping.items():
+        for sd_part, diffusers_part in unet_conversion_map_layer:
+            v = v.replace(diffusers_part, sd_part)
+        mapping[k] = v
+    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
+    return new_state_dict
+
+def convert_controlnet_state_dict_to_diffusers(controlnet_state_dict):
+    unet_conversion_map, unet_conversion_map_resnet, unet_conversion_map_layer = controlnet_conversion_map()
+
+    mapping = {k: k for k in controlnet_state_dict.keys()}
+    for sd_name, diffusers_name in unet_conversion_map:
+        mapping[sd_name] = diffusers_name
+    for k, v in mapping.items():
+        for sd_part, diffusers_part in unet_conversion_map_layer:
+            v = v.replace(sd_part, diffusers_part)
+        mapping[k] = v
+    for k, v in mapping.items():
+        if "resnets" in v:
+            for sd_part, diffusers_part in unet_conversion_map_resnet:
+                v = v.replace(sd_part, diffusers_part)
+            mapping[k] = v
+    new_state_dict = {v: controlnet_state_dict[k] for k, v in mapping.items()}
+    return new_state_dict
 
 # ================#
 # VAE Conversion #
 # ================#
 
 
 def reshape_weight_for_sd(w):
@@ -769,22 +897,32 @@
 
     # this part accounts for mid blocks in both the encoder and the decoder
     for i in range(2):
         hf_mid_res_prefix = f"mid_block.resnets.{i}."
         sd_mid_res_prefix = f"mid.block_{i+1}."
         vae_conversion_map.append((sd_mid_res_prefix, hf_mid_res_prefix))
 
-    vae_conversion_map_attn = [
-        # (stable-diffusion, HF Diffusers)
-        ("norm.", "group_norm."),
-        ("q.", "query."),
-        ("k.", "key."),
-        ("v.", "value."),
-        ("proj_out.", "proj_attn."),
-    ]
+    if diffusers.__version__ < "0.17.0":
+        vae_conversion_map_attn = [
+            # (stable-diffusion, HF Diffusers)
+            ("norm.", "group_norm."),
+            ("q.", "query."),
+            ("k.", "key."),
+            ("v.", "value."),
+            ("proj_out.", "proj_attn."),
+        ]
+    else:
+        vae_conversion_map_attn = [
+            # (stable-diffusion, HF Diffusers)
+            ("norm.", "group_norm."),
+            ("q.", "to_q."),
+            ("k.", "to_k."),
+            ("v.", "to_v."),
+            ("proj_out.", "to_out.0."),
+        ]
 
     mapping = {k: k for k in vae_state_dict.keys()}
     for k, v in mapping.items():
         for sd_part, hf_part in vae_conversion_map:
             v = v.replace(hf_part, sd_part)
         mapping[k] = v
     for k, v in mapping.items():
@@ -793,15 +931,15 @@
                 v = v.replace(hf_part, sd_part)
             mapping[k] = v
     new_state_dict = {v: vae_state_dict[k] for k, v in mapping.items()}
     weights_to_convert = ["q", "k", "v", "proj_out"]
     for k, v in new_state_dict.items():
         for weight_name in weights_to_convert:
             if f"mid.attn_1.{weight_name}.weight" in k:
-                # print(f"Reshaping {k} for SD format")
+                # print(f"Reshaping {k} for SD format: shape {v.shape} -> {v.shape} x 1 x 1")
                 new_state_dict[k] = reshape_weight_for_sd(v)
 
     return new_state_dict
 
 
 # endregion
 
@@ -842,19 +980,19 @@
         state_dict[new_key] = state_dict[key]
         del state_dict[key]
 
     return checkpoint, state_dict
 
 
 # TODO dtype指定の動作が怪しいので確認する text_encoderを指定形式で作れるか未確認
-def load_models_from_stable_diffusion_checkpoint(v2, ckpt_path, device="cpu", dtype=None):
+def load_models_from_stable_diffusion_checkpoint(v2, ckpt_path, device="cpu", dtype=None, unet_use_linear_projection_in_v2=True):
     _, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path, device)
 
     # Convert the UNet2DConditionModel model.
-    unet_config = create_unet_diffusers_config(v2)
+    unet_config = create_unet_diffusers_config(v2, unet_use_linear_projection_in_v2)
     converted_unet_checkpoint = convert_ldm_unet_checkpoint(v2, state_dict, unet_config)
 
     unet = UNet2DConditionModel(**unet_config).to(device)
     info = unet.load_state_dict(converted_unet_checkpoint)
     print("loading u-net:", info)
 
     # Convert the VAE model.
@@ -890,23 +1028,54 @@
             transformers_version="4.25.0.dev0",
         )
         text_model = CLIPTextModel._from_config(cfg)
         info = text_model.load_state_dict(converted_text_encoder_checkpoint)
     else:
         converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v1(state_dict)
 
-        logging.set_verbosity_error()  # don't show annoying warning
-        text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
-        logging.set_verbosity_warning()
-
+        # logging.set_verbosity_error()  # don't show annoying warning
+        # text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
+        # logging.set_verbosity_warning()
+        # print(f"config: {text_model.config}")
+        cfg = CLIPTextConfig(
+            vocab_size=49408,
+            hidden_size=768,
+            intermediate_size=3072,
+            num_hidden_layers=12,
+            num_attention_heads=12,
+            max_position_embeddings=77,
+            hidden_act="quick_gelu",
+            layer_norm_eps=1e-05,
+            dropout=0.0,
+            attention_dropout=0.0,
+            initializer_range=0.02,
+            initializer_factor=1.0,
+            pad_token_id=1,
+            bos_token_id=0,
+            eos_token_id=2,
+            model_type="clip_text_model",
+            projection_dim=768,
+            torch_dtype="float32",
+        )
+        text_model = CLIPTextModel._from_config(cfg)
         info = text_model.load_state_dict(converted_text_encoder_checkpoint)
     print("loading text encoder:", info)
 
     return text_model, vae, unet
 
+def get_model_version_str_for_sd1_sd2(v2, v_parameterization):
+    # only for reference
+    version_str = "sd"
+    if v2:
+        version_str += "_v2"
+    else:
+        version_str += "_v1"
+    if v_parameterization:
+        version_str += "_v"
+    return version_str
 
 def convert_text_encoder_state_dict_to_sd_v2(checkpoint, make_dummy_weights=False):
     def convert_key(key):
         # position_idsの除去
         if ".position_ids" in key:
             return None
```

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/kohya/kohya_utils.py` & `lycoris_lora-1.8.2/lycoris/kohya/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/attention.py` & `lycoris_lora-1.8.2/lycoris/modules/attention.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/dylora.py` & `lycoris_lora-1.8.2/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/glokr.py` & `lycoris_lora-1.8.2/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/glora.py` & `lycoris_lora-1.8.2/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/hypernet/generater.py` & `lycoris_lora-1.8.2/lycoris/modules/hypernet/generater.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from torchvision.transforms.functional import resize
 
 from timm import create_model
 from einops import rearrange
 
 from lycoris.modules.attention import TransformerBlock
+from .text_encoder import FrozenOpenCLIPEmbedder
 
 
 def _get_sinusoid_encoding_table(n_position, d_hid):
     ''' Sinusoid position encoding table '''
     # TODO: make it with torch instead of numpy
 
     def get_position_angle_vec(position):
@@ -112,45 +113,45 @@
             # B, C, H, W -> B, L, C
             test_output = test_output.view(1, test_output.size(1), -1).transpose(1, 2)
         
         self.feature_proj = nn.Linear(test_output.shape[-1], weight_dim, bias=False)
         self.pos_emb_proj = nn.Linear(weight_dim, weight_dim, bias=False)
         self.decoder_model = WeightDecoder(weight_dim, weight_num, decoder_blocks)
     
-    def forward(self, ref_img, iters=None, weight=None):
-        if self.train_encoder:
+    def forward(self, ref_img, iters=None, weight=None, ensure_grad=0):
+        ref_img = resize(ref_img, self.ref_size, antialias=True)
+        if not self.train_encoder:
             with torch.no_grad():
-                features = self.encoder_model.forward_features(resize(ref_img, self.ref_size))
+                features = self.encoder_model.forward_features(ref_img)
         else:
-            features = self.encoder_model.forward_features(resize(ref_img, self.ref_size))
+            features = self.encoder_model.forward_features(ref_img + ensure_grad)
         if isinstance(features, list):
             features = features[-1]
         if len(features.shape) == 4:
             # B, C, H, W -> B, L, C
             features = features.view(features.size(0), features.size(1), -1).transpose(1, 2)
-        features = self.feature_proj(features)
+        features = self.feature_proj(features+ensure_grad)
         
         if weight is None:
             weight = torch.zeros(
                 ref_img.size(0), self.weight_num, self.weight_dim, device=ref_img.device
             )
         
         for iter in range(iters or self.sample_iters):
             weight = self.decoder_model(weight, features)
         return weight
 
 
 class TextWeightGenerator(nn.Module):
     def __init__(
         self, 
-        encoder_model_name: str = "vit_base_patch16_224",
         train_encoder: bool = False,
         reference_size: Tuple[int] = (224, 224), 
         weight_dim: int = 150,                      # 100+50 in paper
-        weight_num: int = 54,
+        weight_num: int = 54,                       # 21*2 in SD UNet + 12 in CLIP-L TE
         decoder_blocks: int = 4,
         sample_iters: int = 1,
     ):
         super(TextWeightGenerator, self).__init__()
         self.ref_size = reference_size
         self.weight_num = weight_num
         self.weight_dim = weight_dim
@@ -158,44 +159,44 @@
         self.train_encoder = train_encoder
         
         self.register_buffer(
             'block_pos_emb', 
             _get_sinusoid_encoding_table(weight_num*2, weight_dim)
         )
         
-        self.encoder_model: nn.Module = create_model(encoder_model_name, pretrained=True)
+        self.encoder_model: nn.Module = FrozenOpenCLIPEmbedder()
         for p in self.encoder_model.parameters():
             p.requires_grad_(train_encoder)
         
-        test_input = torch.randn(1, 3, *reference_size)
-        test_output = self.encoder_model.forward_features(test_input)
+        test_input = ["test"]
+        test_output = self.encoder_model(test_input)
         if isinstance(test_output, list):
             test_output = test_output[-1]
         if len(test_output.shape) == 4:
             # B, C, H, W -> B, L, C
             test_output = test_output.view(1, test_output.size(1), -1).transpose(1, 2)
         
         self.feature_proj = nn.Linear(test_output.shape[-1], weight_dim, bias=False)
         self.pos_emb_proj = nn.Linear(weight_dim, weight_dim, bias=False)
         self.decoder_model = WeightDecoder(weight_dim, weight_num, decoder_blocks)
     
-    def forward(self, ref_img, iters=None, weight=None):
-        if self.train_encoder:
+    def forward(self, caption, iters=None, weight=None, ensure_grad=0):
+        if not self.train_encoder:
             with torch.no_grad():
-                features = self.encoder_model.forward_features(resize(ref_img, self.ref_size))
+                features = self.encoder_model(caption)
         else:
-            features = self.encoder_model.forward_features(resize(ref_img, self.ref_size))
+            features = self.encoder_model(caption)
         if isinstance(features, list):
             features = features[-1]
         if len(features.shape) == 4:
             # B, C, H, W -> B, L, C
             features = features.view(features.size(0), features.size(1), -1).transpose(1, 2)
-        features = self.feature_proj(features)
+        features = self.feature_proj(features+ensure_grad)
         
         if weight is None:
             weight = torch.zeros(
-                ref_img.size(0), self.weight_num, self.weight_dim, device=ref_img.device
+                features.size(0), self.weight_num, self.weight_dim, device=features.device
             )
         
         for iter in range(iters or self.sample_iters):
             weight = self.decoder_model(weight, features)
         return weight
```

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/ia3.py` & `lycoris_lora-1.8.2/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/locon.py` & `lycoris_lora-1.8.2/lycoris/modules/locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/loha.py` & `lycoris_lora-1.8.2/lycoris/modules/loha.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/modules/lokr.py` & `lycoris_lora-1.8.2/lycoris/modules/lokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris/utils/__init__.py` & `lycoris_lora-1.8.2/lycoris/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.1.dev3/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.8.2/lycoris_lora.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 experiments/singular_value_test.py
 experiments/sparse_bias_test.py
 experiments/time_test.py
 experiments/weakre_speed.py
 lycoris/__init__.py
 lycoris/config.py
 lycoris/kohya/__init__.py
-lycoris/kohya/kohya_model_utils.py
-lycoris/kohya/kohya_utils.py
+lycoris/kohya/model_utils.py
+lycoris/kohya/original_unet.py
+lycoris/kohya/sdxl_model_util.py
+lycoris/kohya/sdxl_original_unet.py
+lycoris/kohya/utils.py
 lycoris/modules/__init__.py
 lycoris/modules/attention.py
 lycoris/modules/dylora.py
 lycoris/modules/glokr.py
 lycoris/modules/glora.py
 lycoris/modules/hyperlycoris.py
 lycoris/modules/ia3.py
 lycoris/modules/locon.py
 lycoris/modules/loha.py
 lycoris/modules/lokr.py
 lycoris/modules/hypernet/__init__.py
 lycoris/modules/hypernet/generater.py
+lycoris/modules/hypernet/text_encoder.py
 lycoris/utils/__init__.py
 lycoris/utils/preset.py
 lycoris/utils/xformers_utils.py
 lycoris_lora.egg-info/PKG-INFO
 lycoris_lora.egg-info/SOURCES.txt
 lycoris_lora.egg-info/dependency_links.txt
 lycoris_lora.egg-info/not-zip-safe
```

### Comparing `lycoris_lora-1.8.1.dev3/setup.py` & `lycoris_lora-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.1.dev3',
+    version='1.8.2',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-1.8.1.dev3/tools/extract_locon.py` & `lycoris_lora-1.8.2/tools/extract_locon.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         default=False, action="store_true"
     )
     return parser.parse_args()
 ARGS = get_args()
 
 
 from lycoris.utils import extract_diff
-from lycoris.kohya.kohya_model_utils import load_models_from_stable_diffusion_checkpoint
+from lycoris.kohya.model_utils import load_models_from_stable_diffusion_checkpoint
 
 import torch
 from safetensors.torch import save_file
 
 
 def main():
     args = ARGS
```

### Comparing `lycoris_lora-1.8.1.dev3/tools/merge.py` & `lycoris_lora-1.8.2/tools/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         default='1.0', type=float
     )
     return parser.parse_args()
 ARGS = get_args()
 
 
 from lycoris.utils import merge
-from lycoris.kohya.kohya_model_utils import (
+from lycoris.kohya.model_utils import (
     load_models_from_stable_diffusion_checkpoint,
     save_stable_diffusion_checkpoint,
     load_file
 )
 
 import torch
```

### Comparing `lycoris_lora-1.8.1.dev3/train_hyperdream.py` & `lycoris_lora-1.8.2/train_hyperdream.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,15 @@
         network = lycoris.kohya.create_hypernetwork(
             1.0,
             args.network_dim,
             args.network_alpha,
             vae,
             text_encoder,
             unet,
+            vocab_size=tokenizer.vocab_size,
             neuron_dropout=args.network_dropout,
             **net_kwargs,
         )
 
         if hasattr(network, "prepare_network"):
             network.prepare_network(args)
         if args.scale_weight_norms and not hasattr(network, "apply_max_norm_regularization"):
@@ -859,15 +860,18 @@
 
             for step, batch in enumerate(train_dataloader):
                 current_step.value = global_step
                 with accelerator.accumulate(network):
                     on_step_start(text_encoder, unet)
                     with accelerator.autocast():
                         network: lycoris.kohya.HyperDreamNetwork
-                        network.update_reference(batch["images"].to(dtype=weight_dtype))
+                        network.update_reference(
+                            batch["images"].to(dtype=weight_dtype),
+                            batch["captions"],
+                        )
 
                     with torch.no_grad():
                         if "latents" in batch and batch["latents"] is not None:
                             latents = batch["latents"].to(accelerator.device)
                         else:
                             # latentに変換
                             latents = vae.encode(batch["images"].to(dtype=vae_dtype)).latent_dist.sample()
```

