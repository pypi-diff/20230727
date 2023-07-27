# Comparing `tmp/meta-core-3.7.27.tar.gz` & `tmp/meta-core-3.7.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-core-3.7.27.tar", last modified: Thu Jul 27 03:43:03 2023, max compression
+gzip compressed data, was "dist/meta-core-3.7.28.tar", last modified: Thu Jul 27 09:25:00 2023, max compression
```

## Comparing `meta-core-3.7.27.tar` & `meta-core-3.7.28.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-27 03:43:03.000000 meta-core-3.7.27/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.27/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       55 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-27 03:43:03.000000 meta-core-3.7.27/meta_core.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/metacore/
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.27/metacore/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/metacore/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.27/metacore/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4921 2023-07-27 03:39:39.000000 meta-core-3.7.27/metacore/app/ad_segment.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.27/metacore/app/segment.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/metacore/open_clip/
--rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/coca_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/constants.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.27/metacore/open_clip/factory.py
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/generation_utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/hf_configs.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/hf_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/loss.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/metacore/open_clip/model_configs/
--rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN101.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN50.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN50x16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN50x4.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/RN50x64.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-16-plus.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-H-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-L-14-280.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-L-14-336.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-L-16-320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-L-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-M-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-M-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-M-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-M-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-S-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-S-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-S-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-S-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-bigG-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-e-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/ViT-g-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/coca_ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/coca_ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/coca_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_base_w.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_base_w_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_large.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_large_d.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_large_d_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_small.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_tiny.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_xlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_xxlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/convnext_xxlarge_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)     7207 2023-07-21 11:10:23.000000 meta-core-3.7.27/metacore/open_clip/modified_resnet.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/openai.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/pretrained.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/push_to_hf_hub.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/timm_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.27/metacore/open_clip/tokenizer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/transform.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/transformer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.27/metacore/open_clip/version.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 03:43:03.000000 meta-core-3.7.27/metacore/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.27/metacore/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.27/metacore/utils/f3net.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.27/metacore/utils/model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.27/metacore/utils/prompt_ensemble.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-27 03:43:03.000000 meta-core-3.7.27/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      781 2023-07-27 03:41:15.000000 meta-core-3.7.27/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-27 09:25:00.000000 meta-core-3.7.28/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.28/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       55 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-27 09:25:00.000000 meta-core-3.7.28/meta_core.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/metacore/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.28/metacore/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/metacore/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.28/metacore/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5087 2023-07-27 09:16:31.000000 meta-core-3.7.28/metacore/app/ad_segment.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.28/metacore/app/segment.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/metacore/open_clip/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/coca_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/constants.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.28/metacore/open_clip/factory.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/generation_utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/hf_configs.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/hf_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/loss.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/metacore/open_clip/model_configs/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN101.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN50.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN50x16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN50x4.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/RN50x64.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-16-plus.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-H-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-L-14-280.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-L-14-336.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-L-16-320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-L-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-M-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-M-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-M-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-M-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-S-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-S-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-S-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-S-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-bigG-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-e-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/ViT-g-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/coca_ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/coca_ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/coca_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_base_w.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_base_w_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_large.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_large_d.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_large_d_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_small.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_tiny.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_xlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_xxlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/convnext_xxlarge_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7207 2023-07-21 11:10:23.000000 meta-core-3.7.28/metacore/open_clip/modified_resnet.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/openai.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/pretrained.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/push_to_hf_hub.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/timm_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.28/metacore/open_clip/tokenizer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/transform.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/transformer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.28/metacore/open_clip/version.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-27 09:25:00.000000 meta-core-3.7.28/metacore/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.28/metacore/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.28/metacore/utils/f3net.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.28/metacore/utils/model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.28/metacore/utils/prompt_ensemble.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-27 09:25:00.000000 meta-core-3.7.28/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      781 2023-07-27 09:24:44.000000 meta-core-3.7.28/setup.py
```

### Comparing `meta-core-3.7.27/meta_core.egg-info/SOURCES.txt` & `meta-core-3.7.28/meta_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/app/ad_segment.py` & `meta-core-3.7.28/metacore/app/ad_segment.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         with torch.no_grad(), torch.cuda.amp.autocast():
             image_features, patch_tokens = self.clip.encode_image(image_tensor, self.features_list)
             image_features /= image_features.norm(dim=-1, keepdim=True)
             text_features = []
             for cls in self.obj_list:
                 text_features.append(self.text_prompts[cls])
             text_features = torch.stack(text_features, dim=0)
+            text_probs = (100.0 * image_features @ text_features[0]).softmax(dim=-1)
+            score = round(float(text_probs.data.cpu().numpy()[0][1]), 2)
+
             patch_tokens = self.models[model_index](patch_tokens)
             anomaly_maps = []
             for layer in range(len(patch_tokens)):
                 patch_tokens[layer] /= patch_tokens[layer].norm(dim=-1, keepdim=True)
                 anomaly_map = (100.0 * patch_tokens[layer] @ text_features)
                 B, L, C = anomaly_map.shape
                 H = int(np.sqrt(L))
@@ -94,15 +97,15 @@
                 anomaly_map = torch.softmax(anomaly_map, dim=1)[:, 1, :, :]
                 anomaly_maps.append(anomaly_map.cpu().numpy())
             anomaly_map = np.sum(anomaly_maps, axis=0)
 
         mask = cv2.resize(normalize(anomaly_map[0]), (w, h))
         mask = mask > thre
         torch.cuda.empty_cache()
-        return mask
+        return mask, score
 
     @staticmethod
     def get_rect(mask):
         mask = (mask * 255).astype(np.uint8)
         _, pred = cv2.threshold(mask, 128, 255, cv2.THRESH_BINARY)
         contours, _ = cv2.findContours(pred, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
         if len(contours) < 1:
```

### Comparing `meta-core-3.7.27/metacore/app/segment.py` & `meta-core-3.7.28/metacore/app/segment.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/__init__.py` & `meta-core-3.7.28/metacore/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz` & `meta-core-3.7.28/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/coca_model.py` & `meta-core-3.7.28/metacore/open_clip/coca_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/factory.py` & `meta-core-3.7.28/metacore/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/hf_configs.py` & `meta-core-3.7.28/metacore/open_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/hf_model.py` & `meta-core-3.7.28/metacore/open_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/loss.py` & `meta-core-3.7.28/metacore/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/model.py` & `meta-core-3.7.28/metacore/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/model_configs/coca_ViT-B-32.json` & `meta-core-3.7.28/metacore/open_clip/model_configs/coca_ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/model_configs/coca_ViT-L-14.json` & `meta-core-3.7.28/metacore/open_clip/model_configs/coca_ViT-L-14.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/model_configs/coca_base.json` & `meta-core-3.7.28/metacore/open_clip/model_configs/coca_base.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json` & `meta-core-3.7.28/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/modified_resnet.py` & `meta-core-3.7.28/metacore/open_clip/modified_resnet.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/openai.py` & `meta-core-3.7.28/metacore/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/pretrained.py` & `meta-core-3.7.28/metacore/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/push_to_hf_hub.py` & `meta-core-3.7.28/metacore/open_clip/push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/timm_model.py` & `meta-core-3.7.28/metacore/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/tokenizer.py` & `meta-core-3.7.28/metacore/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/transform.py` & `meta-core-3.7.28/metacore/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/transformer.py` & `meta-core-3.7.28/metacore/open_clip/transformer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/open_clip/utils.py` & `meta-core-3.7.28/metacore/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/utils/f3net.py` & `meta-core-3.7.28/metacore/utils/f3net.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/utils/model.py` & `meta-core-3.7.28/metacore/utils/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/metacore/utils/prompt_ensemble.py` & `meta-core-3.7.28/metacore/utils/prompt_ensemble.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.27/setup.py` & `meta-core-3.7.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'numpy',
     'pillow',
     'torch',
     'ftfy',
     'regex',
 ]
 
-__version__ = 'V3.07.27'
+__version__ = 'V3.07.28'
 
 setup(
     name='meta-core',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

