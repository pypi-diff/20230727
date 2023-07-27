# Comparing `tmp/txrm2tiff-2.0.6.tar.gz` & `tmp/txrm2tiff-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-lchvb1le/txrm2tiff-2.0.6.tar", last modified: Mon Jul 17 14:01:02 2023, max compression
+gzip compressed data, was "/home/rky95813/Documents/Eclipse2/txrm2tiff/dist/.tmp-5klfs9y2/txrm2tiff-2.0.7.tar", last modified: Thu Jul 27 14:17:06 2023, max compression
```

## Comparing `txrm2tiff-2.0.6.tar` & `txrm2tiff-2.0.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-07-10 08:58:14.000000 txrm2tiff-2.0.6/.gitignore
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/.settings/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.6/.settings/org.eclipse.core.resources.prefs
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/.vscode/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.6/.vscode/launch.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-05-30 18:11:44.000000 txrm2tiff-2.0.6/.vscode/settings.json
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.6/LICENSE
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6967 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/README.md
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/conda/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1473 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/conda/meta.yaml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1536 2023-07-07 14:59:26.000000 txrm2tiff-2.0.6/pyproject.toml
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/setup.cfg
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/__main__.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/CallingCode-Regular.otf
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/src/txrm2tiff/font/License.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/src/txrm2tiff/info.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7057 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/main.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/abstract.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12824 2023-05-30 15:24:48.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/annot_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/ref_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3080 2023-05-30 14:59:57.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/save_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/shifts_mixin.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/v3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm/v5.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/general.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/images.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4715 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/logging.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/utils/shortcut_creation.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/enums.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/stream_dtypes.py
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7445 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/PKG-INFO
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/SOURCES.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/dependency_links.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/entry_points.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      170 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/requires.txt
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-07-17 14:01:01.000000 txrm2tiff-2.0.6/src/txrm2tiff.egg-info/top_level.txt
-drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-17 14:01:02.000000 txrm2tiff-2.0.6/tests/
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.6/tests/__init__.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_abstract_txrm.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10711 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_annotator.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_commandline_entrypoint.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5721 2023-07-17 13:59:18.000000 txrm2tiff-2.0.6/tests/test_file_handler.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_image_processing.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/tests/test_inspector.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14713 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_main.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.6/tests/test_metadata.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3858 2023-07-07 17:26:47.000000 txrm2tiff-2.0.6/tests/test_referencer.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.6/tests/test_saver.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.6/tests/test_setup_fuctions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.6/tests/test_shifts.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.6/tests/test_txrm_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.6/tests/test_txrm_property.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.6/tests/test_txrm_v5.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.6/tests/test_txrmv3.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.6/tests/test_util_functions.py
--rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.6/tests/test_with_files.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1290 2023-07-10 08:58:14.000000 txrm2tiff-2.0.7/.gitignore
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/.settings/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       64 2020-03-30 17:10:47.000000 txrm2tiff-2.0.7/.settings/org.eclipse.core.resources.prefs
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/.vscode/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      638 2021-03-02 11:54:13.000000 txrm2tiff-2.0.7/.vscode/launch.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      766 2023-07-26 16:51:44.000000 txrm2tiff-2.0.7/.vscode/settings.json
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1533 2020-03-30 17:10:47.000000 txrm2tiff-2.0.7/LICENSE
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6945 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/README.md
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/conda/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1482 2023-07-27 14:15:28.000000 txrm2tiff-2.0.7/conda/meta.yaml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1544 2023-07-27 14:15:28.000000 txrm2tiff-2.0.7/pyproject.toml
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       38 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/setup.cfg
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      122 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5966 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/__main__.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    42884 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/CallingCode-Regular.otf
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1554 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/src/txrm2tiff/font/License.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       89 2023-07-26 16:21:03.000000 txrm2tiff-2.0.7/src/txrm2tiff/info.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6531 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6992 2023-07-26 16:32:48.000000 txrm2tiff-2.0.7/src/txrm2tiff/main.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       28 2021-12-01 16:06:26.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    18841 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/abstract.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    12885 2023-07-26 17:09:35.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/annot_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1357 2021-12-14 13:07:27.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     8432 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/ref_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3086 2023-07-26 16:28:35.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/save_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1623 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/shifts_mixin.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1560 2023-05-30 10:24:37.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3158 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/v3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2928 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm/v5.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       45 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4667 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/general.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2649 2021-12-01 16:08:13.000000 txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/images.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        0 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4715 2023-07-17 13:59:18.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      415 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6400 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      818 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/logging.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5618 2023-07-07 17:08:26.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2570 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/utils/shortcut_creation.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       50 2021-11-26 16:04:02.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1856 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/enums.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3334 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/stream_dtypes.py
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7423 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/PKG-INFO
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1853 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)        1 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       54 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/entry_points.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      178 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/requires.txt
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)       10 2023-07-27 14:17:05.000000 txrm2tiff-2.0.7/src/txrm2tiff.egg-info/top_level.txt
+drwxrwxr-x   0 rky95813 (1214969) rky95813 (1214969)        0 2023-07-27 14:17:06.000000 txrm2tiff-2.0.7/tests/
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      193 2021-02-08 17:40:15.000000 txrm2tiff-2.0.7/tests/__init__.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    11184 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_abstract_txrm.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    10974 2023-07-26 17:15:31.000000 txrm2tiff-2.0.7/tests/test_annotator.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9650 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_commandline_entrypoint.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5721 2023-07-17 13:59:18.000000 txrm2tiff-2.0.7/tests/test_file_handler.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5849 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_image_processing.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2777 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/tests/test_inspector.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)    14720 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/tests/test_main.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     4036 2023-05-30 10:24:41.000000 txrm2tiff-2.0.7/tests/test_metadata.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3859 2023-07-26 16:31:57.000000 txrm2tiff-2.0.7/tests/test_referencer.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     9936 2023-05-30 16:23:06.000000 txrm2tiff-2.0.7/tests/test_saver.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     1455 2021-12-01 16:07:16.000000 txrm2tiff-2.0.7/tests/test_setup_fuctions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2246 2021-12-01 16:29:22.000000 txrm2tiff-2.0.7/tests/test_shifts.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     5057 2021-12-01 16:07:23.000000 txrm2tiff-2.0.7/tests/test_txrm_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     2682 2023-05-30 10:44:58.000000 txrm2tiff-2.0.7/tests/test_txrm_property.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     3709 2023-05-30 15:25:01.000000 txrm2tiff-2.0.7/tests/test_txrm_v5.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     6007 2023-05-30 15:10:23.000000 txrm2tiff-2.0.7/tests/test_txrmv3.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)      834 2021-12-01 16:07:35.000000 txrm2tiff-2.0.7/tests/test_util_functions.py
+-rw-rw-r--   0 rky95813 (1214969) rky95813 (1214969)     7056 2021-12-14 13:07:27.000000 txrm2tiff-2.0.7/tests/test_with_files.py
```

### Comparing `txrm2tiff-2.0.6/.gitignore` & `txrm2tiff-2.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/.vscode/launch.json` & `txrm2tiff-2.0.7/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/.vscode/settings.json` & `txrm2tiff-2.0.7/.vscode/settings.json`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         "-v",
         "--logging-level=INFO",
         // // optional arguments to skip drmaa job submission and end to end tests
         // "-e=*end*",
         // "-e=*drmaa*",
         // "-e=*test_get_cluster_job_data",
     ],
-    "python.testing.pytestEnabled": true,
-    "python.testing.unittestEnabled": false,
+    "python.testing.pytestEnabled": false,
+    "python.testing.unittestEnabled": true,
     "python.testing.nosetestsEnabled": false,
     "python.testing.unittestArgs": [
         "-v",
         "-s",
         "tests",
         "-p",
         "test_*.py",
```

### Comparing `txrm2tiff-2.0.6/LICENSE` & `txrm2tiff-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/PKG-INFO` & `txrm2tiff-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.6
+Version: 2.0.7
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -52,15 +52,15 @@
 
 \*\* with the exception of images, which do get the image data type saved separately.
 
 **NOTE:** any commands beginning with `txrm2tiff` are essentially equivalent to usng `python -m txrm2tiff` (arguments will be parsed by the same parser via either method). This may be useful if there were any installation issues.
 
 ---
 
-If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tif"/".ome.tiff" as appropriate. The ".ome" signifies the OME XML metadata header.
+If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tiff". The ".ome" signifies the OME XML metadata header.
 
 **dragndrop.bat** has been supplied allowing windows users to drag and drop individual files or entire directories for processing (note: you cannot set output path this way). This may require some setup depending on your Python installation, so please see the file.
 
 ##### Logging options are:
 * debug OR 1
 * info OR 2
 * warning OR 3
@@ -76,24 +76,24 @@
 
 `txrm2tiff -i input.txrm -r ref_stack.txrm`
 Saves "input.ome.tiff" with a reference image applied from running Despeckle \& Average on the the txrm stack. This Despeckle \& Average algorithm is near-identical to the Zeiss algorithm, based on their logic.
 
 `txrm2tiff --input input.txrm --reference ref_single.xrm --ignore-ref`
 Saves "input.ome.tiff" with custom reference applied from a single image (e.g. a Despeckled_Ave.xrm file). If a custom reference is supplied, the ignore reference argument will be ignored.
 
-`txrm2tiff -i input.xrm -o custom-output.ome.tif`
-Saves "custom-output.ome.tif" with reference applied, if available.
+`txrm2tiff -i input.xrm -o custom-output.ome.tiff`
+Saves "custom-output.ome.tiff" with reference applied, if available.
 
 `txrm2tiff -i input.xrm --annotate`
-Saves "input.ome.tiff", as well as a separate file "input_Annotated.tif", which has annotations overlaid (if annotations are found) and scale bar.
+Saves "input.ome.tiff", as well as a separate file "input_Annotated.tiff", which has annotations overlaid (if annotations are found) and scale bar.
 
 `txrm2tiff --input input.xrm --ignore-ref --set-logging debug`
 Saves "input.ome.tiff" and ignores any reference, shows debug and above level log messages.
 
-`txrm2tiff -i input.xrm --output custom-output.ome.tif --set-logging error`
+`txrm2tiff -i input.xrm --output custom-output.ome.tiff --set-logging error`
 Saves "custom-output.ome.tiff", shows error and above level log messages.
 
 **To batch convert:**
 `txrm2tiff --input path/to/inputDirectory/`
 Converts all XRM/TXRM files within input_directory with reference applied, if available.
 
 `txrm2tiff --input path/to/inputDirectory/ --ignore-ref`
```

### Comparing `txrm2tiff-2.0.6/README.md` & `txrm2tiff-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 \*\* with the exception of images, which do get the image data type saved separately.
 
 **NOTE:** any commands beginning with `txrm2tiff` are essentially equivalent to usng `python -m txrm2tiff` (arguments will be parsed by the same parser via either method). This may be useful if there were any installation issues.
 
 ---
 
-If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tif"/".ome.tiff" as appropriate. The ".ome" signifies the OME XML metadata header.
+If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tiff". The ".ome" signifies the OME XML metadata header.
 
 **dragndrop.bat** has been supplied allowing windows users to drag and drop individual files or entire directories for processing (note: you cannot set output path this way). This may require some setup depending on your Python installation, so please see the file.
 
 ##### Logging options are:
 * debug OR 1
 * info OR 2
 * warning OR 3
@@ -62,24 +62,24 @@
 
 `txrm2tiff -i input.txrm -r ref_stack.txrm`
 Saves "input.ome.tiff" with a reference image applied from running Despeckle \& Average on the the txrm stack. This Despeckle \& Average algorithm is near-identical to the Zeiss algorithm, based on their logic.
 
 `txrm2tiff --input input.txrm --reference ref_single.xrm --ignore-ref`
 Saves "input.ome.tiff" with custom reference applied from a single image (e.g. a Despeckled_Ave.xrm file). If a custom reference is supplied, the ignore reference argument will be ignored.
 
-`txrm2tiff -i input.xrm -o custom-output.ome.tif`
-Saves "custom-output.ome.tif" with reference applied, if available.
+`txrm2tiff -i input.xrm -o custom-output.ome.tiff`
+Saves "custom-output.ome.tiff" with reference applied, if available.
 
 `txrm2tiff -i input.xrm --annotate`
-Saves "input.ome.tiff", as well as a separate file "input_Annotated.tif", which has annotations overlaid (if annotations are found) and scale bar.
+Saves "input.ome.tiff", as well as a separate file "input_Annotated.tiff", which has annotations overlaid (if annotations are found) and scale bar.
 
 `txrm2tiff --input input.xrm --ignore-ref --set-logging debug`
 Saves "input.ome.tiff" and ignores any reference, shows debug and above level log messages.
 
-`txrm2tiff -i input.xrm --output custom-output.ome.tif --set-logging error`
+`txrm2tiff -i input.xrm --output custom-output.ome.tiff --set-logging error`
 Saves "custom-output.ome.tiff", shows error and above level log messages.
 
 **To batch convert:**
 `txrm2tiff --input path/to/inputDirectory/`
 Converts all XRM/TXRM files within input_directory with reference applied, if available.
 
 `txrm2tiff --input path/to/inputDirectory/ --ignore-ref`
```

### Comparing `txrm2tiff-2.0.6/conda/meta.yaml` & `txrm2tiff-2.0.7/conda/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% set name = "txrm2tiff" %}
-{% set version = "2.0.6" %}
+{% set version = "2.0.7" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   path: ../
@@ -22,15 +22,15 @@
   run:
     - python
     - numpy >=1.20.0
     - scipy >=1.3.3
     - tifffile >=2020.9.30
     - omexml-dls >=1.1.0
     - olefile >=0.46
-    - pillow >=5.3
+    - pillow >=5.3, <10.0.0
     - pywin32  # [win]
 
 test:
   imports:
     - {{ name }}
     - win32com.client  # [win]
   source_files:
```

### Comparing `txrm2tiff-2.0.6/pyproject.toml` & `txrm2tiff-2.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 dynamic = ["version", "readme"]
 dependencies = [
     "tifffile>=2020.9.30",
     "numpy>=1.20",
     "omexml-dls>=1.1.0",
     "olefile>=0.46",
     "scipy>=1.3.3",
-    "pillow>=5.3",
+    "pillow>=5.3,<10.0.0",
     "pywin32;platform_system=='Windows'",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "txrm2tiff.info.__version__"}
 readme = {file = "README.md", content-type="text/markdown"}
```

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/__main__.py` & `txrm2tiff-2.0.7/src/txrm2tiff/__main__.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/font/CallingCode-Regular.otf` & `txrm2tiff-2.0.7/src/txrm2tiff/font/CallingCode-Regular.otf`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/font/License.txt` & `txrm2tiff-2.0.7/src/txrm2tiff/font/License.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/inspector.py` & `txrm2tiff-2.0.7/src/txrm2tiff/inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/main.py` & `txrm2tiff-2.0.7/src/txrm2tiff/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,12 @@
             return output_path
     return _set_output_suffix(output_path, current_suffix=input_path.suffix)
 
 
 def _set_output_suffix(filepath: Path, current_suffix: Optional[str] = None) -> Path:
     if current_suffix is None:
         current_suffix = filepath.suffix
-    if current_suffix == ".txrm":
+    if current_suffix.lower() in (".txrm", ".xrm"):
         return filepath.with_suffix(".ome.tiff")
-    elif current_suffix == ".xrm":
-        return filepath.with_suffix(".ome.tif")
     else:
         logging.error("Invalid file extension: %s", current_suffix)
         raise NameError(f"Invalid file extension: {current_suffix}")
```

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/abstract.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/abstract.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/annot_mixin.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/annot_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return self.annotated_image
 
     @property
     def thickness_modifier(self) -> float:
         """This set a multiplier so that lines are visible when the image is at a sensible size"""
         if not hasattr(self, "output_shape"):
             return 1.0
-        return np.mean(self.output_shape[0]) / 500.0
+        return np.mean(self.output_shape[1:]) / 500.0
 
     def _create_image_and_draw(self):
         """Create transparent RGBA image with appropriate 2D dimensions for output image(s)"""
         im = Image.new("RGBA", self.output_shape[:0:-1], (0, 0, 0, 0))
         draw = ImageDraw.Draw(im, mode="RGBA")
         return im, draw
 
@@ -178,18 +178,18 @@
     def _not_implemented(*args):
         """Do nothing"""
         pass
 
     def _plot_line(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
-        x1 = self.read_stream(f"{stream_stem}/X1", XDT.XRM_DOUBLE, strict=True)[0]
-        x2 = self.read_stream(f"{stream_stem}/X2", XDT.XRM_DOUBLE, strict=True)[0]
-        y1 = self.read_stream(f"{stream_stem}/Y1", XDT.XRM_DOUBLE, strict=True)[0]
-        y2 = self.read_stream(f"{stream_stem}/Y2", XDT.XRM_DOUBLE, strict=True)[0]
+        x1 = self.read_stream(f"{stream_stem}/X1", XDT.XRM_FLOAT, strict=True)[0]
+        x2 = self.read_stream(f"{stream_stem}/X2", XDT.XRM_FLOAT, strict=True)[0]
+        y1 = self.read_stream(f"{stream_stem}/Y1", XDT.XRM_FLOAT, strict=True)[0]
+        y2 = self.read_stream(f"{stream_stem}/Y2", XDT.XRM_FLOAT, strict=True)[0]
 
         draw.line(self._flip_y((x1, y1), (x2, y2)), fill=colour, width=thickness)
 
     def __extract_rectangle_coords(self, stream_stem: str) -> Tuple[Tuple[int]]:
         x = []
         y = []
         x.append(
@@ -231,34 +231,38 @@
         xy = self.__extract_rectangle_coords(stream_stem)
 
         draw.ellipse(xy, outline=colour, width=thickness)
 
     def _plot_polygon(self, draw: ImageDraw, stream_stem: str) -> None:
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
-        total_points = self.read_stream(f"{stream_stem}/TotalPts", np.uintc)[0]
-        xs = self.read_stream(f"{stream_stem}/PointX", XDT.XRM_DOUBLE, strict=True)[
+        total_points = self.read_stream(
+            f"{stream_stem}/TotalPts", XDT.XRM_UNSIGNED_INT
+        )[0]
+        xs = self.read_stream(f"{stream_stem}/PointX", XDT.XRM_FLOAT, strict=True)[
             :total_points
         ]
-        ys = self.read_stream(f"{stream_stem}/PointY", XDT.XRM_DOUBLE, strict=True)[
+        ys = self.read_stream(f"{stream_stem}/PointY", XDT.XRM_FLOAT, strict=True)[
             :total_points
         ]
         xs.append(xs[0])  # Link beginning and end points
         ys.append(ys[0])
 
         draw.line(self._flip_y(*zip(xs, ys)), fill=colour, width=thickness)
 
     def _plot_polyline(
         self, draw: ImageDraw, stream_stem: str, joint: Optional[str] = None
     ):
         colour = self._get_colour(stream_stem)
         thickness = self._get_thickness(stream_stem)
-        total_points = self.read_stream(f"{stream_stem}/TotalPts", np.uintc)[0]
-        xs = self.read_stream(f"{stream_stem}/PointX", XDT.XRM_DOUBLE, strict=True)
-        ys = self.read_stream(f"{stream_stem}/PointY", XDT.XRM_DOUBLE, strict=True)
+        total_points = self.read_stream(
+            f"{stream_stem}/TotalPts", XDT.XRM_UNSIGNED_INT
+        )[0]
+        xs = self.read_stream(f"{stream_stem}/PointX", XDT.XRM_FLOAT, strict=True)
+        ys = self.read_stream(f"{stream_stem}/PointY", XDT.XRM_FLOAT, strict=True)
 
         draw.line(
             self._flip_y(*zip(xs[:total_points], ys[:total_points])),
             fill=colour,
             width=thickness,
             joint=joint,
         )
```

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/main.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/main.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/ref_mixin.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/ref_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/save_mixin.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/save_mixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,17 +62,17 @@
                 and self.annotated_image is not None
             ):
                 if annotated_path is None:
                     # Generate default path
                     filename = filepath.name
                     if filename.lower().endswith(".ome.tiff"):
                         # Special case for ome.tiff
-                        stem, suffix = filename.rsplit(".ome.")
+                        stem, suffix = filename.rsplit(".ome.", 1)
                     else:
-                        stem, suffix = filename.rsplit(".")
+                        stem, suffix = filename.rsplit(".", 1)
                     annotated_path = filepath.parent / f"{stem}_Annotated.{suffix}"
                 self.save_annotations(annotated_path, mkdir=mkdir, strict=strict)
             return True
         except Exception:
             logging.error("Saving failed", exc_info=not strict)
             if strict:
                 raise
```

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/shifts_mixin.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/shifts_mixin.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/txrm_property.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/v3.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/v3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm/v5.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm/v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/general.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/general.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/txrm_functions/images.py` & `txrm2tiff-2.0.7/src/txrm2tiff/txrm_functions/images.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/utils/file_handler.py` & `txrm2tiff-2.0.7/src/txrm2tiff/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/utils/image_processing.py` & `txrm2tiff-2.0.7/src/txrm2tiff/utils/image_processing.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/utils/logging.py` & `txrm2tiff-2.0.7/src/txrm2tiff/utils/logging.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/utils/metadata.py` & `txrm2tiff-2.0.7/src/txrm2tiff/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/utils/shortcut_creation.py` & `txrm2tiff-2.0.7/src/txrm2tiff/utils/shortcut_creation.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/enums.py` & `txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/enums.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff/xradia_properties/stream_dtypes.py` & `txrm2tiff-2.0.7/src/txrm2tiff/xradia_properties/stream_dtypes.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff.egg-info/PKG-INFO` & `txrm2tiff-2.0.7/src/txrm2tiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txrm2tiff
-Version: 2.0.6
+Version: 2.0.7
 Summary: A converter for Zeiss txrm and xrm files, created by & for B24 of Diamond Light Source
 Author-email: Thomas Fish <thomas.fish@diamond.ac.uk>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -52,15 +52,15 @@
 
 \*\* with the exception of images, which do get the image data type saved separately.
 
 **NOTE:** any commands beginning with `txrm2tiff` are essentially equivalent to usng `python -m txrm2tiff` (arguments will be parsed by the same parser via either method). This may be useful if there were any installation issues.
 
 ---
 
-If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tif"/".ome.tiff" as appropriate. The ".ome" signifies the OME XML metadata header.
+If no output path is supplied, the output file will be placed at the input path with the extension ".ome.tiff". The ".ome" signifies the OME XML metadata header.
 
 **dragndrop.bat** has been supplied allowing windows users to drag and drop individual files or entire directories for processing (note: you cannot set output path this way). This may require some setup depending on your Python installation, so please see the file.
 
 ##### Logging options are:
 * debug OR 1
 * info OR 2
 * warning OR 3
@@ -76,24 +76,24 @@
 
 `txrm2tiff -i input.txrm -r ref_stack.txrm`
 Saves "input.ome.tiff" with a reference image applied from running Despeckle \& Average on the the txrm stack. This Despeckle \& Average algorithm is near-identical to the Zeiss algorithm, based on their logic.
 
 `txrm2tiff --input input.txrm --reference ref_single.xrm --ignore-ref`
 Saves "input.ome.tiff" with custom reference applied from a single image (e.g. a Despeckled_Ave.xrm file). If a custom reference is supplied, the ignore reference argument will be ignored.
 
-`txrm2tiff -i input.xrm -o custom-output.ome.tif`
-Saves "custom-output.ome.tif" with reference applied, if available.
+`txrm2tiff -i input.xrm -o custom-output.ome.tiff`
+Saves "custom-output.ome.tiff" with reference applied, if available.
 
 `txrm2tiff -i input.xrm --annotate`
-Saves "input.ome.tiff", as well as a separate file "input_Annotated.tif", which has annotations overlaid (if annotations are found) and scale bar.
+Saves "input.ome.tiff", as well as a separate file "input_Annotated.tiff", which has annotations overlaid (if annotations are found) and scale bar.
 
 `txrm2tiff --input input.xrm --ignore-ref --set-logging debug`
 Saves "input.ome.tiff" and ignores any reference, shows debug and above level log messages.
 
-`txrm2tiff -i input.xrm --output custom-output.ome.tif --set-logging error`
+`txrm2tiff -i input.xrm --output custom-output.ome.tiff --set-logging error`
 Saves "custom-output.ome.tiff", shows error and above level log messages.
 
 **To batch convert:**
 `txrm2tiff --input path/to/inputDirectory/`
 Converts all XRM/TXRM files within input_directory with reference applied, if available.
 
 `txrm2tiff --input path/to/inputDirectory/ --ignore-ref`
```

### Comparing `txrm2tiff-2.0.6/src/txrm2tiff.egg-info/SOURCES.txt` & `txrm2tiff-2.0.7/src/txrm2tiff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_abstract_txrm.py` & `txrm2tiff-2.0.7/tests/test_abstract_txrm.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_annotator.py` & `txrm2tiff-2.0.7/tests/test_annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         expected_output[y0, x0 : x1 + 1, 1] = fill
         expected_output[y1 : y0 + 1, x0, 1] = fill
         expected_output[y1, x0 : x1 + 1, 1] = fill
         expected_output[y1 : y0 + 1, x1, 1] = fill
 
         assert_array_equal(np.asarray(image), expected_output)
 
+    def test_thickness_modifier(self):
+        ann = annot_mixin.AnnotatorMixin()
+        ann.output_shape = (6, 500, 1500)
+        self.assertEqual(ann.thickness_modifier, 2.0)
+
     def test_line(self):
         fill = 125
         x0, x1 = 1, 4
         y = 4
         im_size = 5
         imshape = (1, im_size, im_size)
         im = Image.new("RGBA", imshape[:0:-1], (0, 0, 0, 0))
@@ -153,15 +158,15 @@
                 ann.read_stream.side_effect = [[xs[0]], [ys[0]], [xs[1]], [ys[1]]]
                 ann._plot_ellipse(draw, "")
 
         output = np.asarray(im)
 
         self.assertTrue((output[:, :, 0] == 0).any())  # Red
         self.assertTrue((output[:, :, 2] == 0).any())  # Blue
-        for (x, y) in ann._flip_y(
+        for x, y in ann._flip_y(
             (x_mid, ys[0]), (xs[0], y_mid), (x_mid, ys[1]), (xs[1], y_mid)
         ):
             self.assertEqual(
                 output[y, x, 1], fill, msg="Failed for y, x of %i, %i" % (y, x)
             )
 
     def test_polyline(self):
@@ -226,22 +231,25 @@
         ann = annot_mixin.AnnotatorMixin()
         ann.output_shape = (z, y, x)
         ann.has_stream = MagicMock(return_value=False)
         im, draw = ann._create_image_and_draw()
         self.assertEqual(np.asarray(im).shape, (y, x, channels))
 
     def test_annotate(self):
+        class TestAnnotator(annot_mixin.AnnotatorMixin):
+            @property
+            def thickness_modifier(self) -> float:
+                return 1
+
         fill = (0, 125, 0)
         x0, x1 = 1, 4
         y = 4
         im = np.zeros((5, 6, 7), dtype=np.uint8)  # Z, Y, X
         num_annotations = 1
-        Ann = annot_mixin.AnnotatorMixin
-        Ann.thickness_modifier = 1
-        ann = Ann()
+        ann = TestAnnotator()
         ann.get_output = MagicMock(return_value=np.flip(im, axis=1))
         ann.output_shape = im.shape
         ann.has_stream = MagicMock(return_value=True)
         ann.read_stream = MagicMock(
             side_effect=[  # Draw a single line with the listed points
                 [num_annotations],
                 [AnnotationTypes.ANN_LINE.value],
@@ -261,18 +269,18 @@
 
             ann.annotate()
 
         ann.read_stream.assert_has_calls(
             [
                 call("Annot/TotalAnn", strict=True),
                 call("Annot/Ann0/AnnType", XrmDataTypes.XRM_INT, strict=True),
-                call("Annot/Ann0/X1", XrmDataTypes.XRM_DOUBLE, strict=True),
-                call("Annot/Ann0/X2", XrmDataTypes.XRM_DOUBLE, strict=True),
-                call("Annot/Ann0/Y1", XrmDataTypes.XRM_DOUBLE, strict=True),
-                call("Annot/Ann0/Y2", XrmDataTypes.XRM_DOUBLE, strict=True),
+                call("Annot/Ann0/X1", XrmDataTypes.XRM_FLOAT, strict=True),
+                call("Annot/Ann0/X2", XrmDataTypes.XRM_FLOAT, strict=True),
+                call("Annot/Ann0/Y1", XrmDataTypes.XRM_FLOAT, strict=True),
+                call("Annot/Ann0/Y2", XrmDataTypes.XRM_FLOAT, strict=True),
             ]
         )
 
         # Extra 3 at the end for RGB
         expected_output = np.zeros((*im.shape, 3), dtype=np.uint8)
         y = expected_output.shape[1] - 1 - y  # Invert y axis
         expected_output[:, y, x0 : x1 + 1, :] = fill
```

### Comparing `txrm2tiff-2.0.6/tests/test_commandline_entrypoint.py` & `txrm2tiff-2.0.7/tests/test_commandline_entrypoint.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_file_handler.py` & `txrm2tiff-2.0.7/tests/test_file_handler.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_image_processing.py` & `txrm2tiff-2.0.7/tests/test_image_processing.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_inspector.py` & `txrm2tiff-2.0.7/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_main.py` & `txrm2tiff-2.0.7/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 
 
 class TestRun(unittest.TestCase):
     def test_set_output_suffix(self):
         txrm_output = _set_output_suffix(Path("file.txrm"))
         self.assertEqual("file.ome.tiff", str(txrm_output))
         xrm_output = _set_output_suffix(Path("file.xrm"))
-        self.assertEqual("file.ome.tif", str(xrm_output))
+        self.assertEqual("file.ome.tiff", str(xrm_output))
         txrm_output2 = _set_output_suffix(Path("file.extension"), ".txrm")
         self.assertEqual("file.ome.tiff", str(txrm_output2))
         xrm_output2 = _set_output_suffix(Path("file.extension"), ".xrm")
-        self.assertEqual("file.ome.tif", str(xrm_output2))
+        self.assertEqual("file.ome.tiff", str(xrm_output2))
         with self.assertRaises(NameError):
             _set_output_suffix(Path("file.bad_extension"), None)
 
     def test_set_output_suffix(self):
         txrm_output = _set_output_suffix(Path("file.txrm"))
         xrm_output = _set_output_suffix(Path("file.xrm"))
         self.assertEqual("file.ome.tiff", str(txrm_output))
-        self.assertEqual("file.ome.tif", str(xrm_output))
+        self.assertEqual("file.ome.tiff", str(xrm_output))
 
     @parameterized.expand([(Txrm3,), (Txrm5,)])
     @patch("txrm2tiff.main.open_txrm")
     def test_convert_and_save(self, TxrmClass, mocked_open_txrm):
         input_filepath = Path("test_file.txrm")
 
         txrm = MagicMock(auto_spec=TxrmClass)
@@ -102,21 +102,21 @@
         input_filepath = Path("test_file.txrm")
         txrm = MagicMock(auto_spec=TxrmClass)
         txrm.path = input_filepath
         txrm.name = input_filepath.name
         _convert_file(txrm, None, True, True)
         txrm.annotate.assert_called_once_with()
 
-    @parameterized.expand([(".txrm", ".ome.tiff"), (".xrm", ".ome.tif")])
+    @parameterized.expand([(".txrm", ".ome.tiff"), (".xrm", ".ome.tiff")])
     def test_decide_output_path(self, input_suffix, output_suffix):
         filepath = Path("./path/to/thisisafile.ext")
         output = _decide_output_path(filepath.with_suffix(input_suffix), None)
         self.assertEqual(output, filepath.with_suffix(output_suffix))
 
-    @parameterized.expand([(".txrm", ".ome.tiff"), (".xrm", ".ome.tif")])
+    @parameterized.expand([(".txrm", ".ome.tiff"), (".xrm", ".ome.tiff")])
     def test_decide_output_path_with_output_dir(self, input_suffix, output_suffix):
         filepath = Path("./path/to/thisisafile.ext")
         output_dir = Path("./a/different/path")
         output = _decide_output_path(filepath.with_suffix(input_suffix), output_dir)
         self.assertEqual(
             output, (output_dir / filepath.name).with_suffix(output_suffix)
         )
@@ -173,15 +173,15 @@
         ]
 
         xrm_files = [
             input_dir / f"{fname}.xrm" for fname in generate_random_strings(num_xrm)
         ]
         input_files = txrm_files + xrm_files
         output_files = [f.with_suffix(".ome.tiff") for f in txrm_files] + [
-            f.with_suffix(".ome.tif") for f in xrm_files
+            f.with_suffix(".ome.tiff") for f in xrm_files
         ]
         mocked_find_files.return_value = input_files
         mocked_suffix_definer.side_effect = output_files
         _batch_convert_files(input_dir)
         mocked_convert_save.assert_has_calls(
             [
                 call(f_in, f_out, None, True, False, None, True, False)
@@ -205,15 +205,15 @@
             Path(f"txrm_dir/{fname}.txrm")
             for fname in generate_random_strings(num_txrm)
         ]
 
         xrm_files = [Path(f"{fname}.xrm") for fname in generate_random_strings(num_xrm)]
         input_files = txrm_files + xrm_files
         output_files = [f.with_suffix(".ome.tiff") for f in txrm_files] + [
-            f.with_suffix(".ome.tif") for f in xrm_files
+            f.with_suffix(".ome.tiff") for f in xrm_files
         ]
         input_paths = [input_dir / s for s in input_files]
         output_paths = [output_dir / s for s in output_files]
         mocked_find_files.return_value = input_paths
         _batch_convert_files(input_dir, output_dir)
         mocked_convert_save.assert_has_calls(
             [
```

### Comparing `txrm2tiff-2.0.6/tests/test_metadata.py` & `txrm2tiff-2.0.7/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_referencer.py` & `txrm2tiff-2.0.7/tests/test_referencer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     def test_apply_reference_tiff(self):
         referencer = ReferenceMixin()
         with patch.object(
             referencer, "apply_custom_reference_from_array"
         ) as mocked_apply_array:
             with TemporaryDirectory("tiff_ref_test_", dir=".") as tmp_dir:
                 array = np.ones((3, 5, 5))
-                tif_path = Path(tmp_dir) / "image.ome.tif"
+                tif_path = Path(tmp_dir) / "image.ome.tiff"
                 manual_save(tif_path, array)
 
                 referencer.apply_reference(tif_path, False)
 
         args = mocked_apply_array.call_args[0]
         kwargs = mocked_apply_array.call_args[1]
         assert_array_equal(args[0], array)
@@ -62,15 +62,15 @@
             with TemporaryDirectory("tiff_ref_test_", dir=".") as tmp_dir:
                 array = np.ones((3, 5, 5))
                 exposures = (1, 2, 3)
                 metadata = OMEXML()
                 metadata.image().Pixels.set_plane_count(len(exposures))
                 for idx, exposure in enumerate(exposures):
                     metadata.image().Pixels.Plane(idx).set_ExposureTime(exposure)
-                tif_path = Path(tmp_dir) / "image.ome.tif"
+                tif_path = Path(tmp_dir) / "image.ome.tiff"
                 manual_save(tif_path, array, metadata=metadata)
 
                 referencer.apply_reference(tif_path, True)
         args = mocked_apply_array.call_args[0]
         kwargs = mocked_apply_array.call_args[1]
         assert_array_equal(args[0], array)
         self.assertEqual(
@@ -78,15 +78,14 @@
         )
 
     @parameterized.expand([(Txrm3,), (Txrm5,)])
     @patch("txrm2tiff.txrm.ref_mixin.file_can_be_opened", MagicMock(return_value=True))
     @patch("txrm2tiff.txrm.ref_mixin.isOleFile", MagicMock(return_value=True))
     @patch("txrm2tiff.txrm.ref_mixin.main.open_txrm")
     def test_apply_refererence_txrm(self, TxrmClass, mocked_open_txrm):
-
         referencer = ReferenceMixin()
         txrm = MagicMock(auto_spec=TxrmClass)
         mocked_open_txrm.return_value.__enter__.return_value = txrm
 
         with patch.object(referencer, "apply_reference_from_txrm") as mocked_from_txrm:
             referencer.apply_reference("test/path.txrm")
             mocked_from_txrm.assert_called_once_with(txrm)
```

### Comparing `txrm2tiff-2.0.6/tests/test_saver.py` & `txrm2tiff-2.0.7/tests/test_saver.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_setup_fuctions.py` & `txrm2tiff-2.0.7/tests/test_setup_fuctions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_shifts.py` & `txrm2tiff-2.0.7/tests/test_shifts.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_txrm_functions.py` & `txrm2tiff-2.0.7/tests/test_txrm_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_txrm_property.py` & `txrm2tiff-2.0.7/tests/test_txrm_property.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_txrm_v5.py` & `txrm2tiff-2.0.7/tests/test_txrm_v5.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_txrmv3.py` & `txrm2tiff-2.0.7/tests/test_txrmv3.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_util_functions.py` & `txrm2tiff-2.0.7/tests/test_util_functions.py`

 * *Files identical despite different names*

### Comparing `txrm2tiff-2.0.6/tests/test_with_files.py` & `txrm2tiff-2.0.7/tests/test_with_files.py`

 * *Files identical despite different names*

