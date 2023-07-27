# Comparing `tmp/mne-pipeline-hd-0.3.2a0.tar.gz` & `tmp/mne-pipeline-hd-0.3.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-pipeline-hd-0.3.2a0.tar", last modified: Sat Aug 27 00:04:35 2022, max compression
+gzip compressed data, was "mne-pipeline-hd-0.3.3a0.tar", last modified: Thu Jul 27 11:12:00 2023, max compression
```

## Comparing `mne-pipeline-hd-0.3.2a0.tar` & `mne-pipeline-hd-0.3.3a0.tar`

### file list

```diff
@@ -1,73 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.687513 mne-pipeline-hd-0.3.2a0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-08-27 00:04:35.687513 mne-pipeline-hd-0.3.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.679513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3887 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.679513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/check_ressources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/dev_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.679513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    58768 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)    28719 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.683513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49434 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/base_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    12351 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     9540 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/education_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    65551 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/function_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    21323 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    85862 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/loading_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    28092 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)    30392 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    71569 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/parameter_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)    23188 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/plot_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     8630 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     6968 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/welcome_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.683513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15286 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)    17250 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/function_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/legacy.py
--rw-r--r--   0 runner    (1001) docker     (121)    60420 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/loading.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)     9614 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    27128 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.687513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/default_settings.json
--rw-r--r--   0 runner    (1001) docker     (121)     8797 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/functions.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/license.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_license.txt
--rw-r--r--   0 runner    (1001) docker     (121)    21717 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    24707 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png
--rw-r--r--   0 runner    (1001) docker     (121)    16878 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.687513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     8139 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_param_guis.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_qsettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_welcome_window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 00:04:35.679513 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4911 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2276 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-27 00:04:35.000000 mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 00:04:35.687513 mne-pipeline-hd-0.3.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-08-27 00:04:26.000000 mne-pipeline-hd-0.3.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.759886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/check_ressources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/dev_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57606 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28799 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.767886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49094 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/base_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/education_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65760 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/function_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84283 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/loading_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27186 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70457 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/parameter_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/plot_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/welcome_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.771885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/function_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59334 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.771885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/default_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/functions.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21717 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24707 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_param_guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_qsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_welcome_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/setup.cfg
```

### Comparing `mne-pipeline-hd-0.3.2a0/PKG-INFO` & `mne-pipeline-hd-0.3.3a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,124 @@
 Metadata-Version: 2.1
 Name: mne-pipeline-hd
-Version: 0.3.2a0
-Summary: A pipeline-GUI for brain-data analysis with MNE-Python
-Home-page: https://github.com/marsipu/mne-pipeline-hd
-Author: Martin Schulz
-Author-email: dev@earthman-music.de
-License: BSD (3-clause)
+Version: 0.3.3a0
+Summary: A Pipeline-GUI for MNE-Python from MEG-Lab Heidelberg
+Author-email: Martin Schulz <dev@mgschulz.de>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/marsipu/mne-pipeline-hd
+Project-URL: Repository, https://github.com/marsipu/mne-pipeline-hd.git
+Keywords: mne-python,meg,eeg,pipeline,gui,heidelberg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # mne-pipeline-hd
-### A [MNE-Python](https://mne.tools/stable/index.html) Pipeline-GUI for MEG-Lab Heidelberg
-###### inspired by: [Andersen L.M. 2018](https://doi.org/10.3389/fnins.2018.00006)
+
+### A Pipeline-GUI for [MNE-Python](https://mne.tools/stable/index.html)  from MEG-Lab Heidelberg
 
 ![mne-pipeline-hd Logo](mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg)
 
 ## Installation
-1. Install MNE-python as instructed on the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
-I would recommend to install in a separate conda environment with:
-`conda env create -n mne_p -f environment.yml`
+
+1. Install MNE-python as instructed on
+   the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
+   I would recommend to install in a separate conda environment with:
+   `conda env create -n mne_p -f environment.yml`
 2. `conda activate mne_p`
 3. `pip install https://github.com/marsipu/mne-pipeline-hd/zipball/main`
 
 ## Update
 
-Just
-run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
-again or use the update-funtion from within the programm (in Settings-Menu).
+Run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
+for an update to the development version
+or `pip install --upgrade mne-pipeline-hd` for the latest release.
 
 ## Start
+
 Run `mne_pipeline_hd` in your mne_pipeline-environment (`conda activate mne_p`)
 
 **or**
 
-run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom, etc.
+run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom,
+etc.
 
-***When using the pipeline and its functions bear in mind that the pipeline is still in development!
-The basic functions supplied are just a suggestion and you should verify before usage if they do what you need.
-They are also partly still adjusted to specific requirements which may not apply to all data.***
+***When using the pipeline and its functions bear in mind that the pipeline is
+still in development!
+The basic functions supplied are just a suggestion and you should verify before
+usage if they do what you need.
+They are also partly still adjusted to specific requirements which may not
+apply to all data.***
 
 ## Bug-Report/Feature-Request
-Please report bugs on GitHub as an issue or to me (dev@earthman-music.de) directly.
+
+Please report bugs on GitHub as an issue or to me (dev@earthman-music.de)
+directly.
 And if you got ideas on how to improve the pipeline or some feature-requests,
 you are welcome to open an issue too or send an e-mail (dev@earthman-music.de)
 
 ## Contribute and build your own functions/fix bugs
+
 I you want to help by contributing, I would be very happy:
 
 You need a [GitHub-Account](https://github.com/)
-and should have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed.
+and should
+have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
+installed.
 
 1. Fork this repository on GitHub
 2. Move to the folder where you want to clone to
 3. Clone **your forked repository** with git from a
    terminal: `git clone <url you get from the green clone-button from your forked repository on GitHub>`
 4. Add upstream to git for
    updates: `git remote add upstream git://github.com/marsipu/mne-pipeline-hd.git`
 5. Install development version with pip: `pip install -e ./`
 6. Create a branch for changes: `git checkout -b <branch-name>`
 7. Commit changes: `git commit -am "<your commit message>"`
 8. Push changes to your forked repository on GitHub: `git push`
 9. Make "New pull request" from your new feature branch
 
-You can always [write me](mailto:dev@earthman-music.de), if you have questions about the contribution-process 
+You can always [write me](mailto:dev@earthman-music.de), if you have questions
+about the contribution-process
 or about the program-structure.
 
 ## Acknowledgments
-This Pipeline is build on top of [MNE-Python](https://mne.tools/stable/index.html)
-> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck, L. Parkkonen, M. Hämäläinen,
-> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1 February 2014, Pages 446-460, ISSN 1053-8119,
+
+This Pipeline is build on top
+of [MNE-Python](https://mne.tools/stable/index.html)
+> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck,
+> L. Parkkonen, M. Hämäläinen,
+> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1
+> February 2014, Pages 446-460, ISSN 1053-8119,
 > [DOI](https://doi.org/10.1016/j.neuroimage.2013.10.027)
 
-It was inspired by a pipeline from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
-> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile Stimulation Paradigm: A Pipeline for
-> Reproducibility at Every Step of Processing, Going from Individual Sensor Space Representations to an across-Group
-> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi: 10.3389/fnins.2018.00006. PMID: 29403349;
+It was inspired by a pipeline
+from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
+> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile
+> Stimulation Paradigm: A Pipeline for
+> Reproducibility at Every Step of Processing, Going from Individual Sensor
+> Space Representations to an across-Group
+> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi:
+> 10.3389/fnins.2018.00006. PMID: 29403349;
 > PMCID: PMC5786561.
 
-This program also integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
-> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre Gramfort. 2017.
-> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage, 159, 417-429.
+This program also
+integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
+> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre
+> Gramfort. 2017.
+> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage,
+> 159, 417-429.
 
-Many ideas and basics for GUI-Programming where taken from [LearnPyQt](https://www.learnpyqt.com/) and numerous
+Many ideas and basics for GUI-Programming where taken
+from [LearnPyQt](https://www.learnpyqt.com/) and numerous
 stackoverflow-questions/solutions.
 
-The development is financially supported by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
+The development is financially supported
+by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
 
-Thank you to the members of my laboratory (especially my supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271)) for their feedback and testing in the early stages of development.
+Thank you to the members of my laboratory (especially my
+supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271))
+for their feedback and testing in the early stages of development.
```

### Comparing `mne-pipeline-hd-0.3.2a0/README.md` & `mne-pipeline-hd-0.3.3a0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,106 @@
 # mne-pipeline-hd
-### A [MNE-Python](https://mne.tools/stable/index.html) Pipeline-GUI for MEG-Lab Heidelberg
-###### inspired by: [Andersen L.M. 2018](https://doi.org/10.3389/fnins.2018.00006)
+
+### A Pipeline-GUI for [MNE-Python](https://mne.tools/stable/index.html)  from MEG-Lab Heidelberg
 
 ![mne-pipeline-hd Logo](mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg)
 
 ## Installation
-1. Install MNE-python as instructed on the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
-I would recommend to install in a separate conda environment with:
-`conda env create -n mne_p -f environment.yml`
+
+1. Install MNE-python as instructed on
+   the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
+   I would recommend to install in a separate conda environment with:
+   `conda env create -n mne_p -f environment.yml`
 2. `conda activate mne_p`
 3. `pip install https://github.com/marsipu/mne-pipeline-hd/zipball/main`
 
 ## Update
 
-Just
-run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
-again or use the update-funtion from within the programm (in Settings-Menu).
+Run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
+for an update to the development version
+or `pip install --upgrade mne-pipeline-hd` for the latest release.
 
 ## Start
+
 Run `mne_pipeline_hd` in your mne_pipeline-environment (`conda activate mne_p`)
 
 **or**
 
-run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom, etc.
+run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom,
+etc.
 
-***When using the pipeline and its functions bear in mind that the pipeline is still in development!
-The basic functions supplied are just a suggestion and you should verify before usage if they do what you need.
-They are also partly still adjusted to specific requirements which may not apply to all data.***
+***When using the pipeline and its functions bear in mind that the pipeline is
+still in development!
+The basic functions supplied are just a suggestion and you should verify before
+usage if they do what you need.
+They are also partly still adjusted to specific requirements which may not
+apply to all data.***
 
 ## Bug-Report/Feature-Request
-Please report bugs on GitHub as an issue or to me (dev@earthman-music.de) directly.
+
+Please report bugs on GitHub as an issue or to me (dev@earthman-music.de)
+directly.
 And if you got ideas on how to improve the pipeline or some feature-requests,
 you are welcome to open an issue too or send an e-mail (dev@earthman-music.de)
 
 ## Contribute and build your own functions/fix bugs
+
 I you want to help by contributing, I would be very happy:
 
 You need a [GitHub-Account](https://github.com/)
-and should have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed.
+and should
+have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
+installed.
 
 1. Fork this repository on GitHub
 2. Move to the folder where you want to clone to
 3. Clone **your forked repository** with git from a
    terminal: `git clone <url you get from the green clone-button from your forked repository on GitHub>`
 4. Add upstream to git for
    updates: `git remote add upstream git://github.com/marsipu/mne-pipeline-hd.git`
 5. Install development version with pip: `pip install -e ./`
 6. Create a branch for changes: `git checkout -b <branch-name>`
 7. Commit changes: `git commit -am "<your commit message>"`
 8. Push changes to your forked repository on GitHub: `git push`
 9. Make "New pull request" from your new feature branch
 
-You can always [write me](mailto:dev@earthman-music.de), if you have questions about the contribution-process 
+You can always [write me](mailto:dev@earthman-music.de), if you have questions
+about the contribution-process
 or about the program-structure.
 
 ## Acknowledgments
-This Pipeline is build on top of [MNE-Python](https://mne.tools/stable/index.html)
-> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck, L. Parkkonen, M. Hämäläinen,
-> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1 February 2014, Pages 446-460, ISSN 1053-8119,
+
+This Pipeline is build on top
+of [MNE-Python](https://mne.tools/stable/index.html)
+> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck,
+> L. Parkkonen, M. Hämäläinen,
+> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1
+> February 2014, Pages 446-460, ISSN 1053-8119,
 > [DOI](https://doi.org/10.1016/j.neuroimage.2013.10.027)
 
-It was inspired by a pipeline from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
-> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile Stimulation Paradigm: A Pipeline for
-> Reproducibility at Every Step of Processing, Going from Individual Sensor Space Representations to an across-Group
-> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi: 10.3389/fnins.2018.00006. PMID: 29403349;
+It was inspired by a pipeline
+from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
+> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile
+> Stimulation Paradigm: A Pipeline for
+> Reproducibility at Every Step of Processing, Going from Individual Sensor
+> Space Representations to an across-Group
+> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi:
+> 10.3389/fnins.2018.00006. PMID: 29403349;
 > PMCID: PMC5786561.
 
-This program also integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
-> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre Gramfort. 2017.
-> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage, 159, 417-429.
+This program also
+integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
+> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre
+> Gramfort. 2017.
+> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage,
+> 159, 417-429.
 
-Many ideas and basics for GUI-Programming where taken from [LearnPyQt](https://www.learnpyqt.com/) and numerous
+Many ideas and basics for GUI-Programming where taken
+from [LearnPyQt](https://www.learnpyqt.com/) and numerous
 stackoverflow-questions/solutions.
 
-The development is financially supported by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
+The development is financially supported
+by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
 
-Thank you to the members of my laboratory (especially my supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271)) for their feedback and testing in the early stages of development.
+Thank you to the members of my laboratory (especially my
+supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271))
+for their feedback and testing in the early stages of development.
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/__main__.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,139 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
+# flake: noqa E402
 
 import logging
 import os
 import sys
 from importlib import resources
 
-import qdarkstyle
 from PyQt5.QtCore import QTimer, Qt
 from PyQt5.QtGui import QIcon, QFont
 from PyQt5.QtWidgets import QApplication
-from qdarkstyle import DarkPalette, LightPalette
 
 from mne_pipeline_hd.gui.gui_utils import StdoutStderrStream, UncaughtHook
 from mne_pipeline_hd.gui.welcome_window import WelcomeWindow
+from mne_pipeline_hd.pipeline.legacy import legacy_import_check
 from mne_pipeline_hd.pipeline.pipeline_utils import ismac, islin, QS
 
+# Check for changes in required packages
+legacy_import_check()
+
+import qdarktheme  # noqa: E402
+
 
 def main():
-    app_name = 'mne-pipeline-hd'
-    organization_name = 'marsipu'
-    domain_name = 'https://github.com/marsipu/mne-pipeline-hd'
+    app_name = "mne-pipeline-hd"
+    organization_name = "marsipu"
+    domain_name = "https://github.com/marsipu/mne-pipeline-hd"
+
+    qdarktheme.enable_hi_dpi()
 
     app = QApplication.instance()
     if not app:
         app = QApplication(sys.argv)
     app.setApplicationName(app_name)
     app.setOrganizationName(organization_name)
     app.setOrganizationDomain(domain_name)
 
     # Disable Help-Button
     try:
         app.setAttribute(Qt.AA_DisableWindowContextHelpButton, True)
     except AttributeError:
-        print('pyqt-Version is < 5.12')
+        print("pyqt-Version is < 5.12")
 
     # Avoid file-dialog-problems with custom file-managers in linux
     if islin:
         app.setAttribute(Qt.AA_DontUseNativeDialogs, True)
 
     # Mac-Workarounds
     if ismac:
         # Workaround for not showing with PyQt < 5.15.2
-        os.environ['QT_MAC_WANTS_LAYER'] = '1'
+        os.environ["QT_MAC_WANTS_LAYER"] = "1"
 
     # Avoid Mayavi-Issues
-    os.environ['ETS_TOOLKIT'] = 'qt4'
-    os.environ['QT_API'] = 'pyqt5'
+    os.environ["ETS_TOOLKIT"] = "qt4"
+    os.environ["QT_API"] = "pyqt5"
 
     # ToDo: MP
     # # Set multiprocessing method to spawn
     # multiprocessing.set_start_method('spawn')
 
     # Redirect stdout to capture it later in GUI
-    sys.stdout = StdoutStderrStream('stdout')
+    sys.stdout = StdoutStderrStream("stdout")
     # Redirect stderr to capture it later in GUI
-    sys.stderr = StdoutStderrStream('stderr')
+    sys.stderr = StdoutStderrStream("stderr")
 
     # Initialize Logger (root)
     logger = logging.getLogger()
-    logger.setLevel(QS().value('log_level', defaultValue=logging.INFO))
-    formatter = logging.Formatter('%(asctime)s: %(message)s',
-                                  datefmt='%Y/%m/%d %H:%M:%S')
+    logger.setLevel(QS().value("log_level", defaultValue=logging.INFO))
+    formatter = logging.Formatter(
+        "%(asctime)s: %(message)s", datefmt="%Y/%m/%d %H:%M:%S"
+    )
     console_handler = logging.StreamHandler()
     console_handler.setFormatter(formatter)
     logger.addHandler(console_handler)
-    logger.info('Starting MNE-Pipeline HD')
+    logger.info("Starting MNE-Pipeline HD")
 
     # Initialize Exception-Hook
     qt_exception_hook = UncaughtHook()
     # this registers the exception_hook() function
     # as hook with the Python interpreter
     sys.excepthook = qt_exception_hook.exception_hook
 
     # Initialize Layout
-    font_family = QS().value('app_font')
-    font_size = QS().value('app_font_size')
+    font_family = QS().value("app_font")
+    font_size = QS().value("app_font_size")
     app.setFont(QFont(font_family, font_size))
 
     # Set Style and Window-Icon
-    app_style = QS().value('app_style')
-    if app_style == 'dark':
-        app.setStyleSheet(qdarkstyle.load_stylesheet(palette=DarkPalette))
-        icon_name = 'mne_pipeline_icon_dark.png'
+    app_style = QS().value("app_style")
+
+    # Legacy 20230717
+    if app_style not in ["dark", "light", "auto"]:
+        app_style = "auto"
+
+    if app_style == "dark":
+        qdarktheme.setup_theme("dark")
+        icon_name = "mne_pipeline_icon_dark.png"
+    elif app_style == "light":
+        qdarktheme.setup_theme("light")
+        icon_name = "mne_pipeline_icon_light.png"
     else:
-        icon_name = 'mne_pipeline_icon_light.png'
-        if app_style == 'light':
-            app.setStyleSheet(qdarkstyle.load_stylesheet(palette=LightPalette))
+        qdarktheme.setup_theme("auto")
+        st = qdarktheme.load_stylesheet("auto")
+        if "background:rgba(32, 33, 36, 1.000)" in st:
+            icon_name = "mne_pipeline_icon_dark.png"
         else:
-            app.setStyle(app_style)
+            icon_name = "mne_pipeline_icon_light.png"
 
-    with resources.path('mne_pipeline_hd.resource', icon_name) as icon_path:
+    with resources.path("mne_pipeline_hd.resource", icon_name) as icon_path:
         app_icon = QIcon(str(icon_path))
     app.setWindowIcon(app_icon)
 
     # Initiate WelcomeWindow
     WelcomeWindow()
 
     # Redirect stdout to capture it later in GUI
-    sys.stdout = StdoutStderrStream('stdout')
+    sys.stdout = StdoutStderrStream("stdout")
     # Redirect stderr to capture it later in GUI
-    sys.stderr = StdoutStderrStream('stderr')
+    sys.stderr = StdoutStderrStream("stderr")
 
     # Command-Line interrupt with Ctrl+C possible
     timer = QTimer()
     timer.timeout.connect(lambda: None)
     timer.start(500)
 
     # For Spyder to make console accessible again
     app.lastWindowClosed.connect(app.quit)
 
     sys.exit(app.exec())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # Todo: Make Exception-Handling for PyQt-Start working (from event-loop?)
     main()
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/conftest.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 from os import mkdir
 
 import pytest
 
 from mne_pipeline_hd.gui.main_window import MainWindow
 from mne_pipeline_hd.pipeline.controller import Controller
@@ -16,18 +14,18 @@
 
 
 @pytest.fixture
 def controller(tmpdir):
     # Initialize testing-environment
     _set_test_run()
     # Create home-path
-    home_path = tmpdir.join('TestHome')
+    home_path = tmpdir.join("TestHome")
     mkdir(home_path)
     # Create Controller
-    ct = Controller(home_path, 'test')
+    ct = Controller(home_path, "test")
 
     return ct
 
 
 @pytest.fixture
 def main_window(controller, qtbot):
     mw = MainWindow(controller)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/check_ressources.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/check_ressources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 from importlib import resources
 
 import pandas as pd
 
 from mne_pipeline_hd.functions import operations, plot
 
 # Check, if the function-arguments saved in functions.csv are the same
 # as in the signature of the actual function
 # (May have changed during development without
 # changing func_args in functions.csv)
-with resources.path('mne_pipeline_hd.resource',
-                    'functions.csv') as pd_funcs_path:
-    pd_funcs = pd.read_csv(str(pd_funcs_path), sep=';', index_col=0)
+with resources.path("mne_pipeline_hd.resource", "functions.csv") as pd_funcs_path:
+    pd_funcs = pd.read_csv(
+        str(pd_funcs_path), sep=";", index_col=0, na_values=[""], keep_default_na=False
+    )
 
 for func_name in pd_funcs.index:
-    module_name = pd_funcs.loc[func_name, 'module']
-    if module_name == 'operations':
+    module_name = pd_funcs.loc[func_name, "module"]
+    if module_name == "operations":
         module = operations
     else:
         module = plot
     try:
         func = getattr(module, func_name)
         real_func_args_list = list(inspect.signature(func).parameters)
-        if 'kwargs' in real_func_args_list:
-            real_func_args_list.remove('kwargs')
-        real_func_args = ','.join(real_func_args_list)
-        loaded_func_args = pd_funcs.loc[func_name, 'func_args']
+        if "kwargs" in real_func_args_list:
+            real_func_args_list.remove("kwargs")
+        real_func_args = ",".join(real_func_args_list)
+        loaded_func_args = pd_funcs.loc[func_name, "func_args"]
 
         if real_func_args != loaded_func_args:
-            pd_funcs.loc[func_name, 'func_args'] = real_func_args
-            print(f'Changed function-arguments for {func_name}\n'
-                  f'from {loaded_func_args}\n'
-                  f'to {real_func_args}\n')
+            pd_funcs.loc[func_name, "func_args"] = real_func_args
+            print(
+                f"Changed function-arguments for {func_name}\n"
+                f"from {loaded_func_args}\n"
+                f"to {real_func_args}\n"
+            )
     except AttributeError:
         pd_funcs.drop(index=func_name, inplace=True)
         print(
-            f'Droped {func_name}, because there is no'
-            f' corresponding function in {module}')
+            f"Droped {func_name}, because there is no"
+            f" corresponding function in {module}"
+        )
 
-with resources.path('mne_pipeline_hd.resource',
-                    'functions.csv') as pd_funcs_path:
-    pd_funcs.to_csv(pd_funcs_path, sep=';')
+with resources.path("mne_pipeline_hd.resource", "functions.csv") as pd_funcs_path:
+    pd_funcs.to_csv(pd_funcs_path, sep=";")
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/development/dev_utils.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/dev_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,29 @@
+"""
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
+"""
+
 import inspect
 import sys
 import traceback
 from ast import literal_eval
 
-from PyQt5.QtWidgets import (QWidget, QVBoxLayout, QGridLayout, QComboBox,
-                             QHBoxLayout, QLineEdit, QPushButton, QDialog,
-                             QApplication)
+from PyQt5.QtWidgets import (
+    QWidget,
+    QVBoxLayout,
+    QGridLayout,
+    QComboBox,
+    QHBoxLayout,
+    QLineEdit,
+    QPushButton,
+    QDialog,
+    QApplication,
+)
 
 from mne_pipeline_hd.gui import parameter_widgets
 from mne_pipeline_hd.gui.base_widgets import SimpleDict
 from mne_pipeline_hd.gui.parameter_widgets import Param
 from mne_pipeline_hd.tests.test_param_guis import gui_kwargs, parameters
 
 
@@ -25,38 +39,39 @@
         test_layout = QVBoxLayout()
         grid_layout = QGridLayout()
         max_cols = 4
 
         param_names = list(parameters.keys())
         for idx, gui_name in enumerate(param_names):
             gui_class = getattr(parameter_widgets, gui_name)
-            gui_parameters = \
-                list(inspect.signature(gui_class).parameters) + \
-                list(inspect.signature(Param).parameters)
-            kwargs = {key: value for key, value in gui_kwargs.items()
-                      if key in gui_parameters}
+            gui_parameters = list(inspect.signature(gui_class).parameters) + list(
+                inspect.signature(Param).parameters
+            )
+            kwargs = {
+                key: value for key, value in gui_kwargs.items() if key in gui_parameters
+            }
             gui = gui_class(data=parameters, name=gui_name, **kwargs)
             grid_layout.addWidget(gui, idx // max_cols, idx % max_cols)
             self.gui_dict[gui_name] = gui
 
         test_layout.addLayout(grid_layout)
 
         set_layout = QHBoxLayout()
         self.gui_cmbx = QComboBox()
         self.gui_cmbx.addItems(self.gui_dict.keys())
         set_layout.addWidget(self.gui_cmbx)
 
         self.set_le = QLineEdit()
         set_layout.addWidget(self.set_le)
 
-        set_bt = QPushButton('Set')
+        set_bt = QPushButton("Set")
         set_bt.clicked.connect(self.set_param)
         set_layout.addWidget(set_bt)
 
-        show_bt = QPushButton('Show Parameters')
+        show_bt = QPushButton("Show Parameters")
         show_bt.clicked.connect(self.show_parameters)
         set_layout.addWidget(show_bt)
 
         test_layout.addLayout(set_layout)
 
         self.setLayout(test_layout)
 
@@ -76,12 +91,12 @@
         dlg = QDialog(self)
         layout = QVBoxLayout()
         layout.addWidget(SimpleDict(parameters))
         dlg.setLayout(layout)
         dlg.open()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app = QApplication.instance() or QApplication(sys.argv)
     test_widget = ParamGuis()
     test_widget.show()
     sys.exit(app.exec())
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/operations.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from __future__ import print_function
 
 import gc
 import logging
 import os
@@ -25,691 +23,876 @@
 import autoreject as ar
 import mne
 import mne_connectivity
 import numpy as np
 from mne.preprocessing import ICA
 
 from mne_pipeline_hd.pipeline.loading import MEEG
-from mne_pipeline_hd.pipeline.pipeline_utils import (check_kwargs,
-                                                     compare_filep,
-                                                     ismac, iswin)
+from mne_pipeline_hd.pipeline.pipeline_utils import (
+    check_kwargs,
+    compare_filep,
+    ismac,
+    iswin,
+)
 
 
 # Todo: Create docstrings for each function
 # =============================================================================
 # PREPROCESSING AND GETTING TO EVOKED AND TFR
 # =============================================================================
-def filter_data(meeg, filter_target, highpass, lowpass, filter_length,
-                l_trans_bandwidth,
-                h_trans_bandwidth, filter_method, iir_params, fir_phase,
-                fir_window,
-                fir_design, skip_by_annotation, fir_pad, n_jobs, enable_cuda,
-                erm_t_limit,
-                bad_interpolation):
+def filter_data(
+    meeg,
+    filter_target,
+    highpass,
+    lowpass,
+    filter_length,
+    l_trans_bandwidth,
+    h_trans_bandwidth,
+    filter_method,
+    iir_params,
+    fir_phase,
+    fir_window,
+    fir_design,
+    skip_by_annotation,
+    fir_pad,
+    n_jobs,
+    enable_cuda,
+    erm_t_limit,
+    bad_interpolation,
+):
     # Compare Parameters from last run
-    filtered_path = meeg.io_dict[filter_target]['path']
-    results = compare_filep(meeg, filtered_path,
-                            ['highpass', 'lowpass', 'bad_interpolation'])
+    filtered_path = meeg.io_dict[filter_target]["path"]
+    results = compare_filep(
+        meeg, filtered_path, ["highpass", "lowpass", "bad_interpolation"]
+    )
 
-    if any([results[key] != 'equal' for key in results]):
+    if any([results[key] != "equal" for key in results]):
         # Load Data
-        data = meeg.io_dict[filter_target]['load']()
+        data = meeg.io_dict[filter_target]["load"]()
 
         # use cuda for filtering if enabled
         if enable_cuda:
             mne.cuda.init_cuda(ignore_config=True)
-            n_jobs = 'cuda'
+            n_jobs = "cuda"
 
         # Filter Data
-        if filter_target == 'evoked':
+        if filter_target == "evoked":
             for evoked in data:
-                evoked.filter(highpass, lowpass, filter_length=filter_length,
-                              l_trans_bandwidth=l_trans_bandwidth,
-                              h_trans_bandwidth=h_trans_bandwidth,
-                              n_jobs=n_jobs, method=filter_method,
-                              iir_params=iir_params, phase=fir_phase,
-                              fir_window=fir_window, fir_design=fir_design,
-                              skip_by_annotation=skip_by_annotation,
-                              pad=fir_pad)
+                evoked.filter(
+                    highpass,
+                    lowpass,
+                    filter_length=filter_length,
+                    l_trans_bandwidth=l_trans_bandwidth,
+                    h_trans_bandwidth=h_trans_bandwidth,
+                    n_jobs=n_jobs,
+                    method=filter_method,
+                    iir_params=iir_params,
+                    phase=fir_phase,
+                    fir_window=fir_window,
+                    fir_design=fir_design,
+                    skip_by_annotation=skip_by_annotation,
+                    pad=fir_pad,
+                )
         else:
-            data.filter(highpass, lowpass, filter_length=filter_length,
-                        l_trans_bandwidth=l_trans_bandwidth,
-                        h_trans_bandwidth=h_trans_bandwidth, n_jobs=n_jobs,
-                        method=filter_method, iir_params=iir_params,
-                        phase=fir_phase, fir_window=fir_window,
-                        fir_design=fir_design,
-                        skip_by_annotation=skip_by_annotation, pad=fir_pad)
+            data.filter(
+                highpass,
+                lowpass,
+                filter_length=filter_length,
+                l_trans_bandwidth=l_trans_bandwidth,
+                h_trans_bandwidth=h_trans_bandwidth,
+                n_jobs=n_jobs,
+                method=filter_method,
+                iir_params=iir_params,
+                phase=fir_phase,
+                fir_window=fir_window,
+                fir_design=fir_design,
+                skip_by_annotation=skip_by_annotation,
+                pad=fir_pad,
+            )
 
         # Save Data
-        if filter_target == 'raw':
-            meeg.io_dict['raw_filtered']['save'](data)
+        if filter_target == "raw":
+            meeg.io_dict["raw_filtered"]["save"](data)
         else:
-            meeg.io_dict[filter_target]['save'](data)
+            meeg.io_dict[filter_target]["save"](data)
 
         # Remove raw to avoid memory overload
         del data
         gc.collect()
 
     else:
         print(
-            f'{meeg.name} already filtered with highpass={highpass} '
-            f'and lowpass={lowpass}')
+            f"{meeg.name} already filtered with highpass={highpass} "
+            f"and lowpass={lowpass}"
+        )
 
     # Filter Empty-Room-Data too
     if meeg.erm:
-        erm_results = compare_filep(meeg, meeg.erm_processed_path,
-                                    ['highpass', 'lowpass',
-                                     'bad_interpolation'])
-        if any([erm_results[key] != 'equal' for key in erm_results]):
+        erm_results = compare_filep(
+            meeg, meeg.erm_processed_path, ["highpass", "lowpass", "bad_interpolation"]
+        )
+        if any([erm_results[key] != "equal" for key in erm_results]):
             erm_raw = meeg.load_erm()
 
             # Crop ERM-Measurement to limit if given
             if erm_t_limit:
-                erm_length = erm_raw.n_times / erm_raw.info['sfreq']  # in s
+                erm_length = erm_raw.n_times / erm_raw.info["sfreq"]  # in s
                 if erm_length > erm_t_limit:
                     diff = erm_length - erm_t_limit
                     tmin = diff / 2
                     tmax = erm_length - diff / 2
                     erm_raw.crop(tmin=tmin, tmax=tmax)
 
-            erm_raw.filter(highpass, lowpass, filter_length=filter_length,
-                           l_trans_bandwidth=l_trans_bandwidth,
-                           h_trans_bandwidth=h_trans_bandwidth, n_jobs=n_jobs,
-                           method=filter_method,
-                           iir_params=iir_params, phase=fir_phase,
-                           fir_window=fir_window, fir_design=fir_design,
-                           skip_by_annotation=skip_by_annotation, pad=fir_pad)
+            erm_raw.filter(
+                highpass,
+                lowpass,
+                filter_length=filter_length,
+                l_trans_bandwidth=l_trans_bandwidth,
+                h_trans_bandwidth=h_trans_bandwidth,
+                n_jobs=n_jobs,
+                method=filter_method,
+                iir_params=iir_params,
+                phase=fir_phase,
+                fir_window=fir_window,
+                fir_design=fir_design,
+                skip_by_annotation=skip_by_annotation,
+                pad=fir_pad,
+            )
 
-            if bad_interpolation == 'raw':
+            if bad_interpolation == "raw":
                 info = meeg.load_info()
-                erm_raw.info['dig'] = info['dig']
+                erm_raw.info["dig"] = info["dig"]
                 erm_raw = erm_raw.interpolate_bads()
 
             meeg.save_erm_processed(erm_raw)
-            print('ERM-Data filtered and saved')
+            print("ERM-Data filtered and saved")
         else:
             print(
-                f'{meeg.erm} already filtered with highpass={highpass} '
-                f'and lowpass={lowpass}')
+                f"{meeg.erm} already filtered with highpass={highpass} "
+                f"and lowpass={lowpass}"
+            )
 
     else:
-        print('no erm_file assigned')
+        print("no erm_file assigned")
 
 
 def interpolate_bads(meeg, bad_interpolation):
-    data = meeg.io_dict[bad_interpolation]['load']()
+    data = meeg.io_dict[bad_interpolation]["load"]()
 
-    if bad_interpolation == 'evoked':
+    if bad_interpolation == "evoked":
         for evoked in data:
             evoked.interpolate_bads()
     else:
         data.interpolate_bads()
 
-    meeg.io_dict[bad_interpolation]['save'](data)
+    meeg.io_dict[bad_interpolation]["save"](data)
 
 
-def add_erm_ssp(meeg, erm_ssp_duration, erm_n_grad, erm_n_mag, erm_n_eeg,
-                n_jobs, show_plots):
+def add_erm_ssp(
+    meeg, erm_ssp_duration, erm_n_grad, erm_n_mag, erm_n_eeg, n_jobs, show_plots
+):
     raw_filtered = meeg.load_filtered()
     erm_filtered = meeg.load_erm_processed()
 
     # Only include channels from Empty-Room-Data,
     # which are present in filtered-data
     erm_filtered = erm_filtered.copy().pick_channels(
-        [ch for ch in erm_filtered.ch_names if ch in raw_filtered.ch_names])
+        [ch for ch in erm_filtered.ch_names if ch in raw_filtered.ch_names]
+    )
 
-    erm_projs = mne.compute_proj_raw(erm_filtered, duration=erm_ssp_duration,
-                                     n_grad=erm_n_grad, n_mag=erm_n_mag,
-                                     n_eeg=erm_n_eeg, n_jobs=n_jobs)
+    erm_projs = mne.compute_proj_raw(
+        erm_filtered,
+        duration=erm_ssp_duration,
+        n_grad=erm_n_grad,
+        n_mag=erm_n_mag,
+        n_eeg=erm_n_eeg,
+        n_jobs=n_jobs,
+    )
 
     raw_filtered.add_proj(erm_projs, remove_existing=True)
     meeg.save_filtered(raw_filtered)
 
-    fig = mne.viz.plot_projs_topomap(erm_projs, erm_filtered.info,
-                                     colorbar=True, show=show_plots)
-    meeg.plot_save('ssp_erm', matplotlib_figure=fig)
+    fig = mne.viz.plot_projs_topomap(
+        erm_projs, erm_filtered.info, colorbar=True, show=show_plots
+    )
+    meeg.plot_save("ssp_erm", matplotlib_figure=fig)
 
 
 def eeg_reference_raw(meeg, ref_channels):
     raw_filtered = meeg.load_filtered()
 
-    if ref_channels == 'REST':
+    if ref_channels == "REST":
         forward = meeg.load_forward()
     else:
         forward = None
 
-    if ref_channels == 'average':
+    if ref_channels == "average":
         projection = True
     else:
         projection = False
 
-    raw_filtered.set_eeg_reference(ref_channels=ref_channels,
-                                   projection=projection, forward=forward)
+    raw_filtered.set_eeg_reference(
+        ref_channels=ref_channels, projection=projection, forward=forward
+    )
     meeg.save_filtered(raw_filtered)
 
 
-def find_events(meeg, stim_channels, min_duration, shortest_event,
-                adjust_timeline_by_msec):
+def find_events(
+    meeg, stim_channels, min_duration, shortest_event, adjust_timeline_by_msec
+):
     raw = meeg.load_raw()  # No copy to consume less memory
 
-    events = mne.find_events(raw, min_duration=min_duration,
-                             shortest_event=shortest_event,
-                             stim_channel=stim_channels)
+    events = mne.find_events(
+        raw,
+        min_duration=min_duration,
+        shortest_event=shortest_event,
+        stim_channel=stim_channels,
+    )
 
     # apply latency correction
-    events[:, 0] = [ts + np.round(adjust_timeline_by_msec * 10 ** -3 *
-                                  raw.info['sfreq']) for ts in events[:, 0]]
+    events[:, 0] = [
+        ts + np.round(adjust_timeline_by_msec * 10**-3 * raw.info["sfreq"])
+        for ts in events[:, 0]
+    ]
 
     ids = np.unique(events[:, 2])
-    print('unique ID\'s found: ', ids)
+    print("unique ID's found: ", ids)
 
     if np.size(events) > 0:
         meeg.save_events(events)
     else:
-        print('No events found')
+        print("No events found")
 
 
-def find_6ch_binary_events(meeg, min_duration, shortest_event,
-                           adjust_timeline_by_msec):
+def find_6ch_binary_events(meeg, min_duration, shortest_event, adjust_timeline_by_msec):
     raw = meeg.load_raw()  # No copy to consume less memory
 
     # Binary Coding of 6 Stim Channels in Biomagenetism Lab Heidelberg
     # prepare arrays
     events = np.ndarray(shape=(0, 3), dtype=np.int32)
     evs = list()
     evs_tol = list()
 
     # Find events for each stim channel, append sample values to list
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 001'])[:, 0])
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 002'])[:, 0])
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 003'])[:, 0])
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 004'])[:, 0])
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 005'])[:, 0])
-    evs.append(mne.find_events(raw, min_duration=min_duration,
-                               shortest_event=shortest_event,
-                               stim_channel=['STI 006'])[:, 0])
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 001"],
+        )[:, 0]
+    )
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 002"],
+        )[:, 0]
+    )
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 003"],
+        )[:, 0]
+    )
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 004"],
+        )[:, 0]
+    )
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 005"],
+        )[:, 0]
+    )
+    evs.append(
+        mne.find_events(
+            raw,
+            min_duration=min_duration,
+            shortest_event=shortest_event,
+            stim_channel=["STI 006"],
+        )[:, 0]
+    )
 
     for i in evs:
-
         # delete events in each channel,
         # which are too close too each other (1ms)
         too_close = np.where(np.diff(i) <= 1)
         if np.size(too_close) >= 1:
             print(
-                f'Two close events (1ms) at samples '
-                f'{i[too_close] + raw.first_samp}, first deleted')
+                f"Two close events (1ms) at samples "
+                f"{i[too_close] + raw.first_samp}, first deleted"
+            )
             i = np.delete(i, too_close, 0)
             evs[evs.index(i)] = i
 
         # add tolerance to each value
         i_tol = np.ndarray(shape=(0, 1), dtype=np.int32)
         for t in i:
             i_tol = np.append(i_tol, t - 1)
             i_tol = np.append(i_tol, t)
             i_tol = np.append(i_tol, t + 1)
 
         evs_tol.append(i_tol)
 
     # Get events from combinated Stim-Channels
-    equals = reduce(np.intersect1d, (evs_tol[0], evs_tol[1], evs_tol[2],
-                                     evs_tol[3], evs_tol[4], evs_tol[5]))
+    equals = reduce(
+        np.intersect1d,
+        (evs_tol[0], evs_tol[1], evs_tol[2], evs_tol[3], evs_tol[4], evs_tol[5]),
+    )
     # elimnate duplicated events
     too_close = np.where(np.diff(equals) <= 1)
     if np.size(too_close) >= 1:
         equals = np.delete(equals, too_close, 0)
         equals -= 1  # correction, because of shift with deletion
 
     for q in equals:
-        if q not in events[:, 0] \
-                and q not in events[:, 0] + 1 \
-                and q not in events[:, 0] - 1:
+        if (
+            q not in events[:, 0]
+            and q not in events[:, 0] + 1
+            and q not in events[:, 0] - 1
+        ):
             events = np.append(events, [[q, 0, 63]], axis=0)
 
     for a, b, c, d, e in combinations(range(6), 5):
-        equals = reduce(np.intersect1d, (evs_tol[a], evs_tol[b], evs_tol[c],
-                                         evs_tol[d], evs_tol[e]))
+        equals = reduce(
+            np.intersect1d, (evs_tol[a], evs_tol[b], evs_tol[c], evs_tol[d], evs_tol[e])
+        )
         too_close = np.where(np.diff(equals) <= 1)
         if np.size(too_close) >= 1:
             equals = np.delete(equals, too_close, 0)
             equals -= 1
 
         for q in equals:
-            if q not in events[:, 0] \
-                    and q not in events[:, 0] + 1 \
-                    and q not in events[:, 0] - 1:
-                events = np.append(events, [
-                    [q, 0, int(2 ** a + 2 ** b + 2 ** c + 2 ** d + 2 ** e)]],
-                                   axis=0)
+            if (
+                q not in events[:, 0]
+                and q not in events[:, 0] + 1
+                and q not in events[:, 0] - 1
+            ):
+                events = np.append(
+                    events,
+                    [[q, 0, int(2**a + 2**b + 2**c + 2**d + 2**e)]],
+                    axis=0,
+                )
 
     for a, b, c, d in combinations(range(6), 4):
-        equals = reduce(np.intersect1d,
-                        (evs_tol[a], evs_tol[b], evs_tol[c], evs_tol[d]))
+        equals = reduce(
+            np.intersect1d, (evs_tol[a], evs_tol[b], evs_tol[c], evs_tol[d])
+        )
         too_close = np.where(np.diff(equals) <= 1)
         if np.size(too_close) >= 1:
             equals = np.delete(equals, too_close, 0)
             equals -= 1
 
         for q in equals:
-            if q not in events[:, 0] \
-                    and q not in events[:, 0] + 1 \
-                    and q not in events[:, 0] - 1:
-                events = np.append(events, [
-                    [q, 0, int(2 ** a + 2 ** b + 2 ** c + 2 ** d)]], axis=0)
+            if (
+                q not in events[:, 0]
+                and q not in events[:, 0] + 1
+                and q not in events[:, 0] - 1
+            ):
+                events = np.append(
+                    events, [[q, 0, int(2**a + 2**b + 2**c + 2**d)]], axis=0
+                )
 
     for a, b, c in combinations(range(6), 3):
         equals = reduce(np.intersect1d, (evs_tol[a], evs_tol[b], evs_tol[c]))
         too_close = np.where(np.diff(equals) <= 1)
         if np.size(too_close) >= 1:
             equals = np.delete(equals, too_close, 0)
             equals -= 1
 
         for q in equals:
-            if q not in events[:, 0] \
-                    and q not in events[:, 0] + 1 \
-                    and q not in events[:, 0] - 1:
-                events = np.append(events,
-                                   [[q, 0, int(2 ** a + 2 ** b + 2 ** c)]],
-                                   axis=0)
+            if (
+                q not in events[:, 0]
+                and q not in events[:, 0] + 1
+                and q not in events[:, 0] - 1
+            ):
+                events = np.append(
+                    events, [[q, 0, int(2**a + 2**b + 2**c)]], axis=0
+                )
 
     for a, b in combinations(range(6), 2):
         equals = np.intersect1d(evs_tol[a], evs_tol[b])
         too_close = np.where(np.diff(equals) <= 1)
         if np.size(too_close) >= 1:
             equals = np.delete(equals, too_close, 0)
             equals -= 1
 
         for q in equals:
-            if q not in events[:, 0] \
-                    and q not in events[:, 0] + 1 \
-                    and q not in events[:, 0] - 1:
-                events = np.append(events, [[q, 0, int(2 ** a + 2 ** b)]],
-                                   axis=0)
+            if (
+                q not in events[:, 0]
+                and q not in events[:, 0] + 1
+                and q not in events[:, 0] - 1
+            ):
+                events = np.append(events, [[q, 0, int(2**a + 2**b)]], axis=0)
 
     # Get single-channel events
     for i in range(6):
         for e in evs[i]:
-            if e not in events[:, 0] \
-                    and e not in events[:, 0] + 1 \
-                    and e not in events[:, 0] - 1:
-                events = np.append(events, [[e, 0, 2 ** i]], axis=0)
+            if (
+                e not in events[:, 0]
+                and e not in events[:, 0] + 1
+                and e not in events[:, 0] - 1
+            ):
+                events = np.append(events, [[e, 0, 2**i]], axis=0)
 
     # sort only along samples(column 0)
     events = events[events[:, 0].argsort()]
 
     # apply latency correction
-    events[:, 0] = [ts + np.round(adjust_timeline_by_msec * 10 ** -3 *
-                                  raw.info['sfreq']) for ts in events[:, 0]]
+    events[:, 0] = [
+        ts + np.round(adjust_timeline_by_msec * 10**-3 * raw.info["sfreq"])
+        for ts in events[:, 0]
+    ]
 
     ids = np.unique(events[:, 2])
-    print('unique ID\'s found: ', ids)
+    print("unique ID's found: ", ids)
 
     if np.size(events) > 0:
         meeg.save_events(events)
     else:
-        print('No events found')
+        print("No events found")
 
 
-def epoch_raw(meeg, ch_types, ch_names, t_epoch, baseline, apply_proj, reject,
-              flat, reject_by_annotation,
-              bad_interpolation, use_autoreject, consensus_percs,
-              n_interpolates, overwrite_ar, decim, n_jobs):
+def epoch_raw(
+    meeg,
+    ch_types,
+    ch_names,
+    t_epoch,
+    baseline,
+    apply_proj,
+    reject,
+    flat,
+    reject_by_annotation,
+    bad_interpolation,
+    use_autoreject,
+    consensus_percs,
+    n_interpolates,
+    overwrite_ar,
+    decim,
+    n_jobs,
+):
     raw_filtered = meeg.load_filtered()
     events = meeg.load_events()
 
     # Pick selected channel_types if not done before
     raw_filtered.pick(ch_types)
 
-    if len(ch_names) > 0 and ch_names != 'all':
+    if len(ch_names) > 0 and ch_names != "all":
         raw_filtered.pick_channels(ch_names)
 
     if bad_interpolation is None:
         # Exclude bad-channels if no Bad-Channel-Interpolation is intended
         # after making the epochs or the Evokeds
-        raw_filtered.pick('all', exclude='bads')
-
-    epochs = mne.Epochs(raw_filtered, events, meeg.event_id, t_epoch[0],
-                        t_epoch[1], baseline,
-                        preload=True, proj=apply_proj, reject=None, flat=None,
-                        decim=decim, on_missing='ignore',
-                        reject_by_annotation=reject_by_annotation)
+        raw_filtered.pick("all", exclude="bads")
 
-    if any([i is not None for i in [use_autoreject, reject,
-                                    flat]]) and bad_interpolation == 'Evokeds':
+    epochs = mne.Epochs(
+        raw_filtered,
+        events,
+        meeg.event_id,
+        t_epoch[0],
+        t_epoch[1],
+        baseline,
+        preload=True,
+        proj=apply_proj,
+        reject=None,
+        flat=None,
+        decim=decim,
+        on_missing="ignore",
+        reject_by_annotation=reject_by_annotation,
+    )
+
+    if (
+        any([i is not None for i in [use_autoreject, reject, flat]])
+        and bad_interpolation == "Evokeds"
+    ):
         raise RuntimeWarning(
             'With bad_interpolation="Evokeds", '
-            'the bad channels are still included and '
-            'may heavily influence the outcome of dropping epochs with reject,'
-            ' flat or autoreject!'
-            '\n(to solve this you could uncheck autoreject, '
-            'reject and flat or set bad_interpolationto another value)')
-
-    existing_ch_types = epochs.get_channel_types(unique=True,
-                                                 only_data_chs=True)
-
-    if use_autoreject == 'Interpolation':
-        ar_object = ar.AutoReject(n_interpolate=n_interpolates,
-                                  consensus=consensus_percs, n_jobs=n_jobs)
+            "the bad channels are still included and "
+            "may heavily influence the outcome of dropping epochs with reject,"
+            " flat or autoreject!"
+            "\n(to solve this you could uncheck autoreject, "
+            "reject and flat or set bad_interpolationto another value)"
+        )
+
+    existing_ch_types = epochs.get_channel_types(unique=True, only_data_chs=True)
+
+    if use_autoreject == "Interpolation":
+        ar_object = ar.AutoReject(
+            n_interpolate=n_interpolates, consensus=consensus_percs, n_jobs=n_jobs
+        )
         epochs, reject_log = ar_object.fit_transform(epochs, return_log=True)
         meeg.save_reject_log(reject_log)
 
     else:
-        if use_autoreject == 'Threshold':
-            reject = meeg.load_json('autoreject_threshold')
+        if use_autoreject == "Threshold":
+            reject = meeg.load_json("autoreject_threshold")
             if reject is None or overwrite_ar:
                 reject = ar.get_rejection_threshold(epochs)
-                meeg.save_json('autoreject_threshold', reject)
-            print(f'Dropping bad epochs with autoreject'
-                  f' rejection-thresholds: {reject}')
+                meeg.save_json("autoreject_threshold", reject)
+            print(
+                f"Dropping bad epochs with autoreject"
+                f" rejection-thresholds: {reject}"
+            )
 
         else:
             # Remove entries from reject if not present in channels
 
             if reject is not None:
                 reject = reject.copy()
                 for key in [k for k in reject if k not in existing_ch_types]:
                     reject.pop(key)
-            print(f'Dropping bad epochs with chosen '
-                  f'rejection-thresholds: {reject}')
+            print(f"Dropping bad epochs with chosen " f"rejection-thresholds: {reject}")
 
         epochs.drop_bad(reject=reject)
 
     if flat is not None:
         # Remove entries from flat if not present in channels
         flat = flat.copy()
         for key in [k for k in flat if k not in existing_ch_types]:
             flat.pop(key)
-        print(f'Dropping bad epochs with chosen flat-thresholds: {flat}')
+        print(f"Dropping bad epochs with chosen flat-thresholds: {flat}")
         epochs.drop_bad(flat=flat)
 
     meeg.save_epochs(epochs)
 
 
-def run_ica(meeg, ica_method, ica_fitto, n_components, ica_noise_cov,
-            ica_remove_proj, ica_reject, ica_autoreject,
-            ch_types, ch_names, reject_by_annotation, ica_eog, eog_channel,
-            ica_ecg, ecg_channel, **kwargs):
-    if ica_fitto == 'epochs':
+def run_ica(
+    meeg,
+    ica_method,
+    ica_fitto,
+    n_components,
+    ica_noise_cov,
+    ica_remove_proj,
+    ica_reject,
+    ica_autoreject,
+    ch_types,
+    ch_names,
+    reject_by_annotation,
+    ica_eog,
+    eog_channel,
+    ica_ecg,
+    ecg_channel,
+    **kwargs,
+):
+    if ica_fitto == "epochs":
         data = meeg.load_epochs()
         # Bad-Channels and Channel-Types are already picked in epoch_raw
     else:
-        if ica_fitto == 'raw':
+        if ica_fitto == "raw":
             data = meeg.load_raw()
 
         else:
             data = meeg.load_filtered()
 
-        data.pick(ch_types, exclude='bads')
-        if len(ch_names) > 0 and ch_names != 'all':
+        data.pick(ch_types, exclude="bads")
+        if len(ch_names) > 0 and ch_names != "all":
             data.pick_channels(ch_names)
 
     # Filter if data is not highpass-filtered >= 1
-    if data.info['highpass'] < 1:
+    if data.info["highpass"] < 1:
         filt_data = data.filter(1, None)
     else:
         filt_data = data
 
     if ica_noise_cov:
         noise_cov = meeg.load_noise_covariance()
     else:
         noise_cov = None
 
     ica_kwargs = check_kwargs(kwargs, ICA)
-    ica = ICA(n_components=n_components, noise_cov=noise_cov, random_state=8,
-              method=ica_method, **ica_kwargs)
+    ica = ICA(
+        n_components=n_components,
+        noise_cov=noise_cov,
+        random_state=8,
+        method=ica_method,
+        **ica_kwargs,
+    )
 
-    if ica_autoreject and ica_fitto != 'epochs':
+    if ica_autoreject and ica_fitto != "epochs":
         # Estimate Reject-Thresholds on simulated epochs
         # Creating simulated epochs with len 1s
         simulated_events = mne.make_fixed_length_events(data, duration=1)
-        simulated_epochs = mne.Epochs(data, simulated_events, baseline=None,
-                                      tmin=0, tmax=1,
-                                      proj=False)
+        simulated_epochs = mne.Epochs(
+            data, simulated_events, baseline=None, tmin=0, tmax=1, proj=False
+        )
         reject = ar.get_rejection_threshold(simulated_epochs)
-        print(f'Autoreject Rejection-Threshold: {reject}')
-    elif ica_autoreject and ica_fitto == 'epochs':
-        reject = meeg.load_json('autoreject_threshold')
+        print(f"Autoreject Rejection-Threshold: {reject}")
+    elif ica_autoreject and ica_fitto == "epochs":
+        reject = meeg.load_json("autoreject_threshold")
         if not reject:
             reject = ar.get_rejection_threshold(data)
-            meeg.save_json('autoreject_threshold', reject)
+            meeg.save_json("autoreject_threshold", reject)
     else:
         reject = ica_reject
 
     # Remove projections
     if ica_remove_proj:
         filt_data.del_proj()
 
     fit_kwargs = check_kwargs(kwargs, ica.fit)
-    ica.fit(filt_data, reject=reject,
-            reject_by_annotation=reject_by_annotation, **fit_kwargs)
+    ica.fit(
+        filt_data,
+        reject=reject,
+        reject_by_annotation=reject_by_annotation,
+        **fit_kwargs,
+    )
 
     # Load raw for EOG/ECG-Detection without picks
     # (e.g. still containing EEG for EOG or EOG channels)
     eog_ecg_raw = meeg.load_filtered()
     # Include EOG/ECG with all the data-channels
-    eog_ecg_raw.pick_types(meg=True, eeg=True, eog=True, ecg=True, seeg=True,
-                           ecog=True, fnirs=True, exclude='bads')
+    eog_ecg_raw.pick_types(
+        meg=True,
+        eeg=True,
+        eog=True,
+        ecg=True,
+        seeg=True,
+        ecog=True,
+        fnirs=True,
+        exclude="bads",
+    )
 
     if ica_eog:
-
-        create_eog_kwargs = check_kwargs(kwargs,
-                                         mne.preprocessing.create_eog_epochs)
+        create_eog_kwargs = check_kwargs(kwargs, mne.preprocessing.create_eog_epochs)
         find_eog_kwargs = check_kwargs(kwargs, ica.find_bads_eog)
 
         # Using an EOG channel to select components if possible
-        if 'eog' in eog_ecg_raw.get_channel_types():
+        if "eog" in eog_ecg_raw.get_channel_types():
             eog_epochs = mne.preprocessing.create_eog_epochs(
-                eog_ecg_raw, **create_eog_kwargs)
-            eog_indices, eog_scores = ica.find_bads_eog(
-                eog_ecg_raw, **find_eog_kwargs)
+                eog_ecg_raw, **create_eog_kwargs
+            )
+            eog_indices, eog_scores = ica.find_bads_eog(eog_ecg_raw, **find_eog_kwargs)
         elif eog_channel and eog_channel in eog_ecg_raw.ch_names:
             eog_epochs = mne.preprocessing.create_eog_epochs(
-                eog_ecg_raw, ch_name=eog_channel, **create_eog_kwargs)
-            eog_indices, eog_scores = ica.find_bads_eog(eog_ecg_raw,
-                                                        ch_name=eog_channel,
-                                                        **find_eog_kwargs)
+                eog_ecg_raw, ch_name=eog_channel, **create_eog_kwargs
+            )
+            eog_indices, eog_scores = ica.find_bads_eog(
+                eog_ecg_raw, ch_name=eog_channel, **find_eog_kwargs
+            )
         else:
             eog_indices, eog_scores, eog_epochs = None, None, None
             print(
-                'No EOG-Channel found or set, '
-                'thus EOG can\'t be used for automatic Component-Selection')
+                "No EOG-Channel found or set, "
+                "thus EOG can't be used for automatic Component-Selection"
+            )
 
         if eog_epochs:
             ica.exclude += eog_indices
             meeg.save_eog_epochs(eog_epochs)
-            meeg.save_json('eog_indices', eog_indices)
-            meeg.save_json('eog_scores', eog_scores)
+            meeg.save_json("eog_indices", eog_indices)
+            meeg.save_json("eog_scores", eog_scores)
 
     if ica_ecg:
-        create_ecg_kwargs = check_kwargs(kwargs,
-                                         mne.preprocessing.create_ecg_epochs)
+        create_ecg_kwargs = check_kwargs(kwargs, mne.preprocessing.create_ecg_epochs)
         find_ecg_kwargs = check_kwargs(kwargs, ica.find_bads_ecg)
 
         # Using an ECG channel to select components
         if ecg_channel and ecg_channel in eog_ecg_raw.ch_names:
             ecg_epochs = mne.preprocessing.create_ecg_epochs(
-                eog_ecg_raw, ch_name=ecg_channel, **create_ecg_kwargs)
+                eog_ecg_raw, ch_name=ecg_channel, **create_ecg_kwargs
+            )
             ecg_indices, ecg_scores = ica.find_bads_ecg(
-                eog_ecg_raw, ch_name=ecg_channel, **find_ecg_kwargs)
-        elif any([ch_type in eog_ecg_raw.get_channel_types() for ch_type in
-                  ['mag', 'grad', 'meg']]):
-            print('ECG-Signal reconstructed from MEG')
+                eog_ecg_raw, ch_name=ecg_channel, **find_ecg_kwargs
+            )
+        elif any(
+            [
+                ch_type in eog_ecg_raw.get_channel_types()
+                for ch_type in ["mag", "grad", "meg"]
+            ]
+        ):
+            print("ECG-Signal reconstructed from MEG")
             ecg_epochs = mne.preprocessing.create_ecg_epochs(
-                eog_ecg_raw, **create_ecg_kwargs)
-            ecg_indices, ecg_scores = ica.find_bads_ecg(
-                eog_ecg_raw, **find_ecg_kwargs)
+                eog_ecg_raw, **create_ecg_kwargs
+            )
+            ecg_indices, ecg_scores = ica.find_bads_ecg(eog_ecg_raw, **find_ecg_kwargs)
         else:
             ecg_indices, ecg_scores, ecg_epochs = None, None, None
-            print('No ECG-Channel found or set and no MEG-Channel '
-                  'for ECG-Detection present, thus ECG can\'t be used for '
-                  'automatic Component-Selection.')
+            print(
+                "No ECG-Channel found or set and no MEG-Channel "
+                "for ECG-Detection present, thus ECG can't be used for "
+                "automatic Component-Selection."
+            )
 
         if ecg_epochs:
             ica.exclude += ecg_indices
             meeg.save_ecg_epochs(ecg_epochs)
-            meeg.save_json('ecg_indices', ecg_indices)
-            meeg.save_json('ecg_scores', ecg_scores)
+            meeg.save_json("ecg_indices", ecg_indices)
+            meeg.save_json("ecg_scores", ecg_scores)
 
     meeg.save_ica(ica)
     # Add components to ica_exclude-dictionary
     meeg.pr.ica_exclude[meeg.name] = ica.exclude
 
 
 def _ica_plotto_helper(meeg, ica_plotto):
     ica = meeg.load_ica()
 
-    if ica_plotto == 'raw':
+    if ica_plotto == "raw":
         data = meeg.load_raw()
 
-    elif ica_plotto == 'raw_filtered':
+    elif ica_plotto == "raw_filtered":
         data = meeg.load_filtered()
 
-    elif ica_plotto == 'epochs':
+    elif ica_plotto == "epochs":
         data = meeg.load_epochs()
 
-    elif ica_plotto == 'epochs_eog':
+    elif ica_plotto == "epochs_eog":
         data = meeg.load_eog_epochs()
 
-    elif ica_plotto == 'epochs_ecg':
+    elif ica_plotto == "epochs_ecg":
         data = meeg.load_ecg_epochs()
 
-    elif ica_plotto == 'evoked':
+    elif ica_plotto == "evoked":
         data = meeg.load_evokeds()
 
-    elif ica_plotto == 'evoked (EOG)':
+    elif ica_plotto == "evoked (EOG)":
         data = meeg.load_eog_epochs().average()
 
-    elif ica_plotto == 'evoked (ECG)':
+    elif ica_plotto == "evoked (ECG)":
         data = meeg.load_ecg_epochs().average()
 
     else:
         data = None
 
     return ica, data
 
 
 def plot_ica_components(meeg, show_plots):
     ica = meeg.load_ica()
     components_fig = ica.plot_components(title=meeg.name, show=show_plots)
-    meeg.plot_save('ica', subfolder='components',
-                   matplotlib_figure=components_fig)
+    meeg.plot_save("ica", subfolder="components", matplotlib_figure=components_fig)
 
     return components_fig, ica
 
 
 def plot_ica_sources(meeg, ica_source_data, show_plots):
     ica, data = _ica_plotto_helper(meeg, ica_source_data)
-    sources_fig = ica.plot_sources(data, stop=ica.n_components,
-                                   title=meeg.name, show=show_plots)
-    meeg.plot_save('ica', subfolder='sources', matplotlib_figure=sources_fig)
+    sources_fig = ica.plot_sources(
+        data, stop=ica.n_components, title=meeg.name, show=show_plots
+    )
+    meeg.plot_save("ica", subfolder="sources", matplotlib_figure=sources_fig)
 
     return sources_fig, ica
 
 
 def plot_ica_overlay(meeg, ica_overlay_data, show_plots):
     ica, data = _ica_plotto_helper(meeg, ica_overlay_data)
     overlay_figs = list()
 
-    if ica_overlay_data == 'Evokeds':
+    if ica_overlay_data == "Evokeds":
         for evoked in [e for e in data if e.comment in meeg.sel_trials]:
-            ovl_fig = ica.plot_overlay(evoked,
-                                       title=f'{meeg.name}-{evoked.comment}',
-                                       show=show_plots)
+            ovl_fig = ica.plot_overlay(
+                evoked, title=f"{meeg.name}-{evoked.comment}", show=show_plots
+            )
             overlay_figs.append(ovl_fig)
     else:
         ovl_fig = ica.plot_overlay(data, title=meeg.name, show=show_plots)
         overlay_figs.append(ovl_fig)
 
-    meeg.plot_save('ica', subfolder='overlay', matplotlib_figure=overlay_figs)
+    meeg.plot_save("ica", subfolder="overlay", matplotlib_figure=overlay_figs)
 
     return overlay_figs
 
 
 def plot_ica_properties(meeg, show_plots):
     ica = meeg.load_ica()
     epochs = meeg.load_epochs()
 
-    eog_indices = meeg.load_json('eog_indices', default=list())
-    ecg_indices = meeg.load_json('ecg_indices', default=list())
-    psd_args = {'fmax': meeg.pa["lowpass"]}
+    eog_indices = meeg.load_json("eog_indices", default=list())
+    ecg_indices = meeg.load_json("ecg_indices", default=list())
+    psd_args = {"fmax": meeg.pa["lowpass"]}
 
     if len(eog_indices) > 0:
         eog_epochs = meeg.load_eog_epochs()
-        eog_prop_figs = ica.plot_properties(eog_epochs, eog_indices,
-                                            psd_args=psd_args,
-                                            show=show_plots)
-        meeg.plot_save('ica', subfolder='properties', trial='eog',
-                       matplotlib_figure=eog_prop_figs)
+        eog_prop_figs = ica.plot_properties(
+            eog_epochs, eog_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="eog", matplotlib_figure=eog_prop_figs
+        )
 
     if len(ecg_indices) > 0:
         ecg_epochs = meeg.load_ecg_epochs()
-        ecg_prop_figs = ica.plot_properties(ecg_epochs, ecg_indices,
-                                            psd_args=psd_args,
-                                            show=show_plots)
-        meeg.plot_save('ica', subfolder='properties', trial='ecg',
-                       matplotlib_figure=ecg_prop_figs)
-
-    remaining_indices = [ix for ix in ica.exclude if
-                         ix not in eog_indices + ecg_indices]
+        ecg_prop_figs = ica.plot_properties(
+            ecg_epochs, ecg_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="ecg", matplotlib_figure=ecg_prop_figs
+        )
+
+    remaining_indices = [
+        ix for ix in ica.exclude if ix not in eog_indices + ecg_indices
+    ]
     if len(remaining_indices) > 0:
-        prop_figs = ica.plot_properties(epochs, remaining_indices,
-                                        psd_args=psd_args, show=show_plots)
-        meeg.plot_save('ica', subfolder='properties', trial='manually',
-                       matplotlib_figure=prop_figs)
+        prop_figs = ica.plot_properties(
+            epochs, remaining_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="manually", matplotlib_figure=prop_figs
+        )
 
 
 def plot_ica_scores(meeg, show_plots):
-    eog_scores = meeg.load_json('eog_scores', default=list())
+    eog_scores = meeg.load_json("eog_scores", default=list())
     if len(eog_scores) > 1:
         ica = meeg.load_ica()
-        eog_score_fig = ica.plot_scores(eog_scores, title=f'{meeg.name}: EOG',
-                                        show=show_plots)
-        meeg.plot_save('ica', subfolder='scores', trial='eog',
-                       matplotlib_figure=eog_score_fig)
+        eog_score_fig = ica.plot_scores(
+            eog_scores, title=f"{meeg.name}: EOG", show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="scores", trial="eog", matplotlib_figure=eog_score_fig
+        )
     else:
         eog_score_fig = None
 
-    ecg_scores = meeg.load_json('ecg_scores', default=list())
+    ecg_scores = meeg.load_json("ecg_scores", default=list())
     if len(ecg_scores) > 1:
         ica = meeg.load_ica()
-        ecg_score_fig = ica.plot_scores(ecg_scores, title=f'{meeg.name}: ECG',
-                                        show=show_plots)
-        meeg.plot_save('ica', subfolder='scores', trial='ecg',
-                       matplotlib_figure=ecg_score_fig)
+        ecg_score_fig = ica.plot_scores(
+            ecg_scores, title=f"{meeg.name}: ECG", show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="scores", trial="ecg", matplotlib_figure=ecg_score_fig
+        )
     else:
         ecg_score_fig = None
 
     return eog_score_fig, ecg_score_fig
 
 
 def apply_ica(meeg, n_pca_components):
     # Check file-parameters to make sure,
     # that ica is not applied twice in a row
     epochs_file = Path(meeg.epochs_path).name
-    if epochs_file in meeg.file_parameters and \
-            meeg.file_parameters[epochs_file]['FUNCTION'] == 'apply_ica':
-        print(f'Not applying ICA because it was already applied to this file '
-              f'on {meeg.file_parameters[epochs_file]["TIME"]}. '
-              f'If you want to apply ICA again, delete the epochs-File in '
-              'FileManagement and redo the epochs.')
+    if (
+        epochs_file in meeg.file_parameters
+        and meeg.file_parameters[epochs_file]["FUNCTION"] == "apply_ica"
+    ):
+        print(
+            f"Not applying ICA because it was already applied to this file "
+            f'on {meeg.file_parameters[epochs_file]["TIME"]}. '
+            f"If you want to apply ICA again, delete the epochs-File in "
+            "FileManagement and redo the epochs."
+        )
     else:
         epochs = meeg.load_epochs()
         ica = meeg.load_ica()
 
         if len(ica.exclude) == 0:
-            print(f'No components excluded for {meeg.name}')
+            print(f"No components excluded for {meeg.name}")
         else:
             ica_epochs = ica.apply(epochs, n_pca_components=n_pca_components)
             meeg.save_epochs(ica_epochs)
 
         # Apply to Empty-Room-Data as well if present
         if meeg.erm:
             try:
@@ -717,16 +900,17 @@
             except FileNotFoundError:
                 erm_data = meeg.load_erm()
             try:
                 ica.apply(erm_data, n_pca_components)
             # Todo: Unmeddling ERM-SSP and ICA stuff
             except ValueError:
                 print(
-                    'There is an unresolved issue with combining SSP '
-                    'from ERM and applying ICA on this ERM')
+                    "There is an unresolved issue with combining SSP "
+                    "from ERM and applying ICA on this ERM"
+                )
             else:
                 meeg.save_erm_processed(erm_data)
 
 
 def get_evokeds(meeg):
     epochs = meeg.load_epochs()
     evokeds = []
@@ -750,69 +934,98 @@
     return gfp_dict
 
 
 def grand_avg_evokeds(group, ga_interpolate_bads, ga_drop_bads):
     trial_dict = {}
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
-        print(f'Add {name} to grand_average')
+        print(f"Add {name} to grand_average")
         evokeds = meeg.load_evokeds()
         for evoked in evokeds:
             if evoked.nave != 0:
                 if evoked.comment in trial_dict:
                     trial_dict[evoked.comment].append(evoked)
                 else:
                     trial_dict.update({evoked.comment: [evoked]})
             else:
-                print(f'{evoked.comment} for {name} got nave=0')
+                print(f"{evoked.comment} for {name} got nave=0")
 
     ga_evokeds = dict()
     for trial in trial_dict:
         if len(trial_dict[trial]) != 0:
-            ga = mne.grand_average(trial_dict[trial],
-                                   interpolate_bads=ga_interpolate_bads,
-                                   drop_bads=ga_drop_bads)
+            ga = mne.grand_average(
+                trial_dict[trial],
+                interpolate_bads=ga_interpolate_bads,
+                drop_bads=ga_drop_bads,
+            )
             ga.comment = trial
             ga_evokeds[trial] = ga
 
     group.save_ga_evokeds(ga_evokeds)
 
 
-def tfr(meeg, tfr_freqs, tfr_n_cycles, tfr_average, tfr_use_fft, tfr_baseline,
-        tfr_baseline_mode,
-        tfr_method, multitaper_bandwidth, stockwell_width, n_jobs, **kwargs):
+def tfr(
+    meeg,
+    tfr_freqs,
+    tfr_n_cycles,
+    tfr_average,
+    tfr_use_fft,
+    tfr_baseline,
+    tfr_baseline_mode,
+    tfr_method,
+    multitaper_bandwidth,
+    stockwell_width,
+    n_jobs,
+    **kwargs,
+):
     powers = list()
     itcs = list()
 
     epochs = meeg.load_epochs()
 
     # Calculate Time-Frequency for each trial from epochs
     # using the selected method
     for trial in meeg.sel_trials:
-        if tfr_method == 'multitaper':
-            multitaper_kwargs = check_kwargs(kwargs,
-                                             mne.time_frequency.tfr_multitaper)
+        if tfr_method == "multitaper":
+            multitaper_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_multitaper)
             tfr_result = mne.time_frequency.tfr_multitaper(
-                epochs[trial], freqs=tfr_freqs, n_cycles=tfr_n_cycles,
-                time_bandwidth=multitaper_bandwidth, n_jobs=n_jobs,
-                use_fft=tfr_use_fft, return_itc=tfr_average,
-                average=tfr_average, **multitaper_kwargs)
-        elif tfr_method == 'stockwell':
+                epochs[trial],
+                freqs=tfr_freqs,
+                n_cycles=tfr_n_cycles,
+                time_bandwidth=multitaper_bandwidth,
+                n_jobs=n_jobs,
+                use_fft=tfr_use_fft,
+                return_itc=tfr_average,
+                average=tfr_average,
+                **multitaper_kwargs,
+            )
+        elif tfr_method == "stockwell":
             fmin, fmax = tfr_freqs[[0, -1]]
-            stockwell_kwargs = check_kwargs(kwargs,
-                                            mne.time_frequency.tfr_stockwell)
+            stockwell_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_stockwell)
             tfr_result = mne.time_frequency.tfr_stockwell(
-                epochs[trial], fmin=fmin, fmax=fmax, width=stockwell_width,
-                n_jobs=n_jobs, return_itc=True, **stockwell_kwargs)
+                epochs[trial],
+                fmin=fmin,
+                fmax=fmax,
+                width=stockwell_width,
+                n_jobs=n_jobs,
+                return_itc=True,
+                **stockwell_kwargs,
+            )
         else:
             morlet_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_morlet)
             tfr_result = mne.time_frequency.tfr_morlet(
-                epochs[trial], freqs=tfr_freqs, n_cycles=tfr_n_cycles,
-                n_jobs=n_jobs, use_fft=tfr_use_fft, return_itc=tfr_average,
-                average=tfr_average, **morlet_kwargs)
+                epochs[trial],
+                freqs=tfr_freqs,
+                n_cycles=tfr_n_cycles,
+                n_jobs=n_jobs,
+                use_fft=tfr_use_fft,
+                return_itc=tfr_average,
+                average=tfr_average,
+                **morlet_kwargs,
+            )
 
         if isinstance(tfr_result, tuple):
             power = tfr_result[0]
             itc = tfr_result[1]
         else:
             power = tfr_result
             itc = None
@@ -826,15 +1039,15 @@
             if itc:
                 itc = itc.apply_baseline(tfr_baseline, mode=tfr_baseline_mode)
 
         powers.append(power)
         if itc:
             itcs.append(itc)
 
-    if tfr_average or tfr_method == 'stockwell':
+    if tfr_average or tfr_method == "stockwell":
         meeg.save_power_tfr_average(powers)
         meeg.save_itc_tfr_average(itcs)
 
     else:
         meeg.save_power_tfr_epochs(powers)
         meeg.save_itc_tfr_epochs(itcs)
 
@@ -846,310 +1059,351 @@
         meeg.save_itc_tfr_average(itcs_ave)
 
 
 def grand_avg_tfr(group):
     trial_dict = dict()
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
-        print(f'Add {name} to grand_average')
+        print(f"Add {name} to grand_average")
         powers = meeg.load_power_tfr_average()
         for pw in powers:
             if pw.nave != 0:
                 if pw.comment in trial_dict:
                     trial_dict[pw.comment].append(pw)
                 else:
                     trial_dict.update({pw.comment: [pw]})
             else:
-                print(f'{pw.comment} for {name} got nave=0')
+                print(f"{pw.comment} for {name} got nave=0")
 
     ga_dict = dict()
     for trial in trial_dict:
         if len(trial_dict[trial]) != 0:
-
             # Make sure, all have the same number of channels
             commons = set()
             for pw in trial_dict[trial]:
                 if len(commons) == 0:
                     for c in pw.ch_names:
                         commons.add(c)
                 commons = commons & set(pw.ch_names)
-            print(f'{trial}:Reducing all n_channels to {len(commons)}')
+            print(f"{trial}:Reducing all n_channels to {len(commons)}")
             for idx, pw in enumerate(trial_dict[trial]):
                 trial_dict[trial][idx] = pw.pick_channels(list(commons))
 
-            ga = mne.grand_average(trial_dict[trial],
-                                   interpolate_bads=True,
-                                   drop_bads=True)
+            ga = mne.grand_average(
+                trial_dict[trial], interpolate_bads=True, drop_bads=True
+            )
             ga.comment = trial
             ga_dict[trial] = ga
 
     group.save_ga_tfr(ga_dict)
 
 
 # ==============================================================================
 # BASH OPERATIONS
 # ==============================================================================
 # These functions do not work on Windows
-
 # local function used in the bash commands below
 def run_freesurfer_subprocess(command, subjects_dir, fs_path, mne_path=None):
     # Several experiments with subprocess showed,
     # that it seems impossible to run commands like "source" from
     # a subprocess to get SetUpFreeSurfer.sh into the environment.
     # Current workaround is adding the binaries to PATH manually,
     # after the user set the path to FREESURFER_HOME
     if fs_path is None:
-        raise RuntimeError(
-            'Path to FREESURFER_HOME not set, can\'t run this function')
+        raise RuntimeError("Path to FREESURFER_HOME not set, can't run this function")
     environment = environ.copy()
-    environment['FREESURFER_HOME'] = fs_path
-    environment['SUBJECTS_DIR'] = subjects_dir
+    environment["FREESURFER_HOME"] = fs_path
+    environment["SUBJECTS_DIR"] = subjects_dir
     if iswin:
-        command.insert(0, 'wsl')
+        command.insert(0, "wsl")
         if mne_path is None:
             raise RuntimeError(
-                'Path to MNE-Environment in Windows-Subsytem for Linux(WSL)'
-                ' not set, can\'t run this function')
+                "Path to MNE-Environment in Windows-Subsytem for Linux(WSL)"
+                " not set, can't run this function"
+            )
 
         # Add Freesurfer-Path, MNE-Path and standard Ubuntu-Paths,
         # which get lost when sharing the Path from Windows
         # to WSL
-        environment['PATH'] = f'{fs_path}/bin:{mne_path}/bin:' \
-                              f'/usr/local/sbin:' \
-                              f'/usr/local/bin:' \
-                              f'/usr/sbin:' \
-                              f'/usr/bin:' \
-                              f'/sbin:' \
-                              f'/bin'
-        environment['WSLENV'] = 'PATH/u:SUBJECTS_DIR/p:FREESURFER_HOME/u'
+        environment["PATH"] = (
+            f"{fs_path}/bin:{mne_path}/bin:"
+            f"/usr/local/sbin:"
+            f"/usr/local/bin:"
+            f"/usr/sbin:"
+            f"/usr/bin:"
+            f"/sbin:"
+            f"/bin"
+        )
+        environment["WSLENV"] = "PATH/u:SUBJECTS_DIR/p:FREESURFER_HOME/u"
     else:
         # Add Freesurfer to Path
-        environment['PATH'] = environment['PATH'] + f':{fs_path}/bin'
+        environment["PATH"] = environment["PATH"] + f":{fs_path}/bin"
 
     # Add Mac-specific Freesurfer-Paths
     # (got them from FreeSurferEnv.sh in FREESURFER_HOME)
     if ismac:
-        if isdir(join(fs_path, 'lib/misc/lib')):
-            environment['PATH'] = environment[
-                                      'PATH'] + f':{fs_path}/lib/misc/bin'
-            environment['MISC_LIB'] = join(fs_path, 'lib/misc/lib')
-            environment['LD_LIBRARY_PATH'] = join(fs_path, 'lib/misc/lib')
-            environment['DYLD_LIBRARY_PATH'] = join(fs_path, 'lib/misc/lib')
+        if isdir(join(fs_path, "lib/misc/lib")):
+            environment["PATH"] = environment["PATH"] + f":{fs_path}/lib/misc/bin"
+            environment["MISC_LIB"] = join(fs_path, "lib/misc/lib")
+            environment["LD_LIBRARY_PATH"] = join(fs_path, "lib/misc/lib")
+            environment["DYLD_LIBRARY_PATH"] = join(fs_path, "lib/misc/lib")
 
-        if isdir(join(fs_path, 'lib/gcc/lib')):
-            environment['DYLD_LIBRARY_PATH'] = join(fs_path, 'lib/gcc/lib')
+        if isdir(join(fs_path, "lib/gcc/lib")):
+            environment["DYLD_LIBRARY_PATH"] = join(fs_path, "lib/gcc/lib")
 
     # Popen is needed, run(which is supposed to be newer)
     # somehow doesn't seem to support live-stream via PIPE?!
-    process = subprocess.Popen(command, env=environment,
-                               stdout=subprocess.PIPE,
-                               stderr=subprocess.STDOUT,
-                               text=True, universal_newlines=True)
+    process = subprocess.Popen(
+        command,
+        env=environment,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.STDOUT,
+        text=True,
+        universal_newlines=True,
+    )
 
     # write subprocess-output to main-tread streams
     while process.poll() is None:
         stdout_line = process.stdout.readline()
         if stdout_line is not None:
             sys.stdout.write(stdout_line)
 
 
 def apply_watershed(fsmri):
-    print('Running Watershed algorithm for: ' + fsmri.name +
-          ". Output is written to the bem folder " +
-          "of the subject's FreeSurfer folder.\n" +
-          'Bash output follows below.\n\n')
+    print(
+        "Running Watershed algorithm for: "
+        + fsmri.name
+        + ". Output is written to the bem folder "
+        + "of the subject's FreeSurfer folder.\n"
+        + "Bash output follows below.\n\n"
+    )
 
     # watershed command
-    command = ['mne', 'watershed_bem',
-               '--subject', fsmri.name,
-               '--overwrite']
+    command = ["mne", "watershed_bem", "--subject", fsmri.name, "--overwrite"]
 
-    run_freesurfer_subprocess(command, fsmri.subjects_dir, fsmri.fs_path,
-                              fsmri.mne_path)
+    run_freesurfer_subprocess(
+        command, fsmri.subjects_dir, fsmri.fs_path, fsmri.mne_path
+    )
 
     if iswin:
         # Copy Watershed-Surfaces because the Links don't work
         # under Windows when made in WSL
-        surfaces = [(f'{fsmri.name}_inner_skull_surface', 'inner_skull.surf'),
-                    (f'{fsmri.name}_outer_skin_surface', 'outer_skin.surf'),
-                    (f'{fsmri.name}_outer_skull_surface', 'outer_skull.surf'),
-                    (f'{fsmri.name}_brain_surface', 'brain.surf')]
-        bem_dir = join(fsmri.subjects_dir, fsmri.name, 'bem')
-        watershed_dir = join(bem_dir, 'watershed')
+        surfaces = [
+            (f"{fsmri.name}_inner_skull_surface", "inner_skull.surf"),
+            (f"{fsmri.name}_outer_skin_surface", "outer_skin.surf"),
+            (f"{fsmri.name}_outer_skull_surface", "outer_skull.surf"),
+            (f"{fsmri.name}_brain_surface", "brain.surf"),
+        ]
+        bem_dir = join(fsmri.subjects_dir, fsmri.name, "bem")
+        watershed_dir = join(bem_dir, "watershed")
         for src, dst in surfaces:
             # Remove faulty link
             os.remove(join(bem_dir, dst))
             # Copy files
             source = join(watershed_dir, src)
-            destination = join(fsmri.subjects_dir, fsmri.name, 'bem', dst)
+            destination = join(fsmri.subjects_dir, fsmri.name, "bem", dst)
             shutil.copy2(source, destination)
 
-            print(f'{dst} was created')
+            print(f"{dst} was created")
 
 
 def make_dense_scalp_surfaces(fsmri):
-    print('Making dense scalp surfacing easing co-registration for ' +
-          'subject: ' + fsmri.name +
-          ". Output is written to the bem folder" +
-          " of the subject's FreeSurfer folder.\n" +
-          'Bash output follows below.\n\n')
-
-    command = ['mne', 'make_scalp_surfaces',
-               '--overwrite',
-               '--subject', fsmri.name,
-               '--force']
-
-    run_freesurfer_subprocess(command, fsmri.subjects_dir, fsmri.fs_path,
-                              fsmri.mne_path)
+    print(
+        "Making dense scalp surfacing easing co-registration for "
+        + "subject: "
+        + fsmri.name
+        + ". Output is written to the bem folder"
+        + " of the subject's FreeSurfer folder.\n"
+        + "Bash output follows below.\n\n"
+    )
+
+    command = [
+        "mne",
+        "make_scalp_surfaces",
+        "--overwrite",
+        "--subject",
+        fsmri.name,
+        "--force",
+    ]
+
+    run_freesurfer_subprocess(
+        command, fsmri.subjects_dir, fsmri.fs_path, fsmri.mne_path
+    )
 
 
 # ==============================================================================
 # MNE SOURCE RECONSTRUCTIONS
 # ==============================================================================
 
+
 def setup_src(fsmri, src_spacing, surface, n_jobs):
-    src = mne.setup_source_space(fsmri.name, spacing=src_spacing,
-                                 surface=surface,
-                                 subjects_dir=fsmri.subjects_dir,
-                                 add_dist=False, n_jobs=n_jobs)
+    src = mne.setup_source_space(
+        fsmri.name,
+        spacing=src_spacing,
+        surface=surface,
+        subjects_dir=fsmri.subjects_dir,
+        add_dist=False,
+        n_jobs=n_jobs,
+    )
     fsmri.save_source_space(src)
 
 
 def setup_vol_src(fsmri, vol_src_spacing):
     bem = fsmri.load_bem_solution()
-    vol_src = mne.setup_volume_src(fsmri.name, pos=vol_src_spacing, bem=bem,
-                                   subjects_dir=fsmri.subjects_dir)
+    vol_src = mne.setup_volume_source_space(
+        fsmri.name, pos=vol_src_spacing, bem=bem, subjects_dir=fsmri.subjects_dir
+    )
     fsmri.save_volume_source_space(vol_src)
 
 
 def compute_src_distances(fsmri, n_jobs):
     src = fsmri.load_source_space()
-    src_computed = mne.add_src_distances(src, n_jobs=n_jobs)
+    src_computed = mne.add_source_space_distances(src, n_jobs=n_jobs)
     fsmri.save_source_space(src_computed)
 
 
 def prepare_bem(fsmri, bem_spacing, bem_conductivity):
-    bem_model = mne.make_bem_model(fsmri.name, subjects_dir=fsmri.subjects_dir,
-                                   ico=bem_spacing,
-                                   conductivity=bem_conductivity)
+    bem_model = mne.make_bem_model(
+        fsmri.name,
+        subjects_dir=fsmri.subjects_dir,
+        ico=bem_spacing,
+        conductivity=bem_conductivity,
+    )
     fsmri.save_bem_model(bem_model)
 
     bem_solution = mne.make_bem_solution(bem_model)
     fsmri.save_bem_solution(bem_solution)
 
 
 def morph_fsmri(meeg, morph_to):
     if meeg.fsmri.name != morph_to:
         forward = meeg.load_forward()
-        morph = mne.compute_source_morph(forward['src'],
-                                         subject_from=meeg.fsmri.name,
-                                         subject_to=morph_to,
-                                         subjects_dir=meeg.subjects_dir)
+        morph = mne.compute_source_morph(
+            forward["src"],
+            subject_from=meeg.fsmri.name,
+            subject_to=morph_to,
+            subjects_dir=meeg.subjects_dir,
+        )
         meeg.save_source_morph(morph)
     else:
         logging.info(
-            f'There is no need to morph the source-space for {meeg.name}, '
+            f"There is no need to morph the source-space for {meeg.name}, "
             f'because the morph-destination "{morph_to}" '
-            f'is the same as the associated FSMRI.')
+            f"is the same as the associated FSMRI."
+        )
 
 
 def morph_labels_from_fsaverage(fsmri):
-    parcellations = ['aparc_sub', 'HCPMMP1_combined', 'HCPMMP1']
-    if not isfile(join(fsmri.subjects_dir, 'fsaverage/label',
-                       'lh.' + parcellations[0] + '.annot')):
+    parcellations = ["aparc_sub", "HCPMMP1_combined", "HCPMMP1"]
+    if not isfile(
+        join(fsmri.subjects_dir, "fsaverage/label", "lh." + parcellations[0] + ".annot")
+    ):
         mne.datasets.fetch_hcp_mmp_parcellation(
-            subjects_dir=fsmri.subjects_dir,
-            verbose=True)
+            subjects_dir=fsmri.subjects_dir, verbose=True
+        )
 
         mne.datasets.fetch_aparc_sub_parcellation(
-            subjects_dir=fsmri.subjects_dir,
-            verbose=True)
+            subjects_dir=fsmri.subjects_dir, verbose=True
+        )
     else:
-        print('You\'ve already downloaded the parcellations, splendid!')
+        print("You've already downloaded the parcellations, splendid!")
 
-    if not isfile(join(fsmri.subjects_dir, fsmri.name, 'label',
-                       'lh.' + parcellations[0] + '.annot')):
+    if not isfile(
+        join(
+            fsmri.subjects_dir, fsmri.name, "label", "lh." + parcellations[0] + ".annot"
+        )
+    ):
         for pc in parcellations:
-            labels = mne.read_labels_from_annot('fsaverage', pc, hemi='both')
-
-            m_labels = mne.morph_labels(labels, fsmri.name, 'fsaverage',
-                                        fsmri.subjects_dir,
-                                        surf_name='pial')
+            labels = mne.read_labels_from_annot("fsaverage", pc, hemi="both")
 
-            mne.write_labels_to_annot(m_labels, subject=fsmri.name, parc=pc,
-                                      subjects_dir=fsmri.subjects_dir,
-                                      overwrite=True)
+            m_labels = mne.morph_labels(
+                labels, fsmri.name, "fsaverage", fsmri.subjects_dir, surf_name="pial"
+            )
+
+            mne.write_labels_to_annot(
+                m_labels,
+                subject=fsmri.name,
+                parc=pc,
+                subjects_dir=fsmri.subjects_dir,
+                overwrite=True,
+            )
 
     else:
-        print(f'{parcellations} already exist')
+        print(f"{parcellations} already exist")
 
 
 def create_forward_solution(meeg, n_jobs, ch_types):
     info = meeg.load_info()
     trans = meeg.load_transformation()
     bem = meeg.fsmri.load_bem_solution()
     src = meeg.fsmri.load_source_space()
 
-    if 'eeg' in ch_types:
+    if "eeg" in ch_types:
         eeg = True
     else:
         eeg = False
 
-    forward = mne.make_forward_solution(info, trans, src, bem, eeg=eeg,
-                                        n_jobs=n_jobs)
+    forward = mne.make_forward_solution(info, trans, src, bem, eeg=eeg, n_jobs=n_jobs)
 
     meeg.save_forward(forward)
 
 
-def estimate_noise_covariance(meeg, baseline, n_jobs, noise_cov_mode,
-                              noise_cov_method, **kwargs):
-    if noise_cov_mode == 'epochs' or meeg.erm is None:
-        print('Noise Covariance on epochs-Baseline')
+def estimate_noise_covariance(
+    meeg, baseline, n_jobs, noise_cov_mode, noise_cov_method, **kwargs
+):
+    # ToDo: method='factor_analysis' can only be used with rank='full'
+    if noise_cov_mode == "epochs" or meeg.erm is None:
+        print("Noise Covariance on epochs-Baseline")
         epochs = meeg.load_epochs()
 
         tmin, tmax = baseline
         kwargs = check_kwargs(kwargs, mne.compute_covariance)
-        noise_covariance = mne.compute_covariance(epochs, tmin=tmin, tmax=tmax,
-                                                  method=noise_cov_method,
-                                                  n_jobs=n_jobs, **kwargs)
+        noise_covariance = mne.compute_covariance(
+            epochs,
+            tmin=tmin,
+            tmax=tmax,
+            method=noise_cov_method,
+            n_jobs=n_jobs,
+            **kwargs,
+        )
         meeg.save_noise_covariance(noise_covariance)
 
     else:
-        print('Noise Covariance on Empty-Room-Data')
+        print("Noise Covariance on Empty-Room-Data")
         erm_filtered = meeg.load_erm_processed()
-        erm_filtered.pick([ch for ch in erm_filtered.ch_names if
-                           ch not in meeg.bad_channels])
+        # Add bad channels to erm-recording
+        erm_filtered.info["bads"] = meeg.bad_channels
 
         kwargs = check_kwargs(kwargs, mne.compute_raw_covariance)
-        noise_covariance = mne.compute_raw_covariance(erm_filtered,
-                                                      n_jobs=n_jobs,
-                                                      method=noise_cov_method,
-                                                      **kwargs)
+        noise_covariance = mne.compute_raw_covariance(
+            erm_filtered, n_jobs=n_jobs, method=noise_cov_method, **kwargs
+        )
         meeg.save_noise_covariance(noise_covariance)
 
 
 def create_inverse_operator(meeg):
     info = meeg.load_info()
     noise_covariance = meeg.load_noise_covariance()
     forward = meeg.load_forward()
 
-    inverse_operator = mne.minimum_norm.make_inverse_operator(info, forward,
-                                                              noise_covariance)
+    inverse_operator = mne.minimum_norm.make_inverse_operator(
+        info, forward, noise_covariance
+    )
     meeg.save_inverse_operator(inverse_operator)
 
 
 def source_estimate(meeg, inverse_method, pick_ori, lambda2):
     inverse_operator = meeg.load_inverse_operator()
     evokeds = meeg.load_evokeds()
 
     stcs = {}
     for evoked in [ev for ev in evokeds if ev.comment in meeg.sel_trials]:
-        stc = mne.minimum_norm.apply_inverse(evoked, inverse_operator, lambda2,
-                                             method=inverse_method,
-                                             pick_ori=pick_ori)
+        stc = mne.minimum_norm.apply_inverse(
+            evoked, inverse_operator, lambda2, method=inverse_method, pick_ori=pick_ori
+        )
         stcs.update({evoked.comment: stc})
 
     meeg.save_source_estimates(stcs)
 
 
 def label_time_course(meeg, target_labels, extract_mode):
     stcs = meeg.load_source_estimates()
@@ -1158,78 +1412,102 @@
 
     ltc_dict = {}
 
     for trial in stcs:
         ltc_dict[trial] = {}
         times = stcs[trial].times
         for label in labels:
-            ltc = stcs[trial].extract_label_time_course(label, src,
-                                                        mode=extract_mode)[0]
+            ltc = stcs[trial].extract_label_time_course(label, src, mode=extract_mode)[
+                0
+            ]
             ltc_dict[trial][label.name] = np.vstack((ltc, times))
 
     meeg.save_ltc(ltc_dict)
 
 
 # Todo: Make mixed-norm more customizable
 
+
 def mixed_norm_estimate(meeg, pick_ori, inverse_method):
     evokeds = meeg.load_evokeds()
     forward = meeg.load_forward()
     noise_cov = meeg.load_noise_covariance()
     inv_op = meeg.load_inverse_operator()
-    if inverse_method == 'dSPM':
-        print('dSPM-Inverse-Solution existent, loading...')
+    if inverse_method == "dSPM":
+        print("dSPM-Inverse-Solution existent, loading...")
         stcs = meeg.load_source_estimates()
     else:
-        print('No dSPM-Inverse-Solution available, calculating...')
+        print("No dSPM-Inverse-Solution available, calculating...")
         stcs = dict()
         snr = 3.0
-        lambda2 = 1.0 / snr ** 2
+        lambda2 = 1.0 / snr**2
         for evoked in evokeds:
             trial = evoked.comment
-            stcs[trial] = mne.minimum_norm.apply_inverse(evoked, inv_op,
-                                                         lambda2,
-                                                         method='dSPM')
+            stcs[trial] = mne.minimum_norm.apply_inverse(
+                evoked, inv_op, lambda2, method="dSPM"
+            )
 
     mixn_dips = {}
     mixn_stcs = {}
 
     for evoked in [ev for ev in evokeds if ev.comment in meeg.sel_trials]:
         alpha = 30  # regularization parameter between 0 and 100 (100 is high)
         n_mxne_iter = 10  # if > 1 use L0.5/L2 reweighted mixed norm solver
         # if n_mxne_iter > 1 dSPM weighting can be avoided.
         trial = evoked.comment
         mixn_dipoles, dip_residual = mne.inverse_sparse.mixed_norm(
-            evoked, forward, noise_cov, alpha, maxit=3000, tol=1e-4,
-            active_set_size=10, debias=True, weights=stcs[trial],
-            n_mxne_iter=n_mxne_iter, return_residual=True,
-            return_as_dipoles=True)
+            evoked,
+            forward,
+            noise_cov,
+            alpha,
+            maxit=3000,
+            tol=1e-4,
+            active_set_size=10,
+            debias=True,
+            weights=stcs[trial],
+            n_mxne_iter=n_mxne_iter,
+            return_residual=True,
+            return_as_dipoles=True,
+        )
         mixn_dips[trial] = mixn_dipoles
 
         mixn_stc, residual = mne.inverse_sparse.mixed_norm(
-            evoked, forward, noise_cov, alpha, maxit=3000, tol=1e-4,
-            active_set_size=10, debias=True, weights=stcs[trial],
-            n_mxne_iter=n_mxne_iter, return_residual=True,
-            return_as_dipoles=False, pick_ori=pick_ori)
+            evoked,
+            forward,
+            noise_cov,
+            alpha,
+            maxit=3000,
+            tol=1e-4,
+            active_set_size=10,
+            debias=True,
+            weights=stcs[trial],
+            n_mxne_iter=n_mxne_iter,
+            return_residual=True,
+            return_as_dipoles=False,
+            pick_ori=pick_ori,
+        )
         mixn_stcs[evoked.comment] = mixn_stc
 
     meeg.save_mixn_dipoles(mixn_dips)
     meeg.save_mixn_source_estimates(mixn_stcs)
 
 
 # Todo: Separate Plot-Functions
 #  (better responsivness of GUI during fit, when running in QThread)
 
+
 def ecd_fit(meeg, ecd_times, ecd_positions, ecd_orientations, t_epoch):
     try:
         ecd_time = ecd_times[meeg.name]
     except KeyError:
-        ecd_time = {'Dip1': (0, t_epoch[1])}
-        print(f'No Dipole times assigned for {meeg.name},'
-              f' Dipole-Times: 0-{t_epoch[1]}')
+        ecd_time = {"Dip1": (0, t_epoch[1])}
+        print(
+            f"No Dipole times assigned for {meeg.name},"
+            f" Dipole-Times: 0-{t_epoch[1]}"
+        )
 
     evokeds = meeg.load_evokeds()
     noise_covariance = meeg.load_noise_covariance()
     bem = meeg.fsmri.load_bem_solution()
     trans = meeg.load_transformation()
 
     ecd_dips = {}
@@ -1243,30 +1521,40 @@
 
             try:
                 ecd_position = ecd_positions[meeg.name][dip]
                 ecd_orientation = ecd_orientations[meeg.name][dip]
             except KeyError:
                 ecd_position = None
                 ecd_orientation = None
-                print(f'No Position&Orientation for Dipole for {meeg.name}'
-                      f' assigned, sequential fitting and free orientation '
-                      'used.')
+                print(
+                    f"No Position&Orientation for Dipole for {meeg.name}"
+                    f" assigned, sequential fitting and free orientation "
+                    "used."
+                )
 
             if ecd_position:
-                dipole, residual = mne.fit_dipole(copy_evoked,
-                                                  noise_covariance, bem,
-                                                  trans=trans,
-                                                  min_dist=3.0, n_jobs=4,
-                                                  pos=ecd_position,
-                                                  ori=ecd_orientation)
+                dipole, residual = mne.fit_dipole(
+                    copy_evoked,
+                    noise_covariance,
+                    bem,
+                    trans=trans,
+                    min_dist=3.0,
+                    n_jobs=4,
+                    pos=ecd_position,
+                    ori=ecd_orientation,
+                )
             else:
-                dipole, residual = mne.fit_dipole(copy_evoked,
-                                                  noise_covariance, bem,
-                                                  trans=trans, min_dist=3.0,
-                                                  n_jobs=4)
+                dipole, residual = mne.fit_dipole(
+                    copy_evoked,
+                    noise_covariance,
+                    bem,
+                    trans=trans,
+                    min_dist=3.0,
+                    n_jobs=4,
+                )
 
             ecd_dips[trial][dip] = dipole
 
     meeg.save_ecd(ecd_dips)
 
 
 def apply_morph(meeg, morph_to):
@@ -1276,149 +1564,172 @@
 
         morphed_stcs = {}
         for trial in stcs:
             morphed_stcs[trial] = morph.apply(stcs[trial])
         meeg.save_morphed_source_estimates(morphed_stcs)
     else:
         logging.info(
-            f'{meeg.name} is already in source-space of {morph_to} '
-            f'and won\'t be morphed')
+            f"{meeg.name} is already in source-space of {morph_to} "
+            f"and won't be morphed"
+        )
 
 
-def src_connectivity(meeg, target_labels, inverse_method,
-                     lambda2, con_methods,
-                     con_fmin, con_fmax, n_jobs):
+def src_connectivity(
+    meeg,
+    target_labels,
+    inverse_method,
+    lambda2,
+    con_methods,
+    con_fmin,
+    con_fmax,
+    n_jobs,
+):
     info = meeg.load_info()
     all_epochs = meeg.load_epochs()
     inverse_operator = meeg.load_inverse_operator()
-    src = inverse_operator['src']
+    src = inverse_operator["src"]
     labels = meeg.fsmri.get_labels(target_labels)
 
     con_dict = {}
 
     for trial in [t for t in all_epochs.event_id if t]:
-        con_dict[trial.split('/')[0]] = {}
-        epochs = all_epochs[trial.split('/')[0]]
+        con_dict[trial.split("/")[0]] = {}
+        epochs = all_epochs[trial.split("/")[0]]
         # Compute inverse solution and for each epoch.
         # By using "return_generator=True" stcs will be a generator object
         # instead of a list.
         stcs = mne.minimum_norm.apply_inverse_epochs(
-            epochs, inverse_operator, lambda2, inverse_method,
-            pick_ori="normal", return_generator=True)
-
-        label_ts = mne.extract_label_time_course(stcs, labels,
-                                                 src, mode='mean_flip',
-                                                 return_generator=True)
-
-        sfreq = info['sfreq']  # the sampling frequency
-        con = mne_connectivity.spectral_connectivity(
-            label_ts, method=con_methods, mode='multitaper', sfreq=sfreq,
-            fmin=con_fmin, fmax=con_fmax, faverage=True, mt_adaptive=True,
-            n_jobs=n_jobs)
+            epochs,
+            inverse_operator,
+            lambda2,
+            inverse_method,
+            pick_ori="normal",
+            return_generator=True,
+        )
+
+        label_ts = mne.extract_label_time_course(
+            stcs, labels, src, mode="mean_flip", return_generator=True
+        )
+
+        sfreq = info["sfreq"]  # the sampling frequency
+        con = mne_connectivity.spectral_connectivity_epochs(
+            label_ts,
+            method=con_methods,
+            mode="multitaper",
+            sfreq=sfreq,
+            fmin=con_fmin,
+            fmax=con_fmax,
+            faverage=True,
+            mt_adaptive=True,
+            n_jobs=n_jobs,
+        )
 
         if not isinstance(con, list):
             con = [con]
 
         # con is a 3D array, get the connectivity for the first (and only)
         # freq. band for each con_method
         for method, c in zip(con_methods, con):
-            con_dict[trial.split('/')[0]][method] = \
-                c.get_data(output='dense')[:, :, 0]
+            con_dict[trial.split("/")[0]][method] = c.get_data(output="dense")[:, :, 0]
 
     meeg.save_connectivity(con_dict)
 
     for trial in all_epochs.event_id:
-        con_dict[trial.split('/')[1]] = {}
+        con_dict[trial.split("/")[1]] = {}
         # epochs = all_epochs[trial.split('/')[1]][:2]
-        epochs = all_epochs[trial.split('/')[1]]
+        epochs = all_epochs[trial.split("/")[1]]
         # Compute inverse solution and for each epoch.
         # By using "return_generator=True" stcs will be a generator object
         # instead of a list.
-        stcs = mne.minimum_norm.apply_inverse_epochs(epochs, inverse_operator,
-                                                     lambda2, inverse_method,
-                                                     pick_ori="normal",
-                                                     return_generator=True)
+        stcs = mne.minimum_norm.apply_inverse_epochs(
+            epochs,
+            inverse_operator,
+            lambda2,
+            inverse_method,
+            pick_ori="normal",
+            return_generator=True,
+        )
 
         # Average the source estimates within each label using
         # sign-flips to reduce signal cancellations, also here we return a
         # generator
 
-        label_ts = mne.extract_label_time_course(stcs, labels,
-                                                 src, mode='mean_flip',
-                                                 return_generator=True)
-
-        sfreq = info['sfreq']  # the sampling frequency
-        con = mne_connectivity.spectral_connectivity(label_ts,
-                                                     method=con_methods,
-                                                     mode='multitaper',
-                                                     sfreq=sfreq,
-                                                     fmin=con_fmin,
-                                                     fmax=con_fmax,
-                                                     faverage=True,
-                                                     mt_adaptive=True,
-                                                     n_jobs=n_jobs)
+        label_ts = mne.extract_label_time_course(
+            stcs, labels, src, mode="mean_flip", return_generator=True
+        )
+
+        sfreq = info["sfreq"]  # the sampling frequency
+        con = mne_connectivity.spectral_connectivity(
+            label_ts,
+            method=con_methods,
+            mode="multitaper",
+            sfreq=sfreq,
+            fmin=con_fmin,
+            fmax=con_fmax,
+            faverage=True,
+            mt_adaptive=True,
+            n_jobs=n_jobs,
+        )
 
         if not isinstance(con, list):
             con = [con]
 
         # con is a 3D array, get the connectivity for the first
         # (and only) freq. band for each con_method
         for method, c in zip(con_methods, con):
-            con_dict[trial.split('/')[1]][method] = \
-                c.get_data(output='dense')[:, :, 0]
+            con_dict[trial.split("/")[1]][method] = c.get_data(output="dense")[:, :, 0]
 
     meeg.save_connectivity(con_dict)
 
 
 def grand_avg_morphed(group, morph_to):
     # for less memory only import data from stcs and add it to one
     # stc in the end!!!
     n_chunks = 8
     # divide in chunks to save memory
     fusion_dict = {}
     for i in range(0, len(group.group_list), n_chunks):
         sub_trial_dict = {}
-        ga_chunk = group.group_list[i:i + n_chunks]
+        ga_chunk = group.group_list[i : i + n_chunks]
         print(ga_chunk)
         for name in ga_chunk:
             meeg = MEEG(name, group.ct)
-            print(f'Add {name} to grand_average')
+            print(f"Add {name} to grand_average")
             if morph_to == meeg.fsmri.name:
                 stcs = meeg.load_source_estimates()
             else:
                 stcs = meeg.load_morphed_source_estimates()
 
             for trial in stcs:
                 if trial in sub_trial_dict:
                     sub_trial_dict[trial].append(stcs[trial])
                 else:
                     sub_trial_dict.update({trial: [stcs[trial]]})
 
         # Average chunks
         for trial in sub_trial_dict:
             if len(sub_trial_dict[trial]) != 0:
-                print(f'grand_average for {trial}-chunk {i}-{i + n_chunks}')
+                print(f"grand_average for {trial}-chunk {i}-{i + n_chunks}")
                 sub_trial_average = sub_trial_dict[trial][0].copy()
                 n_subjects = len(sub_trial_dict[trial])
 
                 for trial_index in range(1, n_subjects):
-                    sub_trial_average.data += sub_trial_dict[trial][
-                        trial_index].data
+                    sub_trial_average.data += sub_trial_dict[trial][trial_index].data
 
                 sub_trial_average.data /= n_subjects
                 sub_trial_average.comment = trial
                 if trial in fusion_dict:
                     fusion_dict[trial].append(sub_trial_average)
                 else:
                     fusion_dict.update({trial: [sub_trial_average]})
 
     ga_stcs = {}
     for trial in fusion_dict:
         if len(fusion_dict[trial]) != 0:
-            print(f'grand_average for {group.name}-{trial}')
+            print(f"grand_average for {group.name}-{trial}")
             trial_average = fusion_dict[trial][0].copy()
             n_subjects = len(fusion_dict[trial])
 
             for trial_index in range(1, n_subjects):
                 trial_average.data += fusion_dict[trial][trial_index].data
 
             trial_average.data /= n_subjects
@@ -1430,37 +1741,35 @@
 
 
 def grand_avg_ltc(group):
     ltc_average_dict = {}
     times = None
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
-        print(f'Add {name} to grand_average')
+        print(f"Add {name} to grand_average")
         ltc_dict = meeg.load_ltc()
         for trial in ltc_dict:
             if trial not in ltc_average_dict:
                 ltc_average_dict[trial] = {}
             for label in ltc_dict[trial]:
                 # First row of array is label-time-course-data,
                 # second row is time-array
                 if label in ltc_average_dict[trial]:
-                    ltc_average_dict[trial][label].append(
-                        ltc_dict[trial][label][0])
+                    ltc_average_dict[trial][label].append(ltc_dict[trial][label][0])
                 else:
-                    ltc_average_dict[trial][label] = [
-                        ltc_dict[trial][label][0]]
+                    ltc_average_dict[trial][label] = [ltc_dict[trial][label][0]]
                 # Should be the same for each trial and label
                 times = ltc_dict[trial][label][1]
 
     ga_ltc = {}
     for trial in ltc_average_dict:
         ga_ltc[trial] = {}
         for label in ltc_average_dict[trial]:
             if len(ltc_average_dict[trial][label]) != 0:
-                print(f'grand_average for {trial}-{label}')
+                print(f"grand_average for {trial}-{label}")
                 ltc_list = ltc_average_dict[trial][label]
                 # Take the absolute values
                 ltc_list = [abs(it) for it in ltc_list]
                 n_subjects = len(ltc_list)
                 average = ltc_list[0]
                 for idx in range(1, n_subjects):
                     average += ltc_list[idx]
@@ -1473,33 +1782,33 @@
 
 
 def grand_avg_connect(group):
     # Prepare the Average-Dict
     con_average_dict = {}
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
-        print(f'Add {name} to grand_average')
+        print(f"Add {name} to grand_average")
         con_dict = meeg.load_connectivity()
         for trial in con_dict:
             if trial not in con_average_dict:
                 con_average_dict[trial] = {}
             for con_method in con_dict[trial]:
                 if con_method in con_average_dict[trial]:
                     con_average_dict[trial][con_method].append(
-                        con_dict[trial][con_method])
+                        con_dict[trial][con_method]
+                    )
                 else:
-                    con_average_dict[trial][con_method] = [
-                        con_dict[trial][con_method]]
+                    con_average_dict[trial][con_method] = [con_dict[trial][con_method]]
 
     ga_con = {}
     for trial in con_average_dict:
         ga_con[trial] = {}
         for con_method in con_average_dict[trial]:
             if len(con_average_dict[trial][con_method]) != 0:
-                print(f'grand_average for {trial}-{con_method}')
+                print(f"grand_average for {trial}-{con_method}")
                 con_list = con_average_dict[trial][con_method]
                 n_subjects = len(con_list)
                 average = con_list[0]
                 for idx in range(1, n_subjects):
                     average += con_list[idx]
 
                 average /= n_subjects
@@ -1508,10 +1817,10 @@
 
     group.save_ga_con(ga_con)
 
 
 def print_info(meeg):
     print(meeg.load_info())
     for n in range(20):
-        print(f'\r{n}', end='')
+        print(f"\r{n}", end="")
         time.sleep(0.1)
-    raise RuntimeError('Test')
+    raise RuntimeError("Test")
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/functions/plot.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from __future__ import print_function
 
 import gc
 import multiprocessing
 from os.path import join
@@ -26,17 +24,17 @@
     from nilearn.plotting import plot_anat
 except (ModuleNotFoundError, ValueError):
     pass
 
 from mne_pipeline_hd.functions import operations as op
 
 
-# =============================================================================
+# ==============================================================================
 # PLOTTING FUNCTIONS
-# =============================================================================
+# ==============================================================================
 
 def plot_raw(meeg, show_plots):
     raw = meeg.load_raw()
 
     try:
         events = meeg.load_events()
     except FileNotFoundError:
@@ -585,15 +583,15 @@
                  sorted(zip(rh_label_ypos, rh_labels))]
 
     # Save the plot order and create a circular layout
     node_order = list()
     node_order.extend(lh_labels[::-1])  # reverse the order
     node_order.extend(rh_labels)
 
-    node_angles = mne_connectivity.viz.circular_layout(
+    node_angles = mne.viz.circular_layout(
         label_names, node_order, start_pos=90,
         group_boundaries=[0, len(label_names) / 2])
 
     # Plot the graph using node colors from the FreeSurfer parcellation.
     # We only show the 300 strongest connections.
     for trial in con_dict:
         for con_method in con_dict[trial]:
@@ -702,34 +700,35 @@
                 plt.show()
 
             group.plot_save('ga_label-time-course', subfolder=label,
                             trial=trial)
 
 
 def plot_grand_avg_connect(group, con_fmin, con_fmax, target_labels,
-                           morph_to, show_plots):
+                           morph_to, show_plots, connectivity_vmin,
+                           connectivity_vmax):
     ga_dict = group.load_ga_con()
 
     # Get labels for FreeSurfer 'aparc' cortical parcellation
     # with 34 labels/hemi
     fsmri = FSMRI(morph_to, group.ct)
     labels = fsmri.get_labels(target_labels)
     if 'unknown-lh' in labels:
-        labels.pop('unknown-lh')
+        labels.remove('unknown-lh')
 
-    label_colors = [label.color for label in labels.values()]
+    label_colors = [label.color for label in labels]
+    label_names = [lb.name for lb in labels]
 
-    label_names = list(labels.keys())
     lh_labels = [l_name for l_name in label_names if l_name.endswith('lh')]
     rh_labels = [l_name for l_name in label_names if l_name.endswith('rh')]
 
     # Get the y-location of the label
-    lh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels.values()
+    lh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
                      if lb.name in lh_labels]
-    rh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels.values()
+    rh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
                      if lb.name in rh_labels]
 
     # Reorder the labels based on their location
     lh_labels = [label for (yp, label) in
                  sorted(zip(lh_label_ypos, lh_labels))]
     rh_labels = [label for (yp, label) in
                  sorted(zip(rh_label_ypos, rh_labels))]
@@ -741,20 +740,22 @@
 
     node_angles = mne.viz.circular_layout(
         label_names, node_order, start_pos=90,
         group_boundaries=[0, len(label_names) / 2])
 
     for trial in ga_dict:
         for method in ga_dict[trial]:
-            fig, axes = mne.viz.plot_connectivity_circle(
+            fig, axes = mne_connectivity.viz.plot_connectivity_circle(
                 ga_dict[trial][method],
                 label_names, n_lines=300,
                 node_angles=node_angles,
                 node_colors=label_colors,
                 title=f'{method}: {str(con_fmin)}-{str(con_fmax)}',
+                vmin=connectivity_vmin,
+                vmax=connectivity_vmax,
                 fontsize_names=16, show=show_plots)
 
             group.plot_save('ga_connectivity', subfolder=method, trial=trial,
                             matplotlib_figure=fig)
 
 
 def close_all():
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/base_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/base_widgets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,55 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import itertools
 import sys
 
 import numpy as np
 import pandas
 from PyQt5.QtCore import QItemSelectionModel, QTimer, Qt, pyqtSignal
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QAbstractItemView, QApplication, QDialog,
-                             QHBoxLayout, QLabel,
-                             QListView, QPushButton, QScrollArea, QSizePolicy,
-                             QSpinBox, QTabWidget, QTableView, QTreeView,
-                             QVBoxLayout, QWidget)
+from PyQt5.QtWidgets import (
+    QAbstractItemView,
+    QApplication,
+    QDialog,
+    QHBoxLayout,
+    QLabel,
+    QListView,
+    QPushButton,
+    QScrollArea,
+    QSizePolicy,
+    QSpinBox,
+    QTabWidget,
+    QTableView,
+    QTreeView,
+    QVBoxLayout,
+    QWidget,
+    QComboBox,
+)
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.gui.gui_utils import get_user_input_string
-from mne_pipeline_hd.gui.models import (BaseDictModel, BaseListModel,
-                                        BasePandasModel,
-                                        CheckDictEditModel, CheckDictModel,
-                                        CheckListModel,
-                                        EditDictModel, EditListModel,
-                                        EditPandasModel,
-                                        FileManagementModel, TreeModel)
+from mne_pipeline_hd.gui.models import (
+    BaseDictModel,
+    BaseListModel,
+    BasePandasModel,
+    CheckDictEditModel,
+    CheckDictModel,
+    CheckListModel,
+    EditDictModel,
+    EditListModel,
+    EditPandasModel,
+    FileManagementModel,
+    TreeModel,
+)
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class Base(QWidget):
     currentChanged = pyqtSignal(object, object)
     selectionChanged = pyqtSignal(object)
     dataChanged = pyqtSignal(object, object)
@@ -51,31 +68,29 @@
 
         if drag_drop:
             self.view.setDragEnabled(True)
             self.view.setAcceptDrops(True)
             self.setDropIndicatorShown(True)
 
         # Connect to custom Selection-Signal
-        self.view.selectionModel().currentChanged.connect(
-            self._current_changed)
-        self.view.selectionModel().selectionChanged.connect(
-            self._selection_changed)
+        self.view.selectionModel().currentChanged.connect(self._current_changed)
+        self.view.selectionModel().selectionChanged.connect(self._selection_changed)
         self.model.dataChanged.connect(self._data_changed)
 
         self.init_ui()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         if self.title:
             title_label = QLabel(self.title)
             if len(self.title) <= 12:
-                title_label.setFont(QFont(QS().value('app_font'), 14))
+                title_label.setFont(QFont(QS().value("app_font"), 14))
             else:
-                title_label.setFont(QFont(QS().value('app_font'), 12))
+                title_label.setFont(QFont(QS().value("app_font"), 12))
             layout.addWidget(title_label)
 
         layout.addWidget(self.view)
         self.setLayout(layout)
 
     def get_current(self):
         try:
@@ -88,74 +103,77 @@
     def _current_changed(self, current_idx, previous_idx):
         current = self.model.getData(current_idx)
         previous = self.model.getData(previous_idx)
 
         self.currentChanged.emit(current, previous)
 
         if self.verbose:
-            print(f'Current changed from {previous} to {current}')
+            print(f"Current changed from {previous} to {current}")
 
     def get_selected(self):
         try:
-            selected = [self.model.getData(idx)
-                        for idx in self.view.selectedIndexes()]
+            selected = [self.model.getData(idx) for idx in self.view.selectedIndexes()]
         except (KeyError, IndexError):
             selected = list()
 
         return selected
 
     def _selection_changed(self):
         # Although the SelectionChanged-Signal sends
         # selected/deselected indexes, I don't use them here, because they
         # don't seem represent the selection.
         selected = self.get_selected()
 
         self.selectionChanged.emit(selected)
 
         if self.verbose:
-            print(f'Selection changed to {selected}')
+            print(f"Selection changed to {selected}")
 
     def _data_changed(self, index, _):
         data = self.model.getData(index)
 
         self.dataChanged.emit(data, index)
         if self.verbose:
-            print(f'{data} changed at {index}')
+            print(f"{data} changed at {index}")
 
     def content_changed(self):
-        """Informs ModelView about external change made in data
-        """
+        """Informs ModelView about external change made in data"""
         self.model.layoutChanged.emit()
 
     def replace_data(self, new_data):
-        """Replaces model._data with new_data
-        """
+        """Replaces model._data with new_data"""
         self.model._data = new_data
         self.content_changed()
 
 
 class BaseList(Base):
-    def __init__(self, model, view, extended_selection=False,
-                 drag_drop=False, parent=None, title=None, verbose=False):
-        super().__init__(model, view, drag_drop, parent,
-                         title, verbose=verbose)
+    def __init__(
+        self,
+        model,
+        view,
+        extended_selection=False,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        verbose=False,
+    ):
+        super().__init__(model, view, drag_drop, parent, title, verbose=verbose)
 
         if extended_selection:
             self.view.setSelectionMode(QAbstractItemView.ExtendedSelection)
 
     def select(self, values, clear_selection=True):
         indices = [i for i, x in enumerate(self.model._data) if x in values]
 
         if clear_selection:
             self.view.selectionModel().clearSelection()
 
         for idx in indices:
             index = self.model.createIndex(idx, 0)
-            self.view.selectionModel().select(index,
-                                              QItemSelectionModel.Select)
+            self.view.selectionModel().select(index, QItemSelectionModel.Select)
 
 
 class SimpleList(BaseList):
     """A basic List-Widget to display the content of a list.
 
     Parameters
     ----------
@@ -177,22 +195,33 @@
     Notes
     -----
     If you change the contents of data outside of this class,
     call content_changed to update this widget.
     If you change the reference to data, call the appropriate replace_data.
     """
 
-    def __init__(self, data=None, extended_selection=False,
-                 show_index=False, drag_drop=False,
-                 parent=None, title=None, verbose=False):
-        super().__init__(model=BaseListModel(data, show_index, drag_drop),
-                         view=QListView(),
-                         extended_selection=extended_selection,
-                         drag_drop=drag_drop,
-                         parent=parent, title=title, verbose=verbose)
+    def __init__(
+        self,
+        data=None,
+        extended_selection=False,
+        show_index=False,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        verbose=False,
+    ):
+        super().__init__(
+            model=BaseListModel(data, show_index, drag_drop),
+            view=QListView(),
+            extended_selection=extended_selection,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
 
 
 class EditList(BaseList):
     """An editable List-Widget to display and manipulate the content of a list.
 
     Parameters
     ----------
@@ -219,65 +248,78 @@
     Notes
     -----
     If you change the contents of the list outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data.
     """
 
-    def __init__(self, data=None, ui_buttons=True, ui_button_pos='right',
-                 extended_selection=False, show_index=False, drag_drop=False,
-                 parent=None, title=None, model=None, verbose=False):
-
+    def __init__(
+        self,
+        data=None,
+        ui_buttons=True,
+        ui_button_pos="right",
+        extended_selection=False,
+        show_index=False,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        model=None,
+        verbose=False,
+    ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         if model is None:
-            model = EditListModel(data, show_index=show_index,
-                                  drag_drop=drag_drop)
+            model = EditListModel(data, show_index=show_index, drag_drop=drag_drop)
 
-        super().__init__(model=model, view=QListView(),
-                         extended_selection=extended_selection,
-                         drag_drop=drag_drop, parent=parent,
-                         title=title, verbose=verbose)
+        super().__init__(
+            model=model,
+            view=QListView(),
+            extended_selection=extended_selection,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
 
     def init_ui(self):
-        if self.ui_button_pos in ['top', 'bottom']:
+        if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
             layout = QHBoxLayout()
             bt_layout = QVBoxLayout()
 
         if self.ui_buttons:
-            addrow_bt = QPushButton('Add')
+            addrow_bt = QPushButton("Add")
             addrow_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             addrow_bt.clicked.connect(self.add_row)
             bt_layout.addWidget(addrow_bt)
 
-            rmrow_bt = QPushButton('Remove')
+            rmrow_bt = QPushButton("Remove")
             rmrow_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             rmrow_bt.clicked.connect(self.remove_row)
             bt_layout.addWidget(rmrow_bt)
 
-            edit_bt = QPushButton('Edit')
+            edit_bt = QPushButton("Edit")
             edit_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             edit_bt.clicked.connect(self.edit_item)
             bt_layout.addWidget(edit_bt)
 
             layout.addLayout(bt_layout)
 
-        if self.ui_button_pos in ['top', 'left']:
+        if self.ui_button_pos in ["top", "left"]:
             layout.addWidget(self.view)
         else:
             layout.insertWidget(0, self.view)
 
         if self.title:
             super_layout = QVBoxLayout()
             title_label = QLabel(self.title)
-            title_label.setFont(QFont(QS().value('app_font'), 14))
+            title_label.setFont(QFont(QS().value("app_font"), 14))
             super_layout.addWidget(title_label)
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     # Todo: Add Rows at all possible positions
@@ -326,81 +368,91 @@
     If you change the contents of data outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data or replace_checked.
     """
 
     checkedChanged = pyqtSignal(list)
 
-    def __init__(self, data=None, checked=None, ui_buttons=True,
-                 ui_button_pos='right', one_check=False, show_index=False,
-                 drag_drop=False, parent=None, title=None, verbose=False):
-
+    def __init__(
+        self,
+        data=None,
+        checked=None,
+        ui_buttons=True,
+        ui_button_pos="right",
+        one_check=False,
+        show_index=False,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        verbose=False,
+    ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         super().__init__(
-            model=CheckListModel(data, checked, one_check, show_index,
-                                 drag_drop),
-            view=QListView(), extended_selection=False, drag_drop=drag_drop,
-            parent=parent, title=title, verbose=verbose)
+            model=CheckListModel(data, checked, one_check, show_index, drag_drop),
+            view=QListView(),
+            extended_selection=False,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
 
         self.model.dataChanged.connect(self._checked_changed)
 
     def init_ui(self):
-
-        if self.ui_button_pos in ['top', 'bottom']:
+        if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
             layout = QHBoxLayout()
             bt_layout = QVBoxLayout()
 
         if self.ui_buttons:
-            all_bt = QPushButton('All')
+            all_bt = QPushButton("All")
             all_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             all_bt.clicked.connect(self.select_all)
             bt_layout.addWidget(all_bt)
 
-            clear_bt = QPushButton('Clear')
+            clear_bt = QPushButton("Clear")
             clear_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             clear_bt.clicked.connect(self.clear_all)
             bt_layout.addWidget(clear_bt)
 
             layout.addLayout(bt_layout)
 
-        if self.ui_button_pos in ['top', 'left']:
+        if self.ui_button_pos in ["top", "left"]:
             layout.addWidget(self.view)
         else:
             layout.insertWidget(0, self.view)
 
         if self.title:
             super_layout = QVBoxLayout()
             title_label = QLabel(self.title)
-            title_label.setFont(QFont(QS().value('app_font'), 14))
+            title_label.setFont(QFont(QS().value("app_font"), 14))
             super_layout.addWidget(title_label)
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     def _checked_changed(self):
         self.checkedChanged.emit(self.model._checked)
         if self.verbose:
-            print(f'Changed values: {self.model._checked}')
+            print(f"Changed values: {self.model._checked}")
 
     def replace_checked(self, new_checked):
-        """Replaces model._checked with new check_dict
-        """
+        """Replaces model._checked with new check_dict"""
         self.model._checked = new_checked
         self.content_changed()
 
     def select_all(self):
         """Select all Items while leaving reference to model._checked intact"""
-        for item in [i for i in self.model._data if
-                     i not in self.model._checked]:
+        for item in [i for i in self.model._data if i not in self.model._checked]:
             self.model._checked.append(item)
         # Inform Model about changes
         self.content_changed()
         self._checked_changed()
 
     def clear_all(self):
         """Deselect all Items while leaving reference
@@ -445,27 +497,41 @@
     If you change the reference to data, call replace_data.
     If you change the reference to check_dict, call replace_check_dict.
 
     Names for QT standard-icons:
     https://doc.qt.io/qt-5/qstyle.html#StandardPixmap-enum
     """
 
-    def __init__(self, data=None, check_dict=None, extended_selection=False,
-                 show_index=False, drag_drop=False, yes_bt=None, no_bt=None,
-                 parent=None, title=None, verbose=False):
+    def __init__(
+        self,
+        data=None,
+        check_dict=None,
+        extended_selection=False,
+        show_index=False,
+        drag_drop=False,
+        yes_bt=None,
+        no_bt=None,
+        parent=None,
+        title=None,
+        verbose=False,
+    ):
         super().__init__(
-            model=CheckDictModel(data, check_dict, show_index, drag_drop,
-                                 yes_bt, no_bt),
+            model=CheckDictModel(
+                data, check_dict, show_index, drag_drop, yes_bt, no_bt
+            ),
             view=QListView(),
-            extended_selection=extended_selection, drag_drop=drag_drop,
-            parent=parent, title=title, verbose=verbose)
+            extended_selection=extended_selection,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
 
     def replace_check_dict(self, new_check_dict=None):
-        """Replaces model.check_dict with new check_dict
-        """
+        """Replaces model.check_dict with new check_dict"""
         if new_check_dict:
             self.model._check_dict = new_check_dict
         self.content_changed()
 
 
 class CheckDictEditList(EditList):
     """A List-Widget to display the items of a list and mark them
@@ -506,45 +572,65 @@
     If you change the reference to data, call replace_data.
     If you change the reference to check_dict, call replace_check_dict.
 
     Names for QT standard-icons:
     https://doc.qt.io/qt-5/qstyle.html#StandardPixmap-enum
     """
 
-    def __init__(self, data=None, check_dict=None, ui_buttons=True,
-                 ui_button_pos='right',
-                 extended_selection=False,
-                 show_index=False, yes_bt=None, no_bt=None, drag_drop=False,
-                 parent=None,
-                 title=None, verbose=False):
-        model = CheckDictEditModel(data, check_dict, show_index=show_index,
-                                   yes_bt=yes_bt,
-                                   no_bt=no_bt)
-        super().__init__(data=data, ui_buttons=ui_buttons,
-                         ui_button_pos=ui_button_pos,
-                         extended_selection=extended_selection,
-                         show_index=show_index,
-                         drag_drop=drag_drop,
-                         parent=parent, title=title, verbose=verbose,
-                         model=model)
+    def __init__(
+        self,
+        data=None,
+        check_dict=None,
+        ui_buttons=True,
+        ui_button_pos="right",
+        extended_selection=False,
+        show_index=False,
+        yes_bt=None,
+        no_bt=None,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        verbose=False,
+    ):
+        model = CheckDictEditModel(
+            data, check_dict, show_index=show_index, yes_bt=yes_bt, no_bt=no_bt
+        )
+        super().__init__(
+            data=data,
+            ui_buttons=ui_buttons,
+            ui_button_pos=ui_button_pos,
+            extended_selection=extended_selection,
+            show_index=show_index,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+            model=model,
+        )
 
     def replace_check_dict(self, new_check_dict=None):
-        """Replaces model.check_dict with new check_dict
-        """
+        """Replaces model.check_dict with new check_dict"""
         if new_check_dict:
             self.model._check_dict = new_check_dict
         self.content_changed()
 
 
 class BaseDict(Base):
-
-    def __init__(self, model, view, drag_drop=False, parent=None, title=None,
-                 resize_rows=False, resize_columns=False, verbose=False):
-        super().__init__(model, view, drag_drop, parent, title,
-                         verbose=verbose)
+    def __init__(
+        self,
+        model,
+        view,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
+        super().__init__(model, view, drag_drop, parent, title, verbose=verbose)
         self.verbose = verbose
 
         if resize_rows:
             model.layoutChanged.connect(self.view.resizeRowsToContents)
             model.layoutChanged.emit()
         if resize_columns:
             model.layoutChanged.connect(self.view.resizeColumnsToContents)
@@ -572,22 +658,21 @@
 
         return key, value
 
     def get_current(self):
         return self.get_keyvalue_by_index(self.view.currentIndex())
 
     def _current_changed(self, current_idx, previous_idx):
-
         current_data = self.get_keyvalue_by_index(current_idx)
         previous_data = self.get_keyvalue_by_index(previous_idx)
 
         self.currentChanged.emit(current_data, previous_data)
 
         if self.verbose:
-            print(f'Current changed from {current_data} to {previous_data}')
+            print(f"Current changed from {current_data} to {previous_data}")
 
     def _selected_keyvalue(self, indexes):
         try:
             return set([self.get_keyvalue_by_index(idx) for idx in indexes])
         except TypeError:
             return [self.get_keyvalue_by_index(idx) for idx in indexes]
 
@@ -596,34 +681,32 @@
 
     def _selection_changed(self):
         selected_data = self.get_selected()
 
         self.selectionChanged.emit(selected_data)
 
         if self.verbose:
-            print(f'Selection to {selected_data}')
+            print(f"Selection to {selected_data}")
 
     def select(self, keys, values, clear_selection=True):
-        key_indices = [i for i, x in enumerate(self.model._data.keys()) if
-                       x in keys]
-        value_indices = [i for i, x in enumerate(self.model._data.values()) if
-                         x in values]
+        key_indices = [i for i, x in enumerate(self.model._data.keys()) if x in keys]
+        value_indices = [
+            i for i, x in enumerate(self.model._data.values()) if x in values
+        ]
 
         if clear_selection:
             self.view.selectionModel().clearSelection()
 
         for idx in key_indices:
             index = self.model.createIndex(idx, 0)
-            self.view.selectionModel().select(index,
-                                              QItemSelectionModel.Select)
+            self.view.selectionModel().select(index, QItemSelectionModel.Select)
 
         for idx in value_indices:
             index = self.model.createIndex(idx, 1)
-            self.view.selectionModel().select(index,
-                                              QItemSelectionModel.Select)
+            self.view.selectionModel().select(index, QItemSelectionModel.Select)
 
 
 class SimpleDict(BaseDict):
     """A Widget to display a Dictionary
 
     Parameters
     ----------
@@ -640,23 +723,34 @@
     resize_columns : bool
         Set True to resize the columns to contents.
     verbose : bool
         Set True to see debugging for signals.
 
     """
 
-    def __init__(self, data=None, drag_drop=False, parent=None, title=None,
-                 resize_rows=False,
-                 resize_columns=False, verbose=False):
-        super().__init__(model=BaseDictModel(data), view=QTableView(),
-                         drag_drop=drag_drop,
-                         parent=parent,
-                         title=title, resize_rows=resize_rows,
-                         resize_columns=resize_columns,
-                         verbose=verbose)
+    def __init__(
+        self,
+        data=None,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
+        super().__init__(
+            model=BaseDictModel(data),
+            view=QTableView(),
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            resize_rows=resize_rows,
+            resize_columns=resize_columns,
+            verbose=verbose,
+        )
 
 
 class EditDict(BaseDict):
     """A Widget to display and edit a Dictionary
 
     Parameters
     ----------
@@ -678,78 +772,91 @@
     resize_columns : bool
         Set True to resize the columns to contents.
     verbose : bool
         Set True to see debugging for signals.
 
     """
 
-    def __init__(self, data=None, ui_buttons=True, ui_button_pos='right',
-                 drag_drop=False,
-                 parent=None, title=None,
-                 resize_rows=False, resize_columns=False, verbose=False):
-
+    def __init__(
+        self,
+        data=None,
+        ui_buttons=True,
+        ui_button_pos="right",
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
-        super().__init__(model=EditDictModel(data), view=QTableView(),
-                         drag_drop=drag_drop,
-                         parent=parent, title=title,
-                         resize_rows=resize_rows,
-                         resize_columns=resize_columns, verbose=verbose)
+        super().__init__(
+            model=EditDictModel(data),
+            view=QTableView(),
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            resize_rows=resize_rows,
+            resize_columns=resize_columns,
+            verbose=verbose,
+        )
 
     def init_ui(self):
-        if self.ui_button_pos in ['top', 'bottom']:
+        if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
             layout = QHBoxLayout()
             bt_layout = QVBoxLayout()
 
         if self.ui_buttons:
-            addrow_bt = QPushButton('Add')
+            addrow_bt = QPushButton("Add")
             addrow_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             addrow_bt.clicked.connect(self.add_row)
             bt_layout.addWidget(addrow_bt)
 
-            rmrow_bt = QPushButton('Remove')
+            rmrow_bt = QPushButton("Remove")
             rmrow_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             rmrow_bt.clicked.connect(self.remove_row)
             bt_layout.addWidget(rmrow_bt)
 
-            edit_bt = QPushButton('Edit')
+            edit_bt = QPushButton("Edit")
             edit_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             edit_bt.clicked.connect(self.edit_item)
             bt_layout.addWidget(edit_bt)
 
             layout.addLayout(bt_layout)
 
-        if self.ui_button_pos in ['top', 'left']:
+        if self.ui_button_pos in ["top", "left"]:
             layout.addWidget(self.view)
         else:
             layout.insertWidget(0, self.view)
 
         if self.title:
             super_layout = QVBoxLayout()
             title_label = QLabel(self.title)
-            title_label.setFont(QFont(QS().value('app_font'), 14))
+            title_label.setFont(QFont(QS().value("app_font"), 14))
             super_layout.addWidget(title_label)
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     def add_row(self):
         row = self.view.selectionModel().currentIndex().row() + 1
         if row == -1:
             row = 0
         self.model.insertRow(row)
 
     def remove_row(self):
-        row_idxs = set([idx.row() for idx in
-                        self.view.selectionModel().selectedIndexes()])
+        row_idxs = set(
+            [idx.row() for idx in self.view.selectionModel().selectedIndexes()]
+        )
         for row_idx in row_idxs:
             self.model.removeRow(row_idx)
 
     def edit_item(self):
         self.view.edit(self.view.selectionModel().currentIndex())
 
 
@@ -765,19 +872,33 @@
         The view for the pandas DataFrame.
     title : str | None
         An optional title.
     verbose : bool
         Set True to see debugging for signals.
     """
 
-    def __init__(self, model, view, drag_drop=False, parent=None, title=None,
-                 resize_rows=False, resize_columns=False, verbose=False):
-        super().__init__(model=model, view=view, drag_drop=drag_drop,
-                         parent=parent, title=title,
-                         verbose=verbose)
+    def __init__(
+        self,
+        model,
+        view,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
+        super().__init__(
+            model=model,
+            view=view,
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
         self.verbose = verbose
 
         if resize_rows:
             model.layoutChanged.connect(self.view.resizeRowsToContents)
             model.layoutChanged.emit()
         if resize_columns:
             model.layoutChanged.connect(self.view.resizeColumnsToContents)
@@ -796,19 +917,20 @@
         Notes
         -----
         Because this function is supposed to be called consecutively,
         the information is stored in an existing list (data_list)
 
         """
         data = self.model.getData(index)
-        row = self.model.headerData(index.row(), orientation=Qt.Vertical,
-                                    role=Qt.DisplayRole)
-        column = self.model.headerData(index.column(),
-                                       orientation=Qt.Horizontal,
-                                       role=Qt.DisplayRole)
+        row = self.model.headerData(
+            index.row(), orientation=Qt.Vertical, role=Qt.DisplayRole
+        )
+        column = self.model.headerData(
+            index.column(), orientation=Qt.Horizontal, role=Qt.DisplayRole
+        )
 
         data_list.append((data, row, column))
 
     def get_current(self):
         current_list = list()
         self.get_rowcol_by_index(self.view.currentIndex(), current_list)
 
@@ -820,15 +942,15 @@
 
         self.get_rowcol_by_index(current_idx, current_list)
         self.get_rowcol_by_index(previous_idx, previous_list)
 
         self.currentChanged.emit(current_list, previous_list)
 
         if self.verbose:
-            print(f'Current changed from {previous_list} to {current_list}')
+            print(f"Current changed from {previous_list} to {current_list}")
 
     def get_selected(self):
         # Somehow, the indexes got from selectionChanged
         # don't appear to be right (maybe some issue with QItemSelection?).
         selection_list = list()
         for idx in self.view.selectedIndexes():
             self.get_rowcol_by_index(idx, selection_list)
@@ -836,18 +958,17 @@
         return selection_list
 
     def _selection_changed(self):
         selection_list = self.get_selected()
         self.selectionChanged.emit(selection_list)
 
         if self.verbose:
-            print(f'Selection changed to {selection_list}')
+            print(f"Selection changed to {selection_list}")
 
-    def select(self, values=None, rows=None, columns=None,
-               clear_selection=True):
+    def select(self, values=None, rows=None, columns=None, clear_selection=True):
         """
         Select items in Pandas DataFrame by value
         or select complete rows/columns.
 
         Parameters
         ----------
         values: list | None
@@ -868,39 +989,35 @@
                 row, column = np.nonzero((self.model._data == value).values)
                 for idx in zip(row, column):
                     indexes.append(idx)
 
         # Select complete rows
         if rows:
             # Convert names into indexes
-            row_idxs = [list(self.model._data.index).index(row) for row in
-                        rows]
+            row_idxs = [list(self.model._data.index).index(row) for row in rows]
             n_cols = len(self.model._data.columns)
             for row in row_idxs:
                 for idx in zip(itertools.repeat(row, n_cols), range(n_cols)):
                     indexes.append(idx)
 
         # Select complete columns
         if columns:
             # Convert names into indexes
-            column_idxs = [list(self.model._data.columns).index(col) for col in
-                           columns]
+            column_idxs = [list(self.model._data.columns).index(col) for col in columns]
             n_rows = len(self.model._data.index)
             for column in column_idxs:
-                for idx in zip(range(n_rows),
-                               itertools.repeat(column, n_rows)):
+                for idx in zip(range(n_rows), itertools.repeat(column, n_rows)):
                     indexes.append(idx)
 
         if clear_selection:
             self.view.selectionModel().clearSelection()
 
         for row, column in indexes:
             index = self.model.createIndex(row, column)
-            self.view.selectionModel().select(index,
-                                              QItemSelectionModel.Select)
+            self.view.selectionModel().select(index, QItemSelectionModel.Select)
 
 
 class SimplePandasTable(BasePandasTable):
     """A Widget to display a pandas DataFrame
 
     Parameters
     ----------
@@ -921,20 +1038,34 @@
 
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
-    def __init__(self, data=None, drag_drop=False, parent=None, title=None,
-                 resize_rows=False, resize_columns=False, verbose=False):
-        super().__init__(model=BasePandasModel(data), view=QTableView(),
-                         drag_drop=drag_drop, parent=parent, title=title,
-                         resize_rows=resize_rows,
-                         resize_columns=resize_columns, verbose=verbose)
+    def __init__(
+        self,
+        data=None,
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
+        super().__init__(
+            model=BasePandasModel(data),
+            view=QTableView(),
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            resize_rows=resize_rows,
+            resize_columns=resize_columns,
+            verbose=verbose,
+        )
 
 
 class EditPandasTable(BasePandasTable):
     """A Widget to display and edit a pandas DataFrame
 
     Parameters
     ----------
@@ -960,94 +1091,105 @@
 
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
-    def __init__(self, data=None, ui_buttons=True, ui_button_pos='right',
-                 drag_drop=False,
-                 parent=None, title=None, resize_rows=False,
-                 resize_columns=False, verbose=False):
-
+    def __init__(
+        self,
+        data=None,
+        ui_buttons=True,
+        ui_button_pos="right",
+        drag_drop=False,
+        parent=None,
+        title=None,
+        resize_rows=False,
+        resize_columns=False,
+        verbose=False,
+    ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
-        super().__init__(model=EditPandasModel(data), view=QTableView(),
-                         drag_drop=drag_drop,
-                         parent=parent,
-                         title=title, resize_rows=resize_rows,
-                         resize_columns=resize_columns,
-                         verbose=verbose)
+        super().__init__(
+            model=EditPandasModel(data),
+            view=QTableView(),
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            resize_rows=resize_rows,
+            resize_columns=resize_columns,
+            verbose=verbose,
+        )
 
     def init_ui(self):
-        if self.ui_button_pos in ['top', 'bottom']:
+        if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
             layout = QHBoxLayout()
             bt_layout = QVBoxLayout()
 
         if self.ui_buttons:
             addr_layout = QHBoxLayout()
-            addr_bt = QPushButton('Add Row')
+            addr_bt = QPushButton("Add Row")
             addr_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             addr_bt.clicked.connect(self.add_row)
             addr_layout.addWidget(addr_bt)
             self.rows_chkbx = QSpinBox()
             self.rows_chkbx.setMinimum(1)
             addr_layout.addWidget(self.rows_chkbx)
             bt_layout.addLayout(addr_layout)
 
             addc_layout = QHBoxLayout()
-            addc_bt = QPushButton('Add Column')
+            addc_bt = QPushButton("Add Column")
             addc_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             addc_bt.clicked.connect(self.add_column)
             addc_layout.addWidget(addc_bt)
             self.cols_chkbx = QSpinBox()
             self.cols_chkbx.setMinimum(1)
             addc_layout.addWidget(self.cols_chkbx)
             bt_layout.addLayout(addc_layout)
 
-            rmr_bt = QPushButton('Remove Row')
+            rmr_bt = QPushButton("Remove Row")
             rmr_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             rmr_bt.clicked.connect(self.remove_row)
             bt_layout.addWidget(rmr_bt)
 
-            rmc_bt = QPushButton('Remove Column')
+            rmc_bt = QPushButton("Remove Column")
             rmc_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             rmc_bt.clicked.connect(self.remove_column)
             bt_layout.addWidget(rmc_bt)
 
-            edit_bt = QPushButton('Edit')
+            edit_bt = QPushButton("Edit")
             edit_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             edit_bt.clicked.connect(self.edit_item)
             bt_layout.addWidget(edit_bt)
 
-            editrh_bt = QPushButton('Edit Row-Header')
+            editrh_bt = QPushButton("Edit Row-Header")
             editrh_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             editrh_bt.clicked.connect(self.edit_row_header)
             bt_layout.addWidget(editrh_bt)
 
-            editch_bt = QPushButton('Edit Column-Header')
+            editch_bt = QPushButton("Edit Column-Header")
             editch_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             editch_bt.clicked.connect(self.edit_col_header)
             bt_layout.addWidget(editch_bt)
 
             layout.addLayout(bt_layout)
 
-        if self.ui_button_pos in ['top', 'left']:
+        if self.ui_button_pos in ["top", "left"]:
             layout.addWidget(self.view)
         else:
             layout.insertWidget(0, self.view)
 
         if self.title:
             super_layout = QVBoxLayout()
             title_label = QLabel(self.title)
-            title_label.setFont(QFont(QS().value('app_font'), 14))
+            title_label.setFont(QFont(QS().value("app_font"), 14))
             super_layout.addWidget(title_label)
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     def update_data(self):
@@ -1075,53 +1217,55 @@
             row = 0
         self.model.insertRows(row, self.rows_chkbx.value())
         self.update_data()
 
     def add_column(self):
         column = self.view.selectionModel().currentIndex().column() + 1
         # Add column to the right if nothing is selected
-        if column == -1 or len(
-                self.view.selectionModel().selectedIndexes()) == 0:
+        if column == -1 or len(self.view.selectionModel().selectedIndexes()) == 0:
             column = 0
         self.model.insertColumns(column, self.cols_chkbx.value())
         self.update_data()
 
     def remove_row(self):
-        rows = sorted(set([ix.row() for ix in
-                           self.view.selectionModel().selectedIndexes()]),
-                      reverse=True)
+        rows = sorted(
+            set([ix.row() for ix in self.view.selectionModel().selectedIndexes()]),
+            reverse=True,
+        )
         for row in rows:
             self.model.removeRow(row)
         self.update_data()
 
     def remove_column(self):
-        columns = sorted(set([ix.column() for ix in
-                              self.view.selectionModel().selectedIndexes()]),
-                         reverse=True)
+        columns = sorted(
+            set([ix.column() for ix in self.view.selectionModel().selectedIndexes()]),
+            reverse=True,
+        )
         for column in columns:
             self.model.removeColumn(column)
         self.update_data()
 
     def edit_item(self):
         self.view.edit(self.view.selectionModel().currentIndex())
 
     def edit_row_header(self):
         row = self.view.selectionModel().currentIndex().row()
         old_value = self.model._data.index[row]
-        text = get_user_input_string(f'Change {old_value} in row {row} to:',
-                                     'Change Row-Header')
+        text = get_user_input_string(
+            f"Change {old_value} in row {row} to:", "Change Row-Header"
+        )
         if text is not None:
             self.model.setHeaderData(row, Qt.Vertical, text)
 
     def edit_col_header(self):
         column = self.view.selectionModel().currentIndex().column()
         old_value = self.model._data.columns[column]
         text = get_user_input_string(
-            f'Change {old_value} in column {column} to:',
-            'Change Column-Header')
+            f"Change {old_value} in column {column} to:", "Change Column-Header"
+        )
         if text is not None:
             self.model.setHeaderData(column, Qt.Horizontal, text)
 
 
 class FilePandasTable(BasePandasTable):
     """A Widget to display the files in a table (stored in a pandas DataFrame)
 
@@ -1139,37 +1283,61 @@
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
     def __init__(self, data=None, parent=None, title=None, verbose=False):
-        super().__init__(model=FileManagementModel(data), view=QTableView(),
-                         parent=parent,
-                         title=title,
-                         resize_rows=True, resize_columns=True,
-                         verbose=verbose)
+        super().__init__(
+            model=FileManagementModel(data),
+            view=QTableView(),
+            parent=parent,
+            title=title,
+            resize_rows=True,
+            resize_columns=True,
+            verbose=verbose,
+        )
 
 
 class DictTree(Base):
-    def __init__(self, data, drag_drop=False, parent=None, title=None,
-                 verbose=False):
-        super().__init__(model=TreeModel(data), view=QTreeView(),
-                         drag_drop=drag_drop,
-                         parent=parent,
-                         title=title, verbose=verbose)
+    def __init__(self, data, drag_drop=False, parent=None, title=None, verbose=False):
+        super().__init__(
+            model=TreeModel(data),
+            view=QTreeView(),
+            drag_drop=drag_drop,
+            parent=parent,
+            title=title,
+            verbose=verbose,
+        )
+
+
+class ComboBox(QComboBox):
+    def __init__(self, scrollable=False, **kwargs):
+        self.scrollable = scrollable
+        super().__init__(**kwargs)
+
+    def wheelEvent(self, event):
+        if self.scrollable:
+            super().wheelEvent(event)
 
 
 class SimpleDialog(QDialog):
-    def __init__(self, widget, parent=None, modal=True, scroll=False,
-                 title=None, window_title=None,
-                 show_close_bt=True):
+    def __init__(
+        self,
+        widget,
+        parent=None,
+        modal=True,
+        scroll=False,
+        title=None,
+        window_title=None,
+        show_close_bt=True,
+    ):
         super().__init__(parent)
 
-        _object_refs['dialogs'][self.__class__.__name__] = self
+        _object_refs["dialogs"][self.__class__.__name__] = self
 
         layout = QVBoxLayout()
 
         if title:
             layout.addWidget(QLabel(title))
 
         if window_title:
@@ -1179,38 +1347,44 @@
             scroll_area = QScrollArea()
             scroll_area.setWidget(widget)
             layout.addWidget(scroll_area)
         else:
             layout.addWidget(widget)
 
         if show_close_bt:
-            close_bt = QPushButton('Close')
+            close_bt = QPushButton("Close")
             close_bt.clicked.connect(self.close)
             layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
         if modal:
             self.open()
         else:
             self.show()
 
     def closeEvent(self, event):
         event.accept()
-        _object_refs['dialogs'].pop(self.__class__.__name__)
+        _object_refs["dialogs"].pop(self.__class__.__name__)
 
 
 class AssignWidget(QWidget):
-    """
-
-    """
+    """ """
 
-    def __init__(self, items, properties, assignments,
-                 properties_editable=False,
-                 parent=None, title=None, subtitles=None, verbose=False):
+    def __init__(
+        self,
+        items,
+        properties,
+        assignments,
+        properties_editable=False,
+        parent=None,
+        title=None,
+        subtitles=None,
+        verbose=False,
+    ):
         super().__init__(parent)
         self.title = title
         self.subtitles = subtitles
         self.verbose = verbose
 
         self.items = items
         self.props = properties
@@ -1224,60 +1398,70 @@
 
         list_layout = QHBoxLayout()
         if self.subtitles is not None and len(self.subtitles) == 2:
             subtitle1, subtitle2 = self.subtitles
         else:
             subtitle1, subtitle2 = None, None
 
-        self.items_w = CheckDictList(self.items, self.assignments,
-                                     extended_selection=True,
-                                     title=subtitle1,
-                                     verbose=self.verbose)
+        self.items_w = CheckDictList(
+            self.items,
+            self.assignments,
+            extended_selection=True,
+            title=subtitle1,
+            verbose=self.verbose,
+        )
         self.items_w.selectionChanged.connect(self.items_selected)
         list_layout.addWidget(self.items_w)
 
         if self.props_editable:
-            self.props_w = EditList(self.props, extended_selection=False,
-                                    title=subtitle2,
-                                    verbose=self.verbose)
+            self.props_w = EditList(
+                self.props,
+                extended_selection=False,
+                title=subtitle2,
+                verbose=self.verbose,
+            )
         else:
-            self.props_w = SimpleList(self.props, extended_selection=False,
-                                      title=subtitle2,
-                                      verbose=self.verbose)
+            self.props_w = SimpleList(
+                self.props,
+                extended_selection=False,
+                title=subtitle2,
+                verbose=self.verbose,
+            )
         list_layout.addWidget(self.props_w)
         layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
-        assign_bt = QPushButton('Assign')
+        assign_bt = QPushButton("Assign")
         assign_bt.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-        assign_bt.setFont(QFont(QS().value('app_font'), 13))
+        assign_bt.setFont(QFont(QS().value("app_font"), 13))
         assign_bt.clicked.connect(self.assign)
         bt_layout.addWidget(assign_bt)
 
-        show_assign_bt = QPushButton('Show Assignments')
+        show_assign_bt = QPushButton("Show Assignments")
         show_assign_bt.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
-        show_assign_bt.setFont(QFont(QS().value('app_font'), 13))
+        show_assign_bt.setFont(QFont(QS().value("app_font"), 13))
         show_assign_bt.clicked.connect(self.show_assignments)
         bt_layout.addWidget(show_assign_bt)
         layout.addLayout(bt_layout)
 
         if self.title:
             super_layout = QVBoxLayout()
             title_label = QLabel(self.title)
-            title_label.setFont(QFont(QS().value('app_font'), 14))
+            title_label.setFont(QFont(QS().value("app_font"), 14))
             super_layout.addWidget(title_label, alignment=Qt.AlignHCenter)
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     def items_selected(self, selected):
         # Get all unique values of selected items
-        values = set([self.assignments[key] for key in selected if
-                      key in self.assignments])
+        values = set(
+            [self.assignments[key] for key in selected if key in self.assignments]
+        )
         self.props_w.select(values)
 
     def assign(self):
         sel_items = self.items_w.get_selected()
         sel_prop = self.props_w.get_current()
 
         for item in sel_items:
@@ -1290,97 +1474,110 @@
         SimpleDialog(EditDict(self.assignments), parent=self, modal=False)
 
 
 class AllBaseWidgets(QWidget):
     def __init__(self):
         super().__init__()
 
-        self.exlist = ['Athena', 'Hephaistos', 'Zeus', 'Ares', 'Aphrodite',
-                       'Poseidon']
-        self.exattributes = ['strong', 'smart', 'bossy', 'fishy']
-        self.exassignments = {'Athena': 'smart',
-                              'Hephaistos': 'strong',
-                              'Zeus': 'bossy',
-                              'Poseidon': 'fishy'}
-        self.exdict = {'Athena': 231,
-                       'Hephaistos': ['44', '333', 34],
-                       'Zeus': 'Boss',
-                       'Ares': self.exassignments}
-        self.exchecked = ['Athena']
+        self.exlist = ["Athena", "Hephaistos", "Zeus", "Ares", "Aphrodite", "Poseidon"]
+        self.exattributes = ["strong", "smart", "bossy", "fishy"]
+        self.exassignments = {
+            "Athena": "smart",
+            "Hephaistos": "strong",
+            "Zeus": "bossy",
+            "Poseidon": "fishy",
+        }
+        self.exdict = {
+            "Athena": 231,
+            "Hephaistos": ["44", "333", 34],
+            "Zeus": "Boss",
+            "Ares": self.exassignments,
+        }
+        self.exchecked = ["Athena"]
         self.expd = pandas.DataFrame(
-            [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]],
-            columns=['A', 'B', 'C', 'D'])
-        self.extree = {'A': {'Aa': 2,
-                             'Ab': {'Ab1': 'Hermes',
-                                    'Ab2': 'Hades'},
-                             'Ac': [1, 2, 3, 4]},
-                       'B': ['Appolo', 42, 128],
-                       'C': (1, 2, 3)}
+            [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]], columns=["A", "B", "C", "D"]
+        )
+        self.extree = {
+            "A": {"Aa": 2, "Ab": {"Ab1": "Hermes", "Ab2": "Hades"}, "Ac": [1, 2, 3, 4]},
+            "B": ["Appolo", 42, 128],
+            "C": (1, 2, 3),
+        }
 
         # self.exlist = None
         # self.exattributes = None
         # self.exchecked = None
         # self.expd = None
         # self.extree = None
         # self.exdict = None
 
-        self.widget_args = {'SimpleList': [self.exlist],
-                            'EditList': [self.exlist],
-                            'CheckList': [self.exlist, self.exchecked],
-                            'CheckDictList': [self.exlist, self.exdict],
-                            'CheckDictEditList': [self.exlist, self.exdict],
-                            'SimpleDict': [self.exdict],
-                            'EditDict': [self.exdict],
-                            'SimplePandasTable': [self.expd],
-                            'EditPandasTable': [self.expd],
-                            'DictTree': [self.extree],
-                            'AssignWidget': [self.exlist, self.exattributes,
-                                             self.exassignments]}
+        self.widget_args = {
+            "SimpleList": [self.exlist],
+            "EditList": [self.exlist],
+            "CheckList": [self.exlist, self.exchecked],
+            "CheckDictList": [self.exlist, self.exdict],
+            "CheckDictEditList": [self.exlist, self.exdict],
+            "SimpleDict": [self.exdict],
+            "EditDict": [self.exdict],
+            "SimplePandasTable": [self.expd],
+            "EditPandasTable": [self.expd],
+            "DictTree": [self.extree],
+            "AssignWidget": [self.exlist, self.exattributes, self.exassignments],
+        }
 
         self.widget_kwargs = {
-            'SimpleList': {'extended_selection': True, 'title': 'BaseList',
-                           'verbose': True},
-            'EditList': {'ui_button_pos': 'bottom', 'extended_selection': True,
-                         'title': 'EditList',
-                         'verbose': True},
-            'CheckList': {'one_check': False, 'title': 'CheckList',
-                          'verbose': True},
-            'CheckDictList': {'extended_selection': True,
-                              'title': 'CheckDictList',
-                              'verbose': True},
-            'CheckDictEditList': {'title': 'CheckDictEditList',
-                                  'verbose': True},
-            'SimpleDict': {'title': 'BaseDict', 'verbose': True},
-            'EditDict': {'ui_button_pos': 'left', 'title': 'EditDict',
-                         'verbose': True},
-            'SimplePandasTable': {'title': 'BasePandasTable', 'verbose': True},
-            'EditPandasTable': {'title': 'EditPandasTable', 'verbose': True},
-            'DictTree': {'title': 'BaseDictTree', 'verbose': True},
-            'AssignWidget': {'properties_editable': True,
-                             'title': 'AssignWidget', 'verbose': True}}
+            "SimpleList": {
+                "extended_selection": True,
+                "title": "BaseList",
+                "verbose": True,
+            },
+            "EditList": {
+                "ui_button_pos": "bottom",
+                "extended_selection": True,
+                "title": "EditList",
+                "verbose": True,
+            },
+            "CheckList": {"one_check": False, "title": "CheckList", "verbose": True},
+            "CheckDictList": {
+                "extended_selection": True,
+                "title": "CheckDictList",
+                "verbose": True,
+            },
+            "CheckDictEditList": {"title": "CheckDictEditList", "verbose": True},
+            "SimpleDict": {"title": "BaseDict", "verbose": True},
+            "EditDict": {"ui_button_pos": "left", "title": "EditDict", "verbose": True},
+            "SimplePandasTable": {"title": "BasePandasTable", "verbose": True},
+            "EditPandasTable": {"title": "EditPandasTable", "verbose": True},
+            "DictTree": {"title": "BaseDictTree", "verbose": True},
+            "AssignWidget": {
+                "properties_editable": True,
+                "title": "AssignWidget",
+                "verbose": True,
+            },
+        }
 
         self.tab_widget = QTabWidget()
 
         self.init_ui()
 
         self.setGeometry(0, 0, 800, 400)
 
     def init_ui(self):
         layout = QVBoxLayout()
         for widget_name in self.widget_args:
-            widget = globals()[widget_name](*self.widget_args[widget_name],
-                                            **self.widget_kwargs[widget_name])
+            widget = globals()[widget_name](
+                *self.widget_args[widget_name], **self.widget_kwargs[widget_name]
+            )
             setattr(self, widget_name, widget)
             self.tab_widget.addTab(widget, widget_name)
 
         layout.addWidget(self.tab_widget)
         self.setLayout(layout)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app = QApplication(sys.argv)
     testw = AllBaseWidgets()
     testw.show()
 
     # Command-Line interrupt with Ctrl+C possible, easier debugging
     timer = QTimer()
     timer.timeout.connect(lambda: testw)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/dialogs.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/dialogs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from collections import Counter
 from importlib import resources
 from pathlib import Path
 
 import mne
-from PyQt5.QtWidgets import (QDialog, QGridLayout, QLabel, QListView,
-                             QPushButton,
-                             QSizePolicy, QTextEdit, QVBoxLayout, QWidget,
-                             QComboBox, QMessageBox)
+from PyQt5.QtWidgets import (
+    QDialog,
+    QGridLayout,
+    QLabel,
+    QListView,
+    QPushButton,
+    QSizePolicy,
+    QTextEdit,
+    QVBoxLayout,
+    QWidget,
+    QComboBox,
+    QMessageBox,
+)
 
 from mne_pipeline_hd.gui.base_widgets import SimpleList, SimpleDialog
 from mne_pipeline_hd.gui.gui_utils import set_ratio_geometry
 from mne_pipeline_hd.gui.models import CheckListModel
 from mne_pipeline_hd.pipeline.loading import MEEG
 from mne_pipeline_hd.pipeline.project import Project
 
@@ -49,33 +56,33 @@
         self.layout = QGridLayout()
 
         self.lv = QListView()
         self.lm = CheckListModel(self.data, self.checked)
         self.lv.setModel(self.lm)
         self.layout.addWidget(self.lv, 0, 0, 1, 2)
 
-        self.do_bt = QPushButton('<Do Something>')
+        self.do_bt = QPushButton("<Do Something>")
         self.do_bt.clicked.connect(lambda: None)
         self.layout.addWidget(self.do_bt, 1, 0)
 
-        self.quit_bt = QPushButton('Quit')
+        self.quit_bt = QPushButton("Quit")
         self.quit_bt.clicked.connect(self.close)
         self.layout.addWidget(self.quit_bt, 1, 1)
 
         self.setLayout(self.layout)
 
 
 class RemoveProjectsDlg(CheckListDlg):
     def __init__(self, main_win, controller):
         self.mw = main_win
         self.ct = controller
         self.rm_list = []
         super().__init__(main_win, self.ct.projects, self.rm_list)
 
-        self.do_bt.setText('Remove Projects')
+        self.do_bt.setText("Remove Projects")
         self.do_bt.clicked.connect(self.remove_selected)
 
         self.open()
 
     def remove_selected(self):
         for project in self.rm_list:
             self.ct.remove_project(project)
@@ -89,15 +96,15 @@
     def __init__(self, main_win):
         super().__init__(main_win)
         layout = QVBoxLayout()
         self.show_widget = QTextEdit()
         self.show_widget.setReadOnly(True)
         layout.addWidget(self.show_widget)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         # Set geometry to ratio of screen-geometry
         set_ratio_geometry(0.4, self)
 
         self.setLayout(layout)
@@ -108,29 +115,31 @@
 
 
 class QuickGuide(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         layout = QVBoxLayout()
 
-        text = '<b>Quick-Guide</b><br>' \
-               '1. Use the Subject-Wizard to add Subjects ' \
-               'and the Subject-Dicts<br>' \
-               '2. Select the files you want to execute<br>' \
-               '3. Select the functions to execute<br>' \
-               '4. If you want to show plots, check Show Plots<br>' \
-               '5. For Source-Space-Operations, you need to run ' \
-               'MRI-Coregistration from the Input-Menu<br>' \
-               '6. For Grand-Averages add a group and add the files, ' \
-               'to which you want apply the grand-average'
+        text = (
+            "<b>Quick-Guide</b><br>"
+            "1. Use the Subject-Wizard to add Subjects "
+            "and the Subject-Dicts<br>"
+            "2. Select the files you want to execute<br>"
+            "3. Select the functions to execute<br>"
+            "4. If you want to show plots, check Show Plots<br>"
+            "5. For Source-Space-Operations, you need to run "
+            "MRI-Coregistration from the Input-Menu<br>"
+            "6. For Grand-Averages add a group and add the files, "
+            "to which you want apply the grand-average"
+        )
 
         self.label = QLabel(text)
         layout.addWidget(self.label)
 
-        ok_bt = QPushButton('OK')
+        ok_bt = QPushButton("OK")
         ok_bt.clicked.connect(self.close)
         layout.addWidget(ok_bt)
 
         self.setLayout(layout)
         self.open()
 
 
@@ -150,19 +159,20 @@
         meeg_list = SimpleList(self.mw.ct.pr.all_meeg)
         meeg_list.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
         meeg_list.currentChanged.connect(self.meeg_selected)
         layout.addWidget(meeg_list, 0, 0)
 
         self.info_label = QTextEdit()
         self.info_label.setReadOnly(True)
-        self.info_label.setSizePolicy(QSizePolicy.MinimumExpanding,
-                                      QSizePolicy.MinimumExpanding)
+        self.info_label.setSizePolicy(
+            QSizePolicy.MinimumExpanding, QSizePolicy.MinimumExpanding
+        )
         layout.addWidget(self.info_label, 0, 1)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt, 1, 0, 1, 2)
 
         self.setLayout(layout)
 
     def meeg_selected(self, meeg_name):
         # Get size in Mebibytes of all files associated to this
@@ -172,117 +182,124 @@
         meeg.get_existing_paths()
         other_infos = dict()
 
         sizes = list()
         for path_type in meeg.existing_paths:
             for path in meeg.existing_paths[path_type]:
                 file_name = Path(path).name
-                if file_name in fp and 'SIZE' in fp[file_name]:
-                    sizes.append(fp[file_name]['SIZE'])
-        other_infos['no_files'] = len(sizes)
+                if file_name in fp and "SIZE" in fp[file_name]:
+                    sizes.append(fp[file_name]["SIZE"])
+        other_infos["no_files"] = len(sizes)
 
         sizes_sum = sum(sizes)
         if sizes_sum / 1024 < 1000:
-            other_infos['size'] = f'{int(sizes_sum / 1024)}'
-            size_unit = 'KB'
+            other_infos["size"] = f"{int(sizes_sum / 1024)}"
+            size_unit = "KB"
         else:
-            other_infos['size'] = f'{int(sizes_sum / 1024 ** 2)}'
-            size_unit = 'MB'
+            other_infos["size"] = f"{int(sizes_sum / 1024 ** 2)}"
+            size_unit = "MB"
 
         ch_type_counter = Counter(
-            [mne.io.pick.channel_type(info, idx)
-             for idx in range(len(info['chs']))])
-        other_infos['ch_types'] = ', '.join(
-            [f'{key}: {value}' for key, value in ch_type_counter.items()])
-
-        key_list = [('no_files', 'Size of all associated files'),
-                    ('size', 'Size of all associated files', size_unit),
-                    ('proj_name', 'Project-Name'),
-                    ('experimenter', 'Experimenter'),
-                    ('line_freq', 'Powerline-Frequency', 'Hz'),
-                    ('sfreq', 'Samplerate', 'Hz'),
-                    ('highpass', 'Highpass', 'Hz'),
-                    ('lowpass', 'Lowpass', 'Hz'),
-                    ('nchan', 'Number of channels'),
-                    ('ch_types', 'Channel-Types'),
-                    ('subject_info', 'Subject-Info'),
-                    ('device_info', 'Device-Info'),
-                    ('helium_info', 'Helium-Info')]
+            [mne.io.pick.channel_type(info, idx) for idx in range(len(info["chs"]))]
+        )
+        other_infos["ch_types"] = ", ".join(
+            [f"{key}: {value}" for key, value in ch_type_counter.items()]
+        )
+
+        key_list = [
+            ("no_files", "Size of all associated files"),
+            ("size", "Size of all associated files", size_unit),
+            ("proj_name", "Project-Name"),
+            ("experimenter", "Experimenter"),
+            ("line_freq", "Powerline-Frequency", "Hz"),
+            ("sfreq", "Samplerate", "Hz"),
+            ("highpass", "Highpass", "Hz"),
+            ("lowpass", "Lowpass", "Hz"),
+            ("nchan", "Number of channels"),
+            ("ch_types", "Channel-Types"),
+            ("subject_info", "Subject-Info"),
+            ("device_info", "Device-Info"),
+            ("helium_info", "Helium-Info"),
+        ]
 
-        self.info_string = f'<h1>{meeg_name}</h1>'
+        self.info_string = f"<h1>{meeg_name}</h1>"
 
         for key_tuple in key_list:
             key = key_tuple[0]
             if key in info:
                 value = info[key]
             elif key in other_infos:
                 value = other_infos[key]
             else:
                 value = None
 
             if len(key_tuple) == 2:
-                self.info_string += f'<b>{key_tuple[1]}:</b> {value}<br>'
+                self.info_string += f"<b>{key_tuple[1]}:</b> {value}<br>"
             else:
-                self.info_string += f'<b>{key_tuple[1]}:</b> {value}' \
-                                    f' <i>{key_tuple[2]}</i><br>'
+                self.info_string += (
+                    f"<b>{key_tuple[1]}:</b> {value}" f" <i>{key_tuple[2]}</i><br>"
+                )
 
         self.info_label.setHtml(self.info_string)
 
 
 class CopyParamsDialog(SimpleDialog):
     def __init__(self, main_win):
         self.main_win = main_win
         self.ct = main_win.ct
         widget = QWidget()
         layout = QGridLayout()
-        layout.addWidget(QLabel('From:'), 0, 0)
+        layout.addWidget(QLabel("From:"), 0, 0)
         self.from_cmbx = QComboBox()
         self.from_cmbx.addItems(self.ct.projects)
         self.from_cmbx.currentTextChanged.connect(self.from_selected)
         layout.addWidget(self.from_cmbx, 1, 0)
-        layout.addWidget(QLabel('Parameter-Preset:'), 2, 0)
+        layout.addWidget(QLabel("Parameter-Preset:"), 2, 0)
         self.from_pp_cmbx = QComboBox()
         layout.addWidget(self.from_pp_cmbx, 3, 0)
 
-        layout.addWidget(QLabel('To:'), 0, 1)
+        layout.addWidget(QLabel("To:"), 0, 1)
         self.to_cmbx = QComboBox()
         self.to_cmbx.currentTextChanged.connect(self.to_selected)
         self.to_cmbx.setEnabled(False)
         layout.addWidget(self.to_cmbx, 1, 1)
-        layout.addWidget(QLabel('Parameter-Preset:'), 2, 1)
+        layout.addWidget(QLabel("Parameter-Preset:"), 2, 1)
         self.to_pp_cmbx = QComboBox()
         self.to_pp_cmbx.setEditable(True)
         layout.addWidget(self.to_pp_cmbx, 3, 1)
 
-        copy_bt = QPushButton('Copy')
+        copy_bt = QPushButton("Copy")
         copy_bt.clicked.connect(self.copy_parameters)
         layout.addWidget(copy_bt, 4, 0)
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt, 4, 1)
 
         widget.setLayout(layout)
-        super().__init__(widget, parent=main_win,
-                         title='Copy Parameters between Projects',
-                         window_title='Copy Parameters', show_close_bt=False)
+        super().__init__(
+            widget,
+            parent=main_win,
+            title="Copy Parameters between Projects",
+            window_title="Copy Parameters",
+            show_close_bt=False,
+        )
 
     def _get_p_presets(self, pr_name):
         if self.ct.pr.name == pr_name:
             project = self.ct.pr
         else:
             project = Project(self.ct, pr_name)
 
         return list(project.parameters.keys())
 
     def from_selected(self, from_name):
         if from_name:
             self.to_cmbx.setEnabled(True)
             self.to_cmbx.clear()
-            self.to_cmbx.addItems([p for p in self.ct.projects
-                                   if p != from_name])
+            self.to_cmbx.addItems([p for p in self.ct.projects if p != from_name])
 
             self.from_pp_cmbx.clear()
             self.from_pp_cmbx.addItems(self._get_p_presets(from_name))
 
     def to_selected(self, to_name):
         if to_name:
             self.to_pp_cmbx.clear()
@@ -290,56 +307,55 @@
 
     def copy_parameters(self):
         from_name = self.from_cmbx.currentText()
         from_pp = self.from_pp_cmbx.currentText()
         to_name = self.to_cmbx.currentText()
         to_pp = self.to_pp_cmbx.currentText()
         if from_name and to_name:
-            self.ct.copy_parameters_between_projects(from_name, from_pp,
-                                                     to_name, to_pp)
+            self.ct.copy_parameters_between_projects(from_name, from_pp, to_name, to_pp)
         if to_name == self.ct.pr.name:
             self.main_win.parameters_dock.redraw_param_widgets()
-        QMessageBox().information(self, 'Finished',
-                                  f'Parameters copied from {from_name} '
-                                  f'to {to_name}!')
+        QMessageBox().information(
+            self, "Finished", f"Parameters copied from {from_name} " f"to {to_name}!"
+        )
 
 
 class AboutDialog(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
-        with resources.open_text('mne_pipeline_hd.resource',
-                                 'license.txt') as file:
+        with resources.open_text("mne_pipeline_hd.resource", "license.txt") as file:
             license_text = file.read()
-        license_text = license_text.replace('\n', '<br>')
-        text = '<h1>MNE-Pipeline HD</h1>' \
-               '<b>A Pipeline-GUI for MNE-Python</b><br>' \
-               '(originally developed for MEG-Lab Heidelberg)<br>' \
-               '<i>Development was initially inspired by: ' \
-               '<a href=https://doi.org/10.3389/fnins.2018.00006>Andersen ' \
-               'L.M. 2018</a></i><br>' \
-               '<br>' \
-               'As for now, this program is still in alpha-state, ' \
-               'so some features may not work as expected. ' \
-               'Be sure to check all the parameters for each step ' \
-               'to be correctly adjusted to your needs.<br>' \
-               '<br>' \
-               '<b>Developed by:</b><br>' \
-               'Martin Schulz (medical student, Heidelberg)<br>' \
-               '<br>' \
-               '<b>Dependencies:</b><br>' \
-               'MNE-Python: <a href=https://github.com/mne-tools/' \
-               'mne-python>Website</a>' \
-               '<a href=https://github.com/mne-tools/mne-python>' \
-               'GitHub</a><br>' \
-               '<a href=https://github.com/ColinDuquesnoy/' \
-               'QDarkStyleSheet>qdarkstyle</a><br>' \
-               '<br>' \
-               '<b>Licensed under:</b><br>' \
-               + license_text
+        license_text = license_text.replace("\n", "<br>")
+        text = (
+            "<h1>MNE-Pipeline HD</h1>"
+            "<b>A Pipeline-GUI for MNE-Python</b><br>"
+            "(originally developed for MEG-Lab Heidelberg)<br>"
+            "<i>Development was initially inspired by: "
+            "<a href=https://doi.org/10.3389/fnins.2018.00006>Andersen "
+            "L.M. 2018</a></i><br>"
+            "<br>"
+            "As for now, this program is still in alpha-state, "
+            "so some features may not work as expected. "
+            "Be sure to check all the parameters for each step "
+            "to be correctly adjusted to your needs.<br>"
+            "<br>"
+            "<b>Developed by:</b><br>"
+            "Martin Schulz (medical student, Heidelberg)<br>"
+            "<br>"
+            "<b>Dependencies:</b><br>"
+            "MNE-Python: <a href=https://github.com/mne-tools/"
+            "mne-python>Website</a>"
+            "<a href=https://github.com/mne-tools/mne-python>"
+            "GitHub</a><br>"
+            "<a href=https://github.com/5yutan5/PyQtDarkTheme>"
+            "pyqtdarktheme</a><br>"
+            "<br>"
+            "<b>Licensed under:</b><br>" + license_text
+        )
 
         layout = QVBoxLayout()
 
         text_widget = QTextEdit()
         text_widget.setReadOnly(True)
         text_widget.setHtml(text)
         layout.addWidget(text_widget)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/education_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/education_widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,72 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import json
 from os import makedirs
 from os.path import isdir, join
 from shutil import copytree
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QComboBox, QFileDialog, QGridLayout, QHBoxLayout,
-                             QLabel, QLineEdit,
-                             QMainWindow, QSizePolicy, QTextBrowser, QTextEdit,
-                             QVBoxLayout,
-                             QWidget, QWizard, QWizardPage)
+from PyQt5.QtWidgets import (
+    QComboBox,
+    QFileDialog,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QMainWindow,
+    QSizePolicy,
+    QTextBrowser,
+    QTextEdit,
+    QVBoxLayout,
+    QWidget,
+    QWizard,
+    QWizardPage,
+)
 
 from mne_pipeline_hd.gui.base_widgets import CheckDictEditList, CheckList
 from mne_pipeline_hd.gui.gui_utils import center, set_ratio_geometry
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class EducationTour(QWizard):
     def __init__(self, main_win, edu_program):
         super().__init__(main_win)
         self.mw = main_win
         self.edu = edu_program
 
-        self.setWindowTitle(self.edu['name'])
+        self.setWindowTitle(self.edu["name"])
         self.setWizardStyle(QWizard.ModernStyle)
         self.setOption(QWizard.HaveHelpButton, False)
 
         set_ratio_geometry(0.4, self)
         center(self)
 
         self.add_pages()
         self.show()
 
     def add_pages(self):
-        for page_name in self.edu['tour_list']:
+        for page_name in self.edu["tour_list"]:
             page = QWizardPage()
             page.setTitle(page_name)
 
             layout = QVBoxLayout()
             page_view = QTextBrowser()
             page_view.setReadOnly(True)
             page_view.setOpenExternalLinks(True)
-            text = self.edu['tour'][page_name]
-            if self.edu['format'] == 'PlainText':
+            text = self.edu["tour"][page_name]
+            if self.edu["format"] == "PlainText":
                 page_view.setPlainText(text)
-            elif self.edu['format'] == 'HTML':
+            elif self.edu["format"] == "HTML":
                 page_view.setHtml(text)
             # Not supported until PyQt>=5.14
             # elif self.edu['format'] == 'Markdown':
             #     page_view.setMarkdown(text)
             layout.addWidget(page_view)
             page.setLayout(layout)
 
@@ -66,187 +75,193 @@
 
 class EducationEditor(QMainWindow):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.edu = dict()
-        self.edu['name'] = 'Education'
-        self.edu['meeg'] = self.ct.pr.sel_meeg.copy()
-        self.edu['fsmri'] = self.ct.pr.sel_fsmri.copy()
-        self.edu['groups'] = self.ct.pr.sel_groups.copy()
-        self.edu['functions'] = [f for f in self.ct.pr.sel_functions if
-                                 f in self.ct.pr.sel_functions]
-        self.edu['dock_kwargs'] = {'meeg_view': False, 'fsmri_view': False,
-                                   'group_view': False}
-        self.edu['format'] = 'PlainText'
-        self.edu['tour_list'] = list()
-        self.edu['tour'] = dict()
+        self.edu["name"] = "Education"
+        self.edu["meeg"] = self.ct.pr.sel_meeg.copy()
+        self.edu["fsmri"] = self.ct.pr.sel_fsmri.copy()
+        self.edu["groups"] = self.ct.pr.sel_groups.copy()
+        self.edu["functions"] = [
+            f for f in self.ct.pr.sel_functions if f in self.ct.pr.sel_functions
+        ]
+        self.edu["dock_kwargs"] = {
+            "meeg_view": False,
+            "fsmri_view": False,
+            "group_view": False,
+        }
+        self.edu["format"] = "PlainText"
+        self.edu["tour_list"] = list()
+        self.edu["tour"] = dict()
 
-        self.edu_folder = join(self.ct.home_path, 'edu_programs')
+        self.edu_folder = join(self.ct.home_path, "edu_programs")
         set_ratio_geometry(0.8, self)
 
         self.init_menu()
         self.init_ui()
         self.show()
 
     def init_menu(self):
-        file_menu = self.menuBar().addMenu('File')
-        file_menu.addAction('&Load', self.load_edu_file)
-        file_menu.addAction('&Save', self.save_edu_file)
+        file_menu = self.menuBar().addMenu("File")
+        file_menu.addAction("&Load", self.load_edu_file)
+        file_menu.addAction("&Save", self.save_edu_file)
         file_menu.addSeparator()
-        file_menu.addAction('&Close', self.close)
+        file_menu.addAction("&Close", self.close)
 
     def init_ui(self):
         layout = QVBoxLayout()
         self.setCentralWidget(QWidget())
 
-        name_label = QLabel('Name:')
-        name_label.setFont(QFont(QS().value('app_font'), 14))
+        name_label = QLabel("Name:")
+        name_label.setFont(QFont(QS().value("app_font"), 14))
         layout.addWidget(name_label)
         self.name_ledit = QLineEdit()
         self.name_ledit.textEdited.connect(self.name_changed)
         layout.addWidget(self.name_ledit)
 
         select_layout = QHBoxLayout()
-        self.meeg_check_list = CheckList(self.ct.pr.all_meeg, self.edu['meeg'],
-                                         title='Select MEEG')
+        self.meeg_check_list = CheckList(
+            self.ct.pr.all_meeg, self.edu["meeg"], title="Select MEEG"
+        )
         select_layout.addWidget(self.meeg_check_list)
 
-        self.fsmri_check_list = CheckList(self.ct.pr.all_fsmri,
-                                          self.edu['fsmri'],
-                                          title='Select FSMRI')
+        self.fsmri_check_list = CheckList(
+            self.ct.pr.all_fsmri, self.edu["fsmri"], title="Select FSMRI"
+        )
         select_layout.addWidget(self.fsmri_check_list)
 
-        self.group_check_list = CheckList(list(self.ct.pr.all_groups.keys()),
-                                          self.edu['groups'],
-                                          title='Select Groups')
+        self.group_check_list = CheckList(
+            list(self.ct.pr.all_groups.keys()),
+            self.edu["groups"],
+            title="Select Groups",
+        )
         select_layout.addWidget(self.group_check_list)
 
-        self.func_check_list = CheckList(self.ct.pd_funcs.index,
-                                         self.edu['functions'],
-                                         title='Select Functions')
+        self.func_check_list = CheckList(
+            self.ct.pd_funcs.index, self.edu["functions"], title="Select Functions"
+        )
         select_layout.addWidget(self.func_check_list)
 
         layout.addLayout(select_layout)
 
-        page_label = QLabel('Make a Tour:')
-        page_label.setFont(QFont(QS().value('app_font'), 14))
+        page_label = QLabel("Make a Tour:")
+        page_label.setFont(QFont(QS().value("app_font"), 14))
         self.format_cmbx = QComboBox()
-        self.format_cmbx.addItems(['PlainText', 'HTML'])
+        self.format_cmbx.addItems(["PlainText", "HTML"])
         self.format_cmbx.currentTextChanged.connect(self.format_changed)
-        self.format_cmbx.setCurrentText('PlainText')
+        self.format_cmbx.setCurrentText("PlainText")
         layout.addWidget(self.format_cmbx)
 
-        self.page_list = CheckDictEditList(self.edu['tour_list'],
-                                           self.edu['tour'], show_index=True)
+        self.page_list = CheckDictEditList(
+            self.edu["tour_list"], self.edu["tour"], show_index=True
+        )
         self.page_list.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.page_list.currentChanged.connect(self.page_changed)
         self.page_list.dataChanged.connect(self.page_edited)
         layout.addWidget(self.page_list)
 
         edit_layout = QGridLayout()
-        edit_label = QLabel('Edit')
+        edit_label = QLabel("Edit")
         edit_layout.addWidget(edit_label, 0, 0, alignment=Qt.AlignHCenter)
         self.page_edit = QTextEdit()
         self.page_edit.textChanged.connect(self.page_text_changed)
         edit_layout.addWidget(self.page_edit, 1, 0)
 
-        preview_label = QLabel('Preview')
+        preview_label = QLabel("Preview")
         edit_layout.addWidget(preview_label, 0, 1, alignment=Qt.AlignHCenter)
         self.page_display = QTextBrowser()
         self.page_display.setOpenExternalLinks(True)
         self.page_display.setReadOnly(True)
         edit_layout.addWidget(self.page_display, 1, 1)
 
         layout.addLayout(edit_layout)
         self.centralWidget().setLayout(layout)
 
     def update_ui(self):
-        self.name_ledit.setText(self.edu['name'])
-        self.meeg_check_list.replace_checked(self.edu['meeg'])
-        self.fsmri_check_list.replace_checked(self.edu['fsmri'])
-        self.group_check_list.replace_checked(self.edu['groups'])
-        self.func_check_list.replace_checked(self.edu['functions'])
-        self.format_cmbx.setCurrentText(self.edu['format'])
-        self.page_list.replace_data(self.edu['tour_list'])
-        self.page_list.replace_check_dict(self.edu['tour'])
+        self.name_ledit.setText(self.edu["name"])
+        self.meeg_check_list.replace_checked(self.edu["meeg"])
+        self.fsmri_check_list.replace_checked(self.edu["fsmri"])
+        self.group_check_list.replace_checked(self.edu["groups"])
+        self.func_check_list.replace_checked(self.edu["functions"])
+        self.format_cmbx.setCurrentText(self.edu["format"])
+        self.page_list.replace_data(self.edu["tour_list"])
+        self.page_list.replace_check_dict(self.edu["tour"])
         self.page_edit.clear()
         self.page_display.clear()
 
     def name_changed(self, text):
-        if text != '':
-            self.edu['name'] = text
+        if text != "":
+            self.edu["name"] = text
 
     def format_changed(self, text):
-        if text != '':
-            self.edu['format'] = text
+        if text != "":
+            self.edu["format"] = text
         self.page_text_changed()
 
     def _set_page_display(self, text):
         self.page_display.clear()
-        if self.edu['format'] == 'PlainText':
+        if self.edu["format"] == "PlainText":
             self.page_display.setPlainText(text)
-        elif self.edu['format'] == 'HTML':
+        elif self.edu["format"] == "HTML":
             self.page_display.setHtml(text)
         # Not supported until PyQt>=5.14
         # elif self.edu['format'] == 'Markdown':
         #     self.page_display.setMarkdown(text)
 
     def page_changed(self, page_name):
-        if page_name in self.edu['tour']:
-            text = self.edu['tour'][page_name]
+        if page_name in self.edu["tour"]:
+            text = self.edu["tour"][page_name]
             self.page_edit.clear()
             self.page_edit.setPlainText(text)
             self._set_page_display(text)
         else:
             self.page_edit.clear()
             self.page_display.clear()
 
     def page_edited(self, new_page_name, index):
         # Rename key in dictionary
         try:
-            old_page_name = list(self.edu['tour'].keys())[index.row()]
+            old_page_name = list(self.edu["tour"].keys())[index.row()]
         except IndexError:
             old_page_name = new_page_name
-        if old_page_name in self.edu['tour']:
-            self.edu['tour'][new_page_name] = \
-                self.edu['tour'].pop(old_page_name)
+        if old_page_name in self.edu["tour"]:
+            self.edu["tour"][new_page_name] = self.edu["tour"].pop(old_page_name)
         else:
-            self.edu['tour'][new_page_name] = ''
+            self.edu["tour"][new_page_name] = ""
 
     def page_text_changed(self):
         current_page = self.page_list.get_current()
         text = self.page_edit.toPlainText()
         self._set_page_display(text)
-        if text != '':
-            self.edu['tour'][current_page] = text
+        if text != "":
+            self.edu["tour"][current_page] = text
 
     def load_edu_file(self):
-        file_path = QFileDialog().getOpenFileName(self,
-                                                  directory=self.edu_folder)[0]
-        if file_path != '':
-            with open(file_path, 'r') as file:
+        file_path = QFileDialog().getOpenFileName(self, directory=self.edu_folder)[0]
+        if file_path != "":
+            with open(file_path, "r") as file:
                 self.edu = json.load(file)
 
         self.update_ui()
 
     def save_edu_file(self):
-        if len(self.edu['meeg']) > 0:
-            self.edu['dock_kwargs']['meeg_view'] = True
-        if len(self.edu['fsmri']) > 0:
-            self.edu['dock_kwargs']['fsmri_view'] = True
-        if len(self.edu['groups']) > 0:
-            self.edu['dock_kwargs']['group_view'] = True
+        if len(self.edu["meeg"]) > 0:
+            self.edu["dock_kwargs"]["meeg_view"] = True
+        if len(self.edu["fsmri"]) > 0:
+            self.edu["dock_kwargs"]["fsmri_view"] = True
+        if len(self.edu["groups"]) > 0:
+            self.edu["dock_kwargs"]["group_view"] = True
 
         if not isdir(self.edu_folder):
             makedirs(self.edu_folder)
 
         edu_path = join(self.edu_folder, f'{self.edu["name"]}-edu.json')
-        with open(edu_path, 'w') as file:
+        with open(edu_path, "w") as file:
             json.dump(self.edu, file, indent=4)
 
-        new_pscripts_path = join(self.ct.pr.project_path,
-                                 f'_pipeline_scripts{self.edu["name"]}')
+        new_pscripts_path = join(
+            self.ct.pr.project_path, f'_pipeline_scripts{self.edu["name"]}'
+        )
         # Copy Pipeline-Scripts
-        copytree(self.ct.pr.pscripts_path, new_pscripts_path,
-                 dirs_exist_ok=True)
+        copytree(self.ct.pr.pscripts_path, new_pscripts_path, dirs_exist_ok=True)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/function_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/function_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 import os
 import shutil
 from ast import literal_eval
 from functools import partial
@@ -17,31 +15,56 @@
 from os.path import isdir, isfile, join
 from pathlib import Path
 from types import FunctionType
 
 import pandas as pd
 from PyQt5.QtCore import QSize, Qt
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QButtonGroup, QComboBox, QDialog, QFileDialog,
-                             QFormLayout,
-                             QGroupBox, QHBoxLayout, QLabel, QLineEdit,
-                             QListView,
-                             QListWidget, QListWidgetItem, QMessageBox,
-                             QPushButton,
-                             QSizePolicy, QStyle, QTabWidget, QVBoxLayout,
-                             QGridLayout, QProgressBar, QCheckBox)
+from PyQt5.QtWidgets import (
+    QButtonGroup,
+    QComboBox,
+    QDialog,
+    QFileDialog,
+    QFormLayout,
+    QGroupBox,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QListView,
+    QListWidget,
+    QListWidgetItem,
+    QMessageBox,
+    QPushButton,
+    QSizePolicy,
+    QStyle,
+    QTabWidget,
+    QVBoxLayout,
+    QGridLayout,
+    QProgressBar,
+    QCheckBox,
+)
 
 from mne_pipeline_hd.gui import parameter_widgets
-from mne_pipeline_hd.gui.base_widgets import (CheckDictList, CheckList,
-                                              EditDict, EditList,
-                                              SimpleDialog, SimpleList)
-from mne_pipeline_hd.gui.gui_utils import (CodeEditor, ErrorDialog, center,
-                                           get_exception_tuple,
-                                           set_ratio_geometry, get_std_icon,
-                                           MainConsoleWidget)
+from mne_pipeline_hd.gui.base_widgets import (
+    CheckDictList,
+    CheckList,
+    EditDict,
+    EditList,
+    SimpleDialog,
+    SimpleList,
+)
+from mne_pipeline_hd.gui.gui_utils import (
+    CodeEditor,
+    ErrorDialog,
+    center,
+    get_exception_tuple,
+    set_ratio_geometry,
+    get_std_icon,
+    MainConsoleWidget,
+)
 from mne_pipeline_hd.gui.models import CustomFunctionModel, RunModel
 from mne_pipeline_hd.pipeline.function_utils import QRunController
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class RunDialog(QDialog):
     def __init__(self, main_win):
@@ -59,34 +82,31 @@
     def init_controller(self):
         self.rc = QRunController(run_dialog=self, controller=self.mw.ct)
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         view_layout = QGridLayout()
-        view_layout.addWidget(QLabel('Objects: '), 0, 0)
+        view_layout.addWidget(QLabel("Objects: "), 0, 0)
         self.object_view = QListView()
-        self.object_model = RunModel(self.rc.all_objects, mode='object')
+        self.object_model = RunModel(self.rc.all_objects, mode="object")
         self.object_view.setModel(self.object_model)
-        self.object_view.setSizePolicy(QSizePolicy.Preferred,
-                                       QSizePolicy.Maximum)
+        self.object_view.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
         view_layout.addWidget(self.object_view, 1, 0)
 
-        view_layout.addWidget(QLabel('Functions: '), 0, 1)
+        view_layout.addWidget(QLabel("Functions: "), 0, 1)
         self.func_view = QListView()
-        self.func_model = RunModel(self.rc.current_all_funcs, mode='func')
+        self.func_model = RunModel(self.rc.current_all_funcs, mode="func")
         self.func_view.setModel(self.func_model)
-        self.func_view.setSizePolicy(QSizePolicy.Preferred,
-                                     QSizePolicy.Maximum)
+        self.func_view.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
         view_layout.addWidget(self.func_view, 1, 1)
 
-        view_layout.addWidget(QLabel('Errors: '), 0, 2)
+        view_layout.addWidget(QLabel("Errors: "), 0, 2)
         self.error_widget = SimpleList(list())
-        self.error_widget.setSizePolicy(QSizePolicy.Preferred,
-                                        QSizePolicy.Maximum)
+        self.error_widget.setSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
         # Connect Signal from error_widget to function
         # to enable inspecting the errors
         self.error_widget.currentChanged.connect(self.show_error)
         view_layout.addWidget(self.error_widget, 1, 2)
 
         layout.addLayout(view_layout)
 
@@ -96,48 +116,48 @@
         self.pgbar = QProgressBar()
         self.pgbar.setValue(0)
         self.pgbar.setMaximum(len(self.rc.all_steps))
         layout.addWidget(self.pgbar)
 
         bt_layout = QHBoxLayout()
 
-        self.continue_bt = QPushButton('Continue')
-        self.continue_bt.setFont(QFont('AnyStyle', 14))
-        self.continue_bt.setIcon(get_std_icon('SP_MediaPlay'))
+        self.continue_bt = QPushButton("Continue")
+        self.continue_bt.setFont(QFont("AnyStyle", 14))
+        self.continue_bt.setIcon(get_std_icon("SP_MediaPlay"))
         self.continue_bt.clicked.connect(self.start)
         bt_layout.addWidget(self.continue_bt)
 
-        self.pause_bt = QPushButton('Pause')
-        self.pause_bt.setFont(QFont('AnyStyle', 14))
-        self.pause_bt.setIcon(get_std_icon('SP_MediaPause'))
+        self.pause_bt = QPushButton("Pause")
+        self.pause_bt.setFont(QFont("AnyStyle", 14))
+        self.pause_bt.setIcon(get_std_icon("SP_MediaPause"))
         self.pause_bt.clicked.connect(self.pause_funcs)
         bt_layout.addWidget(self.pause_bt)
 
-        self.restart_bt = QPushButton('Restart')
-        self.restart_bt.setFont(QFont('AnyStyle', 14))
-        self.restart_bt.setIcon(get_std_icon('SP_BrowserReload'))
+        self.restart_bt = QPushButton("Restart")
+        self.restart_bt.setFont(QFont("AnyStyle", 14))
+        self.restart_bt.setIcon(get_std_icon("SP_BrowserReload"))
         self.restart_bt.clicked.connect(self.restart)
         bt_layout.addWidget(self.restart_bt)
 
-        if QS().value('use_qthread'):
+        if QS().value("use_qthread"):
             self.reload_chbx = None
         else:
-            self.reload_chbx = QCheckBox('Reload Modules')
+            self.reload_chbx = QCheckBox("Reload Modules")
             bt_layout.addWidget(self.reload_chbx)
 
-        self.autoscroll_bt = QPushButton('Auto-Scroll')
+        self.autoscroll_bt = QPushButton("Auto-Scroll")
         self.autoscroll_bt.setCheckable(True)
         self.autoscroll_bt.setChecked(True)
-        self.autoscroll_bt.setIcon(get_std_icon('SP_DialogOkButton'))
+        self.autoscroll_bt.setIcon(get_std_icon("SP_DialogOkButton"))
         self.autoscroll_bt.clicked.connect(self.toggle_autoscroll)
         bt_layout.addWidget(self.autoscroll_bt)
 
-        self.close_bt = QPushButton('Close')
-        self.close_bt.setFont(QFont('AnyStyle', 14))
-        self.close_bt.setIcon(get_std_icon('SP_MediaStop'))
+        self.close_bt = QPushButton("Close")
+        self.close_bt.setFont(QFont("AnyStyle", 14))
+        self.close_bt.setIcon(get_std_icon("SP_MediaStop"))
         self.close_bt.clicked.connect(self.close)
         bt_layout.addWidget(self.close_bt)
         layout.addLayout(bt_layout)
 
         self.setLayout(layout)
 
     def start(self):
@@ -149,16 +169,15 @@
         self.restart_bt.setEnabled(False)
         self.close_bt.setEnabled(False)
 
         self.rc.start()
 
     def pause_funcs(self):
         self.rc.paused = True
-        self.console_widget.write_html(
-            '<br><b>Finishing last function...</b><br>')
+        self.console_widget.write_html("<br><b>Finishing last function...</b><br>")
 
     def restart(self):
         # Reinitialize controller
         self.init_controller()
 
         # ToDo: MP
         # if self.reload_chbx and self.reload_chbx.isChecked():
@@ -200,57 +219,66 @@
     def __init__(self, cf_dialog):
         super().__init__(cf_dialog)
         self.cf = cf_dialog
         self.gui_args = dict()
         self.default_gui_args = dict()
 
         if self.cf.current_parameter:
-            covered_params = ['data', 'name', 'alias', 'default', 'param_unit',
-                              'description']
+            covered_params = [
+                "data",
+                "name",
+                "alias",
+                "default",
+                "param_unit",
+                "description",
+            ]
             # Get possible default GUI-Args additional to those
             # covered by the Main-GUI
-            gui_type = self.cf.add_pd_params.loc[
-                self.cf.current_parameter, 'gui_type']
+            gui_type = self.cf.add_pd_params.loc[self.cf.current_parameter, "gui_type"]
             if pd.notna(gui_type):
                 gui_handle = getattr(parameter_widgets, gui_type)
                 psig = inspect.signature(gui_handle).parameters
-                self.default_gui_args = {p: psig[p].default for p in psig if
-                                         p not in covered_params}
+                self.default_gui_args = {
+                    p: psig[p].default for p in psig if p not in covered_params
+                }
 
             # Get current GUI-Args
             loaded_gui_args = self.cf.add_pd_params.loc[
-                self.cf.current_parameter, 'gui_args']
+                self.cf.current_parameter, "gui_args"
+            ]
             if pd.notna(loaded_gui_args):
                 self.gui_args = literal_eval(loaded_gui_args)
             else:
                 self.gui_args = dict()
 
             # Fill in all possible Options, which are not already changed
-            for arg_key in [ak for ak in self.default_gui_args
-                            if ak not in self.gui_args]:
+            for arg_key in [
+                ak for ak in self.default_gui_args if ak not in self.gui_args
+            ]:
                 self.gui_args[arg_key] = self.default_gui_args[arg_key]
 
             if len(self.gui_args) > 0:
                 self.init_ui()
                 self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
         layout.addWidget(EditDict(data=self.gui_args, ui_buttons=False))
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def closeEvent(self, event):
         # Remove all options which don't differ from the default
-        for arg_key in [ak for ak in self.gui_args if
-                        self.gui_args[ak] == self.default_gui_args[ak]]:
+        for arg_key in [
+            ak for ak in self.gui_args if self.gui_args[ak] == self.default_gui_args[ak]
+        ]:
             self.gui_args.pop(arg_key)
 
         if len(self.gui_args) > 0:
             self.cf.pguiargs_changed(self.gui_args)
 
         event.accept()
 
@@ -265,18 +293,21 @@
         self.init_ui()
         # If open(), execution doesn't stop after the dialog
         self.exec()
 
     def init_ui(self):
         layout = QVBoxLayout()
         layout.addWidget(
-            QLabel(f'For {self.gui_type}, you need to specify'
-                   f' the options to choose from'))
+            QLabel(
+                f"For {self.gui_type}, you need to specify"
+                f" the options to choose from"
+            )
+        )
         layout.addWidget(EditList(data=self.options))
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
         self.setLayout(layout)
 
 
 # ToDo:
 #   Bug1: After saving a new function, the parameters stay in the table-view,
@@ -289,59 +320,79 @@
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.file_path = None
         self.pkg_name = None
         self.current_function = None
         self.current_parameter = None
-        self.oblig_func = ['target', 'tab', 'group', 'matplotlib', 'mayavi']
-        self.oblig_params = ['default', 'gui_type']
+        self.oblig_func = ["target", "tab", "group", "matplotlib", "mayavi"]
+        self.oblig_params = ["default", "gui_type"]
 
         self.exst_functions = list(self.ct.pd_funcs.index)
-        self.exst_parameters = ['mw', 'pr', 'meeg', 'fsmri', 'group']
+        self.exst_parameters = ["mw", "pr", "meeg", "fsmri", "group"]
         self.exst_parameters += list(self.ct.settings.keys())
         self.exst_parameters += list(QS().childKeys())
-        self.exst_parameters += list(self.ct.pr.parameters[
-                                         self.ct.pr.p_preset].keys())
+        self.exst_parameters += list(self.ct.pr.parameters[self.ct.pr.p_preset].keys())
         self.param_exst_dict = dict()
 
         self.code_editor = None
         self.code_dict = dict()
 
         # Get available parameter-guis
-        self.available_param_guis = [pg for pg in dir(parameter_widgets) if
-                                     'Gui' in pg and pg != 'QtGui']
+        self.available_param_guis = [
+            pg for pg in dir(parameter_widgets) if "Gui" in pg and pg != "QtGui"
+        ]
 
         self.add_pd_funcs = pd.DataFrame(
-            columns=['alias', 'target', 'tab', 'group', 'matplotlib',
-                     'mayavi', 'dependencies', 'module', 'func_args',
-                     'ready'])
+            columns=[
+                "alias",
+                "target",
+                "tab",
+                "group",
+                "matplotlib",
+                "mayavi",
+                "dependencies",
+                "module",
+                "func_args",
+                "ready",
+            ]
+        )
         self.add_pd_params = pd.DataFrame(
-            columns=['alias', 'group', 'default', 'unit', 'description',
-                     'gui_type', 'gui_args', 'functions', 'ready'])
+            columns=[
+                "alias",
+                "group",
+                "default",
+                "unit",
+                "description",
+                "gui_type",
+                "gui_args",
+                "functions",
+                "ready",
+            ]
+        )
 
-        self.yes_icon = get_std_icon('SP_DialogApplyButton')
-        self.no_icon = get_std_icon('SP_DialogCancelButton')
+        self.yes_icon = get_std_icon("SP_DialogApplyButton")
+        self.no_icon = get_std_icon("SP_DialogCancelButton")
 
-        self.setWindowTitle('Custom-Functions-Setup')
+        self.setWindowTitle("Custom-Functions-Setup")
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         # Import Button and Combobox
         add_bt_layout = QHBoxLayout()
-        addfn_bt = QPushButton('Load Function/s')
-        addfn_bt.setFont(QFont(QS().value('app_font'), 12))
+        addfn_bt = QPushButton("Load Function/s")
+        addfn_bt.setFont(QFont(QS().value("app_font"), 12))
         addfn_bt.clicked.connect(self.get_functions)
         add_bt_layout.addWidget(addfn_bt)
-        editfn_bt = QPushButton('Edit Function/s')
-        editfn_bt.setFont(QFont(QS().value('app_font'), 12))
+        editfn_bt = QPushButton("Edit Function/s")
+        editfn_bt.setFont(QFont(QS().value("app_font"), 12))
         editfn_bt.clicked.connect(self.edit_functions)
         add_bt_layout.addWidget(editfn_bt)
         layout.addLayout(add_bt_layout)
 
         # Function-ComboBox
         func_cmbx_layout = QHBoxLayout()
         self.func_cmbx = QComboBox()
@@ -354,220 +405,228 @@
         func_cmbx_layout.addWidget(self.func_chkl)
         layout.addLayout(func_cmbx_layout)
 
         # Hint for obligatory items
         # There may be a better way to center the labels
         # instead of with the space-labels
         obl_hint_layout = QHBoxLayout()
-        space_label1 = QLabel('')
+        space_label1 = QLabel("")
         obl_hint_layout.addWidget(space_label1)
         obl_hint_label1 = QLabel()
         obl_hint_label1.setPixmap(self.no_icon.pixmap(16, 16))
         obl_hint_label1.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         obl_hint_layout.addWidget(obl_hint_label1)
         obl_hint_label2 = QLabel()
-        obl_hint_label2.setPixmap(
-            get_std_icon('SP_ArrowForward').pixmap(16, 16))
+        obl_hint_label2.setPixmap(get_std_icon("SP_ArrowForward").pixmap(16, 16))
         obl_hint_label2.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         obl_hint_layout.addWidget(obl_hint_label2)
         obl_hint_label3 = QLabel()
         obl_hint_label3.setPixmap(self.yes_icon.pixmap(16, 16))
         obl_hint_label3.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         obl_hint_layout.addWidget(obl_hint_label3)
-        obl_hint_label4 = QLabel('(= The items marked are obligatory)')
+        obl_hint_label4 = QLabel("(= The items marked are obligatory)")
         obl_hint_label4.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         obl_hint_layout.addWidget(obl_hint_label4)
-        space_label2 = QLabel('')
+        space_label2 = QLabel("")
         obl_hint_layout.addWidget(space_label2)
         layout.addLayout(obl_hint_layout)
 
         setup_layout = QHBoxLayout()
         # The Function-Setup-Groupbox
-        func_setup_gbox = QGroupBox('Function-Setup')
+        func_setup_gbox = QGroupBox("Function-Setup")
         func_setup_gbox.setAlignment(Qt.AlignHCenter)
         func_setup_formlayout = QFormLayout()
 
         self.falias_le = QLineEdit()
-        self.falias_le.setToolTip('Set a name if you want something other'
-                                  ' than the functions-name')
+        self.falias_le.setToolTip(
+            "Set a name if you want something other" " than the functions-name"
+        )
         self.falias_le.textEdited.connect(self.falias_changed)
-        func_setup_formlayout.addRow('Alias', self.falias_le)
+        func_setup_formlayout.addRow("Alias", self.falias_le)
 
         target_layout = QHBoxLayout()
         self.target_cmbx = QComboBox()
-        self.target_cmbx.setToolTip('Set the target on which '
-                                    'the function shall operate')
+        self.target_cmbx.setToolTip(
+            "Set the target on which " "the function shall operate"
+        )
         self.target_cmbx.setEditable(False)
         self.target_cmbx.activated.connect(self.target_cmbx_changed)
         target_layout.addWidget(self.target_cmbx)
         self.target_chkl = QLabel()
         target_layout.addWidget(self.target_chkl)
-        func_setup_formlayout.addRow('Target', target_layout)
+        func_setup_formlayout.addRow("Target", target_layout)
 
         tab_layout = QHBoxLayout()
         self.tab_cmbx = QComboBox()
-        self.tab_cmbx.setToolTip('Choose the Tab for the function '
-                                 '(Compute/Plot/...)')
+        self.tab_cmbx.setToolTip(
+            "Choose the Tab for the function " "(Compute/Plot/...)"
+        )
         self.tab_cmbx.setEditable(True)
         self.tab_cmbx.activated.connect(self.tab_cmbx_changed)
         self.tab_cmbx.editTextChanged.connect(self.tab_cmbx_edited)
         tab_layout.addWidget(self.tab_cmbx)
         self.tab_chkl = QLabel()
         tab_layout.addWidget(self.tab_chkl)
-        func_setup_formlayout.addRow('Tab', tab_layout)
+        func_setup_formlayout.addRow("Tab", tab_layout)
 
         group_layout = QHBoxLayout()
         self.group_cmbx = QComboBox()
-        self.group_cmbx.setToolTip('Choose the function-group for the '
-                                   'function or create a new one')
+        self.group_cmbx.setToolTip(
+            "Choose the function-group for the " "function or create a new one"
+        )
         self.group_cmbx.setEditable(True)
         self.group_cmbx.activated.connect(self.group_cmbx_changed)
         self.group_cmbx.editTextChanged.connect(self.group_cmbx_edited)
         group_layout.addWidget(self.group_cmbx)
         self.group_chkl = QLabel()
         group_layout.addWidget(self.group_chkl)
-        func_setup_formlayout.addRow('Group', group_layout)
+        func_setup_formlayout.addRow("Group", group_layout)
 
         mtpl_layout = QHBoxLayout()
         self.mtpl_bts = QButtonGroup(self)
-        self.mtpl_yesbt = QPushButton('Yes')
+        self.mtpl_yesbt = QPushButton("Yes")
         self.mtpl_yesbt.setCheckable(True)
-        self.mtpl_nobt = QPushButton('No')
+        self.mtpl_nobt = QPushButton("No")
         self.mtpl_nobt.setCheckable(True)
-        self.mtpl_void = QPushButton('')
+        self.mtpl_void = QPushButton("")
         self.mtpl_void.setCheckable(True)
         self.mtpl_bts.addButton(self.mtpl_yesbt)
         self.mtpl_bts.addButton(self.mtpl_nobt)
         self.mtpl_bts.addButton(self.mtpl_void)
         mtpl_layout.addWidget(self.mtpl_yesbt)
         mtpl_layout.addWidget(self.mtpl_nobt)
         self.mtpl_yesbt.setToolTip(
-            'Choose, if the function contains an interactive Matplotlib-Plot')
-        self.mtpl_nobt.setToolTip('Choose, if the function contains '
-                                  'no interactive Matplotlib-Plot')
+            "Choose, if the function contains an interactive Matplotlib-Plot"
+        )
+        self.mtpl_nobt.setToolTip(
+            "Choose, if the function contains " "no interactive Matplotlib-Plot"
+        )
         self.mtpl_bts.buttonToggled.connect(self.mtpl_changed)
         self.mtpl_chkl = QLabel()
         mtpl_layout.addWidget(self.mtpl_chkl)
-        func_setup_formlayout.addRow('Matplotlib?', mtpl_layout)
+        func_setup_formlayout.addRow("Matplotlib?", mtpl_layout)
 
         myv_layout = QHBoxLayout()
         self.myv_bts = QButtonGroup(self)
-        self.myv_yesbt = QPushButton('Yes')
+        self.myv_yesbt = QPushButton("Yes")
         self.myv_yesbt.setCheckable(True)
-        self.myv_nobt = QPushButton('No')
+        self.myv_nobt = QPushButton("No")
         self.myv_nobt.setCheckable(True)
-        self.myv_void = QPushButton('')
+        self.myv_void = QPushButton("")
         self.myv_void.setCheckable(True)
         self.myv_bts.addButton(self.myv_yesbt)
         self.myv_bts.addButton(self.myv_nobt)
         self.myv_bts.addButton(self.myv_void)
         myv_layout.addWidget(self.myv_yesbt)
         myv_layout.addWidget(self.myv_nobt)
-        self.myv_yesbt.setToolTip('Choose, if the function contains '
-                                  'a Pyvista/Mayavi-Plot')
-        self.myv_nobt.setToolTip('Choose, if the function contains '
-                                 'a Pyvista/Mayavi-Plot')
+        self.myv_yesbt.setToolTip(
+            "Choose, if the function contains " "a Pyvista/Mayavi-Plot"
+        )
+        self.myv_nobt.setToolTip(
+            "Choose, if the function contains " "a Pyvista/Mayavi-Plot"
+        )
         self.myv_bts.buttonToggled.connect(self.myv_changed)
         self.myv_chkl = QLabel()
         myv_layout.addWidget(self.myv_chkl)
-        func_setup_formlayout.addRow('Pyvista/Mayavi?', myv_layout)
+        func_setup_formlayout.addRow("Pyvista/Mayavi?", myv_layout)
 
-        self.dpd_bt = QPushButton('Set Dependencies')
+        self.dpd_bt = QPushButton("Set Dependencies")
         self.dpd_bt.setToolTip(
-            'Set the functions that must be activated before or the '
-            'files that must be present for this function to work')
+            "Set the functions that must be activated before or the "
+            "files that must be present for this function to work"
+        )
         self.dpd_bt.clicked.connect(partial(SelectDependencies, self))
-        func_setup_formlayout.addRow('Dependencies', self.dpd_bt)
+        func_setup_formlayout.addRow("Dependencies", self.dpd_bt)
 
         func_setup_gbox.setLayout(func_setup_formlayout)
         setup_layout.addWidget(func_setup_gbox)
 
         # The Parameter-Setup-Group-Box
-        self.param_setup_gbox = QGroupBox('Parameter-Setup')
+        self.param_setup_gbox = QGroupBox("Parameter-Setup")
         self.param_setup_gbox.setAlignment(Qt.AlignHCenter)
         param_setup_layout = QVBoxLayout()
         self.exstparam_l = QLabel()
         self.exstparam_l.setWordWrap(True)
         self.exstparam_l.hide()
         param_setup_layout.addWidget(self.exstparam_l)
 
         self.param_view = QListView()
         self.param_model = CustomFunctionModel(self.add_pd_params)
         self.param_view.setModel(self.param_model)
         self.param_view.selectionModel().currentChanged.connect(
-            self.param_item_selected)
+            self.param_item_selected
+        )
         param_setup_layout.addWidget(self.param_view)
 
         param_setup_formlayout = QFormLayout()
         self.palias_le = QLineEdit()
-        self.palias_le.setToolTip('Set a name if you want something other '
-                                  'than the parameters-name')
+        self.palias_le.setToolTip(
+            "Set a name if you want something other " "than the parameters-name"
+        )
         self.palias_le.textEdited.connect(self.palias_changed)
-        param_setup_formlayout.addRow('Alias', self.palias_le)
+        param_setup_formlayout.addRow("Alias", self.palias_le)
 
         default_layout = QHBoxLayout()
         self.default_le = QLineEdit()
         self.default_le.setToolTip(
-            'Set the default for the parameter (it has to fit the gui-type!)')
+            "Set the default for the parameter (it has to fit the gui-type!)"
+        )
         self.default_le.textEdited.connect(self.pdefault_changed)
         default_layout.addWidget(self.default_le)
         self.default_chkl = QLabel()
         default_layout.addWidget(self.default_chkl)
-        param_setup_formlayout.addRow('Default', default_layout)
+        param_setup_formlayout.addRow("Default", default_layout)
 
         self.unit_le = QLineEdit()
-        self.unit_le.setToolTip('Set the unit for the parameter (optional)')
+        self.unit_le.setToolTip("Set the unit for the parameter (optional)")
         self.unit_le.textEdited.connect(self.punit_changed)
-        param_setup_formlayout.addRow('Unit', self.unit_le)
+        param_setup_formlayout.addRow("Unit", self.unit_le)
 
         self.description_le = QLineEdit()
-        self.description_le.setToolTip(
-            'Short description of the parameter (optional)')
+        self.description_le.setToolTip("Short description of the parameter (optional)")
         self.description_le.textEdited.connect(self.pdescription_changed)
-        param_setup_formlayout.addRow('Description', self.description_le)
+        param_setup_formlayout.addRow("Description", self.description_le)
 
         guitype_layout = QHBoxLayout()
         self.guitype_cmbx = QComboBox()
-        self.guitype_cmbx.setToolTip(
-            'Choose the GUI from the available GUIs')
+        self.guitype_cmbx.setToolTip("Choose the GUI from the available GUIs")
         self.guitype_cmbx.activated.connect(self.guitype_cmbx_changed)
         guitype_layout.addWidget(self.guitype_cmbx)
-        test_bt = QPushButton('Test')
+        test_bt = QPushButton("Test")
         test_bt.clicked.connect(self.show_param_gui)
         guitype_layout.addWidget(test_bt)
         self.guitype_chkl = QLabel()
         guitype_layout.addWidget(self.guitype_chkl)
-        param_setup_formlayout.addRow('GUI-Type', guitype_layout)
+        param_setup_formlayout.addRow("GUI-Type", guitype_layout)
 
-        self.guiargs_bt = QPushButton('Edit')
+        self.guiargs_bt = QPushButton("Edit")
         self.guiargs_bt.clicked.connect(partial(EditGuiArgsDlg, self))
-        self.guiargs_bt.setToolTip(
-            'Set Arguments for the GUI in a dict (optional)')
-        param_setup_formlayout.addRow('Additional Options', self.guiargs_bt)
+        self.guiargs_bt.setToolTip("Set Arguments for the GUI in a dict (optional)")
+        param_setup_formlayout.addRow("Additional Options", self.guiargs_bt)
 
         param_setup_layout.addLayout(param_setup_formlayout)
         self.param_setup_gbox.setLayout(param_setup_layout)
 
         setup_layout.addWidget(self.param_setup_gbox)
         layout.addLayout(setup_layout)
 
         bt_layout = QHBoxLayout()
 
-        save_bt = QPushButton('Save')
-        save_bt.setFont(QFont(QS().value('app_font'), 16))
+        save_bt = QPushButton("Save")
+        save_bt.setFont(QFont(QS().value("app_font"), 16))
         save_bt.clicked.connect(self.save_pkg)
         bt_layout.addWidget(save_bt)
 
-        src_bt = QPushButton('Show Code')
-        src_bt.setFont(QFont(QS().value('app_font'), 16))
+        src_bt = QPushButton("Show Code")
+        src_bt.setFont(QFont(QS().value("app_font"), 16))
         src_bt.clicked.connect(self.show_code)
         bt_layout.addWidget(src_bt)
 
-        close_bt = QPushButton('Quit')
-        close_bt.setFont(QFont(QS().value('app_font'), 16))
+        close_bt = QPushButton("Quit")
+        close_bt.setFont(QFont(QS().value("app_font"), 16))
         close_bt.clicked.connect(self.close)
         bt_layout.addWidget(close_bt)
 
         layout.addLayout(bt_layout)
 
         self.setLayout(layout)
 
@@ -576,16 +635,15 @@
         self.populate_group_cmbx()
         self.populate_guitype_cmbx()
 
     def update_func_cmbx(self):
         self.func_cmbx.clear()
         self.func_cmbx.insertItems(0, self.add_pd_funcs.index)
         try:
-            current_index = \
-                list(self.add_pd_funcs.index).index(self.current_function)
+            current_index = list(self.add_pd_funcs.index).index(self.current_function)
         except ValueError:
             current_index = 0
         self.func_cmbx.setCurrentIndex(current_index)
 
     def clear_func_items(self):
         self.falias_le.clear()
         self.target_cmbx.setCurrentIndex(-1)
@@ -613,459 +671,500 @@
 
     def func_item_selected(self, text):
         if text:
             self.current_function = text
             self.update_code_editor()
             self.update_func_setup()
 
-            if any([self.current_function in str(x)
-                    for x in self.add_pd_params['functions']]):
+            if any(
+                [
+                    self.current_function in str(x)
+                    for x in self.add_pd_params["functions"]
+                ]
+            ):
                 self.param_setup_gbox.setEnabled(True)
                 self.update_param_view()
-                self.current_parameter = \
-                    self.add_pd_params.loc[
-                        [self.current_function in str(x) for x in
-                         self.add_pd_params['functions']]].index[0]
+                self.current_parameter = self.add_pd_params.loc[
+                    [
+                        self.current_function in str(x)
+                        for x in self.add_pd_params["functions"]
+                    ]
+                ].index[0]
                 self.update_exst_param_label()
                 self.update_param_setup()
             else:
                 self.update_exst_param_label()
                 # Clear existing entries
                 self.clear_param_items()
 
     def param_item_selected(self, current):
         self.current_parameter = self.param_model.getData(current)
         self.update_param_setup()
         self.update_code_editor()
 
     def update_func_setup(self):
-        if pd.notna(self.add_pd_funcs.loc[self.current_function, 'alias']):
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "alias"]):
             self.falias_le.setText(
-                self.add_pd_funcs.loc[self.current_function, 'alias'])
+                self.add_pd_funcs.loc[self.current_function, "alias"]
+            )
         else:
             self.falias_le.clear()
-        if pd.notna(self.add_pd_funcs.loc[self.current_function, 'target']):
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "target"]):
             self.target_cmbx.setCurrentText(
-                self.add_pd_funcs.loc[self.current_function, 'target'])
+                self.add_pd_funcs.loc[self.current_function, "target"]
+            )
             self.target_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.target_cmbx.setCurrentIndex(-1)
             self.target_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
-        if pd.notna(self.add_pd_funcs.loc[self.current_function, 'tab']):
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "tab"]):
             self.tab_cmbx.setCurrentText(
-                self.add_pd_funcs.loc[self.current_function, 'tab'])
+                self.add_pd_funcs.loc[self.current_function, "tab"]
+            )
             self.tab_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.tab_cmbx.setCurrentIndex(-1)
             self.tab_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
-        if pd.notna(self.add_pd_funcs.loc[self.current_function, 'group']):
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "group"]):
             self.group_cmbx.setCurrentText(
-                self.add_pd_funcs.loc[self.current_function, 'group'])
+                self.add_pd_funcs.loc[self.current_function, "group"]
+            )
             self.group_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.group_cmbx.setCurrentIndex(-1)
             self.group_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
-        if pd.notna(
-                self.add_pd_funcs.loc[self.current_function, 'matplotlib']):
-            if self.add_pd_funcs.loc[self.current_function, 'matplotlib']:
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "matplotlib"]):
+            if self.add_pd_funcs.loc[self.current_function, "matplotlib"]:
                 self.mtpl_yesbt.setChecked(True)
             else:
                 self.mtpl_nobt.setChecked(True)
             self.mtpl_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.mtpl_void.setChecked(True)
             self.mtpl_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
-        if pd.notna(self.add_pd_funcs.loc[self.current_function, 'mayavi']):
-            if self.add_pd_funcs.loc[self.current_function, 'mayavi']:
+        if pd.notna(self.add_pd_funcs.loc[self.current_function, "mayavi"]):
+            if self.add_pd_funcs.loc[self.current_function, "mayavi"]:
                 self.myv_yesbt.setChecked(True)
             else:
                 self.myv_nobt.setChecked(True)
             self.myv_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.myv_void.setChecked(True)
             self.myv_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
 
     def update_exst_param_label(self):
         if self.current_function:
             if len(self.param_exst_dict[self.current_function]) > 0:
                 self.exstparam_l.setText(
-                    f'Already existing Parameters: '
-                    f'{self.param_exst_dict[self.current_function]}')
+                    f"Already existing Parameters: "
+                    f"{self.param_exst_dict[self.current_function]}"
+                )
                 self.exstparam_l.show()
             else:
                 self.exstparam_l.hide()
 
     def update_param_setup(self):
-        if pd.notna(self.add_pd_params.loc[self.current_parameter, 'alias']):
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "alias"]):
             self.palias_le.setText(
-                self.add_pd_params.loc[self.current_parameter, 'alias'])
+                self.add_pd_params.loc[self.current_parameter, "alias"]
+            )
         else:
             self.palias_le.clear()
-        if pd.notna(self.add_pd_params.loc[self.current_parameter, 'default']):
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "default"]):
             self.default_le.setText(
-                self.add_pd_params.loc[self.current_parameter, 'default'])
+                self.add_pd_params.loc[self.current_parameter, "default"]
+            )
             self.default_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.default_le.clear()
             self.default_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
-        if pd.notna(self.add_pd_params.loc[self.current_parameter, 'unit']):
-            self.unit_le.setText(
-                self.add_pd_params.loc[self.current_parameter, 'unit'])
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "unit"]):
+            self.unit_le.setText(self.add_pd_params.loc[self.current_parameter, "unit"])
         else:
             self.unit_le.clear()
-        if pd.notna(
-                self.add_pd_params.loc[self.current_parameter, 'description']):
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "description"]):
             self.description_le.setText(
-                self.add_pd_params.loc[self.current_parameter, 'description'])
+                self.add_pd_params.loc[self.current_parameter, "description"]
+            )
         else:
             self.description_le.clear()
-        if pd.notna(
-                self.add_pd_params.loc[self.current_parameter, 'gui_type']):
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "gui_type"]):
             self.guitype_cmbx.setCurrentText(
-                self.add_pd_params.loc[self.current_parameter, 'gui_type'])
+                self.add_pd_params.loc[self.current_parameter, "gui_type"]
+            )
             self.guitype_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
         else:
             self.guitype_cmbx.setCurrentIndex(-1)
             self.guitype_chkl.setPixmap(self.no_icon.pixmap(QSize(16, 16)))
 
     def check_func_setup(self):
         # Check, that all obligatory items of the Subject-Setup
         # and the Parameter-Setup are set.
-        if all([pd.notna(self.add_pd_funcs.loc[self.current_function, i]) for i
-                in
-                self.oblig_func]):
+        if all(
+            [
+                pd.notna(self.add_pd_funcs.loc[self.current_function, i])
+                for i in self.oblig_func
+            ]
+        ):
             function_params = self.add_pd_params.loc[
-                [self.current_function in str(x)
-                 for x in self.add_pd_params['functions']]]
-            if pd.notna(
-                    self.add_pd_params.loc[function_params.index,
-                                           self.oblig_params]).all().all():
+                [
+                    self.current_function in str(x)
+                    for x in self.add_pd_params["functions"]
+                ]
+            ]
+            if (
+                pd.notna(
+                    self.add_pd_params.loc[function_params.index, self.oblig_params]
+                )
+                .all()
+                .all()
+            ):
                 self.func_chkl.setPixmap(self.yes_icon.pixmap(16, 16))
-                self.add_pd_funcs.loc[self.current_function, 'ready'] = 1
+                self.add_pd_funcs.loc[self.current_function, "ready"] = 1
             else:
                 self.func_chkl.setPixmap(self.no_icon.pixmap(16, 16))
-                self.add_pd_funcs.loc[self.current_function, 'ready'] = 0
+                self.add_pd_funcs.loc[self.current_function, "ready"] = 0
 
     def update_param_view(self):
         # Update Param-Model with new pd_params of current_function
         current_pd_params = self.add_pd_params.loc[
-            [self.current_function in str(x)
-             for x in self.add_pd_params['functions']]
+            [self.current_function in str(x) for x in self.add_pd_params["functions"]]
         ]
         self.param_model.updateData(current_pd_params)
 
     def check_param_setup(self):
         # Check, that all obligatory items of the Parameter-Setup are set
-        if all([pd.notna(self.add_pd_params.loc[self.current_parameter, i])
-                for i in self.oblig_params]):
-            self.add_pd_params.loc[self.current_parameter, 'ready'] = 1
+        if all(
+            [
+                pd.notna(self.add_pd_params.loc[self.current_parameter, i])
+                for i in self.oblig_params
+            ]
+        ):
+            self.add_pd_params.loc[self.current_parameter, "ready"] = 1
         else:
-            self.add_pd_params.loc[self.current_parameter, 'ready'] = 0
+            self.add_pd_params.loc[self.current_parameter, "ready"] = 0
         self.update_param_view()
 
     # Line-Edit Change-Signals
     def falias_changed(self, text):
         if self.current_function:
-            self.add_pd_funcs.loc[self.current_function, 'alias'] = text
+            self.add_pd_funcs.loc[self.current_function, "alias"] = text
 
     def mtpl_changed(self, current_button, state):
         if self.current_function:
             if state and current_button == self.mtpl_yesbt:
-                self.add_pd_funcs.loc[
-                    self.current_function, 'matplotlib'] = True
+                self.add_pd_funcs.loc[self.current_function, "matplotlib"] = True
             elif state and current_button == self.mtpl_nobt:
-                self.add_pd_funcs.loc[
-                    self.current_function, 'matplotlib'] = False
+                self.add_pd_funcs.loc[self.current_function, "matplotlib"] = False
             if current_button != self.mtpl_void:
                 self.mtpl_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def myv_changed(self, current_button, state):
         if self.current_function:
             if state and current_button == self.myv_yesbt:
-                self.add_pd_funcs.loc[self.current_function, 'mayavi'] = True
+                self.add_pd_funcs.loc[self.current_function, "mayavi"] = True
             elif state and current_button == self.myv_nobt:
-                self.add_pd_funcs.loc[self.current_function, 'mayavi'] = False
+                self.add_pd_funcs.loc[self.current_function, "mayavi"] = False
             if current_button != self.myv_void:
                 self.myv_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def palias_changed(self, text):
         if self.current_parameter:
-            self.add_pd_params.loc[self.current_parameter, 'alias'] = text
+            self.add_pd_params.loc[self.current_parameter, "alias"] = text
 
     def pdefault_changed(self, text):
         if self.current_parameter:
-            self.add_pd_params.loc[self.current_parameter, 'default'] = text
+            self.add_pd_params.loc[self.current_parameter, "default"] = text
             self.default_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_param_setup()
             self.check_func_setup()
 
     def punit_changed(self, text):
         if self.current_parameter:
-            self.add_pd_params.loc[self.current_parameter, 'unit'] = text
+            self.add_pd_params.loc[self.current_parameter, "unit"] = text
 
     def pdescription_changed(self, text):
         if self.current_parameter:
-            self.add_pd_params.loc[self.current_parameter,
-                                   'description'] = text
+            self.add_pd_params.loc[self.current_parameter, "description"] = text
 
     def populate_target_cmbx(self):
-        self.target_cmbx.insertItems(0, ['MEEG', 'FSMRI', 'Group', 'Other'])
+        self.target_cmbx.insertItems(0, ["MEEG", "FSMRI", "Group", "Other"])
 
     def populate_tab_cmbx(self):
         self.tab_cmbx.clear()
-        tab_set = set(self.ct.pd_funcs['tab'])
-        tab_set2 = set(self.add_pd_funcs.loc[
-                           pd.notna(self.add_pd_funcs['tab']), 'tab'])
+        tab_set = set(self.ct.pd_funcs["tab"])
+        tab_set2 = set(self.add_pd_funcs.loc[pd.notna(self.add_pd_funcs["tab"]), "tab"])
         self.tab_cmbx.insertItems(0, tab_set | tab_set2)
 
     def populate_group_cmbx(self):
         self.group_cmbx.clear()
-        tab_set = set(self.ct.pd_funcs['group'])
-        tab_set2 = set(self.add_pd_funcs.loc[pd.notna(
-            self.add_pd_funcs['group']), 'group'])
+        tab_set = set(self.ct.pd_funcs["group"])
+        tab_set2 = set(
+            self.add_pd_funcs.loc[pd.notna(self.add_pd_funcs["group"]), "group"]
+        )
         self.group_cmbx.insertItems(0, tab_set | tab_set2)
 
     def populate_guitype_cmbx(self):
         self.guitype_cmbx.insertItems(0, self.available_param_guis)
 
     def target_cmbx_changed(self, idx):
         if self.current_function:
-            self.add_pd_funcs.loc[self.current_function,
-                                  'target'] = self.target_cmbx.itemText(idx)
+            self.add_pd_funcs.loc[
+                self.current_function, "target"
+            ] = self.target_cmbx.itemText(idx)
             self.target_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def tab_cmbx_changed(self, idx):
         # Insert changes from other functions if edited
         self.populate_tab_cmbx()
         self.tab_cmbx.setCurrentIndex(idx)
         if self.current_function:
-            self.add_pd_funcs.loc[self.current_function,
-                                  'tab'] = self.tab_cmbx.itemText(idx)
+            self.add_pd_funcs.loc[
+                self.current_function, "tab"
+            ] = self.tab_cmbx.itemText(idx)
             self.tab_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def tab_cmbx_edited(self, text):
-        if self.current_function and text != '':
-            self.add_pd_funcs.loc[self.current_function, 'tab'] = text
+        if self.current_function and text != "":
+            self.add_pd_funcs.loc[self.current_function, "tab"] = text
             self.tab_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def group_cmbx_changed(self, idx):
         # Insert changes from other functions if edited
         self.populate_group_cmbx()
         self.group_cmbx.setCurrentIndex(idx)
         group_name = self.group_cmbx.itemText(idx)
         if self.current_function:
-            self.add_pd_funcs.loc[self.current_function, 'group'] = group_name
+            self.add_pd_funcs.loc[self.current_function, "group"] = group_name
             for param in self.add_pd_params.index:
-                self.add_pd_params.loc[param, 'group'] = group_name
+                self.add_pd_params.loc[param, "group"] = group_name
             self.group_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def group_cmbx_edited(self, text):
-        if self.current_function and text != '':
-            self.add_pd_funcs.loc[self.current_function, 'group'] = text
+        if self.current_function and text != "":
+            self.add_pd_funcs.loc[self.current_function, "group"] = text
             for param in self.add_pd_params.index:
-                self.add_pd_params.loc[param, 'group'] = text
+                self.add_pd_params.loc[param, "group"] = text
             self.group_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def guitype_cmbx_changed(self, idx):
         text = self.guitype_cmbx.itemText(idx)
         gui_args = dict()
         options = list()
 
         if self.current_parameter:
             # If ComboGui or CheckListGui, options have to be set:
-            if text in ['ComboGui', 'CheckListGui']:
+            if text in ["ComboGui", "CheckListGui"]:
                 # Check if options already in gui_args
                 loaded_gui_args = self.add_pd_params.loc[
-                    self.current_parameter, 'gui_args']
+                    self.current_parameter, "gui_args"
+                ]
                 if pd.notna(loaded_gui_args):
                     gui_args = literal_eval(loaded_gui_args)
-                    if 'options' in gui_args:
-                        options = gui_args['options']
+                    if "options" in gui_args:
+                        options = gui_args["options"]
 
                 ChooseOptions(self, text, options)
 
                 # Save the gui_args in add_pd_params
-                gui_args['options'] = options
-                self.add_pd_params.loc[self.current_parameter,
-                                       'gui_args'] = str(gui_args)
+                gui_args["options"] = options
+                self.add_pd_params.loc[self.current_parameter, "gui_args"] = str(
+                    gui_args
+                )
 
             # Check, if default_value and gui_type match
-            if pd.notna(self.add_pd_params.loc[self.current_parameter,
-                                               'default']):
+            if pd.notna(self.add_pd_params.loc[self.current_parameter, "default"]):
                 result, _ = self.test_param_gui(
                     default_string=self.add_pd_params.loc[
-                        self.current_parameter, 'default'],
-                    gui_type=text, gui_args=gui_args)
+                        self.current_parameter, "default"
+                    ],
+                    gui_type=text,
+                    gui_args=gui_args,
+                )
             else:
                 result = None
 
             if not result:
-                self.add_pd_params.loc[self.current_parameter,
-                                       'gui_type'] = text
-                self.guitype_chkl.setPixmap(
-                    self.yes_icon.pixmap(QSize(16, 16)))
+                self.add_pd_params.loc[self.current_parameter, "gui_type"] = text
+                self.guitype_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
                 self.check_param_setup()
                 self.check_func_setup()
             else:
                 self.guitype_cmbx.setCurrentIndex(-1)
-                self.add_pd_params.loc[self.current_parameter,
-                                       'gui_type'] = None
+                self.add_pd_params.loc[self.current_parameter, "gui_type"] = None
                 self.check_param_setup()
                 self.check_func_setup()
 
     def pguiargs_changed(self, gui_args):
         if self.current_parameter:
             # Check, if default_value and gui_type match
             if pd.notna(
-                    self.add_pd_params.loc[self.current_parameter,
-                                           ['default', 'gui_type']]).all():
+                self.add_pd_params.loc[self.current_parameter, ["default", "gui_type"]]
+            ).all():
                 result, _ = self.test_param_gui(
                     default_string=self.add_pd_params.loc[
-                        self.current_parameter, 'default'],
-                    gui_type=self.add_pd_params.loc[
-                        self.current_parameter, 'gui_type'],
-                    gui_args=gui_args)
+                        self.current_parameter, "default"
+                    ],
+                    gui_type=self.add_pd_params.loc[self.current_parameter, "gui_type"],
+                    gui_args=gui_args,
+                )
             else:
                 result = None
 
             if not result:
-                self.add_pd_params.loc[self.current_parameter,
-                                       'gui_args'] = str(gui_args)
+                self.add_pd_params.loc[self.current_parameter, "gui_args"] = str(
+                    gui_args
+                )
             else:
-                self.add_pd_params.loc[self.current_parameter,
-                                       'gui_args'] = None
+                self.add_pd_params.loc[self.current_parameter, "gui_args"] = None
 
     def get_functions(self):
         # Clear Function- and Parameter-DataFrame
         self.add_pd_funcs.drop(index=self.add_pd_funcs.index, inplace=True)
         self.add_pd_params.drop(index=self.add_pd_funcs.index, inplace=True)
         self.clear_func_items()
         self.clear_param_items()
 
         # Returns tuple of files-list and file-type
         cf_path_string = QFileDialog.getOpenFileName(
-            self, 'Choose the Python-File containing your function to import',
-            filter='Python-File (*.py)')[0]
+            self,
+            "Choose the Python-File containing your function to import",
+            filter="Python-File (*.py)",
+        )[0]
         if cf_path_string:
             self.file_path = Path(cf_path_string)
             ImportFuncs(self)
 
     def edit_functions(self):
         # Clear Function- and Parameter-DataFrame
         self.add_pd_funcs.drop(index=self.add_pd_funcs.index, inplace=True)
         self.add_pd_params.drop(index=self.add_pd_funcs.index, inplace=True)
         self.clear_func_items()
         self.clear_param_items()
 
         # Returns tuple of files-list and file-type
         cf_path_string = QFileDialog.getOpenFileName(
-            self, 'Choose the Python-File containing the functions to edit',
-            filter='Python-File (*.py)', directory=self.ct.custom_pkg_path)[0]
+            self,
+            "Choose the Python-File containing the functions to edit",
+            filter="Python-File (*.py)",
+            directory=self.ct.custom_pkg_path,
+        )[0]
         if cf_path_string:
             self.file_path = Path(cf_path_string)
             ImportFuncs(self, edit_existing=True)
 
     def test_param_gui(self, default_string, gui_type, gui_args=None):
         # Test ParamGui with Value
         if gui_args is None:
             gui_args = {}
         test_parameters = dict()
         try:
-            test_parameters[self.current_parameter] = \
-                literal_eval(default_string)
+            test_parameters[self.current_parameter] = literal_eval(default_string)
         except (ValueError, SyntaxError):
             # Allow parameters to be defined by functions by numpy, etc.
-            if self.add_pd_params.loc[self.current_parameter, 'gui_type'] \
-                    == 'FuncGui':
+            if self.add_pd_params.loc[self.current_parameter, "gui_type"] == "FuncGui":
                 test_parameters[self.current_parameter] = eval(default_string)
             else:
                 test_parameters[self.current_parameter] = default_string
-        if pd.notna(self.add_pd_params.loc[self.current_parameter, 'alias']):
-            alias = self.add_pd_params.loc[self.current_parameter, 'alias']
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "alias"]):
+            alias = self.add_pd_params.loc[self.current_parameter, "alias"]
         else:
             alias = self.current_parameter
-        if pd.notna(self.add_pd_params.loc[self.current_parameter,
-                                           'description']):
-            description = self.add_pd_params.loc[self.current_parameter,
-                                                 'description']
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "description"]):
+            description = self.add_pd_params.loc[self.current_parameter, "description"]
         else:
             description = None
-        if pd.notna(self.add_pd_params.loc[self.current_parameter, 'unit']):
-            param_unit = self.add_pd_params.loc[self.current_parameter, 'unit']
+        if pd.notna(self.add_pd_params.loc[self.current_parameter, "unit"]):
+            param_unit = self.add_pd_params.loc[self.current_parameter, "unit"]
         else:
             param_unit = None
 
         gui_handle = getattr(parameter_widgets, gui_type)
         handle_params = inspect.signature(gui_handle).parameters
         try:
-            if 'param_unit' in handle_params:
-                gui = gui_handle(data=test_parameters,
-                                 name=self.current_parameter,
-                                 alias=alias, description=description,
-                                 param_unit=param_unit, **gui_args)
+            if "param_unit" in handle_params:
+                gui = gui_handle(
+                    data=test_parameters,
+                    name=self.current_parameter,
+                    alias=alias,
+                    description=description,
+                    param_unit=param_unit,
+                    **gui_args,
+                )
             else:
-                gui = gui_handle(data=test_parameters,
-                                 name=self.current_parameter,
-                                 alias=alias, description=description,
-                                 **gui_args)
+                gui = gui_handle(
+                    data=test_parameters,
+                    name=self.current_parameter,
+                    alias=alias,
+                    description=description,
+                    **gui_args,
+                )
         except Exception as e:
             gui = None
             result = e
-            QMessageBox.warning(self, 'Error in ParamGui',
-                                f'The execution of {gui_type} with '
-                                f'{default_string} as default and '
-                                '{gui_args} as additional parameters raises'
-                                ' the following error:\n'
-                                f'{result}')
+            QMessageBox.warning(
+                self,
+                "Error in ParamGui",
+                f"The execution of {gui_type} with "
+                f"{default_string} as default and "
+                "{gui_args} as additional parameters raises"
+                " the following error:\n"
+                f"{result}",
+            )
         else:
             result = None
 
         return result, gui
 
     def show_param_gui(self):
         if self.current_parameter and pd.notna(
-                self.add_pd_params.loc[self.current_parameter, 'gui_type']):
+            self.add_pd_params.loc[self.current_parameter, "gui_type"]
+        ):
             TestParamGui(self)
 
     def update_code_editor(self):
         if self.code_editor:
             self.code_editor.clear()
-            self.code_editor.insertPlainText(self.code_dict[
-                                                 self.current_function])
+            self.code_editor.insertPlainText(self.code_dict[self.current_function])
 
     def show_code(self):
         self.code_editor = CodeEditor(self)
         self.code_editor.setReadOnly(True)
         self.update_code_editor()
-        code_dialog = SimpleDialog(self.code_editor, parent=self, modal=False,
-                                   window_title='Source-Code')
+        code_dialog = SimpleDialog(
+            self.code_editor, parent=self, modal=False, window_title="Source-Code"
+        )
         set_ratio_geometry(0.5, code_dialog)
         center(code_dialog)
 
     def save_pkg(self):
-        if any(self.add_pd_funcs['ready'] == 1):
+        if any(self.add_pd_funcs["ready"] == 1):
             SavePkgDialog(self)
 
     def closeEvent(self, event):
-        drop_funcs = [f for f in self.add_pd_funcs.index
-                      if not self.add_pd_funcs.loc[f, 'ready']]
+        drop_funcs = [
+            f for f in self.add_pd_funcs.index if not self.add_pd_funcs.loc[f, "ready"]
+        ]
 
         if len(drop_funcs) > 0:
-            answer = QMessageBox.question(self, 'Close Custom-Functions?',
-                                          f'There are still '
-                                          f'unfinished functions:\n'
-                                          f'{drop_funcs}\n'
-                                          f'Do you still want to quit?')
+            answer = QMessageBox.question(
+                self,
+                "Close Custom-Functions?",
+                f"There are still "
+                f"unfinished functions:\n"
+                f"{drop_funcs}\n"
+                f"Do you still want to quit?",
+            )
         else:
             answer = None
 
         if answer == QMessageBox.Yes or answer is None:
             event.accept()
         else:
             event.ignore()
@@ -1090,171 +1189,199 @@
         self.open()
 
     def load_function_list(self):
         # Load .csv-Files if
         try:
             if self.edit_existing:
                 self.cf.pkg_name = self.cf.file_path.parent.name
-                pd_funcs_path = join(self.cf.file_path.parent,
-                                     f'{self.cf.pkg_name}_functions.csv')
-                pd_params_path = join(self.cf.file_path.parent,
-                                      f'{self.cf.pkg_name}_parameters.csv')
-                self.cf.add_pd_funcs = pd.read_csv(pd_funcs_path,
-                                                   sep=';', index_col=0)
-                self.cf.add_pd_params = pd.read_csv(pd_params_path,
-                                                    sep=';', index_col=0)
+                pd_funcs_path = join(
+                    self.cf.file_path.parent, f"{self.cf.pkg_name}_functions.csv"
+                )
+                pd_params_path = join(
+                    self.cf.file_path.parent, f"{self.cf.pkg_name}_parameters.csv"
+                )
+                self.cf.add_pd_funcs = pd.read_csv(
+                    pd_funcs_path,
+                    sep=";",
+                    index_col=0,
+                    na_values=[""],
+                    keep_default_na=False,
+                )
+                self.cf.add_pd_params = pd.read_csv(
+                    pd_params_path,
+                    sep=";",
+                    index_col=0,
+                    na_values=[""],
+                    keep_default_na=False,
+                )
 
                 # Can be removed soon, when nobody uses
                 # old packages anymore (10.11.2020)
-                if 'target' not in self.cf.add_pd_funcs.columns:
-                    self.cf.add_pd_funcs['target'] = None
+                if "target" not in self.cf.add_pd_funcs.columns:
+                    self.cf.add_pd_funcs["target"] = None
             else:
                 self.cf.pkg_name = None
-            spec = util.spec_from_file_location(self.cf.file_path.stem,
-                                                self.cf.file_path)
+            spec = util.spec_from_file_location(
+                self.cf.file_path.stem, self.cf.file_path
+            )
             self.module = util.module_from_spec(spec)
             spec.loader.exec_module(self.module)
-        except:  # noqa: E722
+        except Exception:
             err = get_exception_tuple()
             ErrorDialog(err, self)
         else:
             for func_key in self.module.__dict__:
                 func = self.module.__dict__[func_key]
                 # Only functions are allowed
                 # (Classes should be called from function!)
-                if type(func) == FunctionType \
-                        and func.__module__ == self.module.__name__:
+                if (
+                    type(func) == FunctionType
+                    and func.__module__ == self.module.__name__
+                ):
                     # Check, if function is already existing
                     if func_key in self.cf.exst_functions:
-                        if self.edit_existing \
-                                and func_key in self.cf.add_pd_funcs.index:
+                        if (
+                            self.edit_existing
+                            and func_key in self.cf.add_pd_funcs.index
+                        ):
                             self.edit_loaded_cfs.append(func_key)
                         else:
                             self.already_existing_funcs.append(func_key)
                     else:
                         self.loaded_cfs.append(func_key)
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         if len(self.already_existing_funcs) > 0:
-            exst_label = QLabel(f'These functions already exist: '
-                                f'{self.already_existing_funcs}')
+            exst_label = QLabel(
+                f"These functions already exist: " f"{self.already_existing_funcs}"
+            )
             exst_label.setWordWrap(True)
             layout.addWidget(exst_label)
 
         view_layout = QHBoxLayout()
-        load_list = CheckList(self.loaded_cfs, self.selected_cfs,
-                              ui_button_pos='bottom', title='New functions')
+        load_list = CheckList(
+            self.loaded_cfs,
+            self.selected_cfs,
+            ui_button_pos="bottom",
+            title="New functions",
+        )
         view_layout.addWidget(load_list)
 
         if len(self.edit_loaded_cfs) > 0:
-            edit_list = CheckList(self.edit_loaded_cfs, self.selected_edit_cfs,
-                                  ui_button_pos='bottom',
-                                  title='Functions to edit')
+            edit_list = CheckList(
+                self.edit_loaded_cfs,
+                self.selected_edit_cfs,
+                ui_button_pos="bottom",
+                title="Functions to edit",
+            )
             view_layout.addWidget(edit_list)
 
         layout.addLayout(view_layout)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
-        self.setWindowTitle('Choose Functions')
+        self.setWindowTitle("Choose Functions")
         self.setLayout(layout)
 
     def load_selected_functions(self):
-        selected_funcs = [cf for cf in self.loaded_cfs
-                          if cf in self.selected_cfs] + \
-                         [cf for cf in self.edit_loaded_cfs
-                          if cf in self.selected_edit_cfs]
+        selected_funcs = [cf for cf in self.loaded_cfs if cf in self.selected_cfs] + [
+            cf for cf in self.edit_loaded_cfs if cf in self.selected_edit_cfs
+        ]
         if self.edit_existing:
             # Drop Functions which are not selected
             self.cf.add_pd_funcs.drop(
-                index=[f for f in self.cf.add_pd_funcs.index
-                       if f not in selected_funcs],
-                inplace=True)
+                index=[
+                    f for f in self.cf.add_pd_funcs.index if f not in selected_funcs
+                ],
+                inplace=True,
+            )
 
         for func_key in selected_funcs:
             func = self.module.__dict__[func_key]
 
-            self.cf.add_pd_funcs.loc[func_key, 'module'] = self.module.__name__
-            self.cf.add_pd_funcs.loc[func_key, 'ready'] = 0
+            self.cf.add_pd_funcs.loc[func_key, "module"] = self.module.__name__
+            self.cf.add_pd_funcs.loc[func_key, "ready"] = 0
 
             self.cf.code_dict[func_key] = inspect.getsource(func)
 
             # Get Parameters and divide them in existing and setup
             all_parameters = list(inspect.signature(func).parameters)
-            self.cf.add_pd_funcs.loc[func_key, 'func_args'] = \
-                ','.join(all_parameters)
+            self.cf.add_pd_funcs.loc[func_key, "func_args"] = ",".join(all_parameters)
             existing_parameters = []
 
             for param_key in all_parameters:
                 if param_key in self.cf.exst_parameters:
                     existing_parameters.append(param_key)
                 else:
                     # Check if ready (possible when editing functions)
-                    self.cf.add_pd_params.loc[param_key, 'ready'] = 0
-                    if pd.notna(self.cf.add_pd_params.loc[
-                                    param_key, self.cf.oblig_params]).all():
-                        self.cf.add_pd_params.loc[param_key, 'ready'] = 1
+                    self.cf.add_pd_params.loc[param_key, "ready"] = 0
+                    if pd.notna(
+                        self.cf.add_pd_params.loc[param_key, self.cf.oblig_params]
+                    ).all():
+                        self.cf.add_pd_params.loc[param_key, "ready"] = 1
 
                     # functions (which are using param) is a continuous string
                     # (because pandas can't store a list as item)
                     if param_key in self.cf.add_pd_params.index:
-                        if 'functions' in self.cf.add_pd_params.columns:
-                            if pd.notna(self.cf.add_pd_params.loc[
-                                            param_key, 'functions']):
+                        if "functions" in self.cf.add_pd_params.columns:
+                            if pd.notna(
+                                self.cf.add_pd_params.loc[param_key, "functions"]
+                            ):
                                 self.cf.add_pd_params.loc[
-                                    param_key, 'functions'] += func_key
+                                    param_key, "functions"
+                                ] += func_key
                             else:
                                 self.cf.add_pd_params.loc[
-                                    param_key, 'functions'] = func_key
+                                    param_key, "functions"
+                                ] = func_key
                         else:
-                            self.cf.add_pd_params.loc[
-                                param_key, 'functions'] = func_key
+                            self.cf.add_pd_params.loc[param_key, "functions"] = func_key
                     else:
-                        self.cf.add_pd_params.loc[
-                            param_key, 'functions'] = func_key
+                        self.cf.add_pd_params.loc[param_key, "functions"] = func_key
 
             self.cf.param_exst_dict[func_key] = existing_parameters
 
         # Check, if mandatory columns exist
-        if 'ready' not in self.cf.add_pd_params.columns:
-            self.cf.add_pd_params['ready'] = 0
-        if 'functions' not in self.cf.add_pd_params.columns:
-            self.cf.add_pd_params['functions'] = ''
+        if "ready" not in self.cf.add_pd_params.columns:
+            self.cf.add_pd_params["ready"] = 0
+        if "functions" not in self.cf.add_pd_params.columns:
+            self.cf.add_pd_params["functions"] = ""
 
     def closeEvent(self, event):
         self.load_selected_functions()
         self.cf.update_func_cmbx()
         self.cf.update_exst_param_label()
         if self.cf.code_editor:
             self.cf.code_editor.update_code()
         event.accept()
 
 
 class SelectDependencies(QDialog):
     def __init__(self, cf_dialog):
         super().__init__(cf_dialog)
         self.cf_dialog = cf_dialog
-        if pd.notna(cf_dialog.add_pd_funcs.loc[cf_dialog.current_function,
-                                               'dependencies']):
+        if pd.notna(
+            cf_dialog.add_pd_funcs.loc[cf_dialog.current_function, "dependencies"]
+        ):
             self.dpd_list = literal_eval(
-                cf_dialog.add_pd_funcs.loc[cf_dialog.current_function,
-                                           'dependencies'])
+                cf_dialog.add_pd_funcs.loc[cf_dialog.current_function, "dependencies"]
+            )
         else:
             self.dpd_list = []
 
         layout = QVBoxLayout()
         self.listw = QListWidget()
         self.listw.itemChanged.connect(self.item_checked)
         layout.addWidget(self.listw)
 
-        ok_bt = QPushButton('OK')
+        ok_bt = QPushButton("OK")
         ok_bt.clicked.connect(self.close_dlg)
         layout.addWidget(ok_bt)
 
         self.populate_listw()
         self.setLayout(layout)
         self.open()
 
@@ -1271,58 +1398,59 @@
     def item_checked(self, item):
         if item.checkState == Qt.Checked:
             self.dpd_list.append(item.text())
         elif item.text() in self.dpd_list:
             self.dpd_list.remove(item.text())
 
     def close_dlg(self):
-        self.cf_dialog.add_pd_funcs.loc[self.cf_dialog.current_function,
-                                        'dependencies'] = str(
-            self.dpd_list)
+        self.cf_dialog.add_pd_funcs.loc[
+            self.cf_dialog.current_function, "dependencies"
+        ] = str(self.dpd_list)
         self.close()
 
 
 class TestParamGui(QDialog):
     def __init__(self, cf_dialog):
         super().__init__(cf_dialog)
         self.cf = cf_dialog
         # Dict as Replacement for Parameters in Project for Testing
         self.test_parameters = dict()
 
-        default_string = self.cf.add_pd_params.loc[self.cf.current_parameter,
-                                                   'default']
-        gui_type = self.cf.add_pd_params.loc[self.cf.current_parameter,
-                                             'gui_type']
+        default_string = self.cf.add_pd_params.loc[self.cf.current_parameter, "default"]
+        gui_type = self.cf.add_pd_params.loc[self.cf.current_parameter, "gui_type"]
         try:
             gui_args = literal_eval(
-                self.cf.add_pd_params.loc[self.cf.current_parameter,
-                                          'gui_args'])
+                self.cf.add_pd_params.loc[self.cf.current_parameter, "gui_args"]
+            )
         except (SyntaxError, ValueError):
             gui_args = {}
 
-        self.result, self.gui = self.cf.test_param_gui(default_string,
-                                                       gui_type, gui_args)
+        self.result, self.gui = self.cf.test_param_gui(
+            default_string, gui_type, gui_args
+        )
 
         if not self.result:
             self.init_ui()
             self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         # Allow Enter-Press without closing the dialog
-        if self.cf.add_pd_params.loc[self.cf.current_parameter,
-                                     'gui_type'] == 'FuncGui':
+        if (
+            self.cf.add_pd_params.loc[self.cf.current_parameter, "gui_type"]
+            == "FuncGui"
+        ):
             void_bt = QPushButton()
             void_bt.setDefault(True)
             layout.addWidget(void_bt)
 
         layout.addWidget(self.gui)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
         self.setLayout(layout)
 
 
 class SavePkgDialog(QDialog):
     def __init__(self, cf_dialog):
@@ -1335,199 +1463,235 @@
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         self.func_list = SimpleList(
-            list(self.cf_dialog.add_pd_funcs.loc[
-                     self.cf_dialog.add_pd_funcs['ready'] == 1].index))
+            list(
+                self.cf_dialog.add_pd_funcs.loc[
+                    self.cf_dialog.add_pd_funcs["ready"] == 1
+                ].index
+            )
+        )
         layout.addWidget(self.func_list)
 
-        pkg_name_label = QLabel('Package-Name:')
+        pkg_name_label = QLabel("Package-Name:")
         layout.addWidget(pkg_name_label)
 
         self.pkg_le = QLineEdit()
         if self.cf_dialog.pkg_name:
             self.pkg_le.setText(self.cf_dialog.pkg_name)
         self.pkg_le.textEdited.connect(self.pkg_le_changed)
         layout.addWidget(self.pkg_le)
 
-        save_bt = QPushButton('Save')
+        save_bt = QPushButton("Save")
         save_bt.clicked.connect(self.save_pkg)
         layout.addWidget(save_bt)
 
-        cancel_bt = QPushButton('Cancel')
+        cancel_bt = QPushButton("Cancel")
         cancel_bt.clicked.connect(self.close)
         layout.addWidget(cancel_bt)
         self.setLayout(layout)
 
     def pkg_le_changed(self, text):
-        if text != '':
+        if text != "":
             self.my_pkg_name = text
 
     def save_pkg(self):
         if self.my_pkg_name or self.cf_dialog.pkg_name:
             # Drop all functions with unfinished setup
             # and add the remaining to the main_window-DataFrame
             drop_funcs = self.cf_dialog.add_pd_funcs.loc[
-                self.cf_dialog.add_pd_funcs['ready'] == 0].index
-            final_add_pd_funcs = self.cf_dialog.add_pd_funcs.drop(
-                index=drop_funcs)
+                self.cf_dialog.add_pd_funcs["ready"] == 0
+            ].index
+            final_add_pd_funcs = self.cf_dialog.add_pd_funcs.drop(index=drop_funcs)
 
             drop_params = list()
             for param in self.cf_dialog.add_pd_params.index:
-                if not any([f in str(self.cf_dialog.add_pd_params.loc[
-                                         param, 'functions'])
-                            for f in final_add_pd_funcs.index]):
+                if not any(
+                    [
+                        f in str(self.cf_dialog.add_pd_params.loc[param, "functions"])
+                        for f in final_add_pd_funcs.index
+                    ]
+                ):
                     drop_params.append(param)
-            final_add_pd_params = \
-                self.cf_dialog.add_pd_params.drop(index=drop_params)
+            final_add_pd_params = self.cf_dialog.add_pd_params.drop(index=drop_params)
 
             # Remove no longer needed columns
-            del final_add_pd_funcs['ready']
-            del final_add_pd_params['ready']
-            del final_add_pd_params['functions']
+            del final_add_pd_funcs["ready"]
+            del final_add_pd_params["ready"]
+            del final_add_pd_params["functions"]
 
             # Todo: Make this more failproof
             #  (loading and saving already existing packages)
             # This is only not None, when the function
             # was imported by edit-functions
             if self.cf_dialog.pkg_name:
                 # Update and overwrite existing settings for funcs and params
-                self.pkg_path = join(self.cf_dialog.ct.custom_pkg_path,
-                                     self.cf_dialog.pkg_name)
-                pd_funcs_path = \
-                    join(self.pkg_path,
-                         f'{self.cf_dialog.pkg_name}_functions.csv')
-                pd_params_path = \
-                    join(self.pkg_path,
-                         f'{self.cf_dialog.pkg_name}_parameters.csv')
+                self.pkg_path = join(
+                    self.cf_dialog.ct.custom_pkg_path, self.cf_dialog.pkg_name
+                )
+                pd_funcs_path = join(
+                    self.pkg_path, f"{self.cf_dialog.pkg_name}_functions.csv"
+                )
+                pd_params_path = join(
+                    self.pkg_path, f"{self.cf_dialog.pkg_name}_parameters.csv"
+                )
                 if isfile(pd_funcs_path):
-                    read_pd_funcs = pd.read_csv(pd_funcs_path, sep=';',
-                                                index_col=0)
+                    read_pd_funcs = pd.read_csv(
+                        pd_funcs_path,
+                        sep=";",
+                        index_col=0,
+                        na_values=[""],
+                        keep_default_na=False,
+                    )
                     # Replace indexes from file with same name
-                    drop_funcs = [f for f in read_pd_funcs.index
-                                  if f in final_add_pd_funcs.index]
+                    drop_funcs = [
+                        f for f in read_pd_funcs.index if f in final_add_pd_funcs.index
+                    ]
                     read_pd_funcs.drop(index=drop_funcs, inplace=True)
-                    final_add_pd_funcs = \
-                        read_pd_funcs.append(final_add_pd_funcs)
+                    final_add_pd_funcs = pd.concat([read_pd_funcs, final_add_pd_funcs])
                 if isfile(pd_params_path):
-                    read_pd_params = pd.read_csv(pd_params_path, sep=';',
-                                                 index_col=0)
+                    read_pd_params = pd.read_csv(
+                        pd_params_path,
+                        sep=";",
+                        index_col=0,
+                        na_values=[""],
+                        keep_default_na=False,
+                    )
                     # Replace indexes from file with same name
-                    drop_params = [p for p in read_pd_params.index if
-                                   p in final_add_pd_params.index]
+                    drop_params = [
+                        p
+                        for p in read_pd_params.index
+                        if p in final_add_pd_params.index
+                    ]
                     read_pd_params.drop(index=drop_params, inplace=True)
-                    final_add_pd_params = read_pd_params.append(
-                        final_add_pd_params)
+                    final_add_pd_params = pd.concat(
+                        [read_pd_params, final_add_pd_params]
+                    )
 
-                if self.my_pkg_name \
-                        and self.my_pkg_name != self.cf_dialog.pkg_name:
+                if self.my_pkg_name and self.my_pkg_name != self.cf_dialog.pkg_name:
                     # Rename folder and .csv-files if you enter a new name
-                    new_pkg_path = join(self.cf_dialog.ct.custom_pkg_path,
-                                        self.my_pkg_name)
+                    new_pkg_path = join(
+                        self.cf_dialog.ct.custom_pkg_path, self.my_pkg_name
+                    )
                     os.rename(self.pkg_path, new_pkg_path)
 
-                    new_pd_funcs_path = \
-                        join(new_pkg_path, f'{self.my_pkg_name}_functions.csv')
+                    new_pd_funcs_path = join(
+                        new_pkg_path, f"{self.my_pkg_name}_functions.csv"
+                    )
                     os.rename(pd_funcs_path, new_pd_funcs_path)
                     pd_funcs_path = new_pd_funcs_path
 
-                    new_pd_params_path = \
-                        join(new_pkg_path,
-                             f'{self.my_pkg_name}_parameters.csv')
+                    new_pd_params_path = join(
+                        new_pkg_path, f"{self.my_pkg_name}_parameters.csv"
+                    )
                     os.rename(pd_params_path, new_pd_params_path)
                     pd_params_path = new_pd_params_path
 
             else:
-                self.pkg_path = \
-                    join(self.cf_dialog.ct.custom_pkg_path, self.my_pkg_name)
+                self.pkg_path = join(
+                    self.cf_dialog.ct.custom_pkg_path, self.my_pkg_name
+                )
                 if not isdir(self.pkg_path):
                     mkdir(self.pkg_path)
                 # Create __init__.py to make it a package
-                with open(join(self.pkg_path, '__init__.py'), 'w') as f:
-                    f.write('')
+                with open(join(self.pkg_path, "__init__.py"), "w") as f:
+                    f.write("")
                 # Copy Origin-Script to Destination
-                pd_funcs_path = join(self.pkg_path,
-                                     f'{self.my_pkg_name}_functions.csv')
-                pd_params_path = join(self.pkg_path,
-                                      f'{self.my_pkg_name}_parameters.csv')
+                pd_funcs_path = join(self.pkg_path, f"{self.my_pkg_name}_functions.csv")
+                pd_params_path = join(
+                    self.pkg_path, f"{self.my_pkg_name}_parameters.csv"
+                )
                 dest_path = join(self.pkg_path, self.cf_dialog.file_path.name)
                 shutil.copy2(self.cf_dialog.file_path, dest_path)
 
             # Add pkg_name as column if not already existing
-            if 'pkg_name' in final_add_pd_funcs:
-                final_add_pd_funcs['pkg_name'] = self.my_pkg_name
+            if "pkg_name" in final_add_pd_funcs:
+                final_add_pd_funcs["pkg_name"] = self.my_pkg_name
             else:
-                final_add_pd_funcs.insert(len(final_add_pd_funcs.columns) - 1,
-                                          'pkg_name', self.my_pkg_name)
-
-            final_add_pd_funcs.to_csv(pd_funcs_path, sep=';')
-            final_add_pd_params.to_csv(pd_params_path, sep=';')
-
-            for func in [f for f in final_add_pd_funcs.index if
-                         f in self.cf_dialog.add_pd_funcs.index]:
+                final_add_pd_funcs.insert(
+                    len(final_add_pd_funcs.columns) - 1, "pkg_name", self.my_pkg_name
+                )
+
+            final_add_pd_funcs.to_csv(pd_funcs_path, sep=";")
+            final_add_pd_params.to_csv(pd_params_path, sep=";")
+
+            for func in [
+                f
+                for f in final_add_pd_funcs.index
+                if f in self.cf_dialog.add_pd_funcs.index
+            ]:
                 self.cf_dialog.add_pd_funcs.drop(index=func, inplace=True)
             self.cf_dialog.update_func_cmbx()
-            for param in [p for p in final_add_pd_params.index if
-                          p in self.cf_dialog.add_pd_params]:
+            for param in [
+                p
+                for p in final_add_pd_params.index
+                if p in self.cf_dialog.add_pd_params
+            ]:
                 self.cf_dialog.add_pd_params.drop(index=param, inplace=True)
             self.cf_dialog.clear_func_items()
             self.cf_dialog.clear_param_items()
 
             # Add to selected modules
-            self.cf_dialog.ct.settings['selected_modules'].append(
-                self.cf_dialog.file_path.stem)
+            self.cf_dialog.ct.settings["selected_modules"].append(
+                self.cf_dialog.file_path.stem
+            )
             self.cf_dialog.ct.save_settings()
 
             self.cf_dialog.ct.import_custom_modules()
             self.cf_dialog.mw.redraw_func_and_param()
             # ToDo: MP
             # init_mp_pool()
             self.close()
 
         else:
             # If no valid pkg_name is existing
-            QMessageBox.warning(self, 'No valid Package-Name!',
-                                'You need to enter a valid Package-Name!')
+            QMessageBox.warning(
+                self,
+                "No valid Package-Name!",
+                "You need to enter a valid Package-Name!",
+            )
 
 
 class ChooseCustomModules(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
-        self.modules = {pkg_name: self.ct.all_modules[pkg_name]
-                        for pkg_name in self.ct.all_modules}
-        self.selected_modules = self.ct.get_setting('selected_modules')
+        self.modules = {
+            pkg_name: self.ct.all_modules[pkg_name] for pkg_name in self.ct.all_modules
+        }
+        self.selected_modules = self.ct.get_setting("selected_modules")
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         self.layout = QVBoxLayout()
 
         tab_widget = QTabWidget()
 
         for pkg_name in self.modules:
-            list_widget = CheckList(data=self.modules[pkg_name],
-                                    checked=self.selected_modules)
+            list_widget = CheckList(
+                data=self.modules[pkg_name], checked=self.selected_modules
+            )
             tab_widget.addTab(list_widget, pkg_name)
 
         self.layout.addWidget(tab_widget)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         self.layout.addWidget(close_bt)
 
         self.setLayout(self.layout)
 
     def closeEvent(self, event):
-        self.ct.settings['selected_modules'] = self.selected_modules
+        self.ct.settings["selected_modules"] = self.selected_modules
         self.ct.import_custom_modules()
         self.mw.redraw_func_and_param()
         event.accept()
 
 
 class AddKwargs(QDialog):
     def __init__(self, main_win):
@@ -1538,35 +1702,41 @@
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         list_layout = QHBoxLayout()
-        func_list = CheckDictList(self.ct.pd_funcs.index,
-                                  self.ct.pr.add_kwargs,
-                                  no_bt=QStyle.SP_MessageBoxQuestion)
+        func_list = CheckDictList(
+            self.ct.pd_funcs.index,
+            self.ct.pr.add_kwargs,
+            no_bt=QStyle.SP_MessageBoxQuestion,
+        )
         func_list.currentChanged.connect(self.func_selected)
         list_layout.addWidget(func_list)
 
-        self.kwarg_dict = EditDict(dict(), title='Add Keyword-Arguments:',
-                                   resize_rows=True, resize_columns=True)
+        self.kwarg_dict = EditDict(
+            dict(),
+            title="Add Keyword-Arguments:",
+            resize_rows=True,
+            resize_columns=True,
+        )
         list_layout.addWidget(self.kwarg_dict)
 
         layout.addLayout(list_layout)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def _check_empty(self):
         """Check if the dict for current_func in add_kwargs is empty,
-         then remove it"""
+        then remove it"""
         if self.current_func:
             if self.current_func in self.ct.pr.add_kwargs:
                 if len(self.ct.pr.add_kwargs[self.current_func]) == 0:
                     self.ct.pr.add_kwargs.pop(self.current_func)
 
     def func_selected(self, func_name):
         # Remove dict of previous selected func if empty
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/gui_utils.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/gui_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import io
 import logging
 import multiprocessing
 import sys
 import traceback
 from inspect import signature
 
-from PyQt5.QtCore import (QObject, QProcess, QRunnable, QThreadPool,
-                          Qt, pyqtSignal, pyqtSlot, QTimer)
+from PyQt5.QtCore import (
+    QObject,
+    QProcess,
+    QRunnable,
+    QThreadPool,
+    Qt,
+    pyqtSignal,
+    pyqtSlot,
+    QTimer,
+)
 from PyQt5.QtGui import QFont, QTextCursor
-from PyQt5.QtWidgets import (QApplication, QDesktopWidget, QDialog,
-                             QHBoxLayout,
-                             QLabel, QMessageBox, QProgressBar, QPushButton,
-                             QTextEdit, QVBoxLayout, QStyle, QInputDialog)
+from PyQt5.QtWidgets import (
+    QApplication,
+    QDesktopWidget,
+    QDialog,
+    QHBoxLayout,
+    QLabel,
+    QMessageBox,
+    QProgressBar,
+    QPushButton,
+    QTextEdit,
+    QVBoxLayout,
+    QStyle,
+    QInputDialog,
+)
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 def center(widget):
     qr = widget.frameGeometry()
@@ -43,16 +59,15 @@
     if widget:
         widget.resize(width, height)
 
     return width, height
 
 
 def get_std_icon(icon_name):
-    return QApplication.instance().style().standardIcon(
-        getattr(QStyle, icon_name))
+    return QApplication.instance().style().standardIcon(getattr(QStyle, icon_name))
 
 
 class ExceptionTuple(object):
     def __init__(self, *args):
         self._data = [*args]
 
     def __getitem__(self, idx):
@@ -70,15 +85,15 @@
     exctype, value = sys.exc_info()[:2]
     traceback_str = traceback.format_exc(limit=-10)
     # ToDo: Is this doing what it's supposed to do?
     if is_mp:
         logger = multiprocessing.get_logger()
     else:
         logger = logging.getLogger()
-    logger.error(f'{exctype}: {value}')
+    logger.error(f"{exctype}: {value}")
     exc_tuple = ExceptionTuple(exctype, value, traceback_str)
 
     return exc_tuple
 
 
 class ErrorDialog(QDialog):
     def __init__(self, exception_tuple, parent=None, title=None):
@@ -87,15 +102,15 @@
         else:
             super().__init__()
         self.err = exception_tuple
         self.title = title
         if self.title:
             self.setWindowTitle(self.title)
         else:
-            self.setWindowTitle('An Error ocurred!')
+            self.setWindowTitle("An Error ocurred!")
 
         set_ratio_geometry(0.6, self)
 
         self.init_ui()
 
         if parent:
             self.open()
@@ -104,47 +119,49 @@
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         self.display = QTextEdit()
         self.display.setLineWrapMode(QTextEdit.WidgetWidth)
         self.display.setReadOnly(True)
-        self.formated_tb_text = self.err[2].replace('\n', '<br>')
+        self.formated_tb_text = self.err[2].replace("\n", "<br>")
         if self.title:
-            self.html_text = f'<h1>{self.title}</h1>' \
-                             f'<h2>{self.err[1]}</h2>' \
-                             f'{self.formated_tb_text}'
+            self.html_text = (
+                f"<h1>{self.title}</h1>"
+                f"<h2>{self.err[1]}</h2>"
+                f"{self.formated_tb_text}"
+            )
         else:
-            self.html_text = f'<h1>{self.err[1]}</h1>' \
-                             f'{self.formated_tb_text}'
+            self.html_text = f"<h1>{self.err[1]}</h1>" f"{self.formated_tb_text}"
         self.display.setHtml(self.html_text)
         layout.addWidget(self.display)
 
-        self.close_bt = QPushButton('Close')
+        self.close_bt = QPushButton("Close")
         self.close_bt.clicked.connect(self.close)
         layout.addWidget(self.close_bt)
 
         self.setLayout(layout)
 
 
 def show_error_dialog(exc_str):
     """Checks if a QApplication instance is available
     and shows the Error-Dialog.
      If unavailable (non-console application), log an additional notice.
     """
     if QApplication.instance() is not None:
-        ErrorDialog(exc_str, title='A unexpected error occurred')
+        ErrorDialog(exc_str, title="A unexpected error occurred")
     else:
         logging.debug("No QApplication instance available.")
 
 
 # ToDo: Test
 class UncaughtHook(QObject):
     """This class is a modified version
     of https://timlehr.com/python-exception-hooks-with-qt-message-box/"""
+
     _exception_caught = pyqtSignal(object)
 
     def __init__(self, *args, **kwargs):
         super(UncaughtHook, self).__init__(*args, **kwargs)
 
         # connect signal to execute the message box function
         # always on main thread
@@ -157,35 +174,40 @@
         if issubclass(exc_type, KeyboardInterrupt):
             # ignore keyboard interrupt to support console applications
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
         else:
             # Print Error to Console
             traceback.print_exception(exc_type, exc_value, exc_traceback)
             exc_info = (exc_type, exc_value, exc_traceback)
-            exc_str = (exc_type.__name__, exc_value,
-                       ''.join(traceback.format_tb(exc_traceback)))
-            logging.critical(f'Uncaught exception:\n'
-                             f'{exc_str[0]}: {exc_str[1]}\n'
-                             f'{exc_str[2]}',
-                             exc_info=exc_info)
+            exc_str = (
+                exc_type.__name__,
+                exc_value,
+                "".join(traceback.format_tb(exc_traceback)),
+            )
+            logging.critical(
+                f"Uncaught exception:\n"
+                f"{exc_str[0]}: {exc_str[1]}\n"
+                f"{exc_str[2]}",
+                exc_info=exc_info,
+            )
 
             # trigger showing of error-dialog
             self._exception_caught.emit(exc_str)
 
 
 class CodeEditor(QTextEdit):
     def __init__(self, parent=None):
         super().__init__(parent)
 
 
 def _html_compatible(text):
-    text = text.replace('<', '&lt;')
-    text = text.replace('>', '&gt;')
-    text = text.replace('\n', '<br>')
-    text = text.replace('\x1b', '')
+    text = text.replace("<", "&lt;")
+    text = text.replace(">", "&gt;")
+    text = text.replace("\n", "<br>")
+    text = text.replace("\x1b", "")
 
     return text
 
 
 class ConsoleWidget(QTextEdit):
     """A Widget displaying formatted stdout/stderr-output"""
 
@@ -207,65 +229,65 @@
         self.insertHtml(text)
         if self.autoscroll:
             self.ensureCursorVisible()
 
     def write_buffer(self):
         if len(self.buffer) > 0:
             text, kind = self.buffer.pop(0)
-            if kind == 'html':
+            if kind == "html":
                 self._add_html(text)
 
-            elif kind == 'progress':
-                text = text.replace('\r', '')
+            elif kind == "progress":
+                text = text.replace("\r", "")
                 text = _html_compatible(text)
                 text = f'<font color="green">{text}</font>'
                 # Delete last line
                 cursor = self.textCursor()
                 cursor.select(QTextCursor.LineUnderCursor)
                 cursor.removeSelectedText()
                 self._add_html(text)
 
-            elif kind == 'stdout':
+            elif kind == "stdout":
                 text = _html_compatible(text)
                 self._add_html(text)
 
-            elif kind == 'stderr':
+            elif kind == "stderr":
                 # weird characters in some progress are excluded
                 # (e.g. from autoreject)
-                if '\x1b' not in text:
+                if "\x1b" not in text:
                     text = _html_compatible(text)
                     text = f'<font color="red">{text}</font>'
                     self._add_html(text)
 
     def set_autoscroll(self, autoscroll):
         self.autoscroll = autoscroll
 
     def write_html(self, text):
-        self.buffer.append((text, 'html'))
+        self.buffer.append((text, "html"))
 
     def write_stdout(self, text):
-        self.buffer.append((text, 'stdout'))
+        self.buffer.append((text, "stdout"))
 
     def write_stderr(self, text):
-        self.buffer.append((text, 'stderr'))
+        self.buffer.append((text, "stderr"))
 
     def write_progress(self, text):
-        self.buffer.append((text, 'progress'))
+        self.buffer.append((text, "progress"))
 
     # Make sure cursor is not moved
     def mousePressEvent(self, event):
         event.accept()
 
     def mouseDoubleClickEvent(self, event):
         event.accept()
 
 
 class MainConsoleWidget(ConsoleWidget):
     """A subclass of ConsoleWidget which is linked to stdout/stderr
-     of the main process"""
+    of the main process"""
 
     def __init__(self):
         super().__init__()
 
         # Connect custom stdout and stderr to display-function
         sys.stdout.signal.text_written.connect(self.write_stdout)
         sys.stderr.signal.text_written.connect(self.write_stderr)
@@ -279,40 +301,39 @@
     text_written = pyqtSignal(str)
 
 
 # ToDo: Buffering and halting signal-emission
 #  (continue writing to sys.__stdout__/__stderr__)
 #  when no accepted/printed-signal is coming back from receiving Widget
 class StdoutStderrStream(io.TextIOBase):
-
     def __init__(self, kind):
         super().__init__()
         self.signal = StreamSignals()
-        if kind == 'stdout':
+        if kind == "stdout":
             self.original_stream = sys.__stdout__
         else:
             self.original_stream = sys.__stderr__
 
     def write(self, text):
         # Still send output to the command-line
         self.original_stream.write(text)
 
         # Get progress-text with '\r' as prefix
-        if text[:1] == '\r':
+        if text[:1] == "\r":
             self.signal.text_updated.emit(text)
         else:
             self.signal.text_written.emit(text)
 
     def flush(self):
         self.original_stream.flush()
 
 
 class WorkerSignals(QObject):
-    """Class for standard Worker-Signals
-    """
+    """Class for standard Worker-Signals"""
+
     # Emitted when the function finished and returns the return-value
     finished = pyqtSignal(object)
 
     # Emitted when the function throws an error and returns
     # a tuple with information about the error
     # (see get_exception_tuple)
     error = pyqtSignal(object)
@@ -355,21 +376,21 @@
 
     @pyqtSlot()
     def run(self):
         """
         Initialise the runner function with passed args, kwargs.
         """
         # Add signals to kwargs if in parameters of function
-        if 'worker_signals' in signature(self.function).parameters:
-            self.kwargs['worker_signals'] = self.signals
+        if "worker_signals" in signature(self.function).parameters:
+            self.kwargs["worker_signals"] = self.signals
 
         # Retrieve args/kwargs here; and fire processing using them
         try:
             return_value = self.function(*self.args, **self.kwargs)
-        except:  # noqa: E722
+        except Exception:
             exc_tuple = get_exception_tuple()
             self.signals.error.emit(exc_tuple)
         else:
             self.signals.finished.emit(return_value)  # Done
 
     def start(self):
         QThreadPool.globalInstance().start(self)
@@ -377,19 +398,28 @@
     def cancel(self):
         self.signals.was_canceled = True
 
 
 # ToDo: Make PyQt-independent with tqdm
 class WorkerDialog(QDialog):
     """A Dialog for a Worker doing a function"""
+
     thread_finished = pyqtSignal(object)
 
-    def __init__(self, parent, function, show_buttons=False,
-                 show_console=False, close_directly=True, blocking=False,
-                 title=None, **kwargs):
+    def __init__(
+        self,
+        parent,
+        function,
+        show_buttons=False,
+        show_console=False,
+        close_directly=True,
+        blocking=False,
+        title=None,
+        **kwargs,
+    ):
         super().__init__(parent)
 
         self.show_buttons = show_buttons
         self.show_console = show_console
         self.close_directly = close_directly
         self.title = title
         self.is_finished = False
@@ -414,15 +444,15 @@
             self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         if self.title:
             title_label = QLabel(self.title)
-            title_label.setFont(QFont('AnyType', 18, QFont.Bold))
+            title_label.setFont(QFont("AnyType", 18, QFont.Bold))
             layout.addWidget(title_label)
 
         self.progress_label = QLabel()
         self.progress_label.hide()
         layout.addWidget(self.progress_label, alignment=Qt.AlignHCenter)
 
         self.progress_bar = QProgressBar()
@@ -432,19 +462,19 @@
         if self.show_console:
             self.console_output = MainConsoleWidget()
             layout.addWidget(self.console_output)
 
         if self.show_buttons:
             bt_layout = QHBoxLayout()
 
-            cancel_bt = QPushButton('Cancel')
+            cancel_bt = QPushButton("Cancel")
             cancel_bt.clicked.connect(self.cancel)
             bt_layout.addWidget(cancel_bt)
 
-            self.close_bt = QPushButton('Close')
+            self.close_bt = QPushButton("Close")
             self.close_bt.clicked.connect(self.close)
             self.close_bt.setEnabled(False)
             bt_layout.addWidget(self.close_bt)
 
             layout.addLayout(bt_layout)
 
         self.setLayout(layout)
@@ -476,21 +506,24 @@
         # Can't close Dialog before Thread has finished or threw error
         if self.is_finished:
             self.thread_finished.emit(self.return_value)
             self.deleteLater()
             event.accept()
         else:
             QMessageBox.warning(
-                self, 'Closing not possible!',
-                'You can\'t close this Dialog before this Thread finished!')
+                self,
+                "Closing not possible!",
+                "You can't close this Dialog before this Thread finished!",
+            )
 
 
 # ToDo: WIP
 class QProcessWorker(QObject):
     """A worker for QProcess."""
+
     # Send stdout from current process.
     stdoutSignal = pyqtSignal(str)
     # Send stderr from curren process.
     stderrSignal = pyqtSignal(str)
     # Send when all processes from commands are finished.
     finished = pyqtSignal()
 
@@ -505,43 +538,47 @@
              to be passed to sys.stdout/sys.stderr.
         """
         super().__init__()
 
         # Parse command(s)
         if not isinstance(commands, list):
             commands = [commands]
-        self.commands = [cmd.split(' ') for cmd in commands]
+        self.commands = [cmd.split(" ") for cmd in commands]
         self.printtostd = printtostd
         self.process = None
 
     def handle_stdout(self):
-        text = bytes(self.process.readAllStandardOutput()).decode('utf8')
+        text = bytes(self.process.readAllStandardOutput()).decode("utf8")
         self.stdoutSignal.emit(text)
         if self.printtostd:
             sys.stdout.write(text)
 
     def handle_stderr(self):
-        text = bytes(self.process.readAllStandardError()).decode('utf8')
+        text = bytes(self.process.readAllStandardError()).decode("utf8")
         self.stderrSignal.emit(text)
         if self.printtostd:
             sys.stderr.write(text)
 
     def error_occurred(self):
-        text = f'An error occured with \"{self.process.program()} ' \
-               f'{" ".join(self.process.arguments())}\":\n' \
-               f'{self.process.errorString()}\n'
+        text = (
+            f'An error occured with "{self.process.program()} '
+            f'{" ".join(self.process.arguments())}":\n'
+            f"{self.process.errorString()}\n"
+        )
         self.stderrSignal.emit(text)
         if self.printtostd:
             sys.stderr.write(text)
         self.process_finished()
 
     def process_finished(self):
         if self.process.exitCode() == 1:
-            text = f'\"{self.process.program()} ' \
-                   f'{" ".join(self.process.arguments())}\" has crashed\n'
+            text = (
+                f'"{self.process.program()} '
+                f'{" ".join(self.process.arguments())}" has crashed\n'
+            )
             self.stderrSignal.emit(text)
             if self.printtostd:
                 sys.stderr.write(text)
         if len(self.commands) > 0:
             self.start()
         else:
             self.finished.emit()
@@ -560,17 +597,24 @@
         if kill_all:
             self.commands = list()
         if self.process:
             self.process.kill()
 
 
 class QProcessDialog(QDialog):
-    def __init__(self, parent, commands, show_buttons=True,
-                 show_console=True, close_directly=False,
-                 title=None, blocking=True):
+    def __init__(
+        self,
+        parent,
+        commands,
+        show_buttons=True,
+        show_console=True,
+        close_directly=False,
+        title=None,
+        blocking=True,
+    ):
         super().__init__(parent)
         self.commands = commands
         self.show_buttons = show_buttons
         self.show_console = show_console
         self.close_directly = close_directly
         self.title = title
 
@@ -588,29 +632,29 @@
             self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         if self.title:
             title_label = QLabel(self.title)
-            title_label.setFont(QFont('AnyType', 18, QFont.Bold))
+            title_label.setFont(QFont("AnyType", 18, QFont.Bold))
             layout.addWidget(title_label)
 
         if self.show_console:
             self.console_output = ConsoleWidget()
             layout.addWidget(self.console_output)
 
         if self.show_buttons:
             bt_layout = QHBoxLayout()
 
-            cancel_bt = QPushButton('Cancel')
+            cancel_bt = QPushButton("Cancel")
             cancel_bt.clicked.connect(self.cancel)
             bt_layout.addWidget(cancel_bt)
 
-            self.close_bt = QPushButton('Close')
+            self.close_bt = QPushButton("Close")
             self.close_bt.clicked.connect(self.close)
             self.close_bt.setEnabled(False)
             bt_layout.addWidget(self.close_bt)
 
             layout.addLayout(bt_layout)
 
         self.setLayout(layout)
@@ -624,54 +668,56 @@
 
     def cancel(self):
         self.process_worker.kill(kill_all=True)
 
     def start_process(self):
         self.process_worker = QProcessWorker(self.commands)
         if self.show_console:
-            self.process_worker.stdoutSignal.connect(
-                self.console_output.write_stdout)
-            self.process_worker.stderrSignal.connect(
-                self.console_output.write_stderr)
+            self.process_worker.stdoutSignal.connect(self.console_output.write_stdout)
+            self.process_worker.stderrSignal.connect(self.console_output.write_stderr)
         self.process_worker.finished.connect(self.process_finished)
         self.process_worker.start()
 
     def closeEvent(self, event):
         if self.is_finished:
             self.deleteLater()
             event.accept()
         else:
             event.ignore()
             QMessageBox.warning(
-                self, 'Closing not possible!',
-                'You can\'t close the Dialog before this Process finished!')
+                self,
+                "Closing not possible!",
+                "You can't close the Dialog before this Process finished!",
+            )
 
 
-def get_user_input_string(prompt, title='Input required!', force=False):
+def get_user_input_string(prompt, title="Input required!", force=False):
     # Determine GUI or non-GUI-mode
-    if QS().value('gui') and any([obj is not None
-                                  for obj in _object_refs.values()]):
-        parent = _object_refs['main_window'] or _object_refs['welcome_window']
+    if QS().value("gui") and any([obj is not None for obj in _object_refs.values()]):
+        parent = _object_refs["main_window"] or _object_refs["welcome_window"]
     else:
         parent = None
     if parent is not None:
         user_input, ok = QInputDialog.getText(parent, title, prompt)
     else:
-        user_input = input(f'{title}: {prompt}')
+        user_input = input(f"{title}: {prompt}")
         ok = True
 
     # Check user input
     if not user_input or not ok:
         if force:
             if parent:
                 QMessageBox().warning(
-                    parent, 'Input required!',
-                    'You need to provide an appropriate input to proceed!')
+                    parent,
+                    "Input required!",
+                    "You need to provide an appropriate input to proceed!",
+                )
             else:
                 print(
-                    'Warning: Input required! '
-                    'You need to provide an appropriate input to proceed!')
+                    "Warning: Input required! "
+                    "You need to provide an appropriate input to proceed!"
+                )
             user_input = get_user_input_string(prompt, title, force)
         else:
             user_input = None
 
     return user_input
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/loading_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/loading_widgets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import os
 import re
 import shutil
 import time
 from collections import Counter
@@ -17,36 +15,70 @@
 from pathlib import Path
 
 import mne
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QPixmap
-from PyQt5.QtWidgets import (QAbstractItemView, QCheckBox, QComboBox, QDialog,
-                             QDockWidget, QFileDialog, QGridLayout,
-                             QHBoxLayout, QHeaderView, QLabel, QLineEdit,
-                             QListWidget, QListWidgetItem, QMessageBox,
-                             QProgressBar, QPushButton, QScrollArea,
-                             QSizePolicy, QTabWidget, QTableView, QTreeWidget,
-                             QTreeWidgetItem, QVBoxLayout, QWidget, QWizard,
-                             QWizardPage)
+from PyQt5.QtWidgets import (
+    QAbstractItemView,
+    QCheckBox,
+    QComboBox,
+    QDialog,
+    QDockWidget,
+    QFileDialog,
+    QGridLayout,
+    QHBoxLayout,
+    QHeaderView,
+    QLabel,
+    QLineEdit,
+    QListWidget,
+    QListWidgetItem,
+    QMessageBox,
+    QProgressBar,
+    QPushButton,
+    QScrollArea,
+    QSizePolicy,
+    QTabWidget,
+    QTableView,
+    QTreeWidget,
+    QTreeWidgetItem,
+    QVBoxLayout,
+    QWidget,
+    QWizard,
+    QWizardPage,
+)
 from matplotlib import pyplot as plt
 
-from mne_pipeline_hd.functions.operations import (plot_ica_components,
-                                                  plot_ica_overlay,
-                                                  plot_ica_properties,
-                                                  plot_ica_sources)
-from mne_pipeline_hd.gui.base_widgets import (AssignWidget, CheckDictList,
-                                              CheckList, EditDict, EditList,
-                                              FilePandasTable, SimpleDialog,
-                                              SimpleList, SimplePandasTable)
-from mne_pipeline_hd.gui.gui_utils import (ErrorDialog, Worker, WorkerDialog,
-                                           center, get_exception_tuple,
-                                           set_ratio_geometry,
-                                           get_user_input_string)
+from mne_pipeline_hd.functions.operations import (
+    plot_ica_components,
+    plot_ica_overlay,
+    plot_ica_properties,
+    plot_ica_sources,
+)
+from mne_pipeline_hd.gui.base_widgets import (
+    AssignWidget,
+    CheckDictList,
+    CheckList,
+    EditDict,
+    EditList,
+    FilePandasTable,
+    SimpleDialog,
+    SimpleList,
+    SimplePandasTable,
+)
+from mne_pipeline_hd.gui.gui_utils import (
+    ErrorDialog,
+    Worker,
+    WorkerDialog,
+    center,
+    get_exception_tuple,
+    set_ratio_geometry,
+    get_user_input_string,
+)
 from mne_pipeline_hd.gui.models import AddFilesModel
 from mne_pipeline_hd.gui.parameter_widgets import ComboGui
 from mne_pipeline_hd.pipeline.loading import FSMRI, Group, MEEG
 from mne_pipeline_hd.pipeline.pipeline_utils import compare_filep
 
 
 def index_parser(index, all_items):
@@ -63,65 +95,64 @@
     -------
 
     """
     run = list()
     rm = list()
 
     try:
-        if index == '':
+        if index == "":
             return [], []
-        elif 'all' in index:
-            if ',' in index:
-                splits = index.split(',')
+        elif "all" in index:
+            if "," in index:
+                splits = index.split(",")
                 for sp in splits:
-                    if '!' in sp and '-' in sp:
-                        x, y = sp.split('-')
+                    if "!" in sp and "-" in sp:
+                        x, y = sp.split("-")
                         x = x[1:]
                         for n in range(int(x), int(y) + 1):
                             rm.append(n)
-                    elif '!' in sp:
+                    elif "!" in sp:
                         rm.append(int(sp[1:]))
-                    elif 'all' in sp:
+                    elif "all" in sp:
                         for i in range(len(all_items)):
                             run.append(i)
             else:
                 run = [x for x in range(len(all_items))]
 
-        elif ',' in index and '-' in index:
-            z = index.split(',')
+        elif "," in index and "-" in index:
+            z = index.split(",")
             for i in z:
-                if '-' in i and '!' not in i:
-                    x, y = i.split('-')
+                if "-" in i and "!" not in i:
+                    x, y = i.split("-")
                     for n in range(int(x), int(y) + 1):
                         run.append(n)
-                elif '!' not in i:
+                elif "!" not in i:
                     run.append(int(i))
-                elif '!' in i and '-' in i:
-                    x, y = i.split('-')
+                elif "!" in i and "-" in i:
+                    x, y = i.split("-")
                     x = x[1:]
                     for n in range(int(x), int(y) + 1):
                         rm.append(n)
-                elif '!' in i:
+                elif "!" in i:
                     rm.append(int(i[1:]))
 
-        elif '-' in index and ',' not in index:
-            x, y = index.split('-')
+        elif "-" in index and "," not in index:
+            x, y = index.split("-")
             run = [x for x in range(int(x), int(y) + 1)]
 
-        elif ',' in index and '-' not in index:
-            splits = index.split(',')
+        elif "," in index and "-" not in index:
+            splits = index.split(",")
             for sp in splits:
-                if '!' in sp:
+                if "!" in sp:
                     rm.append(int(sp))
                 else:
                     run.append(int(sp))
 
         else:
-            if len(all_items) < int(index) or int(index) < \
-                    0:
+            if len(all_items) < int(index) or int(index) < 0:
                 run = []
             else:
                 run = [int(index)]
 
         run = [i for i in run if i not in rm]
         files = [x for (i, x) in enumerate(all_items) if i in run]
 
@@ -139,49 +170,47 @@
         self.mode = mode
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
-        label = QLabel(f'Do you really want to remove'
-                       f' the selected {self.mode}?')
+        label = QLabel(f"Do you really want to remove" f" the selected {self.mode}?")
         layout.addWidget(label)
 
-        if self.mode == 'MEEG':
+        if self.mode == "MEEG":
             layout.addWidget(SimpleList(self.pr.sel_meeg))
-        elif self.mode == 'FSMRI':
+        elif self.mode == "FSMRI":
             layout.addWidget(SimpleList(self.pr.sel_fsmri))
 
-        only_list_bt = QPushButton('Remove only from List')
+        only_list_bt = QPushButton("Remove only from List")
         only_list_bt.clicked.connect(partial(self.remove_objects, False))
         layout.addWidget(only_list_bt)
-        remove_files_bt = QPushButton('Remove with all Files')
+        remove_files_bt = QPushButton("Remove with all Files")
         remove_files_bt.clicked.connect(partial(self.remove_objects, True))
         layout.addWidget(remove_files_bt)
-        cancel_bt = QPushButton('Cancel')
+        cancel_bt = QPushButton("Cancel")
         cancel_bt.clicked.connect(self.close)
         layout.addWidget(cancel_bt)
         self.setLayout(layout)
 
     def remove_objects(self, remove_files):
-        if self.mode == 'MEEG':
+        if self.mode == "MEEG":
             self.pr.remove_meeg(remove_files)
             self.pw.meeg_list.content_changed()
-        elif self.mode == 'FSMRI':
+        elif self.mode == "FSMRI":
             self.pr.remove_fsmri(remove_files)
             self.pw.fsmri_list.content_changed()
         self.close()
 
 
 # Todo: File-Selection depending on existence of data-objects
 class FileDock(QDockWidget):
-    def __init__(self, main_win, meeg_view=True, fsmri_view=True,
-                 group_view=True):
-        super().__init__('Object-Selection', main_win)
+    def __init__(self, main_win, meeg_view=True, fsmri_view=True, group_view=True):
+        super().__init__("Object-Selection", main_win)
         # Maintain main-window as top-level object from which the references to
         # the objects of controller and project are taken.
         self.mw = main_win
 
         self.meeg_view = meeg_view
         self.fsmri_view = fsmri_view
         self.group_view = group_view
@@ -190,90 +219,97 @@
         self.init_ui()
 
     def init_ui(self):
         self.central_widget = QWidget(self)
         layout = QVBoxLayout()
         tab_widget = QTabWidget(self)
 
-        idx_example = "Examples:\n" \
-                      "'5' (One File)\n" \
-                      "'1,7,28' (Several Files)\n" \
-                      "'1-5' (From File x to File y)\n" \
-                      "'1-4,7,20-26' (The last two combined)\n" \
-                      "'1-20,!4-6' (1-20 except 4-6)\n" \
-                      "'all' (All files in file_list.py)\n" \
-                      "'all,!4-6' (All files except 4-6)"
+        idx_example = (
+            "Examples:\n"
+            "'5' (One File)\n"
+            "'1,7,28' (Several Files)\n"
+            "'1-5' (From File x to File y)\n"
+            "'1-4,7,20-26' (The last two combined)\n"
+            "'1-20,!4-6' (1-20 except 4-6)\n"
+            "'all' (All files in file_list.py)\n"
+            "'all,!4-6' (All files except 4-6)"
+        )
 
         if self.meeg_view:
             # MEEG-List + Index-Line-Edit
             meeg_widget = QWidget()
             meeg_layout = QVBoxLayout()
-            self.meeg_list = CheckList(self.mw.ct.pr.all_meeg,
-                                       self.mw.ct.pr.sel_meeg,
-                                       ui_button_pos='top',
-                                       show_index=True, title='Select MEG/EEG')
+            self.meeg_list = CheckList(
+                self.mw.ct.pr.all_meeg,
+                self.mw.ct.pr.sel_meeg,
+                ui_button_pos="top",
+                show_index=True,
+                title="Select MEG/EEG",
+            )
             meeg_layout.addWidget(self.meeg_list)
 
             self.meeg_ledit = QLineEdit()
-            self.meeg_ledit.setPlaceholderText('MEEG-Index')
+            self.meeg_ledit.setPlaceholderText("MEEG-Index")
             self.meeg_ledit.textEdited.connect(self.select_meeg)
             self.meeg_ledit.setToolTip(idx_example)
             meeg_layout.addWidget(self.meeg_ledit)
 
             # Add and Remove-Buttons
             meeg_bt_layout = QHBoxLayout()
-            file_add_bt = QPushButton('Add MEEG')
+            file_add_bt = QPushButton("Add MEEG")
             file_add_bt.clicked.connect(partial(AddFilesDialog, self.mw))
             meeg_bt_layout.addWidget(file_add_bt)
-            rename_bt = QPushButton('Rename')
+            rename_bt = QPushButton("Rename")
             rename_bt.clicked.connect(self._rename_meeg)
             meeg_bt_layout.addWidget(rename_bt)
-            file_rm_bt = QPushButton('Remove MEEG')
+            file_rm_bt = QPushButton("Remove MEEG")
             file_rm_bt.clicked.connect(self.remove_meeg)
             meeg_bt_layout.addWidget(file_rm_bt)
 
             meeg_layout.addLayout(meeg_bt_layout)
             meeg_widget.setLayout(meeg_layout)
 
-            tab_widget.addTab(meeg_widget, 'MEG/EEG')
+            tab_widget.addTab(meeg_widget, "MEG/EEG")
 
         if self.fsmri_view:
             # MRI-Subjects-List + Index-Line-Edit
             fsmri_widget = QWidget()
             fsmri_layout = QVBoxLayout()
-            self.fsmri_list = CheckList(self.mw.ct.pr.all_fsmri,
-                                        self.mw.ct.pr.sel_fsmri,
-                                        ui_button_pos='top',
-                                        show_index=True,
-                                        title='Select Freesurfer-MRI')
+            self.fsmri_list = CheckList(
+                self.mw.ct.pr.all_fsmri,
+                self.mw.ct.pr.sel_fsmri,
+                ui_button_pos="top",
+                show_index=True,
+                title="Select Freesurfer-MRI",
+            )
             fsmri_layout.addWidget(self.fsmri_list)
 
             self.fsmri_ledit = QLineEdit()
-            self.fsmri_ledit.setPlaceholderText('FS-MRI-Index')
+            self.fsmri_ledit.setPlaceholderText("FS-MRI-Index")
             self.fsmri_ledit.textEdited.connect(self.select_fsmri)
             self.fsmri_ledit.setToolTip(idx_example)
             fsmri_layout.addWidget(self.fsmri_ledit)
 
             # Add and Remove-Buttons
             fsmri_bt_layout = QHBoxLayout()
-            mri_add_bt = QPushButton('Add FS-MRI')
+            mri_add_bt = QPushButton("Add FS-MRI")
             mri_add_bt.clicked.connect(partial(AddMRIDialog, self.mw))
             fsmri_bt_layout.addWidget(mri_add_bt)
-            mri_rm_bt = QPushButton('Remove FS-MRI')
+            mri_rm_bt = QPushButton("Remove FS-MRI")
             mri_rm_bt.clicked.connect(self.remove_fsmri)
             fsmri_bt_layout.addWidget(mri_rm_bt)
 
             fsmri_layout.addLayout(fsmri_bt_layout)
             fsmri_widget.setLayout(fsmri_layout)
 
-            tab_widget.addTab(fsmri_widget, 'FS-MRI')
+            tab_widget.addTab(fsmri_widget, "FS-MRI")
 
         if self.group_view:
             self.ga_widget = GrandAvgWidget(self.mw)
-            tab_widget.addTab(self.ga_widget, 'Groups')
+            tab_widget.addTab(self.ga_widget, "Groups")
 
         layout.addWidget(tab_widget)
         self.central_widget.setLayout(layout)
         self.setWidget(self.central_widget)
 
     def update_dock(self):
         # Update lists when rereferenced elsewhere
@@ -287,42 +323,40 @@
 
     def reload_dock(self):
         self.init_ui()
         self.central_widget.show()
 
     def select_meeg(self):
         index = self.meeg_ledit.text()
-        self.mw.ct.pr.sel_meeg, idxs = index_parser(index,
-                                                    self.mw.ct.pr.all_meeg)
+        self.mw.ct.pr.sel_meeg, idxs = index_parser(index, self.mw.ct.pr.all_meeg)
         # Replace _checked in CheckListModel because of rereferencing above
         self.meeg_list.replace_checked(self.mw.ct.pr.sel_meeg)
 
     def select_fsmri(self):
         index = self.fsmri_ledit.text()
-        self.mw.ct.pr.sel_fsmri, idxs = index_parser(index,
-                                                     self.mw.ct.pr.all_fsmri)
+        self.mw.ct.pr.sel_fsmri, idxs = index_parser(index, self.mw.ct.pr.all_fsmri)
         # Replace _checked in CheckListModel because of rereferencing above
         self.fsmri_list.replace_checked(self.mw.ct.pr.sel_fsmri)
 
     def _rename_meeg(self):
         current_meeg = self.meeg_list.get_current()
         if current_meeg is not None:
             meeg = MEEG(current_meeg, self.mw.ct)
-            new_name = get_user_input_string('Enter new name:', 'Rename')
+            new_name = get_user_input_string("Enter new name:", "Rename")
             if new_name is not None:
                 meeg.rename(new_name)
                 self.update_dock()
 
     def remove_meeg(self):
         if len(self.mw.ct.pr.sel_meeg) > 0:
-            RemoveDialog(self, 'MEEG')
+            RemoveDialog(self, "MEEG")
 
     def remove_fsmri(self):
         if len(self.mw.ct.pr.sel_fsmri) > 0:
-            RemoveDialog(self, 'FSMRI')
+            RemoveDialog(self, "FSMRI")
 
 
 class GrandAvgWidget(QWidget):
     def __init__(self, main_win):
         super().__init__()
         self.mw = main_win
 
@@ -332,39 +366,40 @@
 
     def init_layout(self):
         self.layout = QVBoxLayout()
         self.treew = QTreeWidget()
         self.treew.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.treew.itemChanged.connect(self.get_treew)
         self.treew.setColumnCount(1)
-        self.treew.setHeaderLabel('Groups:')
+        self.treew.setHeaderLabel("Groups:")
         self.layout.addWidget(self.treew)
 
         self.bt_layout = QHBoxLayout()
-        add_g_bt = QPushButton('Add Group')
+        add_g_bt = QPushButton("Add Group")
         add_g_bt.clicked.connect(self.add_group)
         self.bt_layout.addWidget(add_g_bt)
-        add_file_bt = QPushButton('Add Files')
+        add_file_bt = QPushButton("Add Files")
         add_file_bt.clicked.connect(self.add_files)
         self.bt_layout.addWidget(add_file_bt)
-        self.rm_bt = QPushButton('Remove')
+        self.rm_bt = QPushButton("Remove")
         self.rm_bt.clicked.connect(self.remove_item)
         self.bt_layout.addWidget(self.rm_bt)
         self.layout.addLayout(self.bt_layout)
 
         self.setLayout(self.layout)
 
     def update_treew(self):
         self.treew.clear()
         top_items = []
         for group in self.mw.ct.pr.all_groups:
             top_item = QTreeWidgetItem()
             top_item.setText(0, group)
             top_item.setFlags(
-                top_item.flags() | Qt.ItemIsUserCheckable | Qt.ItemIsEditable)
+                top_item.flags() | Qt.ItemIsUserCheckable | Qt.ItemIsEditable
+            )
             if group in self.mw.ct.pr.sel_groups:
                 top_item.setCheckState(0, Qt.Checked)
             else:
                 top_item.setCheckState(0, Qt.Unchecked)
             for file in self.mw.ct.pr.all_groups[group]:
                 sub_item = QTreeWidgetItem(top_item)
                 sub_item.setText(0, file)
@@ -382,16 +417,15 @@
                 child_item = top_item.child(child_idx)
                 new_dict[top_text].append(child_item.text(0))
             if top_item.checkState(0) == Qt.Checked:
                 self.mw.ct.pr.sel_groups.append(top_text)
         self.mw.ct.pr.all_groups = new_dict
 
     def add_group(self):
-        text = get_user_input_string('Enter the name for a new group:',
-                                     'New Group')
+        text = get_user_input_string("Enter the name for a new group:", "New Group")
         if text is not None:
             top_item = QTreeWidgetItem()
             top_item.setText(0, text)
             top_item.setFlags(top_item.flags() | Qt.ItemIsUserCheckable)
             top_item.setCheckState(0, Qt.Checked)
             self.treew.addTopLevelItem(top_item)
             self.get_treew()
@@ -401,62 +435,60 @@
         if sel_group:
             # When file in group is selected
             if sel_group.parent():
                 sel_group = sel_group.parent()
             GrandAvgFileAdd(self.mw, sel_group, self)
         else:
             msg_box = QMessageBox(self)
-            msg_box.setWindowTitle('Warning')
+            msg_box.setWindowTitle("Warning")
             msg_box.setIcon(QMessageBox.Warning)
-            msg_box.setText('No group has been selected')
+            msg_box.setText("No group has been selected")
             msg_box.open()
 
     def remove_item(self):
         items = self.treew.selectedItems()
         if len(items) > 0:
             for item in items:
                 if item.parent():
                     item.parent().takeChild(item.parent().indexOfChild(item))
                 else:
-                    self.treew.takeTopLevelItem(
-                        self.treew.indexOfTopLevelItem(item))
+                    self.treew.takeTopLevelItem(self.treew.indexOfTopLevelItem(item))
         self.get_treew()
         self.treew.setCurrentItem(None, 0)
 
 
 class GrandAvgFileAdd(QDialog):
     def __init__(self, main_win, group, ga_widget):
         super().__init__(ga_widget)
         self.mw = main_win
 
         self.group = group
         self.ga_widget = ga_widget
-        self.setWindowTitle('Select Files to add')
+        self.setWindowTitle("Select Files to add")
 
         self.init_ui()
 
     def init_ui(self):
-
         dlg_layout = QGridLayout()
         self.listw = QListWidget()
         self.listw.setSelectionMode(QAbstractItemView.ExtendedSelection)
         self.listw.itemSelectionChanged.connect(self.sel_changed)
         self.load_list()
 
         dlg_layout.addWidget(self.listw, 0, 0, 1, 4)
-        add_bt = QPushButton('Add')
+        add_bt = QPushButton("Add")
         add_bt.clicked.connect(self.add)
         dlg_layout.addWidget(add_bt, 1, 0)
-        all_bt = QPushButton('All')
+        all_bt = QPushButton("All")
         all_bt.clicked.connect(self.sel_all)
         dlg_layout.addWidget(all_bt, 1, 1)
-        clear_bt = QPushButton('Clear')
+        clear_bt = QPushButton("Clear")
         clear_bt.clicked.connect(self.clear)
         dlg_layout.addWidget(clear_bt, 1, 2)
-        quit_bt = QPushButton('Quit')
+        quit_bt = QPushButton("Quit")
         quit_bt.clicked.connect(self.close)
         dlg_layout.addWidget(quit_bt, 1, 3)
 
         self.setLayout(dlg_layout)
         self.open()
 
     def sel_changed(self):
@@ -497,93 +529,106 @@
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
         self.layout = QVBoxLayout()
 
-        self.erm_keywords = ['leer', 'Leer', 'erm', 'ERM', 'empty', 'Empty',
-                             'room', 'Room', 'raum',
-                             'Raum']
-        self.supported_file_types = {'.*': 'All Files',
-                                     '.bin': 'Artemis123',
-                                     '.cnt': 'Neuroscan',
-                                     '.ds': 'CTF',
-                                     '.dat': 'Curry',
-                                     '.dap': 'Curry',
-                                     '.rs3': 'Curry',
-                                     '.cdt': 'Curry',
-                                     '.cdt.dpa': 'Curry',
-                                     '.cdt.cef': 'Curry',
-                                     '.cef': 'Curry',
-                                     '.edf': 'European',
-                                     '.bdf': 'BioSemi',
-                                     '.gdf': 'General',
-                                     '.sqd': 'Ricoh/KIT',
-                                     '.data': 'Nicolet',
-                                     '.fif': 'Neuromag',
-                                     '.set': 'EEGLAB',
-                                     '.vhdr': 'Brainvision',
-                                     '.egi': 'EGI',
-                                     '.mff': 'EGI',
-                                     '.mat': 'Fieldtrip',
-                                     '.lay': 'Persyst'}
-
-        self.pd_files = pd.DataFrame([], columns=['Name', 'File-Type',
-                                                  'Empty-Room?', 'Path'])
+        self.erm_keywords = [
+            "leer",
+            "Leer",
+            "erm",
+            "ERM",
+            "empty",
+            "Empty",
+            "room",
+            "Room",
+            "raum",
+            "Raum",
+        ]
+        self.supported_file_types = {
+            ".*": "All Files",
+            ".bin": "Artemis123",
+            ".cnt": "Neuroscan",
+            ".ds": "CTF",
+            ".dat": "Curry",
+            ".dap": "Curry",
+            ".rs3": "Curry",
+            ".cdt": "Curry",
+            ".cdt.dpa": "Curry",
+            ".cdt.cef": "Curry",
+            ".cef": "Curry",
+            ".edf": "European",
+            ".bdf": "BioSemi",
+            ".gdf": "General",
+            ".sqd": "Ricoh/KIT",
+            ".data": "Nicolet",
+            ".fif": "Neuromag",
+            ".set": "EEGLAB",
+            ".vhdr": "Brainvision",
+            ".egi": "EGI",
+            ".mff": "EGI",
+            ".mat": "Fieldtrip",
+            ".lay": "Persyst",
+        }
+
+        self.pd_files = pd.DataFrame(
+            [], columns=["Name", "File-Type", "Empty-Room?", "Path"]
+        )
         self.load_kwargs = {}
 
         self.init_ui()
 
     def init_ui(self):
         # Input Buttons
-        files_bt = QPushButton('File-Import', self)
+        files_bt = QPushButton("File-Import", self)
         files_bt.clicked.connect(self.get_files_path)
-        folder_bt = QPushButton('Folder-Import', self)
+        folder_bt = QPushButton("Folder-Import", self)
         folder_bt.clicked.connect(self.get_folder_path)
         input_bt_layout = QHBoxLayout()
         input_bt_layout.addWidget(files_bt)
         input_bt_layout.addWidget(folder_bt)
         self.layout.addLayout(input_bt_layout)
 
         self.view = QTableView()
         self.model = AddFilesModel(self.pd_files)
         self.view.setModel(self.model)
 
-        self.view.horizontalHeader().setSectionResizeMode(
-            QHeaderView.ResizeToContents)
+        self.view.horizontalHeader().setSectionResizeMode(QHeaderView.ResizeToContents)
         self.view.setToolTip(
-            'These .fif-Files can be imported \n'
-            '(the Empty-Room-Measurements should appear here '
-            'too and will be sorted according to the ERM-Keywords)')
+            "These .fif-Files can be imported \n"
+            "(the Empty-Room-Measurements should appear here "
+            "too and will be sorted according to the ERM-Keywords)"
+        )
         self.layout.addWidget(self.view)
 
         self.main_bt_layout = QHBoxLayout()
-        import_bt = QPushButton('Import', self)
+        import_bt = QPushButton("Import", self)
         import_bt.clicked.connect(self.add_files_starter)
         self.main_bt_layout.addWidget(import_bt)
-        delete_bt = QPushButton('Remove', self)
+        delete_bt = QPushButton("Remove", self)
         delete_bt.clicked.connect(self.delete_item)
         self.main_bt_layout.addWidget(delete_bt)
-        erm_kw_bt = QPushButton('Empty-Room-Keywords')
+        erm_kw_bt = QPushButton("Empty-Room-Keywords")
         erm_kw_bt.clicked.connect(partial(ErmKwDialog, self))
         self.main_bt_layout.addWidget(erm_kw_bt)
-        load_arg_bt = QPushButton('Load-Arguments')
+        load_arg_bt = QPushButton("Load-Arguments")
         load_arg_bt.clicked.connect(partial(LoadArgDialog, self))
         self.main_bt_layout.addWidget(load_arg_bt)
 
         self.layout.addLayout(self.main_bt_layout)
         self.setLayout(self.layout)
 
     def delete_item(self):
         # Sorted indexes in reverse to avoid problems when removing several
         # indices at once
-        row_idxs = sorted(set([idx.row() for idx in
-                               self.view.selectionModel().selectedIndexes()]),
-                          reverse=True)
+        row_idxs = sorted(
+            set([idx.row() for idx in self.view.selectionModel().selectedIndexes()]),
+            reverse=True,
+        )
         for row_idx in row_idxs:
             self.model.removeRow(row_idx)
         # Update pd_files, because reference is changed with model.removeRow()
         self.pd_files = self.model._data
 
     def update_model(self):
         self.model._data = self.pd_files
@@ -593,119 +638,152 @@
         if len(files_list) > 0:
             existing_files = list()
 
             for file_path in files_list:
                 p = Path(file_path)
                 file_name = p.stem
                 # Get already existing files and skip them
-                if file_path in list(self.pd_files['Path']) \
-                        or file_name in self.pr.all_meeg \
-                        or file_name in self.pr.all_erm:
+                if (
+                    file_path in list(self.pd_files["Path"])
+                    or file_name in self.pr.all_meeg
+                    or file_name in self.pr.all_erm
+                ):
                     existing_files.append(file_name)
                     continue
 
                 # Remove -raw from name (put stays in file_name and path later)
-                if file_name[-4:] == '-raw':
+                if file_name[-4:] == "-raw":
                     file_name = file_name[:-4]
 
                 if any(x in file_name for x in self.erm_keywords):
                     erm = 1
                 else:
                     erm = 0
 
-                self.pd_files = self.pd_files.append(
-                    {'Name': file_name, 'File-Type': p.suffix,
-                     'Empty-Room?': erm, 'Path': file_path},
-                    ignore_index=True)
+                self.pd_files = pd.concat(
+                    [
+                        self.pd_files,
+                        pd.DataFrame(
+                            [
+                                {
+                                    "Name": file_name,
+                                    "File-Type": p.suffix,
+                                    "Empty-Room?": erm,
+                                    "Path": file_path,
+                                }
+                            ]
+                        ),
+                    ],
+                    ignore_index=True,
+                )
 
             self.update_model()
 
             if len(existing_files) > 0:
                 QMessageBox.information(
-                    self, 'Existing Files',
-                    f'These files already exist in your meeg.pr:'
-                    f'{existing_files}')
+                    self,
+                    "Existing Files",
+                    f"These files already exist in your meeg.pr:" f"{existing_files}",
+                )
 
     def get_files_path(self):
-        filter_list = [f'{self.supported_file_types[key]} (*{key})' for key in
-                       self.supported_file_types]
-        filter_list.insert(0, 'All Files (*.*)')
-        filter_qstring = ';;'.join(filter_list)
-        files_list = \
-            QFileDialog.getOpenFileNames(self, 'Choose raw-file/s to import',
-                                         filter=filter_qstring)[0]
+        filter_list = [
+            f"{self.supported_file_types[key]} (*{key})"
+            for key in self.supported_file_types
+        ]
+        filter_list.insert(0, "All Files (*.*)")
+        filter_qstring = ";;".join(filter_list)
+        files_list = QFileDialog.getOpenFileNames(
+            self, "Choose raw-file/s to import", filter=filter_qstring
+        )[0]
         self.insert_files(files_list)
 
     def get_folder_path(self):
         folder_path = QFileDialog.getExistingDirectory(
-            self, 'Choose a folder to import your raw-Files from '
-                  '(including subfolders)')
-        if folder_path != '':
+            self,
+            "Choose a folder to import your raw-Files from " "(including subfolders)",
+        )
+        if folder_path != "":
             # create a list of file and obj directories
             # names in the given directory
             list_of_file = os.walk(folder_path)
             files_list = list()
             # Iterate over all the entries
-            for dirpath, dirnames, filenames in list_of_file:
+            for dirpath, _, filenames in list_of_file:
                 for file in filenames:
                     for file_type in self.supported_file_types:
-                        match = re.match(rf'(.+)({file_type})', file)
+                        match = re.match(rf"(.+)({file_type})", file)
                         if match and len(match.group()) == len(file):
                             # Make sure, that no files from Pipeline-Analysis
                             # are included
-                            if not any(x in file for x in
-                                       ['-eve.', '-epo.', '-ica.', '-ave.',
-                                        '-tfr.', '-fwd.',
-                                        '-cov.', '-inv.', '-src.', '-trans.',
-                                        '-bem-sol.']):
+                            if not any(
+                                x in file
+                                for x in [
+                                    "-eve.",
+                                    "-epo.",
+                                    "-ica.",
+                                    "-ave.",
+                                    "-tfr.",
+                                    "-fwd.",
+                                    "-cov.",
+                                    "-inv.",
+                                    "-src.",
+                                    "-trans.",
+                                    "-bem-sol.",
+                                ]
+                            ):
                                 files_list.append(join(dirpath, file))
             self.insert_files(files_list)
 
     def update_erm_checks(self):
         for idx in self.pd_files.index:
-            if any(x in self.pd_files.loc[idx, 'Name'] for x in
-                   self.erm_keywords):
-                self.pd_files.loc[idx, 'Empty-Room?'] = 1
+            if any(x in self.pd_files.loc[idx, "Name"] for x in self.erm_keywords):
+                self.pd_files.loc[idx, "Empty-Room?"] = 1
             else:
-                self.pd_files.loc[idx, 'Empty-Room?'] = 0
+                self.pd_files.loc[idx, "Empty-Room?"] = 0
         self.model.layoutChanged.emit()
 
     def add_files(self, worker_signals):
-
         # Resolve identical file-names (but different types)
-        duplicates = [item for item, i_cnt in
-                      Counter(list(self.pd_files['Name'])).items() if
-                      i_cnt > 1]
+        duplicates = [
+            item
+            for item, i_cnt in Counter(list(self.pd_files["Name"])).items()
+            if i_cnt > 1
+        ]
         for name in duplicates:
-            dupl_df = self.pd_files[self.pd_files['Name'] == name]
+            dupl_df = self.pd_files[self.pd_files["Name"] == name]
             for idx in dupl_df.index:
-                self.pd_files.loc[idx, 'Name'] = \
-                    self.pd_files.loc[idx, 'Name'] + '-' + \
-                    self.pd_files.loc[idx, 'File-Type'][1:]
+                self.pd_files.loc[idx, "Name"] = (
+                    self.pd_files.loc[idx, "Name"]
+                    + "-"
+                    + self.pd_files.loc[idx, "File-Type"][1:]
+                )
 
         worker_signals.pgbar_max.emit(len(self.pd_files.index))
 
         for n, idx in enumerate(self.pd_files.index):
-            name = self.pd_files.loc[idx, 'Name']
+            name = self.pd_files.loc[idx, "Name"]
             if not worker_signals.was_canceled:
-                worker_signals.pgbar_text.emit(f'Copying {name}')
-                file_path = self.pd_files.loc[idx, 'Path']
-                is_erm = self.pd_files.loc[idx, 'Empty-Room?']
+                worker_signals.pgbar_text.emit(f"Copying {name}")
+                file_path = self.pd_files.loc[idx, "Path"]
+                is_erm = self.pd_files.loc[idx, "Empty-Room?"]
                 self.pr.add_meeg(name, file_path, is_erm)
                 worker_signals.pgbar_n.emit(n + 1)
             else:
-                print('Canceled Loading')
+                print("Canceled Loading")
                 break
 
     def add_files_starter(self):
-        WorkerDialog(self, self.add_files, show_buttons=True,
-                     show_console=True, blocking=True)
-
-        self.pd_files = pd.DataFrame([], columns=['Name', 'File-Type',
-                                                  'Empty-Room?', 'Path'])
+        WorkerDialog(
+            self, self.add_files, show_buttons=True, show_console=True, blocking=True
+        )
+
+        self.pd_files = pd.DataFrame(
+            [], columns=["Name", "File-Type", "Empty-Room?", "Path"]
+        )
         self.update_model()
 
         self.pr.save()
         self.mw.file_dock.update_dock()
 
 
 class ErmKwDialog(QDialog):
@@ -718,15 +796,15 @@
 
         self.open()
 
     def init_ui(self):
         self.listw = EditList(self.parent.erm_keywords)
         self.layout.addWidget(self.listw)
 
-        self.close_bt = QPushButton('Close')
+        self.close_bt = QPushButton("Close")
         self.close_bt.clicked.connect(self.close)
         self.layout.addWidget(self.close_bt)
 
         self.setLayout(self.layout)
 
     def close_dlg(self):
         self.parent.update_erm_checks()
@@ -741,29 +819,28 @@
         self.layout = QVBoxLayout()
         self.init_ui()
         self.open()
 
     def init_ui(self):
         self.edit_dict = EditDict(self.parent.load_kwargs)
         self.layout.addWidget(self.edit_dict)
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         self.layout.addWidget(close_bt)
         self.setLayout(self.layout)
 
 
 class AddFilesDialog(AddFilesWidget):
     def __init__(self, main_win):
         super().__init__(main_win)
 
         self.dialog = QDialog(main_win)
-        self.dialog.setSizePolicy(QSizePolicy.MinimumExpanding,
-                                  QSizePolicy.Minimum)
+        self.dialog.setSizePolicy(QSizePolicy.MinimumExpanding, QSizePolicy.Minimum)
 
-        close_bt = QPushButton('Close', self)
+        close_bt = QPushButton("Close", self)
         close_bt.clicked.connect(self.dialog.close)
         self.main_bt_layout.addWidget(close_bt)
 
         self.dialog.setLayout(self.layout)
 
         set_ratio_geometry(0.7, self)
 
@@ -781,51 +858,49 @@
         self.folders = list()
         self.paths = dict()
 
         self.init_ui()
 
     def init_ui(self):
         bt_layout = QHBoxLayout()
-        folder_bt = QPushButton('Import 1 FS-Segmentation', self)
+        folder_bt = QPushButton("Import 1 FS-Segmentation", self)
         folder_bt.clicked.connect(self.import_mri_subject)
         bt_layout.addWidget(folder_bt)
-        folders_bt = QPushButton('Import >1 FS-Segmentations', self)
+        folders_bt = QPushButton("Import >1 FS-Segmentations", self)
         folders_bt.clicked.connect(self.import_mri_subjects)
         bt_layout.addWidget(folders_bt)
         self.layout.addLayout(bt_layout)
 
-        list_label = QLabel('These Freesurfer-Segmentations can be imported:',
-                            self)
+        list_label = QLabel("These Freesurfer-Segmentations can be imported:", self)
         self.layout.addWidget(list_label)
         self.list_widget = QListWidget(self)
         self.layout.addWidget(self.list_widget)
 
         self.main_bt_layout = QHBoxLayout()
-        import_bt = QPushButton('Import', self)
+        import_bt = QPushButton("Import", self)
         import_bt.clicked.connect(self.add_mri_subjects_starter)
         self.main_bt_layout.addWidget(import_bt)
-        rename_bt = QPushButton('Rename File', self)
+        rename_bt = QPushButton("Rename File", self)
         rename_bt.clicked.connect(self.rename_item)
         self.main_bt_layout.addWidget(rename_bt)
-        delete_bt = QPushButton('Delete File', self)
+        delete_bt = QPushButton("Delete File", self)
         delete_bt.clicked.connect(self.delete_item)
         self.main_bt_layout.addWidget(delete_bt)
 
         self.layout.addLayout(self.main_bt_layout)
         self.setLayout(self.layout)
 
     def populate_list_widget(self):
         # List with checkable names
         self.list_widget.clear()
         self.list_widget.addItems(self.folders)
 
         for index in range(self.list_widget.count()):
             item = self.list_widget.item(index)
-            item.setFlags(
-                Qt.ItemIsEnabled | Qt.ItemIsEditable | Qt.ItemIsSelectable)
+            item.setFlags(Qt.ItemIsEnabled | Qt.ItemIsEditable | Qt.ItemIsSelectable)
 
     def delete_item(self):
         i = self.list_widget.currentRow()
         if i >= 0:
             name = self.list_widget.item(i).text()
             self.list_widget.takeItem(i)
             self.folders.remove(name)
@@ -838,61 +913,55 @@
             new_name = self.list_widget.item(i).text()
             repl_ind = self.files.index(old_name)
             self.folders[repl_ind] = new_name
             self.paths[new_name] = self.paths[old_name]
 
     def import_mri_subject(self):
         folder_path = QFileDialog.getExistingDirectory(
-            self, 'Choose a folder with a subject\'s Freesurfe-Segmentation')
+            self, "Choose a folder with a subject's Freesurfe-Segmentation"
+        )
 
-        if folder_path != '':
-            if exists(join(folder_path, 'surf')):
+        if folder_path != "":
+            if exists(join(folder_path, "surf")):
                 fsmri = Path(folder_path).name
-                if fsmri not in self.pr.all_fsmri \
-                        and fsmri not in self.folders:
+                if fsmri not in self.pr.all_fsmri and fsmri not in self.folders:
                     self.folders.append(fsmri)
                     self.paths.update({fsmri: folder_path})
                     self.populate_list_widget()
                 else:
-                    print(
-                        f'{fsmri} already existing in {self.ct.subjects_dir}')
+                    print(f"{fsmri} already existing in {self.ct.subjects_dir}")
             else:
-                print(
-                    'Selected Folder doesn\'t seem to '
-                    'be a Freesurfer-Segmentation')
+                print("Selected Folder doesn't seem to " "be a Freesurfer-Segmentation")
 
     def import_mri_subjects(self):
         parent_folder = QFileDialog.getExistingDirectory(
-            self, 'Choose a folder containting several '
-                  'Freesurfer-Segmentations')
+            self, "Choose a folder containting several " "Freesurfer-Segmentations"
+        )
         folder_list = sorted(
-            [f for f in os.listdir(parent_folder) if not f.startswith('.')],
-            key=str.lower)
+            [f for f in os.listdir(parent_folder) if not f.startswith(".")],
+            key=str.lower,
+        )
 
         for fsmri in folder_list:
             folder_path = join(parent_folder, fsmri)
-            if exists(join(folder_path, 'surf')):
-                if fsmri not in self.pr.all_fsmri \
-                        and fsmri not in self.folders:
+            if exists(join(folder_path, "surf")):
+                if fsmri not in self.pr.all_fsmri and fsmri not in self.folders:
                     self.folders.append(fsmri)
                     self.paths.update({fsmri: folder_path})
                 else:
-                    print(
-                        f'{fsmri} already existing in {self.ct.subjects_dir}')
+                    print(f"{fsmri} already existing in {self.ct.subjects_dir}")
             else:
-                print(
-                    'Selected Folder doesn\'t seem to be '
-                    'a Freesurfer-Segmentation')
+                print("Selected Folder doesn't seem to be " "a Freesurfer-Segmentation")
         self.populate_list_widget()
 
     def add_mri_subjects(self, worker_signals):
         worker_signals.pgbar_max.emit(len(self.folders))
         for n, name in enumerate(self.folders):
             if not worker_signals.was_canceled:
-                worker_signals.pgbar_text.emit(f'Copying {name}')
+                worker_signals.pgbar_text.emit(f"Copying {name}")
                 src = self.paths[name]
                 self.pr.add_fsmri(name, src)
                 worker_signals.pgbar_n.emit(n)
             else:
                 break
 
     def show_errors(self, err):
@@ -911,66 +980,70 @@
 
 class AddMRIDialog(AddMRIWidget):
     def __init__(self, main_win):
         super().__init__(main_win)
 
         self.dialog = QDialog(main_win)
 
-        close_bt = QPushButton('Close', self)
+        close_bt = QPushButton("Close", self)
         close_bt.clicked.connect(self.dialog.close)
         self.main_bt_layout.addWidget(close_bt)
 
         self.dialog.setLayout(self.layout)
         self.dialog.open()
 
 
 class FileDictWidget(QWidget):
     def __init__(self, main_win, mode):
-        """ A widget to assign MRI-Subjects or Empty-Room-Files to file(s)"""
+        """A widget to assign MRI-Subjects or Empty-Room-Files to file(s)"""
 
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
         self.mode = mode
-        if mode == 'mri':
-            self.title = 'Assign MEEG-Files to a FreeSurfer-Subject'
-            self.subtitles = (
-                'Choose a MEEG-File', 'Choose a FreeSurfer-Subject')
+        if mode == "mri":
+            self.title = "Assign MEEG-Files to a FreeSurfer-Subject"
+            self.subtitles = ("Choose a MEEG-File", "Choose a FreeSurfer-Subject")
         else:
-            self.title = 'Assign MEEG-File to a Empty-Room-File'
-            self.subtitles = (
-                'Choose a MEEG-File', 'Choose an Empty-Room-File')
+            self.title = "Assign MEEG-File to a Empty-Room-File"
+            self.subtitles = ("Choose a MEEG-File", "Choose an Empty-Room-File")
 
         self.init_ui()
 
     def init_ui(self):
         layout = QVBoxLayout()
-        if self.mode == 'mri':
-            assign_widget = AssignWidget(self.pr.all_meeg, self.pr.all_fsmri,
-                                         self.pr.meeg_to_fsmri,
-                                         title=self.title,
-                                         subtitles=self.subtitles)
+        if self.mode == "mri":
+            assign_widget = AssignWidget(
+                self.pr.all_meeg,
+                self.pr.all_fsmri,
+                self.pr.meeg_to_fsmri,
+                title=self.title,
+                subtitles=self.subtitles,
+            )
         else:
-            assign_widget = AssignWidget(self.pr.all_meeg, self.pr.all_erm,
-                                         self.pr.meeg_to_erm,
-                                         title=self.title,
-                                         subtitles=self.subtitles)
+            assign_widget = AssignWidget(
+                self.pr.all_meeg,
+                self.pr.all_erm,
+                self.pr.meeg_to_erm,
+                title=self.title,
+                subtitles=self.subtitles,
+            )
         layout.addWidget(assign_widget)
 
         self.setLayout(layout)
 
 
 class FileDictDialog(FileDictWidget):
     def __init__(self, main_win, mode):
         super().__init__(main_win, mode)
 
         dialog = QDialog(main_win)
 
-        close_bt = QPushButton('Close', self)
+        close_bt = QPushButton("Close", self)
         close_bt.clicked.connect(dialog.close)
         self.layout().addWidget(close_bt)
 
         dialog.setLayout(self.layout())
 
         set_ratio_geometry(0.6, self)
 
@@ -999,103 +1072,107 @@
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QGridLayout()
 
-        from_l = QLabel('Copy from:')
+        from_l = QLabel("Copy from:")
         layout.addWidget(from_l, 0, 0)
-        to_l = QLabel('Copy to:')
+        to_l = QLabel("Copy to:")
         layout.addWidget(to_l, 0, 1)
 
         # Preselect the current selected MEEG
         self.copy_from = [self.parent_w.current_obj.name]
         self.copy_tos = list()
 
-        self.listw1 = CheckList(self.all_files, self.copy_from,
-                                ui_buttons=False, one_check=True)
+        self.listw1 = CheckList(
+            self.all_files, self.copy_from, ui_buttons=False, one_check=True
+        )
         self.listw2 = CheckList(self.all_files, self.copy_tos)
 
         layout.addWidget(self.listw1, 1, 0)
         layout.addWidget(self.listw2, 1, 1)
 
-        copy_bt = QPushButton('Copy')
+        copy_bt = QPushButton("Copy")
         copy_bt.clicked.connect(self.copy_bads)
         layout.addWidget(copy_bt, 2, 0)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt, 2, 1)
 
         self.setLayout(layout)
 
     def copy_bads(self):
         # Check, that at least one item is selected in each list
         # and that the copy_from-item is in meeg_bad_channels
-        if len(self.copy_from) * len(self.copy_tos) > 0 \
-                and self.copy_from[0] in self.bad_channels_dict:
+        if (
+            len(self.copy_from) * len(self.copy_tos) > 0
+            and self.copy_from[0] in self.bad_channels_dict
+        ):
             for copy_to in self.copy_tos:
                 copy_bad_chs = self.bad_channels_dict[self.copy_from[0]].copy()
                 copy_to_info = MEEG(copy_to, self.parent_w.mw.ct).load_info()
                 # Make sure, that only channels which exist too
                 # in copy_to are copied
-                for rm_ch in [r for r in copy_bad_chs if
-                              r not in copy_to_info['ch_names']]:
+                for rm_ch in [
+                    r for r in copy_bad_chs if r not in copy_to_info["ch_names"]
+                ]:
                     copy_bad_chs.remove(rm_ch)
                 self.bad_channels_dict[copy_to] = copy_bad_chs
 
 
 class SubBadsWidget(QWidget):
-    """ A Dialog to select Bad-Channels for the files """
+    """A Dialog to select Bad-Channels for the files"""
 
     def __init__(self, main_win):
         """
         :param main_win: The parent-window for the dialog
         """
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
-        self.setWindowTitle('Assign bad_channels for your files')
+        self.setWindowTitle("Assign bad_channels for your files")
         self.bad_chkbts = dict()
         self.info_dict = dict()
         self.current_obj = None
         self.raw = None
         self.raw_fig = None
 
         self.init_ui()
 
     def init_ui(self):
         self.layout = QGridLayout()
 
-        file_list = self.pr.all_meeg + self.pr.all_erm
-        self.files_widget = CheckDictList(file_list, self.pr.meeg_bad_channels,
-                                          title='Files')
+        file_list = self.pr.all_meeg
+        self.files_widget = CheckDictList(
+            file_list, self.pr.meeg_bad_channels, title="Files"
+        )
         self.files_widget.currentChanged.connect(self.bad_dict_selected)
-        self.files_widget.setSizePolicy(QSizePolicy.Maximum,
-                                        QSizePolicy.Preferred)
+        self.files_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
         self.layout.addWidget(self.files_widget, 0, 0)
 
         self.bt_scroll = QScrollArea()
         self.bt_scroll.setWidgetResizable(True)
         self.layout.addWidget(self.bt_scroll, 0, 1)
 
         # Add Buttons
         self.bt_layout = QHBoxLayout()
 
-        plot_bt = QPushButton('Plot raw')
+        plot_bt = QPushButton("Plot raw")
         plot_bt.clicked.connect(self.plot_raw_bad)
         self.bt_layout.addWidget(plot_bt)
 
-        copy_bt = QPushButton('Copy Bads')
+        copy_bt = QPushButton("Copy Bads")
         copy_bt.clicked.connect(partial(CopyBadsDialog, self))
         self.bt_layout.addWidget(copy_bt)
 
-        self.save_raw_annot = QCheckBox('Save Annotations')
+        self.save_raw_annot = QCheckBox("Save Annotations")
         self.bt_layout.addWidget(self.save_raw_annot)
 
         self.layout.addLayout(self.bt_layout, 1, 0, 1, 2)
         self.setLayout(self.layout)
 
     def update_selection(self):
         # Clear entries
@@ -1127,15 +1204,15 @@
         # Currently, you have to fine-tune the max_h_size,
         # because it doesn't seem to reflect exactly the actual width
         max_h_size = int(self.bt_scroll.geometry().width() * 0.85)
 
         self.bad_chkbts = dict()
 
         # Make Checkboxes for channels in info
-        for x, ch_name in enumerate(info['ch_names']):
+        for ch_name in info["ch_names"]:
             chkbt = QCheckBox(ch_name)
             chkbt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             chkbt.clicked.connect(self.bad_ckbx_assigned)
             self.bad_chkbts[ch_name] = chkbt
             h_size += chkbt.sizeHint().width()
             if h_size > max_h_size:
                 column = 0
@@ -1155,87 +1232,88 @@
 
     def make_bad_chbxs(self):
         if self.current_obj:
             # Don't load info twice from file
             if self.current_obj.name in self.info_dict:
                 self._make_bad_chbxs(self.info_dict[self.current_obj.name])
             else:
-                worker_dlg = WorkerDialog(self, self.current_obj.load_info,
-                                          title='Loading Channels...')
+                worker_dlg = WorkerDialog(
+                    self, self.current_obj.load_info, title="Loading Channels..."
+                )
                 worker_dlg.thread_finished.connect(self._make_bad_chbxs)
 
     def bad_dict_selected(self, current, _):
         self.current_obj = MEEG(current, self.ct)
 
         # Close current Plot-Window
         if self.raw_fig:
-            if hasattr(self.raw_fig, 'canvas'):
+            if hasattr(self.raw_fig, "canvas"):
                 plt.close(self.raw_fig)
             else:
                 self.raw_fig.close()
 
         self.make_bad_chbxs()
 
     def _assign_bad_channels(self, bad_channels):
         # Directly replace value in bad_channels_dict
         # (needed for first-time assignment)
-        self.current_obj.pr.meeg_bad_channels[
-            self.current_obj.name] = bad_channels
+        self.current_obj.pr.meeg_bad_channels[self.current_obj.name] = bad_channels
         # Restore/Establish reference to direct object-attribute
         self.current_obj.bad_channels = bad_channels
         self.files_widget.content_changed()
 
     def bad_ckbx_assigned(self):
-        bad_channels = [ch for ch in self.bad_chkbts if
-                        self.bad_chkbts[ch].isChecked()]
+        bad_channels = [ch for ch in self.bad_chkbts if self.bad_chkbts[ch].isChecked()]
         self._assign_bad_channels(bad_channels)
 
     def set_chkbx_enable(self, enable):
         for chkbx in self.bad_chkbts:
             self.bad_chkbts[chkbx].setEnabled(enable)
 
     def get_selected_bads(self, _):
         # In-Place-Operations to maintain reference
         # from current_obj to meeg_bad_channels
-        bad_channels = self.raw.info['bads']
+        bad_channels = self.raw.info["bads"]
         self._assign_bad_channels(bad_channels)
         self.update_selection()
         self.set_chkbx_enable(True)
 
         if self.save_raw_annot.isChecked():
-            WorkerDialog(self, self.current_obj.save_raw, raw=self.raw,
-                         show_console=True,
-                         title='Saving raw with Annotations')
+            WorkerDialog(
+                self,
+                self.current_obj.save_raw,
+                raw=self.raw,
+                show_console=True,
+                title="Saving raw with Annotations",
+            )
 
         self.raw_fig = None
 
     def plot_raw_bad(self):
         # Disable CheckBoxes to avoid confusion
         # (Bad-Selection only goes unidirectional from Plot>GUI)
         self.set_chkbx_enable(False)
 
         plot_dialog = QDialog(self)
-        plot_dialog.setWindowTitle('Opening raw-Plot...')
+        plot_dialog.setWindowTitle("Opening raw-Plot...")
         plot_dialog.open()
         self.raw = self.current_obj.load_raw()
         try:
             events = self.current_obj.load_events()
         except FileNotFoundError:
             events = None
-        self.raw_fig = self.raw.plot(events=events, n_channels=30,
-                                     bad_color='red',
-                                     title=self.current_obj.name)
-        if hasattr(self.raw_fig, 'canvas'):
+        self.raw_fig = self.raw.plot(
+            events=events, n_channels=30, bad_color="red", title=self.current_obj.name
+        )
+        if hasattr(self.raw_fig, "canvas"):
             # Connect Closing of Matplotlib-Figure
             # to assignment of bad-channels
-            self.raw_fig.canvas.mpl_connect('close_event',
-                                            self.get_selected_bads)
+            self.raw_fig.canvas.mpl_connect("close_event", self.get_selected_bads)
         else:
-            self.raw_fig.gotClosed.connect(
-                partial(self.get_selected_bads, None))
+            self.raw_fig.gotClosed.connect(partial(self.get_selected_bads, None))
         plot_dialog.close()
 
     def resizeEvent(self, event):
         if self.current_obj:
             self.make_bad_chbxs()
             self.update_selection()
         event.accept()
@@ -1253,15 +1331,15 @@
         super().__init__(main_win)
 
         layout = QVBoxLayout()
 
         bads_widget = SubBadsWidget(main_win)
         layout.addWidget(bads_widget)
 
-        close_bt = QPushButton('Close', self)
+        close_bt = QPushButton("Close", self)
         close_bt.clicked.connect(self.close)
         bads_widget.bt_layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
         set_ratio_geometry(0.8, self)
 
@@ -1280,43 +1358,40 @@
 
 
 class SubjectWizard(QWizard):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
 
-        self.setWindowTitle('Subject-Wizard')
+        self.setWindowTitle("Subject-Wizard")
         self.setWizardStyle(QWizard.ModernStyle)
         self.setOption(QWizard.HaveHelpButton, False)
 
         set_ratio_geometry(0.6, self)
         center(self)
 
         self.add_pages()
         self.open()
 
     def add_pages(self):
         self.add_files_page = QWizardPage()
-        self.add_files_page.setTitle('Import .fif-Files')
+        self.add_files_page.setTitle("Import .fif-Files")
         layout = QVBoxLayout()
         layout.addWidget(AddFilesWidget(self.mw))
         self.add_files_page.setLayout(layout)
 
         self.add_mri_page = QWizardPage()
-        self.add_mri_page.setTitle('Import MRI-Files')
+        self.add_mri_page.setTitle("Import MRI-Files")
         layout = QVBoxLayout()
         layout.addWidget(AddMRIWidget(self.mw))
         self.add_mri_page.setLayout(layout)
 
-        self.assign_mri_page = FileDictWizardPage(self.mw, 'mri',
-                                                  'Assign File --> MRI')
-        self.assign_erm_page = FileDictWizardPage(self.mw, 'erm',
-                                                  'Assign File --> ERM')
-        self.assign_bad_channels_page = SubBadsWizPage(self.mw,
-                                                       'Assign Bad-Channels')
+        self.assign_mri_page = FileDictWizardPage(self.mw, "mri", "Assign File --> MRI")
+        self.assign_erm_page = FileDictWizardPage(self.mw, "erm", "Assign File --> ERM")
+        self.assign_bad_channels_page = SubBadsWizPage(self.mw, "Assign Bad-Channels")
 
         self.addPage(self.add_files_page)
         self.addPage(self.add_mri_page)
         self.addPage(self.assign_mri_page)
         self.addPage(self.assign_erm_page)
         self.addPage(self.assign_bad_channels_page)
 
@@ -1337,54 +1412,57 @@
         self.init_ui()
 
         self.open()
 
     def init_ui(self):
         list_layout = QHBoxLayout()
 
-        self.files = CheckDictList(self.pr.all_meeg, self.pr.meeg_event_id,
-                                   title='Files')
+        self.files = CheckDictList(
+            self.pr.all_meeg, self.pr.meeg_event_id, title="Files"
+        )
         self.files.currentChanged.connect(self.file_selected)
 
         list_layout.addWidget(self.files)
 
         event_id_layout = QVBoxLayout()
 
-        self.event_id_widget = EditDict(self.event_id, ui_buttons=True,
-                                        title='Event-ID')
+        self.event_id_widget = EditDict(
+            self.event_id, ui_buttons=True, title="Event-ID"
+        )
         # Connect editing of Event-ID-Table to update of Check-List
         self.event_id_widget.dataChanged.connect(self.update_check_list)
         self.event_id_widget.setToolTip(
-            'Add a Trial-Descriptor (as key) for each Event-ID (as value) '
-            'you want to include it in you analysis.\n'
-            'You can assign multiple descriptors per ID by '
-            'separating them by "/"')
+            "Add a Trial-Descriptor (as key) for each Event-ID (as value) "
+            "you want to include it in you analysis.\n"
+            "You can assign multiple descriptors per ID by "
+            'separating them by "/"'
+        )
         event_id_layout.addWidget(self.event_id_widget)
 
         self.event_id_label = QLabel()
         event_id_layout.addWidget(self.event_id_label)
 
         list_layout.addLayout(event_id_layout)
 
-        self.check_widget = CheckList(title='Select IDs')
+        self.check_widget = CheckList(title="Select IDs")
         list_layout.addWidget(self.check_widget)
 
         self.layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
 
-        apply_bt = QPushButton('Apply to')
+        apply_bt = QPushButton("Apply to")
         apply_bt.clicked.connect(partial(EvIDApply, self))
         bt_layout.addWidget(apply_bt)
 
-        show_events = QPushButton('Show events')
+        show_events = QPushButton("Show events")
         show_events.clicked.connect(self.show_events)
         bt_layout.addWidget(show_events)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         bt_layout.addWidget(close_bt)
 
         self.layout.addLayout(bt_layout)
 
         self.setLayout(self.layout)
 
@@ -1397,18 +1475,18 @@
         self.event_id_widget.replace_data(self.event_id)
 
         try:
             # Load events from File
             meeg = MEEG(self.name, self.ct, suppress_warnings=True)
             events = meeg.load_events()
         except FileNotFoundError:
-            self.event_id_label.setText(f'No events found for {self.name}')
+            self.event_id_label.setText(f"No events found for {self.name}")
         else:
             ids = np.unique(events[:, 2])
-            self.event_id_label.setText(f'events found: {ids}')
+            self.event_id_label.setText(f"events found: {ids}")
 
     def save_event_id(self):
         if self.name:
             if len(self.event_id) > 0:
                 # Write Event-ID to Project
                 self.pr.meeg_event_id[self.name] = self.event_id
 
@@ -1428,17 +1506,16 @@
         if self.name in self.pr.sel_event_id:
             self.checked_labels = self.pr.sel_event_id[self.name]
         else:
             self.checked_labels = list()
         self.update_check_list()
 
     def update_check_list(self):
-
         # Get selectable trials and update widget
-        prelabels = [i.split('/') for i in self.event_id.keys() if i != '']
+        prelabels = [i.split("/") for i in self.event_id.keys() if i != ""]
         if len(prelabels) > 0:
             # Concatenate all lists
             conc_labels = prelabels[0]
             if len(prelabels) > 1:
                 for item in prelabels[1:]:
                     conc_labels += item
             # Make sure that only unique labels exist
@@ -1454,19 +1531,17 @@
         self.check_widget.replace_data(self.labels)
         self.check_widget.replace_checked(self.checked_labels)
 
     def show_events(self):
         try:
             meeg = MEEG(self.name, self.ct, suppress_warnings=True)
             events = meeg.load_events()
-            mne.viz.plot_events(events, event_id=self.event_id or None,
-                                show=True)
+            mne.viz.plot_events(events, event_id=self.event_id or None, show=True)
         except FileNotFoundError:
-            QMessageBox.warning(self, 'No events!',
-                                f'No events found for {self.name}')
+            QMessageBox.warning(self, "No events!", f"No events found for {self.name}")
 
     def closeEvent(self, event):
         # Save event_id for last selected file
         self.save_event_id()
         event.accept()
 
 
@@ -1478,27 +1553,27 @@
 
         self.layout = QVBoxLayout()
         self.init_ui()
 
         self.open()
 
     def init_ui(self):
-        label = QLabel(f'Apply {self.p.name} to:')
+        label = QLabel(f"Apply {self.p.name} to:")
         self.layout.addWidget(label)
 
         self.check_listw = CheckList(self.p.pr.all_meeg, self.apply_to)
         self.layout.addWidget(self.check_listw)
 
         bt_layout = QHBoxLayout()
 
-        apply_bt = QPushButton('Apply')
+        apply_bt = QPushButton("Apply")
         apply_bt.clicked.connect(self.apply_evid)
         bt_layout.addWidget(apply_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         bt_layout.addWidget(close_bt)
 
         self.layout.addLayout(bt_layout)
         self.setLayout(self.layout)
 
     def apply_evid(self):
@@ -1520,64 +1595,65 @@
         self.from_meegs = list()
         for meeg_name in self.pr.all_meeg:
             meeg = MEEG(meeg_name, self.ct)
             if isfile(meeg.trans_path):
                 self.from_meegs.append(meeg_name)
 
         # Get the other MEEGs (wihtout trans-file)
-        self.to_meegs = [meeg for meeg in self.pr.all_meeg if
-                         meeg not in self.from_meegs]
+        self.to_meegs = [
+            meeg for meeg in self.pr.all_meeg if meeg not in self.from_meegs
+        ]
 
         self.current_meeg = None
         self.copy_tos = list()
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QGridLayout()
 
-        from_list = SimpleList(self.from_meegs, title='From:')
+        from_list = SimpleList(self.from_meegs, title="From:")
         from_list.currentChanged.connect(self.from_selected)
         layout.addWidget(from_list, 0, 0)
 
-        self.to_list = CheckList(self.to_meegs, self.copy_tos,
-                                 ui_button_pos='bottom', title='To:')
+        self.to_list = CheckList(
+            self.to_meegs, self.copy_tos, ui_button_pos="bottom", title="To:"
+        )
         layout.addWidget(self.to_list, 0, 1)
 
-        copy_bt = QPushButton('Copy')
+        copy_bt = QPushButton("Copy")
         copy_bt.clicked.connect(self.copy_trans)
         layout.addWidget(copy_bt, 1, 0)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt, 1, 1)
 
         self.setLayout(layout)
 
     def _compare_digs(self, worker_signals):
         self.copy_tos.clear()
         # Get Digitization points
-        current_dig = self.current_meeg.load_info()['dig']
+        current_dig = self.current_meeg.load_info()["dig"]
 
         # Add all meeg, which have the exact same digitization points
         # (assuming, that they can use the same trans-file)
         worker_signals.pgbar_max.emit(len(self.to_meegs))
         for n, to_meeg in enumerate(self.to_meegs):
-            worker_signals.pgbar_text.emit(f'Comparing: {to_meeg}')
-            if MEEG(to_meeg, self.ct).load_info()['dig'] == current_dig:
+            worker_signals.pgbar_text.emit(f"Comparing: {to_meeg}")
+            if MEEG(to_meeg, self.ct).load_info()["dig"] == current_dig:
                 self.copy_tos.append(to_meeg)
             worker_signals.pgbar_n.emit(n + 1)
 
         self.to_list.content_changed()
 
     def from_selected(self, current_meeg):
         self.current_meeg = MEEG(current_meeg, self.ct)
-        WorkerDialog(self, self._compare_digs, show_buttons=False,
-                     show_console=False)
+        WorkerDialog(self, self._compare_digs, show_buttons=False, show_console=False)
 
     def copy_trans(self):
         if self.current_meeg:
             from_path = self.current_meeg.trans_path
 
             for copy_to in self.copy_tos:
                 to_meeg = MEEG(copy_to, self.ct)
@@ -1626,84 +1702,86 @@
 
         set_ratio_geometry(0.8, self)
         self.show()
 
         self.start_load_threads()
 
     def get_file_tables(self, kind):
-
-        if kind == 'MEEG':
+        if kind == "MEEG":
             obj_list = self.pr.all_meeg
             obj_pd = self.pd_meeg
             obj_pd_time = self.pd_meeg_time
             obj_pd_size = self.pd_meeg_size
-        elif kind == 'FSMRI':
+        elif kind == "FSMRI":
             obj_list = self.pr.all_fsmri
             obj_pd = self.pd_fsmri
             obj_pd_time = self.pd_fsmri_time
             obj_pd_size = self.pd_fsmri_size
         else:
             obj_list = self.pr.all_groups
             obj_pd = self.pd_group
             obj_pd_time = self.pd_group_time
             obj_pd_size = self.pd_group_size
-        print(f'Loading {kind}')
+        print(f"Loading {kind}")
 
         for obj_name in obj_list:
-            if kind == 'MEEG':
+            if kind == "MEEG":
                 obj = MEEG(obj_name, self.ct)
-            elif kind == 'FSMRI':
+            elif kind == "FSMRI":
                 obj = FSMRI(obj_name, self.ct)
             else:
                 obj = Group(obj_name, self.ct)
 
             obj.get_existing_paths()
             self.param_results[obj_name] = dict()
 
             for path_type in obj.existing_paths:
                 if len(obj.existing_paths[path_type]) > 0:
-                    obj_pd.loc[obj_name, path_type] = 'exists'
+                    obj_pd.loc[obj_name, path_type] = "exists"
                     obj_pd_size.loc[obj_name, path_type] = 0
 
                     for path in obj.existing_paths[path_type]:
                         try:
                             # Add Time
                             # Last entry in TIME should be the most recent one
-                            obj_pd_time.loc[obj_name, path_type] = \
-                                obj.file_parameters[Path(path).name]['TIME']
+                            obj_pd_time.loc[obj_name, path_type] = obj.file_parameters[
+                                Path(path).name
+                            ]["TIME"]
                             # Add Size (accumulate, if there are several files)
-                            obj_pd_size.loc[obj_name, path_type] += \
-                                obj.file_parameters[Path(path).name]['SIZE']
+                            obj_pd_size.loc[obj_name, path_type] += obj.file_parameters[
+                                Path(path).name
+                            ]["SIZE"]
                         except KeyError:
                             pass
 
                         # Compare all parameters from last run to now
                         result_dict = compare_filep(obj, path, verbose=False)
                         # Store parameter-conflicts for later retrieval
                         self.param_results[obj_name][path_type] = result_dict
 
                         # Change status of path_type
                         # from object if there are conflicts
                         for parameter in result_dict:
                             if isinstance(result_dict[parameter], tuple):
                                 if result_dict[parameter][2]:
-                                    obj_pd.loc[obj_name, path_type] = \
-                                        'critical_conflict'
+                                    obj_pd.loc[
+                                        obj_name, path_type
+                                    ] = "critical_conflict"
                                 else:
-                                    obj_pd.loc[obj_name, path_type] = \
-                                        'possible_conflict'
+                                    obj_pd.loc[
+                                        obj_name, path_type
+                                    ] = "possible_conflict"
 
     def open_prog_dlg(self):
         # Create Progress-Dialog
         self.prog_bar = QProgressBar()
         self.prog_bar.setMinimum(0)
         self.prog_bar.setMaximum(3)
 
-        self.prog_dlg = SimpleDialog(self.prog_bar, self,
-                                     title='Loading Files...')
+        self.prog_dlg = SimpleDialog(self.prog_bar, self, title="Loading Files...")
 
     def thread_finished(self, _):
         self.load_prog += 1
         self.prog_bar.setValue(self.load_prog)
         if self.load_prog == 3:
             self.prog_dlg.close()
             self.meeg_table.content_changed()
@@ -1713,34 +1791,34 @@
     def thread_error(self, err):
         self.thread_finished(None)
         ErrorDialog(err, self)
 
     def start_load_threads(self):
         self.open_prog_dlg()
 
-        meeg_worker = Worker(function=self.get_file_tables, kind='MEEG')
+        meeg_worker = Worker(function=self.get_file_tables, kind="MEEG")
         meeg_worker.signals.error.connect(self.thread_error)
         meeg_worker.signals.finished.connect(self.thread_finished)
         meeg_worker.start()
 
-        fsmri_worker = Worker(function=self.get_file_tables, kind='FSMRI')
+        fsmri_worker = Worker(function=self.get_file_tables, kind="FSMRI")
         fsmri_worker.signals.error.connect(self.thread_error)
         fsmri_worker.signals.finished.connect(self.thread_finished)
         fsmri_worker.start()
 
-        group_worker = Worker(function=self.get_file_tables, kind='Group')
+        group_worker = Worker(function=self.get_file_tables, kind="Group")
         group_worker.signals.error.connect(self.thread_error)
         group_worker.signals.finished.connect(self.thread_finished)
         group_worker.start()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         mode_cmbx = QComboBox()
-        mode_cmbx.addItems(['Existence', 'Time', 'Size'])
+        mode_cmbx.addItems(["Existence", "Time", "Size"])
         mode_cmbx.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         mode_cmbx.currentTextChanged.connect(self.mode_changed)
         layout.addWidget(mode_cmbx, alignment=Qt.AlignLeft)
 
         tab_widget = QTabWidget()
 
         # MEEG
@@ -1748,97 +1826,97 @@
         meeg_layout = QVBoxLayout()
 
         self.meeg_table = FilePandasTable(self.pd_meeg)
         meeg_layout.addWidget(self.meeg_table)
 
         meeg_bt_layout = QHBoxLayout()
 
-        meeg_showp_bt = QPushButton('Show Parameters')
-        meeg_showp_bt.clicked.connect(partial(self.show_parameters, 'MEEG'))
+        meeg_showp_bt = QPushButton("Show Parameters")
+        meeg_showp_bt.clicked.connect(partial(self.show_parameters, "MEEG"))
         meeg_bt_layout.addWidget(meeg_showp_bt)
 
-        meeg_remove_bt = QPushButton('Remove File')
-        meeg_remove_bt.clicked.connect(partial(self.remove_file, 'MEEG'))
+        meeg_remove_bt = QPushButton("Remove File")
+        meeg_remove_bt.clicked.connect(partial(self.remove_file, "MEEG"))
         meeg_bt_layout.addWidget(meeg_remove_bt)
 
         meeg_layout.addLayout(meeg_bt_layout)
         meeg_widget.setLayout(meeg_layout)
 
-        tab_widget.addTab(meeg_widget, 'MEEG')
+        tab_widget.addTab(meeg_widget, "MEEG")
 
         # FSMRI
         fsmri_widget = QWidget()
         fsmri_layout = QVBoxLayout()
 
         self.fsmri_table = FilePandasTable(self.pd_fsmri)
         fsmri_layout.addWidget(self.fsmri_table)
 
         fsmri_bt_layout = QHBoxLayout()
 
-        fsmri_showp_bt = QPushButton('Show Parameters')
-        fsmri_showp_bt.clicked.connect(partial(self.show_parameters, 'FSMRI'))
+        fsmri_showp_bt = QPushButton("Show Parameters")
+        fsmri_showp_bt.clicked.connect(partial(self.show_parameters, "FSMRI"))
         fsmri_bt_layout.addWidget(fsmri_showp_bt)
 
-        fsmri_remove_bt = QPushButton('Remove File')
-        fsmri_remove_bt.clicked.connect(partial(self.remove_file, 'FSMRI'))
+        fsmri_remove_bt = QPushButton("Remove File")
+        fsmri_remove_bt.clicked.connect(partial(self.remove_file, "FSMRI"))
         fsmri_bt_layout.addWidget(fsmri_remove_bt)
 
         fsmri_layout.addLayout(fsmri_bt_layout)
         fsmri_widget.setLayout(fsmri_layout)
 
-        tab_widget.addTab(fsmri_widget, 'FSMRI')
+        tab_widget.addTab(fsmri_widget, "FSMRI")
 
         # Group
         group_widget = QWidget()
         group_layout = QVBoxLayout()
 
         self.group_table = FilePandasTable(self.pd_group)
         group_layout.addWidget(self.group_table)
 
         group_bt_layout = QHBoxLayout()
 
-        group_showp_bt = QPushButton('Show Parameters')
-        group_showp_bt.clicked.connect(partial(self.show_parameters, 'Group'))
+        group_showp_bt = QPushButton("Show Parameters")
+        group_showp_bt.clicked.connect(partial(self.show_parameters, "Group"))
         group_bt_layout.addWidget(group_showp_bt)
 
-        group_remove_bt = QPushButton('Remove File')
-        group_remove_bt.clicked.connect(partial(self.remove_file, 'Group'))
+        group_remove_bt = QPushButton("Remove File")
+        group_remove_bt.clicked.connect(partial(self.remove_file, "Group"))
         group_bt_layout.addWidget(group_remove_bt)
 
         group_layout.addLayout(group_bt_layout)
         group_widget.setLayout(group_layout)
 
-        tab_widget.addTab(group_widget, 'Group')
+        tab_widget.addTab(group_widget, "Group")
 
         layout.addWidget(tab_widget)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def mode_changed(self, mode):
-        if mode == 'Existence':
+        if mode == "Existence":
             self.meeg_table.replace_data(self.pd_meeg)
             self.fsmri_table.replace_data(self.pd_fsmri)
             self.group_table.replace_data(self.pd_group)
-        elif mode == 'Time':
+        elif mode == "Time":
             self.meeg_table.replace_data(self.pd_meeg_time)
             self.fsmri_table.replace_data(self.pd_fsmri_time)
             self.group_table.replace_data(self.pd_group_time)
-        elif mode == 'Size':
+        elif mode == "Size":
             self.meeg_table.replace_data(self.pd_meeg_size)
             self.fsmri_table.replace_data(self.pd_fsmri_size)
             self.group_table.replace_data(self.pd_group_size)
 
     def _get_current(self, kind):
-        if kind == 'MEEG':
+        if kind == "MEEG":
             current_list = self.meeg_table.get_current()
-        elif kind == 'FSMRI':
+        elif kind == "FSMRI":
             current_list = self.fsmri_table.get_current()
         else:
             current_list = self.group_table.get_current()
 
         if len(current_list) > 0:
             obj_name = current_list[0][1]
             path_type = current_list[0][2]
@@ -1854,51 +1932,62 @@
         Parameters
         ----------
         kind : str
             If it is MEEG, FSMRI or Group
         """
 
         # Pandas DataFrame to store parameters to be compared
-        compare_pd = pd.DataFrame(columns=['Previous', 'Current', 'Critical?'])
+        compare_pd = pd.DataFrame(columns=["Previous", "Current", "Critical?"])
 
         obj_name, path_type = self._get_current(kind)
 
-        if obj_name and path_type \
-                and obj_name in self.param_results \
-                and path_type in \
-                self.param_results[obj_name]:
+        if (
+            obj_name
+            and path_type
+            and obj_name in self.param_results
+            and path_type in self.param_results[obj_name]
+        ):
             result_dict = self.param_results[obj_name][path_type]
 
             for param in result_dict:
                 if isinstance(result_dict[param], tuple):
                     compare_pd.loc[param] = result_dict[param]
 
             if len(compare_pd.index) > 0:
                 # Show changed parameters
-                SimpleDialog(widget=SimplePandasTable(
-                    compare_pd, title='Changed Parameters', resize_rows=True,
-                    resize_columns=True), parent=self, scroll=False)
+                SimpleDialog(
+                    widget=SimplePandasTable(
+                        compare_pd,
+                        title="Changed Parameters",
+                        resize_rows=True,
+                        resize_columns=True,
+                    ),
+                    parent=self,
+                    scroll=False,
+                )
 
             else:
                 QMessageBox.information(
-                    self, 'All parameters equal!',
-                    'For the selected file all parameters are equal!')
+                    self,
+                    "All parameters equal!",
+                    "For the selected file all parameters are equal!",
+                )
 
     def _file_remover(self, selected_files, kind, worker_signals):
         worker_signals.pgbar_max.emit(len(selected_files))
         for idx, (_, obj_name, path_type) in enumerate(selected_files):
             if worker_signals.was_canceled:
-                worker_signals.pgbar_text.emit('Removing canceled')
+                worker_signals.pgbar_text.emit("Removing canceled")
                 break
-            if kind == 'MEEG':
+            if kind == "MEEG":
                 obj = MEEG(obj_name, self.ct)
                 obj_pd = self.pd_meeg
                 obj_pd_time = self.pd_meeg_time
                 obj_pd_size = self.pd_meeg_size
-            elif kind == 'FSMRI':
+            elif kind == "FSMRI":
                 obj = FSMRI(obj_name, self.ct)
                 obj_pd = self.pd_fsmri
                 obj_pd_time = self.pd_fsmri_time
                 obj_pd_size = self.pd_fsmri_size
             else:
                 obj = Group(obj_name, self.ct)
                 obj_pd = self.pd_group
@@ -1906,69 +1995,76 @@
                 obj_pd_size = self.pd_group_size
 
             obj_pd.loc[obj_name, path_type] = None
             obj_pd_time.loc[obj_name, path_type] = None
             obj_pd_size.loc[obj_name, path_type] = None
 
             # Remove File
-            worker_signals.pgbar_text.emit(f'Removing: {path_type}')
+            worker_signals.pgbar_text.emit(f"Removing: {path_type}")
             obj.remove_path(path_type)
             worker_signals.pgbar_n.emit(idx + 1)
 
     def _remove_finished(self, kind):
         # Update Table-Widget
-        if kind == 'MEEG':
+        if kind == "MEEG":
             obj_table = self.meeg_table
-        elif kind == 'FSMRI':
+        elif kind == "FSMRI":
             obj_table = self.fsmri_table
         else:
             obj_table = self.group_table
         obj_table.content_changed()
 
     def remove_file(self, kind):
-        """ Remove the file at the path of the current cell
+        """Remove the file at the path of the current cell
 
         Parameters
         ----------
         kind : str
             If it is MEEG, FSMRI or Group
 
         """
 
         msgbx = QMessageBox.question(
-            self, 'Remove files?',
-            'Do you really want to remove the selected Files?')
+            self, "Remove files?", "Do you really want to remove the selected Files?"
+        )
 
         if msgbx == QMessageBox.Yes:
-            if kind == 'MEEG':
+            if kind == "MEEG":
                 selected_files = self.meeg_table.get_selected()
-            elif kind == 'FSMRI':
+            elif kind == "FSMRI":
                 selected_files = self.fsmri_table.get_selected()
             else:
                 selected_files = self.group_table.get_selected()
-            wd = WorkerDialog(self, self._file_remover,
-                              selected_files=selected_files,
-                              kind=kind, show_buttons=True, show_console=True,
-                              title='Removing Files')
+            wd = WorkerDialog(
+                self,
+                self._file_remover,
+                selected_files=selected_files,
+                kind=kind,
+                show_buttons=True,
+                show_console=True,
+                title="Removing Files",
+            )
             wd.thread_finished.connect(partial(self._remove_finished, kind))
 
 
 class ICASelect(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
         self.current_obj = None
         self.parameters = dict()
         self.chkbxs = dict()
-        self.offline_plots = ['plot_ica_components',
-                              'plot_ica_sources',
-                              'plot_ica_scores',
-                              'plot_ica_overlay']
+        self.offline_plots = [
+            "plot_ica_components",
+            "plot_ica_sources",
+            "plot_ica_scores",
+            "plot_ica_overlay",
+        ]
         self.selected_offline_plots = list()
 
         self.max_width, self.max_height = set_ratio_geometry(0.8)
         self.setMaximumSize(self.max_width, self.max_height)
 
         self.init_ui()
         self.show()
@@ -1982,15 +2078,15 @@
         list_layout.addWidget(self.file_list)
 
         # Add Checkboxes for Components
         comp_scroll = QScrollArea()
         comp_widget = QWidget()
         self.comp_chkbx_layout = QGridLayout()
 
-        n_components = self.pr.parameters[self.pr.p_preset]['n_components']
+        n_components = self.pr.parameters[self.pr.p_preset]["n_components"]
         for idx in range(n_components):
             chkbx = QCheckBox(str(idx))
             chkbx.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             chkbx.clicked.connect(self.component_selected)
             self.chkbxs[idx] = chkbx
             self.comp_chkbx_layout.addWidget(chkbx, idx // 5, idx % 5)
 
@@ -2002,53 +2098,68 @@
         # offline_plot_list = CheckList(self.offline_plots,
         #                               self.selected_offline_plots,
         #                               title='Offline-Plots to select')
         # list_layout.addWidget(offline_plot_list)
 
         bt_layout = QVBoxLayout()
 
-        plot_comp_bt = QPushButton('Plot Components')
+        plot_comp_bt = QPushButton("Plot Components")
         plot_comp_bt.clicked.connect(self.plot_components)
         bt_layout.addWidget(plot_comp_bt)
 
         # Create Parameter-GUI which stores parameter in dictionary
         # (not the same as project.parameters)
-        ica_source_data_param = ComboGui(self.parameters, 'ica_source_data',
-                                         options=['raw', 'raw_filtered',
-                                                  'epochs', 'epochs_eog',
-                                                  'epochs (ECG)',
-                                                  'Evokeds', 'Evokeds (EOG)',
-                                                  'Evokeds (ECG)'],
-                                         default='raw_filtered')
+        ica_source_data_param = ComboGui(
+            self.parameters,
+            "ica_source_data",
+            options=[
+                "raw",
+                "raw_filtered",
+                "epochs",
+                "epochs_eog",
+                "epochs (ECG)",
+                "Evokeds",
+                "Evokeds (EOG)",
+                "Evokeds (ECG)",
+            ],
+            default="raw_filtered",
+        )
         bt_layout.addWidget(ica_source_data_param)
 
-        plot_source_bt = QPushButton('Plot Source')
+        plot_source_bt = QPushButton("Plot Source")
         plot_source_bt.clicked.connect(self.plot_sources)
         bt_layout.addWidget(plot_source_bt)
 
-        ica_overlay_data_param = ComboGui(self.parameters, 'ica_overlay_data',
-                                          options=['raw', 'raw_filtered',
-                                                   'Evokeds', 'Evokeds (EOG)',
-                                                   'Evokeds (ECG)'],
-                                          default='raw_filtered')
+        ica_overlay_data_param = ComboGui(
+            self.parameters,
+            "ica_overlay_data",
+            options=[
+                "raw",
+                "raw_filtered",
+                "Evokeds",
+                "Evokeds (EOG)",
+                "Evokeds (ECG)",
+            ],
+            default="raw_filtered",
+        )
         bt_layout.addWidget(ica_overlay_data_param)
 
-        plot_overlay_bt = QPushButton('Plot Overlay')
+        plot_overlay_bt = QPushButton("Plot Overlay")
         plot_overlay_bt.clicked.connect(self.plot_overlay)
         bt_layout.addWidget(plot_overlay_bt)
 
-        plot_overlay_bt = QPushButton('Plot Properties')
+        plot_overlay_bt = QPushButton("Plot Properties")
         plot_overlay_bt.clicked.connect(self.plot_properties)
         bt_layout.addWidget(plot_overlay_bt)
 
-        close_plots_bt = QPushButton('Close Plots')
-        close_plots_bt.clicked.connect(partial(plt.close, 'all'))
+        close_plots_bt = QPushButton("Close Plots")
+        close_plots_bt.clicked.connect(partial(plt.close, "all"))
         bt_layout.addWidget(close_plots_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         bt_layout.addWidget(close_bt)
 
         list_layout.addLayout(bt_layout)
         self.main_layout.addLayout(list_layout)
 
         self.setLayout(self.main_layout)
@@ -2073,18 +2184,20 @@
                 self.pr.ica_exclude[self.current_obj.name].remove(idx)
 
     def update_plots(self):
         # Remove old layout with plots
         if self.main_layout.count() > 1:
             old_layout = self.main_layout.itemAt(self.main_layout.count() - 1)
             self.main_layout.removeItem(old_layout)
-            for sub_layout in [old_layout.itemAt(idx).layout() for idx in
-                               range(old_layout.count())]:
-                for widget in [sub_layout.itemAt(idx).widget() for idx in
-                               range(sub_layout.count())]:
+            for sub_layout in [
+                old_layout.itemAt(idx).layout() for idx in range(old_layout.count())
+            ]:
+                for widget in [
+                    sub_layout.itemAt(idx).widget() for idx in range(sub_layout.count())
+                ]:
                     widget.deleteLater()
             del old_layout
 
         plot_layout = QHBoxLayout()
 
         for plot_func in self.selected_offline_plots:
             sub_plot_layout = QVBoxLayout()
@@ -2107,16 +2220,17 @@
     def obj_selected(self, current_name):
         self.current_obj = MEEG(current_name, self.ct)
         self.update_chkbxs()
         self.update_plots()
 
     def component_selected(self):
         if self.current_obj:
-            self.pr.ica_exclude[self.current_obj.name] = \
-                [idx for idx in self.chkbxs if self.chkbxs[idx].isChecked()]
+            self.pr.ica_exclude[self.current_obj.name] = [
+                idx for idx in self.chkbxs if self.chkbxs[idx].isChecked()
+            ]
         self.file_list.content_changed()
 
     def set_chkbx_enable(self, enable):
         for chkbx in self.chkbxs:
             self.chkbxs[chkbx].setEnabled(enable)
 
     def get_selected_components(self, ica, _):
@@ -2127,102 +2241,108 @@
 
     def plot_components(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
-            dialog.setWindowTitle('Opening...')
+            dialog.setWindowTitle("Opening...")
             dialog.open()
             try:
-                figs, ica = plot_ica_components(meeg=self.current_obj,
-                                                show_plots=True)
+                figs, ica = plot_ica_components(meeg=self.current_obj, show_plots=True)
                 if not isinstance(figs, list):
                     figs = [figs]
                 for fig in figs:
-                    fig.canvas.mpl_connect('close_event',
-                                           partial(
-                                               self.get_selected_components,
-                                               ica))
-            except:  # noqa: E722
+                    fig.canvas.mpl_connect(
+                        "close_event", partial(self.get_selected_components, ica)
+                    )
+            except Exception:
                 err_tuple = get_exception_tuple()
-                QMessageBox.critical(self, 'An Error ocurred!',
-                                     f'{err_tuple[0]}: {err_tuple[1]}\n'
-                                     f'{err_tuple[2]}')
+                QMessageBox.critical(
+                    self,
+                    "An Error ocurred!",
+                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
+                )
                 self.set_chkbx_enable(True)
             finally:
                 dialog.close()
 
     def plot_sources(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
-            dialog.setWindowTitle('Opening...')
+            dialog.setWindowTitle("Opening...")
             dialog.open()
             try:
-                figs, ica = plot_ica_sources(meeg=self.current_obj,
-                                             ica_source_data=self.parameters[
-                                                 'ica_source_data'],
-                                             show_plots=True)
+                figs, ica = plot_ica_sources(
+                    meeg=self.current_obj,
+                    ica_source_data=self.parameters["ica_source_data"],
+                    show_plots=True,
+                )
                 if not isinstance(figs, list):
                     figs = [figs]
                 for fig in figs:
-                    fig.canvas.mpl_connect('close_event',
-                                           partial(
-                                               self.get_selected_components,
-                                               ica))
-            except:  # noqa: E722
+                    fig.canvas.mpl_connect(
+                        "close_event", partial(self.get_selected_components, ica)
+                    )
+            except Exception:
                 err_tuple = get_exception_tuple()
-                QMessageBox.critical(self, 'An Error ocurred!',
-                                     f'{err_tuple[0]}: {err_tuple[1]}\n'
-                                     f'{err_tuple[2]}')
+                QMessageBox.critical(
+                    self,
+                    "An Error ocurred!",
+                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
+                )
                 self.set_chkbx_enable(False)
             finally:
                 dialog.close()
 
     def plot_overlay(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
-            dialog.setWindowTitle('Opening...')
+            dialog.setWindowTitle("Opening...")
             dialog.open()
             try:
-                plot_ica_overlay(meeg=self.current_obj,
-                                 ica_overlay_data=self.parameters[
-                                     'ica_overlay_data'],
-                                 show_plots=True)
-            except:  # noqa: E722
+                plot_ica_overlay(
+                    meeg=self.current_obj,
+                    ica_overlay_data=self.parameters["ica_overlay_data"],
+                    show_plots=True,
+                )
+            except Exception:
                 err_tuple = get_exception_tuple()
-                QMessageBox.critical(self, 'An Error ocurred!',
-                                     f'{err_tuple[0]}: {err_tuple[1]}\n'
-                                     f'{err_tuple[2]}')
+                QMessageBox.critical(
+                    self,
+                    "An Error ocurred!",
+                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
+                )
                 self.set_chkbx_enable(False)
             finally:
                 dialog.close()
 
     def plot_properties(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
-            dialog.setWindowTitle('Opening...')
+            dialog.setWindowTitle("Opening...")
             dialog.open()
             try:
-                plot_ica_properties(meeg=self.current_obj,
-                                    show_plots=True)
-            except:  # noqa: E722
+                plot_ica_properties(meeg=self.current_obj, show_plots=True)
+            except Exception:
                 err_tuple = get_exception_tuple()
-                QMessageBox.critical(self, 'An Error ocurred!',
-                                     f'{err_tuple[0]}: {err_tuple[1]}\n'
-                                     f'{err_tuple[2]}')
+                QMessageBox.critical(
+                    self,
+                    "An Error ocurred!",
+                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
+                )
                 self.set_chkbx_enable(False)
             finally:
                 dialog.close()
 
 
 class ReloadRaw(QDialog):
     def __init__(self, main_win):
@@ -2233,45 +2353,47 @@
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
-        self.raw_list = SimpleList(self.pr.all_meeg,
-                                   title='Select raw to reload')
+        self.raw_list = SimpleList(self.pr.all_meeg, title="Select raw to reload")
         layout.addWidget(self.raw_list)
 
-        reload_bt = QPushButton('Reload')
+        reload_bt = QPushButton("Reload")
         reload_bt.clicked.connect(self.start_reload)
         layout.addWidget(reload_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def reload_raw(self, selected_raw, raw_path):
         meeg = MEEG(selected_raw, self.ct)
         raw = mne.io.read_raw(raw_path, preload=True)
         meeg.save_raw(raw)
-        print(f'Reloaded raw for {selected_raw}')
+        print(f"Reloaded raw for {selected_raw}")
 
     def start_reload(self):
         # Not with partial because otherwise the clicked-arg
         # from clicked goes into *args
         selected_raw = self.raw_list.get_current()
-        raw_path = QFileDialog.getOpenFileName(self, 'Select raw for Reload')[
-            0]
+        raw_path = QFileDialog.getOpenFileName(self, "Select raw for Reload")[0]
         if raw_path:
-            WorkerDialog(self, self.reload_raw, selected_raw=selected_raw,
-                         raw_path=raw_path,
-                         show_console=True,
-                         title=f'Reloading raw for {selected_raw}')
+            WorkerDialog(
+                self,
+                self.reload_raw,
+                selected_raw=selected_raw,
+                raw_path=raw_path,
+                show_console=True,
+                title=f"Reloading raw for {selected_raw}",
+            )
 
 
 class ExportDialog(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
@@ -2292,47 +2414,52 @@
             if isinstance(self.common_types, list):
                 self.common_types = type_set
             else:
                 self.common_types = self.common_types & type_set
             self.export_paths[meeg_name] = meeg.existing_paths
 
     def _get_destination(self):
-        dest = \
-            QFileDialog.getExistingDirectory(
-                self, 'Select Destination-Folder')[0]
+        dest = QFileDialog.getExistingDirectory(self, "Select Destination-Folder")[0]
         if dest:
             self.dest_path = dest
 
     def _init_ui(self):
         layout = QVBoxLayout()
-        self.dest_label = QLabel('<No Destination-Folder set>')
+        self.dest_label = QLabel("<No Destination-Folder set>")
         layout.addWidget(self.dest_label)
-        dest_bt = QPushButton('Set Destination-Folder')
+        dest_bt = QPushButton("Set Destination-Folder")
         dest_bt.clicked.connect(self._get_destination)
         layout.addWidget(dest_bt)
         layout.addWidget(QLabel())
-        layout.addWidget(SimpleList(self.ct.pr.sel_meeg,
-                                    title='Export selected data for the '
-                                          'following MEEG-Files:'))
         layout.addWidget(
-            CheckList(list(self.common_types), self.selected_types,
-                      title='Selected Data-Types'))
-        export_bt = QPushButton('Export')
+            SimpleList(
+                self.ct.pr.sel_meeg,
+                title="Export selected data for the " "following MEEG-Files:",
+            )
+        )
+        layout.addWidget(
+            CheckList(
+                list(self.common_types),
+                self.selected_types,
+                title="Selected Data-Types",
+            )
+        )
+        export_bt = QPushButton("Export")
         export_bt.clicked.connect(self.export_data)
         layout.addWidget(export_bt)
         self.setLayout(layout)
 
     def export_data(self):
         if self.dest_path:
-            print('Starting Export\n')
+            print("Starting Export\n")
             for meeg_name, path_types in self.export_paths.items():
                 os.mkdir(join(self.dest_path, meeg_name))
-                for path_type in [pt for pt in path_types if
-                                  pt in self.selected_types]:
+                for path_type in [pt for pt in path_types if pt in self.selected_types]:
                     paths = path_types[path_type]
                     for src_path in paths:
                         dest_name = Path(src_path).name
-                        shutil.copy2(src_path, join(self.dest_path, meeg_name,
-                                                    dest_name))
-                    print(f'\r{meeg_name}: Copying {path_type}...')
+                        shutil.copy2(
+                            src_path, join(self.dest_path, meeg_name, dest_name)
+                        )
+                    print(f"\r{meeg_name}: Copying {path_type}...")
         else:
-            QMessageBox.warning(self, 'Ups!', 'Destination-Path not set!')
+            QMessageBox.warning(self, "Ups!", "Destination-Path not set!")
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/main_window.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/main_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,110 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import sys
 from functools import partial
 
 import mne
 import pandas as pd
 from PyQt5.QtCore import Qt, pyqtSignal
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QAction, QApplication, QComboBox, QFileDialog,
-                             QGridLayout, QGroupBox, QHBoxLayout, QLabel,
-                             QMainWindow, QMessageBox, QPushButton,
-                             QScrollArea, QSizePolicy, QTabWidget,
-                             QVBoxLayout, QWidget)
+from PyQt5.QtWidgets import (
+    QAction,
+    QApplication,
+    QComboBox,
+    QFileDialog,
+    QGridLayout,
+    QGroupBox,
+    QHBoxLayout,
+    QLabel,
+    QMainWindow,
+    QMessageBox,
+    QPushButton,
+    QScrollArea,
+    QSizePolicy,
+    QTabWidget,
+    QVBoxLayout,
+    QWidget,
+)
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.functions.plot import close_all
-from mne_pipeline_hd.gui.dialogs import (QuickGuide, RawInfo,
-                                         RemoveProjectsDlg,
-                                         SysInfoMsg, AboutDialog,
-                                         CopyParamsDialog)
-from mne_pipeline_hd.gui.education_widgets import (EducationEditor,
-                                                   EducationTour)
-from mne_pipeline_hd.gui.function_widgets import (AddKwargs,
-                                                  ChooseCustomModules,
-                                                  CustomFunctionImport,
-                                                  RunDialog)
-from mne_pipeline_hd.gui.gui_utils import (QProcessDialog, WorkerDialog,
-                                           center,
-                                           set_ratio_geometry, get_std_icon,
-                                           get_user_input_string)
-from mne_pipeline_hd.gui.loading_widgets import (AddFilesDialog, AddMRIDialog,
-                                                 CopyTrans, EventIDGui,
-                                                 FileDictDialog, FileDock,
-                                                 FileManagment, ICASelect,
-                                                 ReloadRaw, SubBadsDialog,
-                                                 SubjectWizard, ExportDialog)
-from mne_pipeline_hd.gui.parameter_widgets import (BoolGui, IntGui,
-                                                   ParametersDock, SettingsDlg)
+from mne_pipeline_hd.gui.dialogs import (
+    QuickGuide,
+    RawInfo,
+    RemoveProjectsDlg,
+    SysInfoMsg,
+    AboutDialog,
+    CopyParamsDialog,
+)
+from mne_pipeline_hd.gui.education_widgets import EducationEditor, EducationTour
+from mne_pipeline_hd.gui.function_widgets import (
+    AddKwargs,
+    ChooseCustomModules,
+    CustomFunctionImport,
+    RunDialog,
+)
+from mne_pipeline_hd.gui.gui_utils import (
+    QProcessDialog,
+    WorkerDialog,
+    center,
+    set_ratio_geometry,
+    get_std_icon,
+    get_user_input_string,
+)
+from mne_pipeline_hd.gui.loading_widgets import (
+    AddFilesDialog,
+    AddMRIDialog,
+    CopyTrans,
+    EventIDGui,
+    FileDictDialog,
+    FileDock,
+    FileManagment,
+    ICASelect,
+    ReloadRaw,
+    SubBadsDialog,
+    SubjectWizard,
+    ExportDialog,
+)
+from mne_pipeline_hd.gui.parameter_widgets import (
+    BoolGui,
+    IntGui,
+    ParametersDock,
+    SettingsDlg,
+)
 from mne_pipeline_hd.gui.plot_widgets import PlotViewSelection
 from mne_pipeline_hd.gui.tools import DataTerminal
 from mne_pipeline_hd.pipeline.controller import Controller
-from mne_pipeline_hd.pipeline.pipeline_utils import (restart_program, ismac,
-                                                     QS, _run_from_script,
-                                                     iswin)
+from mne_pipeline_hd.pipeline.pipeline_utils import (
+    restart_program,
+    ismac,
+    QS,
+    _run_from_script,
+    iswin,
+)
 
 
 class MainWindow(QMainWindow):
     # Define Main-Window-Signals to send into QThread
     # to control function execution
     cancel_functions = pyqtSignal(bool)
     plot_running = pyqtSignal(bool)
 
     def __init__(self, controller):
         super().__init__()
-        _object_refs['main_window'] = self
-        self.setWindowTitle('MNE-Pipeline HD')
+        _object_refs["main_window"] = self
+        self.setWindowTitle("MNE-Pipeline HD")
 
         # Set QThread as default (ToDo: MP)
-        QS().setValue('use_qthread', True)
+        QS().setValue("use_qthread", True)
 
         # Initiate attributes for Main-Window
         self.ct = controller
         self.pr = controller.pr
         self.edu_tour = None
         self.bt_dict = dict()
         # For functions, which should or should not
@@ -91,59 +127,63 @@
         self.init_edu()
 
         center(self)
 
         self.first_init = False
 
     def update_project_ui(self):
-
         # Redraw function-buttons and parameter-widgets
         self.redraw_func_and_param()
         # Update Subject-Lists
         self.file_dock.update_dock()
         # Update Project-Box
         self.update_project_box()
         # Update Statusbar
-        self.statusBar().showMessage(f'Home-Path: {self.ct.home_path}, '
-                                     f'Project: {self.pr.name}')
+        self.statusBar().showMessage(
+            f"Home-Path: {self.ct.home_path}, " f"Project: {self.pr.name}"
+        )
 
     def change_home_path(self):
         # First save the former projects-data
         WorkerDialog(self, self.ct.save, blocking=True)
 
         new_home_path = QFileDialog.getExistingDirectory(
-            self, 'Change your Home-Path (top-level folder of Pipeline-Data)')
-        if new_home_path != '':
+            self, "Change your Home-Path (top-level folder of Pipeline-Data)"
+        )
+        if new_home_path != "":
             try:
                 new_controller = Controller(new_home_path)
             except RuntimeError as err:
-                QMessageBox.critical(self, 'Error with selected Home-Path',
-                                     str(err))
+                QMessageBox.critical(self, "Error with selected Home-Path", str(err))
             else:
                 if new_controller.pr is None:
                     new_project = get_user_input_string(
-                        'There is no project in this Home-Path,'
-                        ' please enter a name for a new project:',
-                        'Add Project!', force=True)
+                        "There is no project in this Home-Path,"
+                        " please enter a name for a new project:",
+                        "Add Project!",
+                        force=True,
+                    )
                     self.pr = new_controller.change_project(new_project)
 
                 self.ct = new_controller
-                welcome_window = _object_refs['welcome_window']
+                welcome_window = _object_refs["welcome_window"]
                 if welcome_window is not None:
                     welcome_window.ct = new_controller
-                self.statusBar().showMessage(f'Home-Path: {self.ct.home_path},'
-                                             f' Project: {self.pr.name}')
+                self.statusBar().showMessage(
+                    f"Home-Path: {self.ct.home_path}," f" Project: {self.pr.name}"
+                )
                 self.update_project_ui()
 
     def add_project(self):
         # First save the former projects-data
         WorkerDialog(self, self.pr.save, blocking=True)
 
-        new_project = get_user_input_string('Enter a name for a new project',
-                                            'Add Project')
+        new_project = get_user_input_string(
+            "Enter a name for a new project", "Add Project"
+        )
         if new_project is not None:
             self.pr = self.ct.change_project(new_project)
             self.update_project_ui()
 
     def remove_project(self):
         # First save the former projects-data
         WorkerDialog(self, self.pr.save, blocking=True)
@@ -159,227 +199,262 @@
 
         # Change project
         self.pr = self.ct.change_project(project)
 
         self.update_project_ui()
 
     def pr_clean_fp(self):
-        WorkerDialog(self, self.pr.clean_file_parameters, show_buttons=True,
-                     show_console=True, close_directly=False,
-                     title='Cleaning File-Parameters')
+        WorkerDialog(
+            self,
+            self.pr.clean_file_parameters,
+            show_buttons=True,
+            show_console=True,
+            close_directly=False,
+            title="Cleaning File-Parameters",
+        )
 
     def pr_clean_pf(self):
-        WorkerDialog(self, self.pr.clean_plot_files, show_buttons=True,
-                     show_console=True, close_directly=False,
-                     title='Cleaning Plot-Files')
+        WorkerDialog(
+            self,
+            self.pr.clean_plot_files,
+            show_buttons=True,
+            show_console=True,
+            close_directly=False,
+            title="Cleaning Plot-Files",
+        )
 
     def pr_copy_parameters(self):
         CopyParamsDialog(self)
 
     def update_project_box(self):
         self.project_box.clear()
         self.project_box.addItems(self.ct.projects)
         if self.pr is not None:
             self.project_box.setCurrentText(self.pr.name)
 
     def init_edu(self):
-        if QS().value('education') and \
-                self.ct.edu_program and \
-                len(self.ct.edu_program['tour_list']) > 0:
+        if (
+            QS().value("education")
+            and self.ct.edu_program
+            and len(self.ct.edu_program["tour_list"]) > 0
+        ):
             self.edu_tour = EducationTour(self, self.ct.edu_program)
 
     def init_menu(self):
         # & in front of text-string creates automatically a shortcut
         # with Alt + <letter after &>
         # Input
-        import_menu = self.menuBar().addMenu('&Import')
+        import_menu = self.menuBar().addMenu("&Import")
 
-        aaddfiles = QAction('Add MEEG', parent=self)
-        aaddfiles.setShortcut('Ctrl+M')
-        aaddfiles.setStatusTip('Add your MEG-Files here')
+        aaddfiles = QAction("Add MEEG", parent=self)
+        aaddfiles.setShortcut("Ctrl+M")
+        aaddfiles.setStatusTip("Add your MEG-Files here")
         aaddfiles.triggered.connect(partial(AddFilesDialog, self))
         import_menu.addAction(aaddfiles)
 
-        import_menu.addAction('Add Sample-Dataset', self.add_sample_dataset)
-        import_menu.addAction('Add Test-Dataset', self.add_test_dataset)
-        import_menu.addAction('Reload raw', partial(ReloadRaw, self))
+        import_menu.addAction("Add Sample-Dataset", self.add_sample_dataset)
+        import_menu.addAction("Add Test-Dataset", self.add_test_dataset)
+        import_menu.addAction("Reload raw", partial(ReloadRaw, self))
 
         import_menu.addSeparator()
 
-        aaddmri = QAction('Add Freesurfer-MRI', self)
-        aaddmri.setShortcut('Ctrl+F')
-        aaddmri.setStatusTip('Add your Freesurfer-Segmentations here')
+        aaddmri = QAction("Add Freesurfer-MRI", self)
+        aaddmri.setShortcut("Ctrl+F")
+        aaddmri.setStatusTip("Add your Freesurfer-Segmentations here")
         aaddmri.triggered.connect(partial(AddMRIDialog, self))
         import_menu.addAction(aaddmri)
 
-        import_menu.addAction('Add fsaverage', self.add_fsaverage)
+        import_menu.addAction("Add fsaverage", self.add_fsaverage)
 
         import_menu.addSeparator()
 
-        import_menu.addAction('Show Info', partial(RawInfo, self))
-        import_menu.addAction('File-Management', partial(FileManagment, self))
+        import_menu.addAction("Show Info", partial(RawInfo, self))
+        import_menu.addAction("File-Management", partial(FileManagment, self))
 
-        export_menu = self.menuBar().addMenu('&Export')
-        export_menu.addAction('Export MEEG', partial(ExportDialog, self))
+        export_menu = self.menuBar().addMenu("&Export")
+        export_menu.addAction("Export MEEG", partial(ExportDialog, self))
 
-        prep_menu = self.menuBar().addMenu('&Preparation')
-        prep_menu.addAction('Subject-Wizard', partial(SubjectWizard, self))
+        prep_menu = self.menuBar().addMenu("&Preparation")
+        prep_menu.addAction("Subject-Wizard", partial(SubjectWizard, self))
 
         prep_menu.addSeparator()
 
-        prep_menu.addAction('Assign MEEG --> Freesurfer-MRI',
-                            partial(FileDictDialog, self, 'mri'))
-        prep_menu.addAction('Assign MEEG --> Empty-Room',
-                            partial(FileDictDialog, self, 'erm'))
-        prep_menu.addAction('Assign Bad-Channels --> MEEG',
-                            partial(SubBadsDialog, self))
-        prep_menu.addAction('Assign Event-IDs --> MEEG',
-                            partial(EventIDGui, self))
-        prep_menu.addAction('Select ICA-Components', partial(ICASelect, self))
+        prep_menu.addAction(
+            "Assign MEEG --> Freesurfer-MRI", partial(FileDictDialog, self, "mri")
+        )
+        prep_menu.addAction(
+            "Assign MEEG --> Empty-Room", partial(FileDictDialog, self, "erm")
+        )
+        prep_menu.addAction(
+            "Assign Bad-Channels --> MEEG", partial(SubBadsDialog, self)
+        )
+        prep_menu.addAction("Assign Event-IDs --> MEEG", partial(EventIDGui, self))
+        prep_menu.addAction("Select ICA-Components", partial(ICASelect, self))
 
         prep_menu.addSeparator()
 
-        prep_menu.addAction('MRI-Coregistration', mne.gui.coregistration)
-        prep_menu.addAction('Copy Transformation', partial(CopyTrans, self))
+        prep_menu.addAction("MRI-Coregistration", mne.gui.coregistration)
+        prep_menu.addAction("Copy Transformation", partial(CopyTrans, self))
 
         prep_menu.addSeparator()
 
         # Project
-        project_menu = self.menuBar().addMenu('&Project')
-        project_menu.addAction('&Clean File-Parameters', self.pr_clean_fp)
-        project_menu.addAction('&Clean Plot-Files', self.pr_clean_pf)
-        project_menu.addAction('&Copy Parameters between Projects',
-                               self.pr_copy_parameters)
+        project_menu = self.menuBar().addMenu("&Project")
+        project_menu.addAction("&Clean File-Parameters", self.pr_clean_fp)
+        project_menu.addAction("&Clean Plot-Files", self.pr_clean_pf)
+        project_menu.addAction(
+            "&Copy Parameters between Projects", self.pr_copy_parameters
+        )
 
         # Custom-Functions
-        func_menu = self.menuBar().addMenu('&Functions')
-        func_menu.addAction('&Import Custom',
-                            partial(CustomFunctionImport, self))
+        func_menu = self.menuBar().addMenu("&Functions")
+        func_menu.addAction("&Import Custom", partial(CustomFunctionImport, self))
 
-        func_menu.addAction('&Choose Custom-Modules',
-                            partial(ChooseCustomModules, self))
+        func_menu.addAction(
+            "&Choose Custom-Modules", partial(ChooseCustomModules, self)
+        )
 
-        func_menu.addAction('&Reload Modules', self.ct.reload_modules)
+        func_menu.addAction("&Reload Modules", self.ct.reload_modules)
         func_menu.addSeparator()
-        func_menu.addAction('Additional Keyword-Arguments',
-                            partial(AddKwargs, self))
+        func_menu.addAction("Additional Keyword-Arguments", partial(AddKwargs, self))
 
         # Education
-        education_menu = self.menuBar().addMenu('&Education')
+        education_menu = self.menuBar().addMenu("&Education")
         if self.ct.edu_program is None:
-            education_menu.addAction('&Education-Editor',
-                                     partial(EducationEditor, self))
+            education_menu.addAction(
+                "&Education-Editor", partial(EducationEditor, self)
+            )
         else:
-            education_menu.addAction('&Start Education-Tour', self.init_edu)
+            education_menu.addAction("&Start Education-Tour", self.init_edu)
 
         # Tools
-        tool_menu = self.menuBar().addMenu('&Tools')
-        tool_menu.addAction('&Data-Terminal', partial(DataTerminal, self))
-        tool_menu.addAction('&Plot-Viewer', partial(PlotViewSelection, self))
+        tool_menu = self.menuBar().addMenu("&Tools")
+        tool_menu.addAction("&Data-Terminal", partial(DataTerminal, self))
+        tool_menu.addAction("&Plot-Viewer", partial(PlotViewSelection, self))
 
         # View
-        self.view_menu = self.menuBar().addMenu('&View')
+        self.view_menu = self.menuBar().addMenu("&View")
         if not ismac:
-            self.view_menu.addAction('&Full-Screen',
-                                     self.full_screen).setCheckable(True)
+            self.view_menu.addAction("&Full-Screen", self.full_screen).setCheckable(
+                True
+            )
 
         # Settings
-        settings_menu = self.menuBar().addMenu('&Settings')
+        settings_menu = self.menuBar().addMenu("&Settings")
 
-        settings_menu.addAction('&Open Settings',
-                                partial(SettingsDlg, self, self.ct))
-        settings_menu.addAction('&Change Home-Path', self.change_home_path)
+        settings_menu.addAction("&Open Settings", partial(SettingsDlg, self, self.ct))
+        settings_menu.addAction("&Change Home-Path", self.change_home_path)
         settings_menu.addSeparator()
-        settings_menu.addAction('&Update Pipeline (stable)',
-                                partial(self.update_pipeline, 'stable'))
-        settings_menu.addAction('&Update Pipeline (dev)',
-                                partial(self.update_pipeline, 'dev'))
-        settings_menu.addAction('&Update MNE-Python', self.update_mne)
-        settings_menu.addAction('&Restart', self.restart)
+        # ToDo: Needs to be thoroughly tested on all OS
+        # settings_menu.addAction('&Update Pipeline (stable)',
+        #                         partial(self.update_pipeline, 'stable'))
+        # settings_menu.addAction('&Update Pipeline (dev)',
+        #                         partial(self.update_pipeline, 'dev'))
+        # settings_menu.addAction('&Update MNE-Python', self.update_mne)
+        settings_menu.addAction("&Restart", self.restart)
 
         # About
-        about_menu = self.menuBar().addMenu('About')
+        about_menu = self.menuBar().addMenu("About")
         # about_menu.addAction('Update Pipeline', self.update_pipeline)
         # about_menu.addAction('Update MNE-Python', self.update_mne)
-        about_menu.addAction('Quick-Guide', partial(QuickGuide, self))
-        about_menu.addAction('MNE System-Info', self.show_sys_info)
-        about_menu.addAction('About', partial(AboutDialog, self))
-        about_menu.addAction('About QT', QApplication.instance().aboutQt)
+        about_menu.addAction("Quick-Guide", partial(QuickGuide, self))
+        about_menu.addAction("MNE System-Info", self.show_sys_info)
+        about_menu.addAction("About", partial(AboutDialog, self))
+        about_menu.addAction("About QT", QApplication.instance().aboutQt)
 
     def init_toolbar(self):
-        self.toolbar = self.addToolBar('Tools')
+        self.toolbar = self.addToolBar("Tools")
         # Add Project-UI
-        proj_box_label = QLabel('<b>Project: </b>')
+        proj_box_label = QLabel("<b>Project: </b>")
         self.toolbar.addWidget(proj_box_label)
 
         self.project_box = QComboBox()
         self.project_box.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.project_box.activated.connect(self.project_changed)
         self.update_project_box()
         self.toolbar.addWidget(self.project_box)
 
-        add_action = QAction(parent=self,
-                             icon=get_std_icon('SP_FileDialogNewFolder'))
+        add_action = QAction(parent=self, icon=get_std_icon("SP_FileDialogNewFolder"))
         add_action.triggered.connect(self.add_project)
         self.toolbar.addAction(add_action)
 
-        remove_action = QAction(parent=self,
-                                icon=get_std_icon('SP_DialogDiscardButton'))
+        remove_action = QAction(
+            parent=self, icon=get_std_icon("SP_DialogDiscardButton")
+        )
         remove_action.triggered.connect(self.remove_project)
         self.toolbar.addAction(remove_action)
         self.toolbar.addSeparator()
 
         self.toolbar.addWidget(
-            IntGui(data=QS(), name='n_jobs', min_val=-1,
-                   special_value_text='Auto',
-                   description='Set to the amount of (virtual) cores '
-                               'of your machine you want '
-                               'to use for multiprocessing.',
-                   default=-1, groupbox_layout=False))
+            IntGui(
+                data=QS(),
+                name="n_jobs",
+                min_val=-1,
+                special_value_text="Auto",
+                description="Set to the amount of (virtual) cores "
+                "of your machine you want "
+                "to use for multiprocessing.",
+                default=-1,
+                groupbox_layout=False,
+            )
+        )
         # self.toolbar.addWidget(
         #     IntGui(data=QS(), name='n_parallel', min_val=1,
         #            description='Set to the amount of threads you want '
         #                        'to run simultaneously in the pipeline',
         #            default=1, groupbox_layout=False))
         # self.toolbar.addWidget(
         #     BoolGui(data=QS(), name='use_qthread', alias='Use QThreads',
         #             description='Check to use QThreads for running '
         #                         'the pipeline.\n'
         #                         'This is faster than the default'
         #                         ' with separate processes, '
         #                         'but has a few limitations',
         #             default=0, return_integer=True))
-        self.toolbar.addWidget(BoolGui(data=self.ct.settings, name='overwrite',
-                                       alias='Overwrite',
-                                       description='Check to overwrite files'
-                                                   ' even if their parameters '
-                                                   'where unchanged.',
-                                       groupbox_layout=False))
-        self.toolbar.addWidget(BoolGui(data=self.ct.settings,
-                                       name='show_plots', alias='Show Plots',
-                                       description='Do you want to show'
-                                                   ' plots?\n'
-                                                   '(or just save them without'
-                                                   ' showing, then just check'
-                                                   ' "Save Plots").',
-
-                                       groupbox_layout=False))
-        self.toolbar.addWidget(BoolGui(data=self.ct.settings,
-                                       name='save_plots', alias='Save Plots',
-                                       description='Do you want to save the '
-                                                   'plots made to a file?',
-                                       groupbox_layout=False))
-        self.toolbar.addWidget(BoolGui(data=self.ct.settings, name='shutdown',
-                                       alias='Shutdown',
-                                       description='Do you want to shut your '
-                                                   'system down after '
-                                                   ' execution of all '
-                                                   'subjects?',
-                                       groupbox_layout=False))
-        close_all_bt = QPushButton('Close All Plots')
+        # self.toolbar.addWidget(BoolGui(data=self.ct.settings, name='overwrite',
+        #                                alias='Overwrite',
+        #                                description='Check to overwrite files'
+        #                                            ' even if their parameters '
+        #                                            'where unchanged.',
+        #                                groupbox_layout=False))
+        self.toolbar.addWidget(
+            BoolGui(
+                data=self.ct.settings,
+                name="show_plots",
+                alias="Show Plots",
+                description="Do you want to show"
+                " plots?\n"
+                "(or just save them without"
+                " showing, then just check"
+                ' "Save Plots").',
+                groupbox_layout=False,
+            )
+        )
+        self.toolbar.addWidget(
+            BoolGui(
+                data=self.ct.settings,
+                name="save_plots",
+                alias="Save Plots",
+                description="Do you want to save the " "plots made to a file?",
+                groupbox_layout=False,
+            )
+        )
+        self.toolbar.addWidget(
+            BoolGui(
+                data=self.ct.settings,
+                name="shutdown",
+                alias="Shutdown",
+                description="Do you want to shut your "
+                "system down after "
+                " execution of all "
+                "subjects?",
+                groupbox_layout=False,
+            )
+        )
+        close_all_bt = QPushButton("Close All Plots")
         close_all_bt.pressed.connect(close_all)
         self.toolbar.addWidget(close_all_bt)
 
     def init_main_widget(self):
         self.setCentralWidget(QWidget(self))
         self.general_layout = QGridLayout()
         self.centralWidget().setLayout(self.general_layout)
@@ -392,85 +467,83 @@
         self.show()
         self.general_layout.invalidate()
 
         # Add Function-Buttons
         self.add_func_bts()
 
         # Add Main-Buttons
-        clear_bt = QPushButton('Clear')
-        start_bt = QPushButton('Start')
-        stop_bt = QPushButton('Quit')
-
-        clear_bt.setFont(QFont(QS().value('app_font'), 18))
-        start_bt.setFont(QFont(QS().value('app_font'), 18))
-        stop_bt.setFont(QFont(QS().value('app_font'), 18))
+        clear_bt = QPushButton("Clear")
+        start_bt = QPushButton("Start")
+        stop_bt = QPushButton("Quit")
+
+        clear_bt.setFont(QFont(QS().value("app_font"), 18))
+        start_bt.setFont(QFont(QS().value("app_font"), 18))
+        stop_bt.setFont(QFont(QS().value("app_font"), 18))
 
         clear_bt.clicked.connect(self.clear)
         start_bt.clicked.connect(self.start)
         stop_bt.clicked.connect(self.close)
 
         self.general_layout.addWidget(clear_bt, 1, 0)
         self.general_layout.addWidget(start_bt, 1, 1)
         self.general_layout.addWidget(stop_bt, 1, 2)
 
     # Todo: Make Buttons more appealing, mark when check
     #   make button-dependencies
     def add_func_bts(self):
         # Drop custom-modules, which aren't selected
         cleaned_pd_funcs = self.ct.pd_funcs.loc[
-            self.ct.pd_funcs['module'].isin(
-                self.ct.get_setting('selected_modules'))].copy()
+            self.ct.pd_funcs["module"].isin(self.ct.get_setting("selected_modules"))
+        ].copy()
         # Horizontal Border for Function-Groups
         max_h_size = self.tab_func_widget.geometry().width()
 
         # Assert, that cleaned_pd_funcs is not empty
         # (possible, when deselecting all modules)
         if len(cleaned_pd_funcs) != 0:
-            tabs_grouped = cleaned_pd_funcs.groupby('tab')
+            tabs_grouped = cleaned_pd_funcs.groupby("tab")
             # Add tabs
             for tab_name, group in tabs_grouped:
-                group_grouped = group.groupby('group', sort=False)
+                group_grouped = group.groupby("group", sort=False)
                 tab = QScrollArea()
                 child_w = QWidget()
                 tab_v_layout = QVBoxLayout()
                 tab_h_layout = QHBoxLayout()
                 h_size = 0
                 # Add groupbox for each group
                 for function_group, _ in group_grouped:
                     group_box = QGroupBox(function_group, self)
-                    group_box.setSizePolicy(QSizePolicy.Maximum,
-                                            QSizePolicy.Maximum)
-                    setattr(self, f'{function_group}_gbox', group_box)
+                    group_box.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
+                    setattr(self, f"{function_group}_gbox", group_box)
                     group_box.setCheckable(True)
                     group_box.toggled.connect(self.func_group_toggled)
                     group_box_layout = QVBoxLayout()
                     # Add button for each function
                     for function in group_grouped.groups[function_group]:
-                        if pd.notna(cleaned_pd_funcs.loc[function, 'alias']):
-                            alias_name = cleaned_pd_funcs.loc[
-                                function, 'alias']
+                        if pd.notna(cleaned_pd_funcs.loc[function, "alias"]):
+                            alias_name = cleaned_pd_funcs.loc[function, "alias"]
                         else:
                             alias_name = function
                         pb = QPushButton(alias_name)
                         pb.setCheckable(True)
                         self.bt_dict[function] = pb
                         if function in self.pr.sel_functions:
                             pb.setChecked(True)
-                        pb.clicked.connect(
-                            partial(self.func_selected, function))
+                        pb.clicked.connect(partial(self.func_selected, function))
                         group_box_layout.addWidget(pb)
 
                     group_box.setLayout(group_box_layout)
                     h_size += group_box.sizeHint().width()
                     if h_size > max_h_size:
                         tab_v_layout.addLayout(tab_h_layout)
                         h_size = group_box.sizeHint().width()
                         tab_h_layout = QHBoxLayout()
                     tab_h_layout.addWidget(
-                        group_box, alignment=Qt.AlignLeft | Qt.AlignTop)
+                        group_box, alignment=Qt.AlignLeft | Qt.AlignTop
+                    )
 
                 if tab_h_layout.count() > 0:
                     tab_v_layout.addLayout(tab_h_layout)
 
                 child_w.setLayout(tab_v_layout)
                 tab.setWidget(child_w)
                 self.tab_func_widget.addTab(tab, tab_name)
@@ -493,73 +566,90 @@
         if checked:
             if function not in self.pr.sel_functions:
                 self.pr.sel_functions.append(function)
         elif function in self.pr.sel_functions:
             self.pr.sel_functions.remove(function)
 
     def func_selected(self, function):
-        self._update_selected_functions(function,
-                                        self.bt_dict[function].isChecked())
+        self._update_selected_functions(function, self.bt_dict[function].isChecked())
 
     def func_group_toggled(self):
         for function in self.bt_dict:
-            self._update_selected_functions(function,
-                                            self.bt_dict[
-                                                function].isChecked() and
-                                            self.bt_dict[function].isEnabled())
+            self._update_selected_functions(
+                function,
+                self.bt_dict[function].isChecked()
+                and self.bt_dict[function].isEnabled(),
+            )
 
     def update_selected_funcs(self):
         for function in self.bt_dict:
             self.bt_dict[function].setChecked(False)
             if function in self.pr.sel_functions:
                 self.bt_dict[function].setChecked(True)
 
     def init_docks(self):
         if self.ct.edu_program:
-            dock_kwargs = self.ct.edu_program['dock_kwargs']
+            dock_kwargs = self.ct.edu_program["dock_kwargs"]
         else:
             dock_kwargs = dict()
         self.file_dock = FileDock(self, **dock_kwargs)
         self.addDockWidget(Qt.LeftDockWidgetArea, self.file_dock)
         self.view_menu.addAction(self.file_dock.toggleViewAction())
 
         self.parameters_dock = ParametersDock(self)
         self.addDockWidget(Qt.RightDockWidgetArea, self.parameters_dock)
         self.view_menu.addAction(self.parameters_dock.toggleViewAction())
 
     def add_sample_dataset(self):
-        if '_sample_' in self.pr.all_meeg:
-            QMessageBox.information(self, '_sample_ exists!',
-                                    'The sample-dataset is already '
-                                    'imported as _sample_!')
-        else:
-            WorkerDialog(self, partial(self.pr.add_meeg, '_sample_'),
-                         show_console=True,
-                         title='Loading Sample...', blocking=True)
+        if "_sample_" in self.pr.all_meeg:
+            QMessageBox.information(
+                self,
+                "_sample_ exists!",
+                "The sample-dataset is already " "imported as _sample_!",
+            )
+        else:
+            WorkerDialog(
+                self,
+                partial(self.pr.add_meeg, "_sample_"),
+                show_console=True,
+                title="Loading Sample...",
+                blocking=True,
+            )
             self.file_dock.update_dock()
 
     def add_test_dataset(self):
-        if '_test_' in self.pr.all_meeg:
-            QMessageBox.information(self, '_test_ exists!',
-                                    'The test-dataset is already '
-                                    'imported as _test_!')
-        else:
-            WorkerDialog(self, partial(self.pr.add_meeg, '_test_'),
-                         show_console=True,
-                         title='Loading Sample...', blocking=True)
+        if "_test_" in self.pr.all_meeg:
+            QMessageBox.information(
+                self,
+                "_test_ exists!",
+                "The test-dataset is already " "imported as _test_!",
+            )
+        else:
+            WorkerDialog(
+                self,
+                partial(self.pr.add_meeg, "_test_"),
+                show_console=True,
+                title="Loading Sample...",
+                blocking=True,
+            )
             self.file_dock.update_dock()
 
     def add_fsaverage(self):
-        if 'fsaverage' in self.pr.all_fsmri:
-            QMessageBox.information(self, 'fsaverage exists!',
-                                    'fsaverage is already imported!')
-        else:
-            WorkerDialog(self, partial(self.pr.add_fsmri, 'fsaverage'),
-                         show_console=True, title='Loading fsaverage...',
-                         blocking=True)
+        if "fsaverage" in self.pr.all_fsmri:
+            QMessageBox.information(
+                self, "fsaverage exists!", "fsaverage is already imported!"
+            )
+        else:
+            WorkerDialog(
+                self,
+                partial(self.pr.add_fsmri, "fsaverage"),
+                show_console=True,
+                title="Loading fsaverage...",
+                blocking=True,
+            )
             self.file_dock.update_dock()
 
     def full_screen(self):
         if self.isFullScreen():
             self.showNormal()
         else:
             self.showFullScreen()
@@ -567,61 +657,85 @@
     def clear(self):
         for x in self.bt_dict:
             self.bt_dict[x].setChecked(False)
         self.pr.sel_functions.clear()
 
     def start(self):
         if self.pipeline_running:
-            QMessageBox.warning(self, 'Already running!',
-                                'The Pipeline is already running!')
-        else:
-            WorkerDialog(self, self.ct.save, show_buttons=False,
-                         show_console=False,
-                         blocking=True)
+            QMessageBox.warning(
+                self, "Already running!", "The Pipeline is already running!"
+            )
+        else:
+            WorkerDialog(
+                self,
+                self.ct.save,
+                show_buttons=False,
+                show_console=False,
+                blocking=True,
+            )
             self.run_dialog = RunDialog(self)
 
     def restart(self):
         self.restarting = True
         self.close()
         restart_program()
 
     def update_pipeline(self, version):
-        if version == 'stable':
-            command = 'pip install --upgrade mne_pipeline_hd'
+        if version == "stable":
+            command = "pip install --upgrade mne_pipeline_hd"
         else:
-            command = 'pip install ' \
-                      'https://github.com/marsipu/mne-pipeline-hd/zipball/main'
+            command = (
+                "pip install " "https://github.com/marsipu/mne-pipeline-hd/zipball/main"
+            )
         if iswin and not _run_from_script():
             QMessageBox.information(
-                self, 'Manual install required!',
-                f'To update you need to exit the program '
-                f'and type "{command}" into the terminal!')
-        else:
-            QProcessDialog(self, command, show_buttons=True, show_console=True,
-                           close_directly=True, title='Updating Pipeline...',
-                           blocking=True)
+                self,
+                "Manual install required!",
+                f"To update you need to exit the program "
+                f'and type "{command}" into the terminal!',
+            )
+        else:
+            QProcessDialog(
+                self,
+                command,
+                show_buttons=True,
+                show_console=True,
+                close_directly=True,
+                title="Updating Pipeline...",
+                blocking=True,
+            )
 
             answer = QMessageBox.question(
-                self, 'Do you want to restart?',
-                'Please restart the Pipeline-Program '
-                'to apply the changes from the Update!')
+                self,
+                "Do you want to restart?",
+                "Please restart the Pipeline-Program "
+                "to apply the changes from the Update!",
+            )
 
             if answer == QMessageBox.Yes:
                 self.restart()
 
     def update_mne(self):
-        command = 'pip install --upgrade mne'
-        QProcessDialog(self, command, show_buttons=True, show_console=True,
-                       close_directly=True, title='Updating MNE-Python...',
-                       blocking=True)
+        command = "pip install --upgrade mne"
+        QProcessDialog(
+            self,
+            command,
+            show_buttons=True,
+            show_console=True,
+            close_directly=True,
+            title="Updating MNE-Python...",
+            blocking=True,
+        )
 
         answer = QMessageBox.question(
-            self, 'Do you want to restart?',
-            'Please restart the Pipeline-Program '
-            'to apply the changes from the Update!')
+            self,
+            "Do you want to restart?",
+            "Please restart the Pipeline-Program "
+            "to apply the changes from the Update!",
+        )
 
         if answer == QMessageBox.Yes:
             self.restart()
 
     def show_sys_info(self):
         sys_info_msg = SysInfoMsg(self)
         sys.stdout.signal.text_written.connect(sys_info_msg.add_text)
@@ -629,30 +743,32 @@
 
     def resizeEvent(self, event):
         if not self.first_init:
             self.update_func_bts()
         event.accept()
 
     def closeEvent(self, event):
-        welcome_window = _object_refs['welcome_window']
+        welcome_window = _object_refs["welcome_window"]
         if self.restarting or welcome_window is None:
             answer = QMessageBox.No
         else:
             answer = QMessageBox.question(
-                self, 'Closing MNE-Pipeline',
-                'Do you want to return to the Welcome-Window?',
+                self,
+                "Closing MNE-Pipeline",
+                "Do you want to return to the Welcome-Window?",
                 buttons=QMessageBox.Yes | QMessageBox.No | QMessageBox.Cancel,
-                defaultButton=QMessageBox.Yes)
+                defaultButton=QMessageBox.Yes,
+            )
         if answer not in [QMessageBox.Yes, QMessageBox.No]:
             event.ignore()
         else:
             if self.edu_tour:
                 self.edu_tour.close()
             event.accept()
-            _object_refs['main_window'] = None
+            _object_refs["main_window"] = None
 
             if welcome_window is not None:
                 if answer == QMessageBox.Yes:
                     welcome_window.update_widgets()
                     welcome_window.show()
 
                 elif answer == QMessageBox.No:
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/models.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from ast import literal_eval
 from datetime import datetime
 
 import pandas as pd
-from PyQt5.QtCore import (QAbstractItemModel, QAbstractListModel,
-                          QAbstractTableModel, QModelIndex, Qt)
+from PyQt5.QtCore import (
+    QAbstractItemModel,
+    QAbstractListModel,
+    QAbstractTableModel,
+    QModelIndex,
+    Qt,
+)
 from PyQt5.QtGui import QBrush, QFont
 
 from mne_pipeline_hd.gui.gui_utils import get_std_icon
 
 
 class BaseListModel(QAbstractListModel):
-    """ A basic List-Model
+    """A basic List-Model
 
     Parameters
     ----------
     data : list()
         input existing list here, otherwise defaults to empty list
     show_index : bool
         Set True if you want to display the list-index in front of each value
@@ -42,48 +45,47 @@
 
     def getData(self, index):
         return self._data[index.row()]
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             if self.show_index:
-                return f'{index.row()}: {self.getData(index)}'
+                return f"{index.row()}: {self.getData(index)}"
             else:
                 return str(self.getData(index))
         elif role == Qt.EditRole:
             return str(self.getData(index))
 
-    def rowCount(self, index=QModelIndex()):
+    def rowCount(self, *args, **kwargs):
         return len(self._data)
 
-    def insertRows(self, row, count, index=QModelIndex()):
-        self.beginInsertRows(index, row, row + count - 1)
+    def insertRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginInsertRows(parent, row, row + count - 1)
         n = 0
         for pos in range(row, row + count):
-            item_name = f'__new{n}__'
+            item_name = f"__new{n}__"
             while item_name in self._data:
                 n += 1
-                item_name = f'__new{n}__'
+                item_name = f"__new{n}__"
             self._data.insert(pos, item_name)
         self.endInsertRows()
         return True
 
-    def removeRows(self, row, count, index=QModelIndex()):
-        self.beginRemoveRows(index, row, row + count - 1)
+    def removeRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginRemoveRows(parent, row, row + count - 1)
         for item in [self._data[i] for i in range(row, row + count)]:
             self._data.remove(item)
         self.endRemoveRows()
         return True
 
     def flags(self, index):
         default_flags = QAbstractListModel.flags(self, index)
         if self.drag_drop:
             if index.isValid():
-                return default_flags | Qt.ItemIsDragEnabled \
-                       | Qt.ItemIsDropEnabled
+                return default_flags | Qt.ItemIsDragEnabled | Qt.ItemIsDropEnabled
             else:
                 return default_flags | Qt.ItemIsDropEnabled
         else:
             return default_flags
 
     def supportedDragActions(self):
         if self.drag_drop:
@@ -102,15 +104,15 @@
     drag_drop: bool
         Set True to enable Drag&Drop.
     """
 
     def __init__(self, data, show_index=False, drag_drop=False, **kwargs):
         super().__init__(data, show_index, drag_drop, **kwargs)
 
-    def flags(self, index=QModelIndex()):
+    def flags(self, index):
         default_flags = BaseListModel.flags(self, index)
         if index.isValid():
             return default_flags | Qt.ItemIsEditable
         else:
             return default_flags
 
     def setData(self, index, value, role=None):
@@ -137,36 +139,43 @@
     show_index: bool
         Set True if you want to display the list-index in front of each value
     drag_drop: bool
         Set True to enable Drag&Drop.
 
     """
 
-    def __init__(self, data, checked, one_check=False, show_index=False,
-                 drag_drop=False, **kwargs):
+    def __init__(
+        self,
+        data,
+        checked,
+        one_check=False,
+        show_index=False,
+        drag_drop=False,
+        **kwargs,
+    ):
         super().__init__(data, show_index, drag_drop, **kwargs)
         self.one_check = one_check
 
         if data is None:
             self._data = list()
         else:
             self._data = data
 
         if checked is None:
             self._checked = list()
         else:
             self._checked = checked
 
-    def getChecked(self, index=QModelIndex()):
+    def getChecked(self, index):
         return self.checked[index.row()]
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             if self.show_index:
-                return f'{index.row()}: {self.getData(index)}'
+                return f"{index.row()}: {self.getData(index)}"
             else:
                 return str(self.getData(index))
 
         if role == Qt.CheckStateRole:
             if self.getData(index) in self._checked:
                 return Qt.Checked
             else:
@@ -181,15 +190,15 @@
             else:
                 if self.getData(index) in self._checked:
                     self._checked.remove(self.getData(index))
             self.dataChanged.emit(index, index)
             return True
         return False
 
-    def flags(self, index=QModelIndex()):
+    def flags(self, index):
         return QAbstractItemModel.flags(self, index) | Qt.ItemIsUserCheckable
 
 
 class CheckDictModel(BaseListModel):
     """
     A Model for a list, which marks items which are present in a dictionary
 
@@ -212,26 +221,34 @@
 
     Notes
     -----
     Names for QT standard-icons:
     https://doc.qt.io/qt-5/qstyle.html#StandardPixmap-enum
     """
 
-    def __init__(self, data, check_dict, show_index=False, drag_drop=False,
-                 yes_bt=None, no_bt=None, **kwargs):
+    def __init__(
+        self,
+        data,
+        check_dict,
+        show_index=False,
+        drag_drop=False,
+        yes_bt=None,
+        no_bt=None,
+        **kwargs,
+    ):
         super().__init__(data, show_index, drag_drop, **kwargs)
         self._check_dict = check_dict
 
-        self.yes_bt = yes_bt or 'SP_DialogApplyButton'
-        self.no_bt = no_bt or 'SP_DialogCancelButton'
+        self.yes_bt = yes_bt or "SP_DialogApplyButton"
+        self.no_bt = no_bt or "SP_DialogCancelButton"
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             if self.show_index:
-                return f'{index.row()}: {self.getData(index)}'
+                return f"{index.row()}: {self.getData(index)}"
             else:
                 return str(self.getData(index))
         elif role == Qt.EditRole:
             return str(self.getData(index))
 
         elif role == Qt.DecorationRole:
             if self.getData(index) in self._check_dict:
@@ -262,18 +279,24 @@
 
     Notes
     -----
     Names for QT standard-icons:
     https://doc.qt.io/qt-5/qstyle.html#StandardPixmap-enum
     """
 
-    def __init__(self, data, check_dict, show_index=False, drag_drop=False,
-                 yes_bt=None, no_bt=None):
-        super().__init__(data, check_dict, show_index, drag_drop, yes_bt,
-                         no_bt)
+    def __init__(
+        self,
+        data,
+        check_dict,
+        show_index=False,
+        drag_drop=False,
+        yes_bt=None,
+        no_bt=None,
+    ):
+        super().__init__(data, check_dict, show_index, drag_drop, yes_bt, no_bt)
         # EditListModel doesn't have to be initialized
         # because in __init__ of EditListModel
         # only BaseListModel is initialized which is already done
         # in __init__ of CheckDictModel
 
 
 class BaseDictModel(QAbstractTableModel):
@@ -294,43 +317,43 @@
     def __init__(self, data=None, **kwargs):
         super().__init__(**kwargs)
         if data is None:
             self._data = dict()
         else:
             self._data = data
 
-    def getData(self, index=QModelIndex()):
+    def getData(self, index):
         try:
             if index.column() == 0:
                 return list(self._data.keys())[index.row()]
             elif index.column() == 1:
                 return list(self._data.values())[index.row()]
         # Happens, when a duplicate key is entered
         except IndexError:
             self.layoutChanged.emit()
-            return ''
+            return ""
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole or role == Qt.EditRole:
             return str(self.getData(index))
 
     def headerData(self, idx, orientation, role=None):
         if role == Qt.DisplayRole:
             if orientation == Qt.Horizontal:
                 if idx == 0:
-                    return 'Key'
+                    return "Key"
                 elif idx == 1:
-                    return 'Value'
+                    return "Value"
             elif orientation == Qt.Vertical:
                 return str(idx)
 
-    def rowCount(self, index=QModelIndex()):
+    def rowCount(self, parent=None, *args, **kwargs):
         return len(self._data)
 
-    def columnCount(self, index=QModelIndex()):
+    def columnCount(self, parent=None, *args, **kwargs):
         return 2
 
 
 class EditDictModel(BaseDictModel):
     """An editable model for Dictionaries
 
     Parameters
@@ -355,50 +378,49 @@
     def setData(self, index, value, role=None):
         if role == Qt.EditRole:
             try:
                 value = literal_eval(value)
             except (SyntaxError, ValueError):
                 pass
             if index.column() == 0:
-                self._data[value] = self._data.pop(
-                    list(self._data.keys())[index.row()])
+                self._data[value] = self._data.pop(list(self._data.keys())[index.row()])
             elif index.column() == 1:
                 self._data[list(self._data.keys())[index.row()]] = value
             else:
                 return False
 
             self.dataChanged.emit(index, index, [role])
             return True
 
         return False
 
-    def flags(self, index=QModelIndex()):
+    def flags(self, index):
         if not self.only_edit:
             return QAbstractItemModel.flags(self, index) | Qt.ItemIsEditable
-        elif index.column() == 0 and self.only_edit == 'keys':
+        elif index.column() == 0 and self.only_edit == "keys":
             return QAbstractItemModel.flags(self, index) | Qt.ItemIsEditable
-        elif index.column() == 1 and self.only_edit == 'values':
+        elif index.column() == 1 and self.only_edit == "values":
             return QAbstractItemModel.flags(self, index) | Qt.ItemIsEditable
         else:
             return QAbstractItemModel.flags(self, index)
 
-    def insertRows(self, row, count, index=QModelIndex()):
-        self.beginInsertRows(index, row, row + count - 1)
+    def insertRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginInsertRows(parent, row, row + count - 1)
         for n in range(count):
-            key_name = f'__new{n}__'
+            key_name = f"__new{n}__"
             while key_name in self._data.keys():
                 n += 1
-                key_name = f'__new{n}__'
-            self._data[key_name] = ''
+                key_name = f"__new{n}__"
+            self._data[key_name] = ""
         self.endInsertRows()
 
         return True
 
-    def removeRows(self, row, count, index=QModelIndex()):
-        self.beginRemoveRows(index, row, row + count - 1)
+    def removeRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginRemoveRows(parent, row, row + count - 1)
         for n in range(count):
             self._data.pop(list(self._data.keys())[row + n])
         self.endRemoveRows()
 
         return True
 
 
@@ -415,37 +437,37 @@
     def __init__(self, data=None, **kwargs):
         super().__init__(**kwargs)
         if data is None:
             self._data = pd.DataFrame([])
         else:
             self._data = data
 
-    def getData(self, index=QModelIndex()):
+    def getData(self, index):
         return self._data.iloc[index.row(), index.column()]
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole or role == Qt.EditRole:
             return str(self.getData(index))
 
     def headerData(self, idx, orientation, role=None):
         if role == Qt.DisplayRole:
             if orientation == Qt.Horizontal:
                 return str(self._data.columns[idx])
             elif orientation == Qt.Vertical:
                 return str(self._data.index[idx])
 
-    def rowCount(self, index=QModelIndex()):
+    def rowCount(self, parent=None, *args, **kwargs):
         return len(self._data.index)
 
-    def columnCount(self, index=QModelIndex()):
+    def columnCount(self, parent=None, *args, **kwargs):
         return len(self._data.columns)
 
 
 class EditPandasModel(BasePandasModel):
-    """ Editable TableModel for Pandas DataFrames
+    """Editable TableModel for Pandas DataFrames
     Parameters
     ----------
     data : pandas.DataFrame | None
         pandas DataFrame with contents to be displayed,
          defaults to empty DataFrame
 
     Notes
@@ -491,75 +513,81 @@
                 new_columns[index] = value
                 self._data.columns = new_columns
                 self.headerDataChanged.emit(Qt.Horizontal, index, index)
                 return True
 
         return False
 
-    def flags(self, index=QModelIndex()):
+    def flags(self, index):
         return QAbstractItemModel.flags(self, index) | Qt.ItemIsEditable
 
-    def insertRows(self, row, count, index=QModelIndex()):
-        self.beginInsertRows(index, row, row + count - 1)
-        add_data = pd.DataFrame(columns=self._data.columns,
-                                index=[r for r in range(count)])
+    def insertRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginInsertRows(parent, row, row + count - 1)
+        add_data = pd.DataFrame(
+            columns=self._data.columns, index=[r for r in range(count)]
+        )
         if row == 0:
             self._data = pd.concat([add_data, self._data])
         elif row == len(self._data.index):
             self._data = self._data.append(add_data)
         else:
-            self._data = pd.concat([self._data.iloc[:row], add_data,
-                                    self._data.iloc[row:]])
+            self._data = pd.concat(
+                [self._data.iloc[:row], add_data, self._data.iloc[row:]]
+            )
         self.endInsertRows()
 
         return True
 
-    def insertColumns(self, column, count, index=QModelIndex()):
-        self.beginInsertColumns(index, column, column + count - 1)
-        add_data = pd.DataFrame(index=self._data.index,
-                                columns=[c for c in range(count)])
+    def insertColumns(self, column, count, parent=None, *args, **kwargs):
+        self.beginInsertColumns(parent, column, column + count - 1)
+        add_data = pd.DataFrame(
+            index=self._data.index, columns=[c for c in range(count)]
+        )
         if column == 0:
             self._data = pd.concat([add_data, self._data], axis=1)
         elif column == len(self._data.columns):
             self._data = pd.concat([self._data, add_data], axis=1)
         else:
             self._data = pd.concat(
-                [self._data.iloc[:, :column], add_data,
-                 self._data.iloc[:, column:]], axis=1)
+                [self._data.iloc[:, :column], add_data, self._data.iloc[:, column:]],
+                axis=1,
+            )
         self.endInsertColumns()
 
         return True
 
-    def removeRows(self, row, count, index=QModelIndex()):
-        self.beginRemoveRows(index, row, row + count - 1)
+    def removeRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginRemoveRows(parent, row, row + count - 1)
         # Can't use DataFrame.drop() here,
         # because there could be rows with similar index-labels
         if row == 0:
-            self._data = self._data.iloc[row + count:]
+            self._data = self._data.iloc[row + count :]
         elif row + count >= len(self._data.index):
             self._data = self._data.iloc[:row]
         else:
-            self._data = pd.concat([self._data.iloc[:row],
-                                    self._data.iloc[row + count:]])
+            self._data = pd.concat(
+                [self._data.iloc[:row], self._data.iloc[row + count :]]
+            )
         self.endRemoveRows()
 
         return True
 
-    def removeColumns(self, column, count, index=QModelIndex()):
-        self.beginRemoveColumns(index, column, column + count - 1)
+    def removeColumns(self, column, count, parent=None, *args, **kwargs):
+        self.beginRemoveColumns(parent, column, column + count - 1)
         # Can't use DataFrame.drop() here,
         # because there could be columns with similar column-labels
         if column == 0:
-            self._data = self._data.iloc[:, column + count:]
+            self._data = self._data.iloc[:, column + count :]
         elif column + count >= len(self._data.columns):
             self._data = self._data.iloc[:, :column]
         else:
             self._data = pd.concat(
-                [self._data.iloc[:, :column],
-                 self._data.iloc[:, column + count:]], axis=1)
+                [self._data.iloc[:, :column], self._data.iloc[:, column + count :]],
+                axis=1,
+            )
         self.endRemoveColumns()
 
         return True
 
 
 class TreeItem:
     """TreeItem as in
@@ -594,27 +622,28 @@
             self._data[column] = value
             return True
         return False
 
     def insertChild(self, position):
         if 0 <= position < len(self._children):
             self._children.insert(
-                position, TreeItem([f'__new__{len(self._children)}'], self))
+                position, TreeItem([f"__new__{len(self._children)}"], self)
+            )
             return True
         return False
 
     def removeChild(self, position):
         if 0 <= position < len(self._children):
             self._children.remove(self._children[position])
             return True
         return False
 
     def insertColumn(self, position):
         if 0 <= position < len(self._data):
-            self._data.insert(position, f'__new__{len(self._data)}')
+            self._data.insert(position, f"__new__{len(self._data)}")
             for child in self._children:
                 child.insertColumns(position)
             return True
         return False
 
     def removeColumn(self, position):
         if 0 <= position < len(self._data):
@@ -623,154 +652,154 @@
                 child.removeColumns(position)
             return True
         return False
 
 
 class TreeModel(QAbstractItemModel):
     """Tree-Model as in
-     https://doc.qt.io/qt-5/qtwidgets-itemviews-simpletreemodel-example.html"""
+    https://doc.qt.io/qt-5/qtwidgets-itemviews-simpletreemodel-example.html"""
 
     def __init__(self, data, n_columns=1, headers=None, parent=None):
         super().__init__(parent)
         self._data = data
         self._n_columns = n_columns
         if headers is None:
-            headers = ['' for i in range(n_columns)]
+            headers = ["" for _ in range(n_columns)]
         elif len(headers) < n_columns:
-            headers += ['' for i in range(n_columns - headers)]
+            headers += ["" for _ in range(n_columns - headers)]
         elif len(headers) > n_columns:
             headers = headers[:n_columns]
         self._headers = headers
         self._parent = parent
 
         self.root_item = self.dict_to_items(self._data)
 
     def dict_to_items(self, datadict, parent=None):
         if parent is None:
             parent = TreeItem(self._headers)
 
         for key, value in datadict.items():
-            data = [key] + ['' for i in range(self._n_columns - 1)]
+            data = [key] + ["" for _ in range(self._n_columns - 1)]
             tree_item = TreeItem(data, parent)
             if isinstance(value, dict):
                 child_item = self.dict_to_items(value, tree_item)
                 tree_item._children.append(child_item)
             parent._children.append(tree_item)
 
         return parent
 
     # noinspection PyMethodMayBeStatic
     def getData(self, index):
         if index.isValid():
             item = index.internalPointer()
             return item.data(index.column())
 
-    def data(self, index: QModelIndex, role: int = ...) -> object:
+    def data(self, index, role=None):
         if role == Qt.DisplayRole:
             return self.getData(index)
 
-    def index(self, row: int, column: int, parent: QModelIndex = ...) \
-            -> QModelIndex:
+    def index(self, row, column, parent=None, *args, **kwargs):
         if self.hasIndex(row, column, parent):
             if parent.isValid():
-                parentItem = parent.internalPointer()
+                parent_item = parent.internalPointer()
             else:
-                parentItem = self.root_item
+                parent_item = self.root_item
 
-            childItem = parentItem.child(row)
-            if childItem is not None:
-                return self.createIndex(row, column, childItem)
+            child_item = parent_item.child(row)
+            if child_item is not None:
+                return self.createIndex(row, column, child_item)
         return QModelIndex()
 
-    def parent(self, child: QModelIndex) -> QModelIndex:
+    def parent(self, child=None):
         if child.isValid():
-            childItem = child.internalPointer()
-            parentItem = childItem._parent
+            child_item = child.internalPointer()
+            parent_item = child_item._parent
 
-            if parentItem != self.root_item:
-                return self.createIndex(parentItem.row(), 0, parentItem)
+            if parent_item != self.root_item:
+                return self.createIndex(parent_item.row(), 0, parent_item)
         return QModelIndex()
 
-    def rowCount(self, parent: QModelIndex = ...) -> int:
+    def rowCount(self, parent=None, *args, **kwargs):
         if parent.column() > 0:
             return 0
 
         if parent.isValid():
-            parentItem = parent.internalPointer()
+            parent_item = parent.internalPointer()
         else:
-            parentItem = self.root_item
+            parent_item = self.root_item
 
-        return parentItem.childCount()
+        return parent_item.childCount()
 
-    def columnCount(self, parent: QModelIndex = ...) -> int:
+    def columnCount(self, parent=None, *args, **kwargs):
         if parent.isValid():
             return parent.internalPointer().columnCount()
         return self.root_item.columnCount()
 
-    def flags(self, index: QModelIndex) -> Qt.ItemFlags:
+    def flags(self, index):
         if index.isValid():
             return QAbstractItemModel.flags(self, index)
         return Qt.NoItemFlags
 
-    def headerData(self, section: int,
-                   orientation: Qt.Orientation, role: int = ...) -> object:
+    def headerData(self, section, orientation, role=None):
         if orientation == Qt.Horizontal and role == Qt.DisplayRole:
             self.root_item.data(section)
 
 
 class AddFilesModel(BasePandasModel):
     def __init__(self, data, **kwargs):
         super().__init__(data, **kwargs)
 
     def data(self, index, role=None):
         column = self._data.columns[index.column()]
 
         if role == Qt.DisplayRole:
-            if column != 'Empty-Room?':
+            if column != "Empty-Room?":
                 return str(self.getData(index))
             else:
-                return ''
+                return ""
 
         elif role == Qt.CheckStateRole:
-            if column == 'Empty-Room?':
+            if column == "Empty-Room?":
                 if self.getData(index):
                     return Qt.Checked
                 else:
                     return Qt.Unchecked
 
     def setData(self, index, value, role=None):
-        if role == Qt.CheckStateRole \
-                and self._data.columns[index.column()] == 'Empty-Room?':
+        if (
+            role == Qt.CheckStateRole
+            and self._data.columns[index.column()] == "Empty-Room?"
+        ):
             if value == Qt.Checked:
                 self._data.iloc[index.row(), index.column()] = 1
             else:
                 self._data.iloc[index.row(), index.column()] = 0
             self.dataChanged.emit(index, index, [role])
             return True
 
         return False
 
-    def flags(self, index=QModelIndex()):
-        if self._data.columns[index.column()] == 'Empty-Room?':
-            return QAbstractItemModel.flags(self, index) \
-                   | Qt.ItemIsUserCheckable
+    def flags(self, index):
+        if self._data.columns[index.column()] == "Empty-Room?":
+            return QAbstractItemModel.flags(self, index) | Qt.ItemIsUserCheckable
 
         return QAbstractItemModel.flags(self, index)
 
-    def removeRows(self, row, count, index=QModelIndex()):
-        self.beginRemoveRows(index, row, row + count - 1)
+    def removeRows(self, row, count, parent=None, *args, **kwargs):
+        self.beginRemoveRows(parent, row, row + count - 1)
         # Can't use DataFrame.drop() here,
         # because there could be rows with similar index-labels
         if row == 0:
-            self._data = self._data.iloc[row + count:]
+            self._data = self._data.iloc[row + count :]
         elif row + count >= len(self._data.index):
             self._data = self._data.iloc[:row]
         else:
-            self._data = pd.concat([self._data.iloc[:row],
-                                    self._data.iloc[row + count:]])
+            self._data = pd.concat(
+                [self._data.iloc[:row], self._data.iloc[row + count :]]
+            )
         self.endRemoveRows()
 
         return True
 
 
 class FileManagementModel(BasePandasModel):
     """A model for the Pandas-DataFrames containing information
@@ -778,45 +807,48 @@
 
     def __init__(self, data, **kwargs):
         super().__init__(data, **kwargs)
 
     def data(self, index, role=None):
         value = self.getData(index)
         if role == Qt.DisplayRole:
-            if pd.isna(value) or value in ['existst', 'possible_conflict',
-                                           'critical_conflict']:
+            if pd.isna(value) or value in [
+                "existst",
+                "possible_conflict",
+                "critical_conflict",
+            ]:
                 pass
             elif isinstance(value, datetime):
-                return value.strftime('%d.%m.%y %H:%M')
+                return value.strftime("%d.%m.%y %H:%M")
             elif isinstance(value, float):
                 if value == 0:
                     pass
                 elif value / 1024 < 1000:
-                    return f'{int(value / 1024)} KB'
+                    return f"{int(value / 1024)} KB"
                 else:
-                    return f'{int(value / (1024 ** 2))} MB'
+                    return f"{int(value / (1024 ** 2))} MB"
 
         if role == Qt.DecorationRole:
             if pd.isna(value) or value == 0:
-                return get_std_icon('SP_DialogCancelButton')
-            elif value == 'exists':
-                return get_std_icon('SP_DialogApplyButton')
-            elif value == 'possible_conflict':
-                return get_std_icon('SP_MessageBoxQuestion')
-            elif value == 'critical_conflict':
-                return get_std_icon('SP_MessageBoxWarning')
+                return get_std_icon("SP_DialogCancelButton")
+            elif value == "exists":
+                return get_std_icon("SP_DialogApplyButton")
+            elif value == "possible_conflict":
+                return get_std_icon("SP_MessageBoxQuestion")
+            elif value == "critical_conflict":
+                return get_std_icon("SP_MessageBoxWarning")
 
         elif role == Qt.BackgroundRole:
             if pd.isna(value) or value == 0:
                 return QBrush(Qt.darkRed)
-            elif value == 'exists':
+            elif value == "exists":
                 return QBrush(Qt.green)
-            elif value == 'possible_conflict':
+            elif value == "possible_conflict":
                 return QBrush(Qt.lightGray)
-            elif value == 'critical_conflict':
+            elif value == "critical_conflict":
                 return QBrush(Qt.darkYellow)
 
 
 class CustomFunctionModel(QAbstractListModel):
     """A Model for the Pandas-DataFrames containing information about
      new custom functions/their paramers to display only their name
      and if they are ready.
@@ -827,60 +859,59 @@
     add_pd_funcs or add_pd_params
     """
 
     def __init__(self, data, **kwargs):
         super().__init__(**kwargs)
         self._data = data
 
-    def getData(self, index=QModelIndex()):
+    def getData(self, index):
         return self._data.index[index.row()]
 
     def updateData(self, new_data):
         self._data = new_data
         self.layoutChanged.emit()
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             return str(self.getData(index))
 
         elif role == Qt.DecorationRole:
-            if self._data.loc[self.getData(index), 'ready']:
-                return get_std_icon('SP_DialogApplyButton')
+            if self._data.loc[self.getData(index), "ready"]:
+                return get_std_icon("SP_DialogApplyButton")
             else:
-                return get_std_icon('SP_DialogCancelButton')
+                return get_std_icon("SP_DialogCancelButton")
 
-    def rowCount(self, index=QModelIndex()):
+    def rowCount(self, parent=None, *args, **kwargs):
         return len(self._data.index)
 
 
 class RunModel(QAbstractListModel):
-    """A model for the items/functions of a Pipeline-Run
-    """
+    """A model for the items/functions of a Pipeline-Run"""
 
-    def __init__(self, data, mode):
-        super().__init__()
+    def __init__(self, data, mode, **kwargs):
+        super().__init__(**kwargs)
         self._data = data
         self.mode = mode
 
-    def getKey(self, index=QModelIndex()):
+    def getKey(self, index):
         return list(self._data.keys())[index.row()]
 
-    def getValue(self, index=QModelIndex()):
-        if self.mode == 'object':
-            return self._data[self.getKey(index)]['status']
+    def getValue(self, index):
+        if self.mode == "object":
+            return self._data[self.getKey(index)]["status"]
         else:
             return self._data[self.getKey(index)]
 
-    def getType(self, index=QModelIndex()):
-        return self._data[self.getKey(index)]['type']
+    def getType(self, index):
+        return self._data[self.getKey(index)]["type"]
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
-            if self.mode == 'object':
-                return f'{self.getType(index)}: {self.getKey(index)}'
+            if self.mode == "object":
+                return f"{self.getType(index)}: {self.getKey(index)}"
             return self.getKey(index)
 
         # Object/Function-States:
         # 0 = Finished
         # 1 = Pending
         # 2 = Currently Runnning
         # Return Foreground depending on state of object/function
@@ -895,19 +926,19 @@
             if self.getValue(index) == 2:
                 return QBrush(Qt.darkGreen)
 
         # Mark objects/functions if they are already done,
         # mark objects according to their type (color-code)
         elif role == Qt.DecorationRole:
             if self.getValue(index) == 0:
-                return get_std_icon('SP_DialogApplyButton')
+                return get_std_icon("SP_DialogApplyButton")
             elif self.getValue(index) == 2:
-                return get_std_icon('SP_ArrowRight')
+                return get_std_icon("SP_ArrowRight")
 
         elif role == Qt.FontRole:
             if self.getValue(index) == 2:
                 bold_font = QFont()
                 bold_font.setBold(True)
                 return bold_font
 
-    def rowCount(self, index=QModelIndex()):
+    def rowCount(self, parent=None, *args, **kwargs):
         return len(self._data)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/parameter_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/parameter_widgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,95 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 from ast import literal_eval
 from functools import partial
 
 import numpy as np
 import pandas as pd
 from PyQt5.QtCore import Qt, pyqtSignal
 from PyQt5.QtGui import QFontDatabase, QFont, QPixmap
-from PyQt5.QtWidgets import (QCheckBox, QComboBox, QDialog, QDoubleSpinBox,
-                             QGridLayout, QGroupBox, QHBoxLayout, QLabel,
-                             QLineEdit, QPushButton, QSizePolicy, QSlider,
-                             QSpinBox, QVBoxLayout, QWidget, QDockWidget,
-                             QTabWidget, QScrollArea, QMessageBox,
-                             QStyleFactory, QColorDialog)
+from PyQt5.QtWidgets import (
+    QCheckBox,
+    QComboBox,
+    QDialog,
+    QDoubleSpinBox,
+    QGridLayout,
+    QGroupBox,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
+    QSizePolicy,
+    QSlider,
+    QSpinBox,
+    QVBoxLayout,
+    QWidget,
+    QDockWidget,
+    QTabWidget,
+    QScrollArea,
+    QMessageBox,
+    QColorDialog,
+)
 from mne.viz import Brain
 from mne_qt_browser._pg_figure import _get_color
 from vtkmodules.vtkCommonCore import vtkCommand
 from vtkmodules.vtkRenderingCore import vtkCellPicker
 
 from mne_pipeline_hd import _object_refs
-from mne_pipeline_hd.gui.base_widgets import (CheckList, EditDict, EditList,
-                                              SimpleList, SimpleDialog)
+from mne_pipeline_hd.gui.base_widgets import (
+    CheckList,
+    EditDict,
+    EditList,
+    SimpleList,
+    SimpleDialog,
+    ComboBox,
+)
 from mne_pipeline_hd.gui.dialogs import CheckListDlg
-from mne_pipeline_hd.gui.gui_utils import (get_std_icon, WorkerDialog,
-                                           get_exception_tuple,
-                                           get_user_input_string, center)
+from mne_pipeline_hd.gui.gui_utils import (
+    get_std_icon,
+    WorkerDialog,
+    get_exception_tuple,
+    get_user_input_string,
+    center,
+)
 from mne_pipeline_hd.pipeline.controller import Controller
 from mne_pipeline_hd.pipeline.loading import FSMRI
-from mne_pipeline_hd.pipeline.pipeline_utils import (QS,
-                                                     iswin)
+from mne_pipeline_hd.pipeline.pipeline_utils import QS, iswin
 
 
 class Param(QWidget):
     """
     Base-Class Parameter-GUIs, not to be called directly
     Inherited Clases should have "Gui" in their name to get
     identified correctly.
 
     Attributes
     ----------
     paramChanged : pyqtSignal
         This signal is emmited when the parameter changes.
     """
+
     paramChanged = pyqtSignal(object)
 
-    def __init__(self, data, name, alias=None, default=None,
-                 param_unit=None, groupbox_layout=True,
-                 none_select=False, description=None, depending_on=None):
+    def __init__(
+        self,
+        data,
+        name,
+        alias=None,
+        default=None,
+        param_unit=None,
+        groupbox_layout=True,
+        none_select=False,
+        description=None,
+        depending_on=None,
+    ):
         """
         Parameters
         ----------
         data : dict | Controller | QSettings
             The data-structure, in which the value of the parameter is stored
             (depends on the scenario how the Parameter-Widget is used,
              e.g. displaying parameters from Project or displaying Settings
@@ -104,26 +137,25 @@
 
         # Making sure, that groupbox_layout is on when none_select is one
         # (Selection of None works by checking/unchecking the GroupBox)
         if self.none_select:
             self.groupbox_layout = True
 
         # Connect widget on which this widget depends on
-        dep_widget = _object_refs['parameter_widgets'].get(depending_on,
-                                                           None)
+        dep_widget = _object_refs["parameter_widgets"].get(depending_on, None)
         if dep_widget is not None:
             dep_widget.paramChanged.connect(self.set_param)
 
         # Add to object-reference
-        _object_refs['parameter_widgets'][self.name] = self
+        _object_refs["parameter_widgets"][self.name] = self
 
     def init_ui(self, layout=None):
         """Base layout initialization, which adds the given layout to a
         group-box with the parameters name if groupbox_layout is enabled.
-        Else the layout will be horizontal with a QLabel for the name """
+        Else the layout will be horizontal with a QLabel for the name"""
 
         main_layout = QHBoxLayout()
 
         if self.groupbox_layout:
             self.group_box = QGroupBox(self.alias)
             self.group_box.setLayout(layout)
 
@@ -138,15 +170,15 @@
             else:
                 self.group_box.setCheckable(False)
 
             main_layout.addWidget(self.group_box)
 
         else:
             # Add this to get no label in MultiTypeGui
-            if self.alias != '':
+            if self.alias != "":
                 main_layout.addWidget(QLabel(self.alias))
             main_layout.addLayout(layout)
 
         self.setLayout(main_layout)
 
     def groupbox_toggled(self, checked):
         if checked:
@@ -203,16 +235,15 @@
             else:
                 value = self.default
 
         # get data from Parameters in Project in MainWindow
         # (depending on selected parameter-preset and selected Project)
         elif isinstance(self.data, Controller):
             if name in self.data.pr.parameters[self.data.pr.p_preset]:
-                value = \
-                    self.data.pr.parameters[self.data.pr.p_preset][name]
+                value = self.data.pr.parameters[self.data.pr.p_preset][name]
             else:
                 value = self.default
 
         # get data from QSettings
         elif isinstance(self.data, QS):
             if name in self.data.childKeys():
                 value = self.data.value(name)
@@ -224,28 +255,26 @@
     def read_param(self):
         self.param_value = self._read_data(self.name)
 
     def _save_data(self, name, value):
         if isinstance(self.data, dict):
             self.data[name] = value
         elif isinstance(self.data, Controller):
-            self.data.pr.parameters[self.data.pr.p_preset][
-                name] = value
+            self.data.pr.parameters[self.data.pr.p_preset][name] = value
         elif isinstance(self.data, QS):
             self.data.setValue(name, value)
 
     def save_param(self):
         self._save_data(self.name, self.param_value)
 
 
 class IntGui(Param):
     """A GUI for Integer-Parameters"""
 
-    def __init__(self, min_val=0, max_val=1000,
-                 special_value_text=None, **kwargs):
+    def __init__(self, min_val=0, max_val=1000, special_value_text=None, **kwargs):
         """
         Parameters
         ----------
         min_val : int
             Set the minimumx value, defaults to 0.
         max_val : int
             Set the maximum value, defaults to 100.
@@ -256,20 +285,19 @@
         """
 
         super().__init__(**kwargs)
 
         self.param_widget = QSpinBox()
         self.param_widget.setMinimum(min_val)
         self.param_widget.setMaximum(max_val)
-        self.param_widget.setToolTip(
-            f'MinValue = {min_val}\nMaxValue = {max_val}')
+        self.param_widget.setToolTip(f"MinValue = {min_val}\nMaxValue = {max_val}")
         if special_value_text:
             self.param_widget.setSpecialValueText(special_value_text)
         if self.param_unit:
-            self.param_widget.setSuffix(f' {self.param_unit}')
+            self.param_widget.setSuffix(f" {self.param_unit}")
         self.param_widget.valueChanged.connect(self._get_param)
 
         self.read_param()
         self._init_layout()
         self._set_param()
         self.save_param()
 
@@ -284,17 +312,15 @@
     def get_value(self):
         return self.param_widget.value()
 
 
 class FloatGui(Param):
     """A GUI for Float-Parameters"""
 
-    def __init__(self, min_val=-1000.,
-                 max_val=1000., step=0.1,
-                 decimals=2, **kwargs):
+    def __init__(self, min_val=-1000.0, max_val=1000.0, step=0.1, decimals=2, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to -100..
         max_val : int | float
             Set the maximum value, defaults to 100..
@@ -308,18 +334,17 @@
 
         super().__init__(**kwargs)
         self.param_widget = QDoubleSpinBox()
         self.param_widget.setMinimum(min_val)
         self.param_widget.setMaximum(max_val)
         self.param_widget.setSingleStep(step)
         self.param_widget.setDecimals(decimals)
-        self.param_widget.setToolTip(
-            f'MinValue = {min_val}\nMaxVal = {max_val}')
+        self.param_widget.setToolTip(f"MinValue = {min_val}\nMaxVal = {max_val}")
         if self.param_unit:
-            self.param_widget.setSuffix(f' {self.param_unit}')
+            self.param_widget.setSuffix(f" {self.param_unit}")
         self.param_widget.valueChanged.connect(self._get_param)
 
         self.read_param()
         self._init_layout()
         self._set_param()
         self.save_param()
 
@@ -370,49 +395,49 @@
 
     def get_value(self):
         return self.param_widget.text()
 
 
 def _eval_param(param_exp):
     try:
-        return eval(param_exp, {'np': np})
+        return eval(param_exp, {"np": np})
     except (NameError, SyntaxError, ValueError, TypeError):
         return None
 
 
 class FuncGui(Param):
-    """A GUI for Parameters defined by small functions, e.g from numpy
-    """
+    """A GUI for Parameters defined by small functions, e.g from numpy"""
 
     def __init__(self, **kwargs):
         """
         Parameters
         ----------
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
         super().__init__(**kwargs)
         self.param_exp = None
         self.param_widget = QLineEdit()
         self.param_widget.setToolTip(
-            'Use of functions also allowed '
-            '(from already imported modules + numpy as np)\n'
-            'Be carefull as everything entered will be executed!')
+            "Use of functions also allowed "
+            "(from already imported modules + numpy as np)\n"
+            "Be carefull as everything entered will be executed!"
+        )
         self.param_widget.editingFinished.connect(self._get_param)
 
         self.display_widget = QLabel()
         self.read_param()
         self.init_func_layout()
         self._set_param()
         self.save_param()
 
     def init_func_layout(self):
         func_layout = QGridLayout()
-        label1 = QLabel('Insert Function/Value here')
-        label2 = QLabel('Output')
+        label1 = QLabel("Insert Function/Value here")
+        label2 = QLabel("Output")
         func_layout.addWidget(label1, 0, 0)
         func_layout.addWidget(label2, 0, 1, 1, 2)
         func_layout.addWidget(self.param_widget, 1, 0)
         func_layout.addWidget(self.display_widget, 1, 1)
         if self.param_unit:
             func_layout.addWidget(QLabel(self.param_unit))
         self.init_ui(func_layout)
@@ -443,27 +468,27 @@
             self._get_param()
 
     def read_param(self):
         # Get not only param_value, but also param_exp storing
         # the exact expression which is evaluated
         super().read_param()
         real_value = self.param_value
-        self.name = self.name + '_exp'
+        self.name = self.name + "_exp"
         super().read_param()
-        if self.param_value != '' and self.param_value is not None:
+        if self.param_value != "" and self.param_value is not None:
             self.param_exp = self.param_value
         else:
             self.param_exp = real_value
         self.param_value = real_value
         self.name = self.name[:-4]
 
     def save_param(self):
         super().save_param()
         real_value = self.param_value
-        self.name = self.name + '_exp'
+        self.name = self.name + "_exp"
         self.param_value = self.param_exp
         super().save_param()
         self.name = self.name[:-4]
         self.param_value = real_value
 
 
 class BoolGui(Param):
@@ -504,15 +529,15 @@
 
         return value
 
 
 class TupleGui(Param):
     """A GUI for Tuple-Parameters"""
 
-    def __init__(self, min_val=-1000., max_val=1000., step=.1, **kwargs):
+    def __init__(self, min_val=-1000.0, max_val=1000.0, step=0.1, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to -100..
         max_val : int | float
             Set the maximum value, defaults to 100..
@@ -528,37 +553,39 @@
             self.param_widget1 = QSpinBox()
             self.param_widget2 = QSpinBox()
             min_val = int(min_val)
             max_val = int(max_val)
         else:
             self.param_widget1 = QDoubleSpinBox()
             self.param_widget2 = QDoubleSpinBox()
-            decimals = len(str(step)[str(step).find('.'):]) - 1
+            decimals = len(str(step)[str(step).find(".") :]) - 1
             self.param_widget1.setDecimals(decimals)
             self.param_widget2.setDecimals(decimals)
 
         self._external_set = False
 
         self.param_widget1.setToolTip(
-            f'MinValue = {min_val}\nMaxVal = {max_val}\nStep = {step}\n')
+            f"MinValue = {min_val}\nMaxVal = {max_val}\nStep = {step}\n"
+        )
         self.param_widget2.setToolTip(
-            f'MinValue = {min_val}\nMaxVal = {max_val}\nStep = {step}\n')
+            f"MinValue = {min_val}\nMaxVal = {max_val}\nStep = {step}\n"
+        )
 
         self.param_widget1.setMinimum(min_val)
         self.param_widget1.setMaximum(max_val)
         self.param_widget1.setSingleStep(step)
         if self.param_unit:
-            self.param_widget1.setSuffix(f' {self.param_unit}')
+            self.param_widget1.setSuffix(f" {self.param_unit}")
         self.param_widget1.valueChanged.connect(self._get_param)
 
         self.param_widget2.setMinimum(min_val)
         self.param_widget2.setMaximum(max_val)
         self.param_widget2.setSingleStep(step)
         if self.param_unit:
-            self.param_widget2.setSuffix(f' {self.param_unit}')
+            self.param_widget2.setSuffix(f" {self.param_unit}")
         self.param_widget2.valueChanged.connect(self._get_param)
 
         self.read_param()
         self.init_tuple_layout()
         self._set_param()
         self.save_param()
 
@@ -597,15 +624,15 @@
             If supplied a dictionary, dictionary-values are
             taken as aliases for the keys.
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
         super().__init__(**kwargs)
         self.options = options
-        self.param_widget = QComboBox()
+        self.param_widget = ComboBox(scrollable=False)
         self.param_widget.activated.connect(self._get_param)
         for option in self.options:
             if isinstance(self.options, dict):
                 self.param_widget.addItem(str(self.options[option]))
             else:
                 self.param_widget.addItem(str(option))
 
@@ -619,23 +646,25 @@
         layout.addWidget(self.param_widget)
         if self.param_unit is not None:
             layout.addWidget(QLabel(self.param_unit))
         self.init_ui(layout)
 
     def set_value(self, value):
         if isinstance(self.options, dict):
-            self.param_widget.setCurrentText(
-                str(self.options[value]))
+            self.param_widget.setCurrentText(str(self.options[value]))
         else:
             self.param_widget.setCurrentText(str(value))
 
     def get_value(self):
         if isinstance(self.options, dict):
-            text = [key for key, value in self.options.items()
-                    if value == self.param_widget.currentText()][0]
+            text = [
+                key
+                for key, value in self.options.items()
+                if value == self.param_widget.currentText()
+            ][0]
         else:
             text = self.param_widget.currentText()
         try:
             value = literal_eval(text)
         except (SyntaxError, ValueError):
             value = text
 
@@ -649,15 +678,15 @@
 
         self._init_layout()
         self.open()
 
     def _init_layout(self):
         layout = QVBoxLayout()
         layout.addWidget(EditList(self.paramw.param_value))
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
         self.setLayout(layout)
 
     def closeEvent(self, event):
         self.paramw._set_param()
         self.paramw.save_param()
@@ -690,39 +719,36 @@
 
     def _init_layout(self):
         list_layout = QHBoxLayout()
 
         self.value_label = QLabel()
         list_layout.addWidget(self.value_label)
 
-        self.param_widget = QPushButton('Edit')
-        self.param_widget.setSizePolicy(QSizePolicy.Maximum,
-                                        QSizePolicy.Maximum)
+        self.param_widget = QPushButton("Edit")
+        self.param_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.param_widget.clicked.connect(partial(ListDialog, self))
         list_layout.addWidget(self.param_widget, alignment=Qt.AlignCenter)
 
         self.init_ui(list_layout)
 
     def set_value(self, value):
         if value is not None:
             self.cached_value = value
         self.check_groupbox_state()
-        if value is not None:
+        if isinstance(value, list):
             if self.param_unit:
-                val_str = ', '.join(
-                    [f'{item} {self.param_unit}' for item in value])
+                val_str = ", ".join([f"{item} {self.param_unit}" for item in value])
             else:
-                val_str = ', '.join([str(item) for item in value])
+                val_str = ", ".join([str(item) for item in value])
             if len(val_str) >= self.value_string_length:
-                self.value_label.setText(
-                    f'{val_str[:self.value_string_length]} ...')
+                self.value_label.setText(f"{val_str[:self.value_string_length]} ...")
             else:
                 self.value_label.setText(val_str)
         else:
-            self.value_label.setText('None')
+            self.value_label.setText("None")
 
     def get_value(self):
         if self.param_value is None:
             if self.cached_value is not None:
                 value = self.cached_value
             else:
                 value = list()
@@ -739,36 +765,38 @@
         self.paramw = paramw
 
         self._init_layout()
         self.open()
 
     def _init_layout(self):
         layout = QVBoxLayout()
-        layout.addWidget(CheckList(data=self.paramw.options,
-                                   checked=self.paramw.param_value,
-                                   one_check=self.paramw.one_check))
+        layout.addWidget(
+            CheckList(
+                data=self.paramw.options,
+                checked=self.paramw.param_value,
+                one_check=self.paramw.one_check,
+            )
+        )
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def closeEvent(self, event):
         self.paramw._set_param()
         self.paramw.save_param()
         event.accept()
 
 
 class CheckListGui(Param):
-    """A GUI to select items from a list of options
-    """
+    """A GUI to select items from a list of options"""
 
-    def __init__(self, options, value_string_length=30, one_check=False,
-                 **kwargs):
+    def __init__(self, options, value_string_length=30, one_check=False, **kwargs):
         """
         Parameters
         ----------
         options : list
             The items from which to choose
         value_string_length : int | None
             Set the limit of characters to which the value converted to a
@@ -777,15 +805,15 @@
             Set to True, if only one item should be selectable
              (or use ComboGUI).
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
 
         if not isinstance(options, list) or len(options) == 0:
-            options = ['Empty']
+            options = ["Empty"]
 
         super().__init__(**kwargs)
         self.options = options
         self.value_string_length = value_string_length
         self.one_check = one_check
         # Cache param_value to use after
         self.cached_value = None
@@ -797,39 +825,36 @@
 
     def _init_layout(self):
         check_list_layout = QHBoxLayout()
 
         self.value_label = QLabel()
         check_list_layout.addWidget(self.value_label)
 
-        self.param_widget = QPushButton('Edit')
-        self.param_widget.setSizePolicy(QSizePolicy.Maximum,
-                                        QSizePolicy.Maximum)
+        self.param_widget = QPushButton("Edit")
+        self.param_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.param_widget.clicked.connect(partial(CheckListDialog, self))
         check_list_layout.addWidget(self.param_widget)
 
         self.init_ui(check_list_layout)
 
     def set_value(self, value):
         if value is not None:
             self.cached_value = value
         self.check_groupbox_state()
-        if value is not None:
+        if isinstance(value, list):
             if self.param_unit:
-                val_str = ', '.join(
-                    [f'{item} {self.param_unit}' for item in value])
+                val_str = ", ".join([f"{item} {self.param_unit}" for item in value])
             else:
-                val_str = ', '.join([str(item) for item in value])
+                val_str = ", ".join([str(item) for item in value])
             if len(val_str) >= self.value_string_length:
-                self.value_label.setText(
-                    f'{val_str[:self.value_string_length]} ...')
+                self.value_label.setText(f"{val_str[:self.value_string_length]} ...")
             else:
                 self.value_label.setText(val_str)
         else:
-            self.value_label.setText('None')
+            self.value_label.setText("None")
 
     def get_value(self):
         if self.param_value is None:
             if self.cached_value:
                 value = self.cached_value
             else:
                 value = list()
@@ -847,15 +872,15 @@
 
         self._init_layout()
         self.open()
 
     def _init_layout(self):
         layout = QVBoxLayout()
         layout.addWidget(EditDict(self.paramw.param_value))
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
         self.setLayout(layout)
 
     def closeEvent(self, event):
         self.paramw._set_param()
         self.paramw.save_param()
@@ -890,41 +915,43 @@
 
     def _init_layout(self):
         dict_layout = QHBoxLayout()
 
         self.value_label = QLabel()
         dict_layout.addWidget(self.value_label)
 
-        self.param_widget = QPushButton('Edit')
-        self.param_widget.setSizePolicy(QSizePolicy.Maximum,
-                                        QSizePolicy.Maximum)
+        self.param_widget = QPushButton("Edit")
+        self.param_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.param_widget.clicked.connect(partial(DictDialog, self))
         dict_layout.addWidget(self.param_widget)
 
         self.init_ui(dict_layout)
 
+    # ToDo: improve None-handling, maybe generalize
+    #  (sometimes error when value=float, probably nan)
     def set_value(self, value):
         if value is not None:
             self.cached_value = value
         self.check_groupbox_state()
-        if value is not None:
+        if isinstance(value, dict):
             if self.param_unit:
-                val_str = ', '.join(
-                    [f'{key} {self.param_unit}: {value} {self.param_unit}'
-                     for key, value in value.items()])
+                val_str = ", ".join(
+                    [
+                        f"{k} {self.param_unit}: {v} {self.param_unit}"
+                        for k, v in value.items()
+                    ]
+                )
             else:
-                val_str = ', '.join([f'{key}: {value}' for key, value in
-                                     value.items()])
+                val_str = ", ".join([f"{k}: {v}" for k, v in value.items()])
             if len(val_str) > self.value_string_length:
-                self.value_label.setText(
-                    f'{val_str[:self.value_string_length]} ...')
+                self.value_label.setText(f"{val_str[:self.value_string_length]} ...")
             else:
                 self.value_label.setText(val_str)
         else:
-            self.value_label.setText('None')
+            self.value_label.setText("None")
 
     def get_value(self):
         if self.param_value is None:
             if self.cached_value:
                 value = self.cached_value
             else:
                 value = dict()
@@ -934,16 +961,15 @@
 
         return value
 
 
 class SliderGui(Param):
     """A GUI to show a slider for Int/Float-Parameters"""
 
-    def __init__(self, min_val=0, max_val=100, step=1, tracking=True,
-                 **kwargs):
+    def __init__(self, min_val=0, max_val=100, step=1, tracking=True, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to 0.
         max_val : int | float
             Set the maximum value, defaults to 100..
@@ -956,38 +982,38 @@
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
         super().__init__(**kwargs)
         self.min_val = min_val
         self.max_val = max_val
         self.param_widget = QSlider()
-        self.param_widget.setSizePolicy(QSizePolicy.Expanding,
-                                        QSizePolicy.Maximum)
+        self.param_widget.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Maximum)
         self.decimal_count = max(
-            [len(str(value)[str(value).find('.'):]) - 1 for value in
-             [min_val, max_val, step]])
+            [
+                len(str(value)[str(value).find(".") :]) - 1
+                for value in [min_val, max_val, step]
+            ]
+        )
         if self.decimal_count > 0:
-            self.param_widget.setMinimum(
-                int(self.min_val * 10 ** self.decimal_count))
-            self.param_widget.setMaximum(
-                int(self.max_val * 10 ** self.decimal_count))
+            self.param_widget.setMinimum(int(self.min_val * 10**self.decimal_count))
+            self.param_widget.setMaximum(int(self.max_val * 10**self.decimal_count))
         else:
             self.param_widget.setMinimum(self.min_val)
             self.param_widget.setMaximum(self.max_val)
         self.param_widget.setSingleStep(int(step))
         self.param_widget.setOrientation(Qt.Horizontal)
         # Only change value when slider is released
         self.param_widget.setTracking(tracking)
         self.param_widget.setToolTip(
-            f'MinValue = {min_val}\nMaxValue = {max_val}\nStep = {step}')
+            f"MinValue = {min_val}\nMaxValue = {max_val}\nStep = {step}"
+        )
         self.param_widget.valueChanged.connect(self._get_param)
 
         self.display_widget = QLineEdit()
-        self.display_widget.setSizePolicy(QSizePolicy.Maximum,
-                                          QSizePolicy.Maximum)
+        self.display_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.display_widget.setAlignment(Qt.AlignRight)
         self.display_widget.editingFinished.connect(self.display_edited)
 
         self.read_param()
         self.init_slider_ui()
         self._set_param()
         self.save_param()
@@ -1004,41 +1030,38 @@
     def display_edited(self):
         try:
             new_value = literal_eval(self.display_widget.text())
         except (ValueError, SyntaxError):
             new_value = None
         if new_value:
             self.param_value = new_value
-            self.param_widget.setValue(
-                int(new_value * 10 ** self.decimal_count))
+            self.param_widget.setValue(int(new_value * 10**self.decimal_count))
 
     def set_value(self, value):
         self.check_groupbox_state()
         if value is not None:
             if self.decimal_count > 0:
-                self.param_widget.setValue(
-                    int(value * 10 ** self.decimal_count))
+                self.param_widget.setValue(int(value * 10**self.decimal_count))
             else:
                 self.param_widget.setValue(value)
             self.display_widget.setText(str(value))
 
     def get_value(self):
         value = self.param_widget.value()
         if self.decimal_count > 0:
-            value /= 10 ** self.decimal_count
+            value /= 10**self.decimal_count
         self.display_widget.setText(str(value))
 
         return value
 
 
 class MultiTypeGui(Param):
     """A GUI which accepts multiple types of values in a single LineEdit"""
 
-    def __init__(self, type_selection=False, types=None, type_kwargs=None,
-                 **kwargs):
+    def __init__(self, type_selection=False, types=None, type_kwargs=None, **kwargs):
         """
         Parameters
         ----------
         type_selection : bool
             If True, the use can choose in a QComboBox which type they want
             to enter and then use the appropriate GUI.
         types : list of str | None
@@ -1049,43 +1072,43 @@
             (look into their documentation),
             the key is the name of the GUI (e.g. IntGui).
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
         super().__init__(**kwargs)
         self.type_selection = type_selection
-        self.types = types or ['int', 'float', 'bool', 'str', 'list', 'dict',
-                               'tuple']
+        self.types = types or ["int", "float", "bool", "str", "list", "dict", "tuple"]
         self.type_kwargs = type_kwargs or dict()
 
         # A dictionary to map possible types with their GUI
-        self.gui_types = {'int': 'IntGui',
-                          'float': 'FloatGui',
-                          'bool': 'BoolGui',
-                          'str': 'StringGui',
-                          'list': 'ListGui',
-                          'dict': 'DictGui',
-                          'tuple': 'TupleGui'}
+        self.gui_types = {
+            "int": "IntGui",
+            "float": "FloatGui",
+            "bool": "BoolGui",
+            "str": "StringGui",
+            "list": "ListGui",
+            "dict": "DictGui",
+            "tuple": "TupleGui",
+        }
 
         if self.type_selection:
             self.type_cmbx = QComboBox()
-            self.type_cmbx.setSizePolicy(QSizePolicy.Maximum,
-                                         QSizePolicy.Maximum)
+            self.type_cmbx.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
             self.type_cmbx.addItems(self.types)
             self.type_cmbx.activated.connect(self.change_type)
         else:
             self.param_widget = QLineEdit()
             self.param_widget.textEdited.connect(self._get_param)
             self.type_display = QLabel()
 
         self.read_param()
 
         # Get current type (NoneType not allowed)
         self.param_type = type(self.param_value).__name__
-        if self.param_type == 'NoneType':
+        if self.param_type == "NoneType":
             self.param_type = self.types[0]
         if self.type_selection:
             self.type_cmbx.setCurrentText(self.param_type)
 
         self._init_layout()
         self._set_param()
         self.save_param()
@@ -1096,22 +1119,22 @@
         # Load specifc keyword-arguments if given
         if gui_name in self.type_kwargs:
             kwargs = self.type_kwargs[gui_name]
         else:
             kwargs = dict()
 
         # Set standard parameter-keyword-arguments as given to MultiTypeGui
-        kwargs['data'] = self.data
-        kwargs['name'] = self.name
-        kwargs['alias'] = ''
-        kwargs['default'] = self.default
-        kwargs['groupbox_layout'] = False
-        kwargs['none_select'] = False
-        kwargs['description'] = self.description
-        kwargs['param_unit'] = self.param_unit
+        kwargs["data"] = self.data
+        kwargs["name"] = self.name
+        kwargs["alias"] = ""
+        kwargs["default"] = self.default
+        kwargs["groupbox_layout"] = False
+        kwargs["none_select"] = False
+        kwargs["description"] = self.description
+        kwargs["param_unit"] = self.param_unit
 
         self.param_widget = globals()[gui_name](**kwargs)
         self.param_widget.param_value = self.param_value
         self.param_widget._get_param()
         self.param_widget._set_param()
         self.type_layout.addWidget(self.param_widget)
 
@@ -1145,96 +1168,98 @@
     def set_value(self, value):
         self.check_groupbox_state()
         if self.type_selection:
             self.param_widget.param_value = value
             self.param_widget._set_param()
         elif value is not None:
             self.param_widget.setText(str(value))
-            self.type_display.setText(
-                f'Type: {type(value).__name__}')
+            self.type_display.setText(f"Type: {type(value).__name__}")
 
     def get_value(self):
         if self.type_selection:
             self.param_widget._get_param()
             value = self.param_widget.param_value
         else:
             text = self.param_widget.text()
             try:
                 value = literal_eval(text)
                 self.param_type = type(value).__name__
             except ValueError:
                 value = text
-                self.param_type = 'str'
+                self.param_type = "str"
             except SyntaxError:
                 value = None
-                self.param_type = 'error'
-            self.type_display.setText(f'Type: {self.param_type}')
+                self.param_type = "error"
+            self.type_display.setText(f"Type: {self.param_type}")
             self.save_param()
 
         return value
 
 
 class LabelPicker(Brain):
     def __init__(self, paramdlg, *args, **kwargs):
         try:
             super().__init__(*args, **kwargs)
         except TypeError:
             # Backwards compatibility mne==0.24
-            kwargs.pop('block')
+            kwargs.pop("block")
             super().__init__(*args, **kwargs)
         self.paramdlg = paramdlg
         self.paramw = paramdlg.paramw
 
         self._shown_labels = list()
 
         self._set_annotations()
         self._init_picking()
-        self.add_text(0, 0.9, 'Pick labels', 'title', font_size=14)
+        self.add_text(0, 0.9, "Pick labels", "title", font_size=14)
 
     def _set_annotations(self):
         fsmri = self.paramdlg._fsmri
         parcellation = self.paramdlg._parcellation
         self.clear_glyphs()
         self.remove_labels()
         self.remove_annotations()
-        self.add_annotation(parcellation, color='w', alpha=0.75)
+        self.add_annotation(parcellation, color="w", alpha=0.75)
 
-        for parc in [parcellation, 'Other']:
-            labels = fsmri.labels.get(parc)
-            if labels is not None:
+        for parc in [parcellation, "Other"]:
+            if parc in fsmri.labels:
+                labels = fsmri.labels[parc]
                 for hemi in self._hemis:
-                    hemi_labels = [lb for lb in labels.values()
-                                   if lb.hemi == hemi]
+                    hemi_labels = [lb for lb in labels if lb.hemi == hemi]
                     self._vertex_to_label_id[hemi] = np.full(
-                        self.geo[hemi].coords.shape[0], -1)
+                        self.geo[hemi].coords.shape[0], -1
+                    )
                     self._annotation_labels[hemi] = hemi_labels
                     for idx, label in enumerate(hemi_labels):
                         self._vertex_to_label_id[hemi][label.vertices] = idx
 
     def _init_picking(self):
         self._mouse_no_mvt = -1
         add_obs = self._renderer.plotter.iren.add_observer
         add_obs(vtkCommand.RenderEvent, self._on_mouse_move)
         add_obs(vtkCommand.LeftButtonPressEvent, self._on_button_press)
         add_obs(vtkCommand.EndInteractionEvent, self._on_button_release)
         self._renderer.plotter.picker = vtkCellPicker()
-        self._renderer.plotter.picker.AddObserver(vtkCommand.EndPickEvent,
-                                                  self._label_picked)
+        self._renderer.plotter.picker.AddObserver(
+            vtkCommand.EndPickEvent, self._label_picked
+        )
 
     def _label_picked(self, vtk_picker, _):
         cell_id = vtk_picker.GetCellId()
         mesh = vtk_picker.GetDataSet()
         if mesh is not None:
             hemi = mesh._hemi
             if mesh is None or cell_id == -1 or not self._mouse_no_mvt:
                 return  # don't pick
             pos = np.array(vtk_picker.GetPickPosition())
             vtk_cell = mesh.GetCell(cell_id)
-            cell = [vtk_cell.GetPointId(point_id) for point_id
-                    in range(vtk_cell.GetNumberOfPoints())]
+            cell = [
+                vtk_cell.GetPointId(point_id)
+                for point_id in range(vtk_cell.GetNumberOfPoints())
+            ]
             vertices = mesh.points[cell]
             idx = np.argmin(abs(vertices - pos), axis=0)
             vertex_id = cell[idx[0]]
 
             label_id = self._vertex_to_label_id[hemi][vertex_id]
             label = self._annotation_labels[hemi][label_id]
 
@@ -1265,17 +1290,21 @@
         self.paramdlg._label_picker = None
         super().closeEvent(event)
 
 
 class LabelDialog(SimpleDialog):
     def __init__(self, paramw):
         self.main_widget = QWidget()
-        super().__init__(self.main_widget, parent=paramw,
-                         title='Choose a label!',
-                         window_title='Label Picker', modal=False)
+        super().__init__(
+            self.main_widget,
+            parent=paramw,
+            title="Choose a label!",
+            window_title="Label Picker",
+            modal=False,
+        )
         self.paramw = paramw
         self.ct = paramw.data
         self.params = self.ct.pr.parameters[self.ct.pr.p_preset]
         self.param_value = paramw.param_value
 
         self._label_picker = None
         self._fsmri = None
@@ -1297,74 +1326,77 @@
         self.fsmri_cmbx.activated.connect(self._subject_changed)
         layout.addWidget(self.fsmri_cmbx)
 
         self.parcellation_cmbx = QComboBox()
         self.parcellation_cmbx.activated.connect(self._parc_changed)
         layout.addWidget(self.parcellation_cmbx)
 
-        self.label_list = CheckList(data=self._all_label_names,
-                                    checked=self._selected_labels,
-                                    ui_buttons=True, ui_button_pos='bottom')
+        self.label_list = CheckList(
+            data=self._all_label_names,
+            checked=self._selected_labels,
+            ui_buttons=True,
+            ui_button_pos="bottom",
+        )
         self.label_list.checkedChanged.connect(self._labels_changed)
         layout.addWidget(self.label_list)
 
-        slider_kwargs = {'max_val': 360, 'tracking': False}
-        self.elevation_slider = SliderGui(data=self.paramw.data,
-                                          name='stc_elevation',
-                                          **slider_kwargs)
-        self.elevation_slider.paramChanged.connect(self._slider_changed)
-        layout.addWidget(self.elevation_slider)
-
-        self.roll_slider = SliderGui(data=self.paramw.data,
-                                     name='stc_roll',
-                                     **slider_kwargs)
-        self.roll_slider.paramChanged.connect(self._slider_changed)
-        layout.addWidget(self.roll_slider)
-
-        self.azimuth_slider = SliderGui(data=self.paramw.data,
-                                        name='stc_azimuth',
-                                        **slider_kwargs)
-        self.azimuth_slider.paramChanged.connect(self._slider_changed)
-        layout.addWidget(self.azimuth_slider)
-
-        choose_bt = QPushButton('Choose Labels')
-        choose_bt.clicked.connect(self._open_label_picker)
-        layout.addWidget(choose_bt)
+        # ToDo: fix Brain-Picker (errors and somehow all labels are selected)
+        # slider_kwargs = {'max_val': 360, 'tracking': False}
+        # self.elevation_slider = SliderGui(data=self.paramw.data,
+        #                                   name='stc_elevation',
+        #                                   **slider_kwargs)
+        # self.elevation_slider.paramChanged.connect(self._slider_changed)
+        # layout.addWidget(self.elevation_slider)
+        #
+        # self.roll_slider = SliderGui(data=self.paramw.data,
+        #                              name='stc_roll',
+        #                              **slider_kwargs)
+        # self.roll_slider.paramChanged.connect(self._slider_changed)
+        # layout.addWidget(self.roll_slider)
+        #
+        # self.azimuth_slider = SliderGui(data=self.paramw.data,
+        #                                 name='stc_azimuth',
+        #                                 **slider_kwargs)
+        # self.azimuth_slider.paramChanged.connect(self._slider_changed)
+        # layout.addWidget(self.azimuth_slider)
+        #
+        # choose_bt = QPushButton('Choose Labels')
+        # choose_bt.clicked.connect(self._open_label_picker)
+        # layout.addWidget(choose_bt)
 
         # Initialize with first items
         self._subject_changed()
         self._parc_changed()
 
     def _subject_changed(self):
-        self._fsmri = FSMRI(self.fsmri_cmbx.currentText(), self.ct)
+        self._fsmri = FSMRI(self.fsmri_cmbx.currentText(), self.ct, load_labels=True)
 
         self.parcellation_cmbx.clear()
         self.parcellation_cmbx.addItems(self._fsmri.parcellations)
-        param_parc = self.ct.pr.parameters[self.ct.pr.p_preset]['parcellation']
-        if param_parc in self._fsmri.parcellations:
-            self.parcellation_cmbx.setCurrentText(param_parc)
         self._parc_changed()
 
     def _parc_changed(self):
         # Keep reference for inplace change
         self._all_label_names.clear()
         self._selected_labels.clear()
 
         # Add single labels
-        self._all_label_names += list(self._fsmri.labels['Other'].keys())
+        self._all_label_names += [lb.name for lb in self._fsmri.labels["Other"]]
 
         # Add parcellation labels
         self._parcellation = self.parcellation_cmbx.currentText()
-        parc_labels = self._fsmri.labels.get(self._parcellation)
-        if parc_labels is not None:
-            self._all_label_names += list(parc_labels.keys())
+        if self._parcellation in self._fsmri.labels:
+            self._all_label_names += [
+                lb.name for lb in self._fsmri.labels[self._parcellation]
+            ]
 
         # get selected
-        self._selected_labels += [lb for lb in self.paramw.param_value
-                                  if lb in self._all_label_names]
+        self._selected_labels += [
+            lb for lb in self.paramw.param_value if lb in self._all_label_names
+        ]
         self.label_list.content_changed()
 
         if self._label_picker is not None:
             self._label_picker._set_annotations()
 
     def _labels_changed(self, labels):
         if self._label_picker is not None:
@@ -1378,26 +1410,32 @@
 
     def _slider_changed(self, _):
         if self._label_picker is not None:
             roll = self.roll_slider.param_value
             elevation = self.elevation_slider.param_value
             azimuth = self.azimuth_slider.param_value
             for row, col in [(0, 0), (0, 1), (1, 0), (1, 1)]:
-                self._label_picker.show_view(roll=roll, elevation=elevation,
-                                             azimuth=azimuth, row=row,
-                                             col=col)
+                self._label_picker.show_view(
+                    roll=roll, elevation=elevation, azimuth=azimuth, row=row, col=col
+                )
 
     def _open_label_picker(self):
-        background = self.params['stc_background']
+        background = self.params["stc_background"]
 
         self._label_picker = LabelPicker(
-            self, self._fsmri.name, hemi='split', views=['lat', 'med'],
-            surf='inflated', title='Pick labels',
-            subjects_dir=self.ct.subjects_dir, block=False,
-            background=background)
+            self,
+            self._fsmri.name,
+            hemi="split",
+            views=["lat", "med"],
+            surf="inflated",
+            title="Pick labels",
+            subjects_dir=self.ct.subjects_dir,
+            block=False,
+            background=background,
+        )
         self._slider_changed(None)
 
     def closeEvent(self, event):
         event.accept()
         self.paramw.param_value = self._selected_labels
         self.paramw._get_param()
         self.paramw._set_param()
@@ -1420,51 +1458,51 @@
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
 
         super().__init__(**kwargs)
         self.value_string_length = value_string_length
         if not isinstance(self.data, Controller):
-            raise RuntimeError('LabelGui can only used with an instance of '
-                               'Controller passed as data.')
+            raise RuntimeError(
+                "LabelGui can only used with an instance of "
+                "Controller passed as data."
+            )
         self.read_param()
         self._init_layout()
         self._set_param()
         self.save_param()
 
     def _init_layout(self):
         check_list_layout = QHBoxLayout()
 
         self.value_label = QLabel()
         check_list_layout.addWidget(self.value_label)
 
-        self.param_widget = QPushButton('Edit')
-        self.param_widget.setSizePolicy(QSizePolicy.Maximum,
-                                        QSizePolicy.Maximum)
+        self.param_widget = QPushButton("Edit")
+        self.param_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         self.param_widget.clicked.connect(partial(LabelDialog, self))
         check_list_layout.addWidget(self.param_widget)
 
         self.init_ui(check_list_layout)
 
     def set_value(self, value):
         if value is not None:
             self.cached_value = value
         self.check_groupbox_state()
-        if value is not None:
+        if isinstance(value, list):
             if self.param_unit:
-                val_str = ', '.join([f'{item}' for item in value])
+                val_str = ", ".join([f"{item}" for item in value])
             else:
-                val_str = ', '.join([str(item) for item in value])
+                val_str = ", ".join([str(item) for item in value])
             if len(val_str) >= self.value_string_length:
-                self.value_label.setText(
-                    f'{val_str[:self.value_string_length]} ...')
+                self.value_label.setText(f"{val_str[:self.value_string_length]} ...")
             else:
                 self.value_label.setText(val_str)
         else:
-            self.value_label.setText('None')
+            self.value_label.setText("None")
 
     def get_value(self):
         if self.param_value is None:
             if self.cached_value:
                 value = self.cached_value
             else:
                 value = list()
@@ -1508,51 +1546,53 @@
         layout = QHBoxLayout()
         self.select_widget = QComboBox()
         self.select_widget.setEditable(True)
         self.select_widget.addItems([str(k) for k in self.keys])
         self.select_widget.activated.connect(self._change_display_color)
         layout.addWidget(self.select_widget)
         self.display_widget = QLabel()
-        self.display_widget.setSizePolicy(QSizePolicy.Maximum,
-                                          QSizePolicy.Preferred)
+        self.display_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
         layout.addWidget(self.display_widget)
-        self.param_widget = QPushButton('Pick Color')
+        self.param_widget = QPushButton("Pick Color")
         self.param_widget.clicked.connect(self._pick_color)
         layout.addWidget(self.param_widget)
         self.init_ui(layout)
 
     def _change_display_color(self):
         key = self.select_widget.currentText()
         if key in self._cached_value:
             color = _get_color(self._cached_value[key])
             pixmap = QPixmap(20, 20)
             pixmap.fill(color)
             self.display_widget.setPixmap(pixmap)
         else:
-            self.display_widget.setText('None')
+            self.display_widget.setText("None")
 
     def set_value(self, value):
         self._cached_value = value
         self.keys = value.keys()
         self._change_display_color()
 
     def get_value(self):
         return self._cached_value
 
     def _pick_color(self):
         key = self.select_widget.currentText()
         if key in self._cached_value:
             previous_color = _get_color(self._cached_value[key])
             color = QColorDialog.getColor(
-                initial=previous_color, parent=self,
-                title=f'Pick a color for {self.name}')
+                initial=previous_color,
+                parent=self,
+                title=f"Pick a color for {self.name}",
+            )
         else:
             # blocking
             color = QColorDialog.getColor(
-                parent=self, title=f'Pick a color for {self.name}')
+                parent=self, title=f"Pick a color for {self.name}"
+            )
         self._cached_value[key] = color.name()
         self._change_display_color()
         self._set_param()
         self._get_param()
 
 
 # Todo: Ordering Parameters in Tabs and add Find-Command
@@ -1563,34 +1603,36 @@
         self.selected_params = list()
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
-        layout.addWidget(CheckList(
-            list(self.pd.ct.pr.parameters[self.pd.ct.pr.p_preset].keys()),
-            self.selected_params,
-            title='Select the Parameters to reset'))
-        reset_bt = QPushButton('Reset')
+        layout.addWidget(
+            CheckList(
+                list(self.pd.ct.pr.parameters[self.pd.ct.pr.p_preset].keys()),
+                self.selected_params,
+                title="Select the Parameters to reset",
+            )
+        )
+        reset_bt = QPushButton("Reset")
         reset_bt.clicked.connect(self.reset_params)
         layout.addWidget(reset_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def reset_params(self):
         for name in self.selected_params:
             self.pd.ct.pr.load_default_param(name)
-            print(f'Reset {name}')
-        WorkerDialog(self, self.pd.ct.pr.save, title='Saving project...',
-                     blocking=True)
+            print(f"Reset {name}")
+        WorkerDialog(self, self.pd.ct.pr.save, title="Saving project...", blocking=True)
         self.pd.update_all_param_guis()
         self.close()
 
 
 class CopyPDialog(QDialog):
     def __init__(self, p_dock):
         super().__init__(p_dock)
@@ -1617,152 +1659,149 @@
         self.copy_ps = CheckList(checked=self.selected_ps)
         list_layout.addWidget(self.copy_ps)
 
         layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
 
-        copy_bt = QPushButton('Copy')
+        copy_bt = QPushButton("Copy")
         copy_bt.clicked.connect(self.copy_parameters)
         bt_layout.addWidget(copy_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         bt_layout.addWidget(close_bt)
 
         layout.addLayout(bt_layout)
 
         self.setLayout(layout)
 
     def from_selected(self, current):
         self.selected_from = current
-        self.copy_to.replace_data(
-            [pp for pp in self.p.keys() if pp != current])
+        self.copy_to.replace_data([pp for pp in self.p.keys() if pp != current])
         self.copy_ps.replace_data([p for p in self.p[current]])
 
     def copy_parameters(self):
         if len(self.selected_to) > 0:
             for p_preset in self.selected_to:
                 for parameter in self.selected_ps:
-                    self.p[p_preset][parameter] = self.p[self.selected_from][
-                        parameter]
+                    self.p[p_preset][parameter] = self.p[self.selected_from][parameter]
 
-            WorkerDialog(self, self.pd.ct.pr.save, title='Saving project...',
-                         blocking=True)
+            WorkerDialog(
+                self, self.pd.ct.pr.save, title="Saving project...", blocking=True
+            )
             self.pd.update_all_param_guis()
             self.close()
 
 
 class RemovePPresetDlg(CheckListDlg):
     def __init__(self, parent):
         self.parent = parent
-        self.preset_list = [p for p in self.parent.ct.pr.parameters if
-                            p != 'Default']
+        self.preset_list = [p for p in self.parent.ct.pr.parameters if p != "Default"]
         self.rm_list = []
 
         super().__init__(parent, self.preset_list, self.rm_list)
 
-        self.do_bt.setText('Remove Parameter-Preset')
+        self.do_bt.setText("Remove Parameter-Preset")
         self.do_bt.clicked.connect(self.remove_selected)
 
         self.open()
 
     def remove_selected(self):
         for p_preset in self.rm_list:
             self.preset_list.remove(p_preset)
             self.lm.layoutChanged.emit()
             # Remove from Parameters
             self.parent.ct.pr.parameters.pop(p_preset)
             self.parent.update_ppreset_cmbx()
 
         # If current Parameter-Preset was deleted
         if self.parent.ct.pr.p_preset not in self.parent.ct.pr.parameters:
-            self.parent.ct.pr.p_preset = \
-                list(self.parent.ct.pr.parameters.keys())[0]
+            self.parent.ct.pr.p_preset = list(self.parent.ct.pr.parameters.keys())[0]
             self.parent.update_all_param_guis()
 
         self.close()
 
 
 class ParametersDock(QDockWidget):
     def __init__(self, main_win):
-        super().__init__('Parameters', main_win)
+        super().__init__("Parameters", main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.setAllowedAreas(Qt.RightDockWidgetArea)
         self.main_widget = QWidget()
         self.param_guis = {}
 
         self.dropgroup_params()
         self.init_ui()
 
     def dropgroup_params(self):
         # Create a set of all unique parameters used by functions
         # in selected_modules
         sel_pdfuncs = self.ct.pd_funcs.loc[
-            self.ct.pd_funcs['module'].isin(
-                self.ct.get_setting('selected_modules'))]
+            self.ct.pd_funcs["module"].isin(self.ct.get_setting("selected_modules"))
+        ]
         # Remove rows with NaN in func_args
-        sel_pdfuncs = sel_pdfuncs.loc[sel_pdfuncs['func_args'].notna()]
-        all_used_params_str = ','.join(sel_pdfuncs['func_args'])
+        sel_pdfuncs = sel_pdfuncs.loc[sel_pdfuncs["func_args"].notna()]
+        all_used_params_str = ",".join(sel_pdfuncs["func_args"])
         # Make sure there are no spaces left
-        all_used_params_str = all_used_params_str.replace(' ', '')
-        all_used_params = set(all_used_params_str.split(','))
+        all_used_params_str = all_used_params_str.replace(" ", "")
+        all_used_params = set(all_used_params_str.split(","))
         drop_idx_list = list()
         self.cleaned_pd_params = self.ct.pd_params.copy()
         for param in self.cleaned_pd_params.index:
             if param in all_used_params:
                 # Group-Name (if not given, set to 'Various')
-                group_name = self.cleaned_pd_params.loc[param, 'group']
+                group_name = self.cleaned_pd_params.loc[param, "group"]
                 if pd.isna(group_name):
-                    self.cleaned_pd_params.loc[param, 'group'] = 'Various'
+                    self.cleaned_pd_params.loc[param, "group"] = "Various"
             else:
                 # Drop Parameters which aren't used by functions
                 drop_idx_list.append(param)
         self.cleaned_pd_params.drop(index=drop_idx_list, inplace=True)
 
     def init_ui(self):
         self.general_layout = QVBoxLayout()
 
         # Add Parameter-Preset-ComboBox
         title_layouts = QVBoxLayout()
         title_layout1 = QHBoxLayout()
-        p_preset_l = QLabel('Parameter-Presets: ')
+        p_preset_l = QLabel("Parameter-Presets: ")
         title_layout1.addWidget(p_preset_l)
         self.p_preset_cmbx = QComboBox()
         self.p_preset_cmbx.setSizeAdjustPolicy(QComboBox.AdjustToContents)
         self.p_preset_cmbx.activated.connect(self.p_preset_changed)
         self.update_ppreset_cmbx()
         title_layout1.addWidget(self.p_preset_cmbx)
 
-        add_bt = QPushButton(icon=get_std_icon('SP_FileDialogNewFolder'))
+        add_bt = QPushButton(icon=get_std_icon("SP_FileDialogNewFolder"))
         add_bt.clicked.connect(self.add_p_preset)
         title_layout1.addWidget(add_bt)
 
-        rm_bt = QPushButton(icon=get_std_icon('SP_DialogDiscardButton'))
+        rm_bt = QPushButton(icon=get_std_icon("SP_DialogDiscardButton"))
         rm_bt.clicked.connect(partial(RemovePPresetDlg, self))
         title_layout1.addWidget(rm_bt)
 
         title_layouts.addLayout(title_layout1)
 
         title_layout2 = QHBoxLayout()
-        copy_bt = QPushButton('Copy')
-        copy_bt.setFont(QFont(QS().value('app_font'), 16))
+        copy_bt = QPushButton("Copy")
+        copy_bt.setFont(QFont(QS().value("app_font"), 16))
         copy_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         copy_bt.clicked.connect(partial(CopyPDialog, self))
         title_layout2.addWidget(copy_bt)
 
-        reset_bt = QPushButton('Reset')
-        reset_bt.setFont(QFont(QS().value('app_font'), 16))
+        reset_bt = QPushButton("Reset")
+        reset_bt.setFont(QFont(QS().value("app_font"), 16))
         reset_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         reset_bt.clicked.connect(partial(ResetDialog, self))
         title_layout2.addWidget(reset_bt)
 
-        reset_all_bt = QPushButton('Reset All')
-        reset_all_bt.setFont(QFont(QS().value('app_font'), 16))
+        reset_all_bt = QPushButton("Reset All")
+        reset_all_bt.setFont(QFont(QS().value("app_font"), 16))
         reset_all_bt.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         reset_all_bt.clicked.connect(self.reset_all_parameters)
         title_layout2.addWidget(reset_all_bt)
 
         title_layouts.addLayout(title_layout2)
         self.general_layout.addLayout(title_layouts)
 
@@ -1771,65 +1810,68 @@
         self.main_widget.setLayout(self.general_layout)
         self.setWidget(self.main_widget)
 
     def add_param_guis(self):
         # Create Tab-Widget for Parameters, grouped by group
         self.tab_param_widget = QTabWidget()
 
-        grouped_params = self.cleaned_pd_params.groupby('group', sort=False)
+        grouped_params = self.cleaned_pd_params.groupby("group", sort=False)
 
         for group_name, group in grouped_params:
             layout = QVBoxLayout()
             tab = QScrollArea()
             child_w = QWidget()
             for idx, parameter in group.iterrows():
-
                 # Get Parameters for Gui-Call
-                if pd.notna(parameter['alias']):
-                    alias = parameter['alias']
+                if pd.notna(parameter["alias"]):
+                    alias = parameter["alias"]
                 else:
                     alias = idx
-                if pd.notna(parameter['gui_type']):
-                    gui_name = parameter['gui_type']
+                if pd.notna(parameter["gui_type"]):
+                    gui_name = parameter["gui_type"]
                 else:
-                    gui_name = 'FuncGui'
+                    gui_name = "FuncGui"
                 try:
-                    default = literal_eval(parameter['default'])
+                    default = literal_eval(parameter["default"])
                 except (SyntaxError, ValueError):
-                    if gui_name == 'FuncGui':
-                        default = _eval_param(parameter['default'])
+                    if gui_name == "FuncGui":
+                        default = _eval_param(parameter["default"])
                     else:
-                        default = parameter['default']
-                if pd.notna(parameter['description']):
-                    description = parameter['description']
+                        default = parameter["default"]
+                if pd.notna(parameter["description"]):
+                    description = parameter["description"]
                 else:
-                    description = ''
-                if pd.notna(parameter['unit']):
-                    unit = parameter['unit']
+                    description = ""
+                if pd.notna(parameter["unit"]):
+                    unit = parameter["unit"]
                 else:
                     unit = None
                 try:
-                    gui_args = literal_eval(parameter['gui_args'])
+                    gui_args = literal_eval(parameter["gui_args"])
                 except (SyntaxError, ValueError):
                     gui_args = {}
 
                 try:
                     self.param_guis[idx] = globals()[gui_name](
                         data=self.ct,
                         name=idx,
                         alias=alias,
                         default=default,
                         description=description,
                         param_unit=unit,
-                        **gui_args)
-                except:  # noqa: E722
+                        **gui_args,
+                    )
+                except Exception:
                     err_tuple = get_exception_tuple()
                     raise RuntimeError(
-                        f'Initiliazation of Parameter-Widget "{idx}" failed:\n'
-                        f'{err_tuple[1]}')
+                        f'Initialization of Parameter-Widget "{idx}" '
+                        f"with value={default} "
+                        f"failed:\n"
+                        f"{err_tuple[1]}"
+                    )
 
                 layout.addWidget(self.param_guis[idx])
 
             child_w.setLayout(layout)
             tab.setWidget(child_w)
             self.tab_param_widget.addTab(tab, group_name)
 
@@ -1839,25 +1881,24 @@
     def update_ppreset_cmbx(self):
         self.p_preset_cmbx.clear()
         for p_preset in self.ct.pr.parameters.keys():
             self.p_preset_cmbx.addItem(p_preset)
         if self.ct.pr.p_preset in self.ct.pr.parameters.keys():
             self.p_preset_cmbx.setCurrentText(self.ct.pr.p_preset)
         else:
-            self.p_preset_cmbx.setCurrentText(
-                list(self.ct.pr.parameters.keys())[0])
+            self.p_preset_cmbx.setCurrentText(list(self.ct.pr.parameters.keys())[0])
 
     def p_preset_changed(self, idx):
         self.ct.pr.p_preset = self.p_preset_cmbx.itemText(idx)
         self.update_all_param_guis()
 
     def add_p_preset(self):
         preset_name = get_user_input_string(
-            'Enter a name for a new Parameter-Preset:',
-            'Add Parameter-Preset')
+            "Enter a name for a new Parameter-Preset:", "Add Parameter-Preset"
+        )
         if preset_name is not None:
             self.ct.pr.p_preset = preset_name
             self.ct.pr.load_default_parameters()
             self.p_preset_cmbx.addItem(preset_name)
             self.p_preset_cmbx.setCurrentText(preset_name)
 
     def redraw_param_widgets(self):
@@ -1871,157 +1912,156 @@
     def update_all_param_guis(self):
         for gui_name in self.param_guis:
             param_gui = self.param_guis[gui_name]
             param_gui.read_param()
             param_gui._set_param()
 
     def reset_all_parameters(self):
-        msgbox = QMessageBox.question(self, 'Reset all Parameters?',
-                                      'Do you really want to reset all '
-                                      'parameters to their default?',
-                                      QMessageBox.Yes | QMessageBox.No,
-                                      QMessageBox.No)
+        msgbox = QMessageBox.question(
+            self,
+            "Reset all Parameters?",
+            "Do you really want to reset all " "parameters to their default?",
+            QMessageBox.Yes | QMessageBox.No,
+            QMessageBox.No,
+        )
         if msgbox == QMessageBox.Yes:
             self.ct.pr.load_default_parameters()
             self.update_all_param_guis()
 
 
 class SettingsDlg(QDialog):
     def __init__(self, parent_widget, controller):
         super().__init__(parent_widget)
         self.ct = controller
 
         self.settings_items = {
-            'app_style': {
-                'gui_type': 'ComboGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'Application Style',
-                    'description': 'Changes the application style '
-                                   '(Restart required).',
-                    'options': ['light', 'dark'] + QStyleFactory().keys(),
-                }
+            "app_style": {
+                "gui_type": "ComboGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "Application Style",
+                    "description": "Changes the application style "
+                    "(Restart required).",
+                    "options": ["light", "dark", "auto"],
+                },
+            },
+            "app_font": {
+                "gui_type": "ComboGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "Application Font",
+                    "description": "Changes default application font "
+                    "(Restart required).",
+                    "options": QFontDatabase().families(QFontDatabase.Latin),
+                },
             },
-            'app_font': {
-                'gui_type': 'ComboGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'Application Font',
-                    'description': 'Changes default application font '
-                                   '(Restart required).',
-                    'options': QFontDatabase().families(QFontDatabase.Latin)
-                }
+            "app_font_size": {
+                "gui_type": "IntGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "Font Size",
+                    "description": "Changes default application font-size "
+                    "(Restart required).",
+                    "min_val": 5,
+                    "max_val": 20,
+                },
             },
-            'app_font_size': {
-                'gui_type': 'IntGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'Font Size',
-                    'description': 'Changes default application font-size '
-                                   '(Restart required).',
-                    'min_val': 5,
-                    'max_val': 20
-                }
+            "img_format": {
+                "gui_type": "ComboGui",
+                "data_type": "Settings",
+                "gui_kwargs": {
+                    "alias": "Image Format",
+                    "description": "Choose the image format for plots.",
+                    "options": [".png", ".jpg", ".tiff"],
+                },
             },
-            'img_format': {
-                'gui_type': 'ComboGui',
-                'data_type': 'Settings',
-                'gui_kwargs': {
-                    'alias': 'Image Format',
-                    'description': 'Choose the image format for plots.',
-                    'options': ['.png', '.jpg', '.tiff'],
-                }
+            "dpi": {
+                "gui_type": "IntGui",
+                "data_type": "Settings",
+                "gui_kwargs": {
+                    "alias": "DPI",
+                    "description": "Set dpi for saved plots.",
+                    "min_val": 10,
+                    "max_val": 5000,
+                },
             },
-            'dpi': {
-                'gui_type': 'IntGui',
-                'data_type': 'Settings',
-                'gui_kwargs': {
-                    'alias': 'DPI',
-                    'description': 'Set dpi for saved plots.',
-                    'min_val': 10,
-                    'max_val': 5000
-                }
+            "enable_cuda": {
+                "gui_type": "BoolGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "Enable CUDA",
+                    "description": "Enable for CUDA support "
+                    "(system has to be setup for cuda "
+                    "as in https://mne.tools/stable/install/"
+                    "advanced.html#gpu-acceleration-with-cuda)",
+                    "return_integer": True,
+                },
             },
-            'enable_cuda': {
-                'gui_type': 'BoolGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'Enable CUDA',
-                    'description': 'Enable for CUDA support '
-                                   '(system has to be setup for cuda '
-                                   'as in https://mne.tools/stable/install/'
-                                   'advanced.html#gpu-acceleration-with-cuda)',
-                    'return_integer': True
-                }
+            "save_ram": {
+                "gui_type": "BoolGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "Save RAM",
+                    "description": "Set to True on low RAM-Machines to avoid"
+                    " the process to be killed by the OS due "
+                    "to low Memory (with leaving it off, "
+                    "the pipeline goes a bit faster, because "
+                    "the data can be saved in memory).",
+                    "return_integer": True,
+                },
             },
-            'save_ram': {
-                'gui_type': 'BoolGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'Save RAM',
-                    'description': 'Set to True on low RAM-Machines to avoid'
-                                   ' the process to be killed by the OS due '
-                                   'to low Memory (with leaving it off, '
-                                   'the pipeline goes a bit faster, because '
-                                   'the data can be saved in memory).',
-                    'return_integer': True
-                }
+            "fs_path": {
+                "gui_type": "StringGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "FREESURFER_HOME-Path",
+                    "description": 'Set the Path to the "freesurfer"-directory'
+                    " of your Freesurfer-Installation "
+                    "(for Windows to the LINUX-Path of the "
+                    "Freesurfer-Installation in "
+                    "Windows-Subsystem for Linux(WSL))",
+                    "none_select": True,
+                },
             },
-            'fs_path': {
-                'gui_type': 'StringGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'FREESURFER_HOME-Path',
-                    'description': 'Set the Path to the "freesurfer"-directory'
-                                   ' of your Freesurfer-Installation '
-                                   '(for Windows to the LINUX-Path of the '
-                                   'Freesurfer-Installation in '
-                                   'Windows-Subsystem for Linux(WSL))',
-                    'none_select': True
-                }
+            "mne_path": {
+                "gui_type": "StringGui",
+                "data_type": "QSettings",
+                "gui_kwargs": {
+                    "alias": "MNE-WSL-Path",
+                    "description": "Set the LINUX-Path to the mne-environment "
+                    "(e.g ...anaconda3/envs/mne) in "
+                    "Windows-Subsystem for Linux(WSL))",
+                    "none_select": True,
+                },
             },
-            'mne_path': {
-                'gui_type': 'StringGui',
-                'data_type': 'QSettings',
-                'gui_kwargs': {
-                    'alias': 'MNE-WSL-Path',
-                    'description': 'Set the LINUX-Path to the mne-environment '
-                                   '(e.g ...anaconda3/envs/mne) in '
-                                   'Windows-Subsystem for Linux(WSL))',
-                    'none_select': True
-                }
-            }
         }
 
         if not iswin:
-            self.settings_items.pop('mne_path')
+            self.settings_items.pop("mne_path")
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         for setting in self.settings_items:
-            gui_handle = globals()[self.settings_items[setting]['gui_type']]
-            data_type = self.settings_items[setting]['data_type']
-            gui_kwargs = self.settings_items[setting]['gui_kwargs']
-            if data_type == 'QSettings':
-                gui_kwargs['data'] = QS()
-                gui_kwargs['default'] = self.ct.default_settings['qsettings'][
-                    setting]
-            elif data_type == 'Controller':
-                gui_kwargs['data'] = self.mw.ct
-                gui_kwargs['default'] = self.ct.pd_params.loc[
-                    setting, 'default']
-            else:
-                gui_kwargs['data'] = self.ct.settings
-                gui_kwargs['default'] = self.ct.default_settings['settings'][
-                    setting]
-            gui_kwargs['name'] = setting
+            gui_handle = globals()[self.settings_items[setting]["gui_type"]]
+            data_type = self.settings_items[setting]["data_type"]
+            gui_kwargs = self.settings_items[setting]["gui_kwargs"]
+            if data_type == "QSettings":
+                gui_kwargs["data"] = QS()
+                gui_kwargs["default"] = self.ct.default_settings["qsettings"][setting]
+            elif data_type == "Controller":
+                gui_kwargs["data"] = self.mw.ct
+                gui_kwargs["default"] = self.ct.pd_params.loc[setting, "default"]
+            else:
+                gui_kwargs["data"] = self.ct.settings
+                gui_kwargs["default"] = self.ct.default_settings["settings"][setting]
+            gui_kwargs["name"] = setting
             layout.addWidget(gui_handle(**gui_kwargs))
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/plot_widgets.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/plot_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 import logging
 from functools import partial
 from importlib import import_module
 from os.path import join, isfile
 
 from PyQt5.QtCore import Qt, QThreadPool
 from PyQt5.QtGui import QPixmap, QFont
-from PyQt5.QtWidgets import (QMainWindow, QWidget, QGridLayout, QComboBox,
-                             QTabWidget, QVBoxLayout, QDialog, QHBoxLayout,
-                             QCheckBox, QPushButton, QMessageBox,
-                             QProgressDialog, QLabel, QScrollArea, QToolBar,
-                             QSpinBox)
+from PyQt5.QtWidgets import (
+    QMainWindow,
+    QWidget,
+    QGridLayout,
+    QComboBox,
+    QTabWidget,
+    QVBoxLayout,
+    QDialog,
+    QHBoxLayout,
+    QCheckBox,
+    QPushButton,
+    QMessageBox,
+    QProgressDialog,
+    QLabel,
+    QScrollArea,
+    QToolBar,
+    QSpinBox,
+)
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
 from mne.viz import Brain
 from mne_qt_browser._pg_figure import MNEQtBrowser
 
 try:
@@ -84,50 +95,54 @@
             self.plots[name][func_name] = list()
             self.func_list.model._data.append(func_name)
             self.func_list.content_changed()
 
         for subplot in plot:
             if isinstance(subplot, Figure):
                 plot_widget = FigureCanvasQTAgg(subplot)
-                plot_widget.setFocusPolicy(Qt.FocusPolicy(Qt.StrongFocus |
-                                                          Qt.WheelFocus))
+                plot_widget.setFocusPolicy(
+                    Qt.FocusPolicy(Qt.StrongFocus | Qt.WheelFocus)
+                )
                 plot_widget.setFocus()
             elif isinstance(subplot, MNEQtBrowser):
                 plot_widget = subplot
             elif isinstance(subplot, Brain):
                 plot_widget = subplot
             elif isinstance(subplot, Figure3D):
                 plot_widget = subplot
             else:
-                logging.error(f'Unrecognized type "{type(subplot)}" '
-                              f'for "{func_name}"')
+                logging.error(
+                    f'Unrecognized type "{type(subplot)}" ' f'for "{func_name}"'
+                )
                 plot_widget = QWidget()
 
             self.plots[name][func_name].append(plot_widget)
 
-            if self.name_cmbx.currentText() == name \
-                    and self.func_list.get_current() == func_name:
+            if (
+                self.name_cmbx.currentText() == name
+                and self.func_list.get_current() == func_name
+            ):
                 self.update_plots(only_add=True)
 
     def closeEvent(self, event):
-        _object_refs['plot_manager'] = None
+        _object_refs["plot_manager"] = None
         event.accept()
 
 
 def show_plot_manager():
-    if _object_refs['plot_manager'] is None:
+    if _object_refs["plot_manager"] is None:
         plot_manager = PlotManager()
-        _object_refs['plot_manager'] = plot_manager
+        _object_refs["plot_manager"] = plot_manager
 
-    return _object_refs['plot_manager']
+    return _object_refs["plot_manager"]
 
 
 class PlotViewSelection(QDialog):
     """The user selects the plot-function and the objects
-     to show for this plot_function
+    to show for this plot_function
     """
 
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
 
@@ -147,206 +162,215 @@
         self.init_ui()
         self.show()
 
     def init_ui(self):
         layout = QVBoxLayout()
         list_layout = QHBoxLayout()
 
-        func_list = \
-            self.ct.pd_funcs[self.ct.pd_funcs['matplotlib']
-                             | self.ct.pd_funcs['mayavi']].index
-        func_select = SimpleList(func_list, title='Select Plot-Function')
+        func_list = self.ct.pd_funcs[
+            self.ct.pd_funcs["matplotlib"] | self.ct.pd_funcs["mayavi"]
+        ].index
+        func_select = SimpleList(func_list, title="Select Plot-Function")
         func_select.currentChanged.connect(self.func_selected)
         list_layout.addWidget(func_select)
 
-        self.p_preset_select = CheckList(list(self.ct.pr.parameters.keys()),
-                                         self.selected_ppresets,
-                                         title='Select Parameter-Preset')
+        self.p_preset_select = CheckList(
+            list(self.ct.pr.parameters.keys()),
+            self.selected_ppresets,
+            title="Select Parameter-Preset",
+        )
         self.p_preset_select.checkedChanged.connect(self.update_objects)
         list_layout.addWidget(self.p_preset_select)
 
-        self.obj_select = CheckList(data=self.objects,
-                                    checked=self.selected_objs,
-                                    title='Select Objects')
+        self.obj_select = CheckList(
+            data=self.objects, checked=self.selected_objs, title="Select Objects"
+        )
         list_layout.addWidget(self.obj_select)
 
         layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
         # Interactive not useful at the moment
         # because the plots loose interactivity when coming from the thread
-        self.interactive_chkbx = QCheckBox('Interactive Plots?')
+        self.interactive_chkbx = QCheckBox("Interactive Plots?")
         self.interactive_chkbx.toggled.connect(self.interactive_toggled)
         # bt_layout.addWidget(self.interactive_chkbx)
 
-        start_bt = QPushButton('Start')
+        start_bt = QPushButton("Start")
         start_bt.clicked.connect(self.load_plots)
         bt_layout.addWidget(start_bt)
 
-        cancel_bt = QPushButton('Cancel')
+        cancel_bt = QPushButton("Cancel")
         cancel_bt.clicked.connect(self.close)
         bt_layout.addWidget(cancel_bt)
 
         layout.addLayout(bt_layout)
         self.setLayout(layout)
 
     def update_objects(self):
         self.objects.clear()
         if self.selected_func is not None and self.target is not None:
             # Load object-list according to target
-            if self.target == 'MEEG':
+            if self.target == "MEEG":
                 target_objects = self.ct.pr.all_meeg
-            elif self.target == 'FSMRI':
+            elif self.target == "FSMRI":
                 target_objects = self.ct.pr.all_fsmri
-            elif self.target == 'Group':
+            elif self.target == "Group":
                 target_objects = list(self.ct.pr.all_groups.keys())
             else:
                 target_objects = list()
 
             # If non-interactive only list objects
             # where a plot-image already was saved
             if not self.interactive:
                 for ob in target_objects:
                     if ob in self.ct.pr.plot_files:
                         for p_preset in self.selected_ppresets:
                             if p_preset in self.ct.pr.plot_files[ob]:
-                                if self.selected_func in \
-                                        self.ct.pr.plot_files[ob][p_preset]:
+                                if (
+                                    self.selected_func
+                                    in self.ct.pr.plot_files[ob][p_preset]
+                                ):
                                     if ob not in self.objects:
                                         self.objects.append(ob)
             else:
                 self.objects = target_objects
 
         self.obj_select.replace_data(self.objects)
 
     def func_selected(self, func):
         """Get selected function and adjust contents
         of Object-Selection to target"""
         self.selected_func = func
-        self.target = self.ct.pd_funcs.loc[func, 'target']
+        self.target = self.ct.pd_funcs.loc[func, "target"]
         self.update_objects()
 
     def interactive_toggled(self, checked):
         self.interactive = checked
         self.update_objects()
 
     def load_plots(self):
         # Clear previous dictionaries
         self.all_images.clear()
         self.all_figs.clear()
 
         # Show ProgressBar
-        self.total_loads = len(self.selected_objs) * len(
-            self.selected_ppresets)
+        self.total_loads = len(self.selected_objs) * len(self.selected_ppresets)
         if self.total_loads == 0:
-            QMessageBox.warning(self, 'Not enought selected!',
-                                'An important parameter seems to be missing')
+            QMessageBox.warning(
+                self,
+                "Not enought selected!",
+                "An important parameter seems to be missing",
+            )
         else:
             self.prog_dlg = QProgressDialog()
-            self.prog_dlg.setLabelText('Loading Plots...')
+            self.prog_dlg.setLabelText("Loading Plots...")
             self.prog_dlg.setMaximum(self.total_loads)
             self.prog_dlg.setCancelButton(None)
             self.prog_dlg.setMinimumDuration(0)
             self.prog_cnt = 0
             self.prog_dlg.setValue(self.prog_cnt)
 
             for p_preset in self.selected_ppresets:
                 self.all_images[p_preset] = dict()
                 self.all_figs[p_preset] = dict()
                 for obj_name in self.selected_objs:
-                    if self.target == 'MEEG':
+                    if self.target == "MEEG":
                         obj = MEEG(obj_name, self.ct)
-                    elif self.target == 'FSMRI':
+                    elif self.target == "FSMRI":
                         obj = FSMRI(obj_name, self.ct)
-                    elif self.target == 'Group':
+                    elif self.target == "Group":
                         obj = Group(obj_name, self.ct)
                     else:
                         break
 
                     # Replace Parameter-Preset for the loaded object
                     # and reload load/save-paths
                     if p_preset != obj.p_preset:
                         obj.p_preset = p_preset
                         obj.init_parameters()
                         obj.init_paths()
 
                     # Load Matplotlib-Plots
                     if self.interactive_chkbx.isChecked():
                         # Get module of plot_function
-                        module_name = self.ct.pd_funcs.loc[
-                            self.selected_func, 'module']
+                        module_name = self.ct.pd_funcs.loc[self.selected_func, "module"]
                         module = import_module(module_name)
                         plot_func = getattr(module, self.selected_func)
 
                         # Get Arguments for Plot-Function
                         keyword_arguments = get_arguments(plot_func, obj)
                         # Make sure that "show_plots" is False
-                        keyword_arguments['show_plots'] = False
+                        keyword_arguments["show_plots"] = False
 
                         # Create Thread for Plot-Function
                         worker = Worker(plot_func, **keyword_arguments)
 
                         # Pass Object-Name into the plot_finished-Slot
                         # (needs to be set as default
                         # in lambda-function to survive loop)
 
-                        def finished_func(val, o_name=obj_name,
-                                          ppreset=p_preset):
+                        def finished_func(val, o_name=obj_name, ppreset=p_preset):
                             self.plot_finished(val, o_name, ppreset)
 
                         worker.signals.finished.connect(finished_func)
 
-                        def error_func(err_tuple, o_name=obj_name,
-                                       ppreset=p_preset):
-                            self.thread_error(err_tuple, o_name, ppreset,
-                                              'plot')
+                        def error_func(err_tuple, o_name=obj_name, ppreset=p_preset):
+                            self.thread_error(err_tuple, o_name, ppreset, "plot")
 
                         worker.signals.error.connect(error_func)
-                        print(f'Starting Thread for Object= {obj_name} '
-                              f'and Parameter-Preset= {p_preset}')
+                        print(
+                            f"Starting Thread for Object= {obj_name} "
+                            f"and Parameter-Preset= {p_preset}"
+                        )
                         QThreadPool.globalInstance().start(worker)
 
                     # Load Plot-Images
                     else:
                         try:
-                            image_paths = [join(obj.figures_path, p) for p in
-                                           obj.plot_files[self.selected_func]]
+                            image_paths = [
+                                join(obj.figures_path, p)
+                                for p in obj.plot_files[self.selected_func]
+                            ]
                         except KeyError as ke:
                             self.all_images[p_preset][
-                                obj_name] = f'{ke} not found for {obj_name}'
+                                obj_name
+                            ] = f"{ke} not found for {obj_name}"
                             self.thread_finished(None)
                         else:
                             # Load pixmaps from Image-Paths
                             pixmaps = list()
 
                             for image_path in image_paths:
                                 if isfile(image_path):
                                     pixmap = QPixmap(image_path)
                                     pixmaps.append(pixmap)
 
                             self.all_images[p_preset][obj_name] = pixmaps
 
                             self.thread_finished(None)
 
-    def thread_finished(self, _, ):
+    def thread_finished(
+        self,
+        _,
+    ):
         self.prog_cnt += 1
         self.prog_dlg.setValue(self.prog_cnt)
 
         if self.prog_cnt == self.total_loads:
             # Start PlotViewer
             interactive = self.interactive_chkbx.isChecked()
             if interactive:
                 items = self.all_figs
             else:
                 items = self.all_images
             PlotViewer(self, items, interactive, True)
             self.hide()
 
     def plot_finished(self, return_value, obj_name, p_preset):
-
         # Check if multiple figures are given
         if not isinstance(return_value, list):
             # Make sure, that return_value is a list
             return_value = [return_value]
 
         fig_list = list()
         for fig in return_value:
@@ -354,20 +378,18 @@
             fig_list.append((fig, fig.get_size_inches()))
 
         self.all_figs[p_preset][obj_name] = fig_list
 
         self.thread_finished(None)
 
     def thread_error(self, error_tuple, obj_name, p_preset, kind):
-        if kind == 'image':
-            self.all_images[p_preset][
-                obj_name] = f'{error_tuple[0]}: {error_tuple[1]}'
+        if kind == "image":
+            self.all_images[p_preset][obj_name] = f"{error_tuple[0]}: {error_tuple[1]}"
         else:
-            self.all_figs[p_preset][
-                obj_name] = f'{error_tuple[0]}: {error_tuple[1]}'
+            self.all_figs[p_preset][obj_name] = f"{error_tuple[0]}: {error_tuple[1]}"
 
         self.thread_finished(None)
 
     def closeEvent(self, event):
         for p_preset in self.all_figs:
             for obj_name in self.all_figs[p_preset]:
                 for fig_tuple in self.all_figs[p_preset][obj_name]:
@@ -391,118 +413,114 @@
     def _setup_views(self):
         viewer_layout = QHBoxLayout()
 
         # Get the figures/images
         for p_preset in self.items:
             p_preset_layout = QVBoxLayout()
             p_preset_label = QLabel(p_preset)
-            p_preset_label.setFont(QFont('AnyStlye', 16, QFont.Bold))
-            p_preset_layout.addWidget(p_preset_label,
-                                      alignment=Qt.AlignHCenter)
+            p_preset_label.setFont(QFont("AnyStlye", 16, QFont.Bold))
+            p_preset_layout.addWidget(p_preset_label, alignment=Qt.AlignHCenter)
 
             scroll_area = QScrollArea()
             scroll_widget = QWidget()
             scroll_layout = QGridLayout()
 
             for obj_idx, obj_name in enumerate(self.items[p_preset]):
                 obj_items = self.items[p_preset][obj_name]
                 row = obj_idx // self.column_count
                 col = obj_idx % self.column_count
 
                 # Add name-label
                 name_label = QLabel(str(obj_name))
-                name_label.setFont(QFont('AnyType', 14))
+                name_label.setFont(QFont("AnyType", 14))
 
                 if isinstance(obj_items, str):
                     # This displays errors
                     error_layout = QVBoxLayout()
-                    error_layout.addWidget(name_label,
-                                           alignment=Qt.AlignHCenter)
+                    error_layout.addWidget(name_label, alignment=Qt.AlignHCenter)
                     error_layout.addWidget(QLabel(obj_items))
                     scroll_layout.addLayout(error_layout, row, col)
 
                 elif isinstance(obj_items, list):
                     tab_widget = QTabWidget()
                     obj_layout = QVBoxLayout()
                     for item_idx, item in enumerate(obj_items):
                         if self.interactive:
                             fig, default_size = item
                             # Zoom Figure
-                            fig.set_size_inches(
-                                default_size * (self.zoom_factor / 100))
+                            fig.set_size_inches(default_size * (self.zoom_factor / 100))
                             view_widget = FigureCanvasQTAgg(fig)
                         else:
                             view_widget = QLabel()
                             # Zoom Pixmap
                             view_widget.setPixmap(
                                 item.scaled(
                                     item.size() * (self.zoom_factor / 100),
                                     Qt.KeepAspectRatio,
-                                    Qt.SmoothTransformation))
+                                    Qt.SmoothTransformation,
+                                )
+                            )
 
                         if len(obj_items) > 1:
                             tab_widget.addTab(view_widget, str(item_idx))
                         else:
-                            obj_layout.addWidget(name_label,
-                                                 alignment=Qt.AlignHCenter)
+                            obj_layout.addWidget(name_label, alignment=Qt.AlignHCenter)
                             # Add view-widget if not enough items
                             # for Tab-Widget
                             obj_layout.addWidget(view_widget)
                             scroll_layout.addLayout(obj_layout, row, col)
 
                     if len(obj_items) > 1:
                         frame_widget = QWidget()
                         frame_layout = QVBoxLayout()
-                        frame_layout.addWidget(name_label,
-                                               alignment=Qt.AlignHCenter)
+                        frame_layout.addWidget(name_label, alignment=Qt.AlignHCenter)
                         frame_layout.addWidget(tab_widget)
-                        show_bt = QPushButton('Show')
+                        show_bt = QPushButton("Show")
                         show_bt.clicked.connect(
-                            partial(self.show_single_items, p_preset,
-                                    obj_name))
+                            partial(self.show_single_items, p_preset, obj_name)
+                        )
                         frame_layout.addWidget(show_bt)
                         frame_widget.setLayout(frame_layout)
                         scroll_layout.addWidget(frame_widget, row, col)
 
             scroll_widget.setLayout(scroll_layout)
             scroll_area.setWidget(scroll_widget)
             p_preset_layout.addWidget(scroll_area)
 
             viewer_layout.addLayout(p_preset_layout)
 
         self.main_layout.addLayout(viewer_layout)
 
     def init_ui(self):
-
-        toolbar = QToolBar('Plot-Tools')
+        toolbar = QToolBar("Plot-Tools")
         self.addToolBar(toolbar)
 
         # Zoom-Control
-        toolbar.addAction('-- Zoom', partial(self.zoom_items, '--'))
-        toolbar.addAction('- Zoom', partial(self.zoom_items, '-'))
-        self.zoom_label = QLabel(f'{self.zoom_factor} %')
+        toolbar.addAction("-- Zoom", partial(self.zoom_items, "--"))
+        toolbar.addAction("- Zoom", partial(self.zoom_items, "-"))
+        self.zoom_label = QLabel(f"{self.zoom_factor} %")
         toolbar.addWidget(self.zoom_label)
-        toolbar.addAction('+ Zoom', partial(self.zoom_items, '+'))
-        toolbar.addAction('++ Zoom', partial(self.zoom_items, '++'))
+        toolbar.addAction("+ Zoom", partial(self.zoom_items, "+"))
+        toolbar.addAction("++ Zoom", partial(self.zoom_items, "++"))
 
         # Column-Control
-        toolbar.addAction('- Column', partial(self.change_columns, '-'))
-        self.column_label = QLabel(f'{self.column_count} Columns')
+        toolbar.addAction("- Column", partial(self.change_columns, "-"))
+        self.column_label = QLabel(f"{self.column_count} Columns")
         toolbar.addWidget(self.column_label)
-        toolbar.addAction('+ Column', partial(self.change_columns, '+'))
+        toolbar.addAction("+ Column", partial(self.change_columns, "+"))
 
         # Add control for all tab-widgets to turn all to selected tab(index)
-        tab_sel_label = QLabel('Select Tab')
+        tab_sel_label = QLabel("Select Tab")
         toolbar.addWidget(tab_sel_label)
         tab_selection = QSpinBox()
         tab_selection.valueChanged.connect(self.tab_selected)
         tab_selection.setWrapping(True)
         toolbar.addWidget(tab_selection)
 
-        toolbar.addAction('Close', self.close)
+        toolbar.addAction("Close", self.close)
 
         # Central Widget
         widget = QWidget()
         self.main_layout = QVBoxLayout()
 
         self._setup_views()
 
@@ -519,70 +537,69 @@
         for n in range(viewer_layout.count()):
             scroll_area = viewer_layout.itemAt(n).itemAt(1).widget()
             grid_layout = scroll_area.widget().layout()
             for c in range(grid_layout.count()):
                 row = c // self.column_count
                 col = c % self.column_count
                 item_widget = grid_layout.itemAtPosition(row, col).widget()
-                if not isinstance(item_widget,
-                                  QLabel) and item_widget is not None:
+                if not isinstance(item_widget, QLabel) and item_widget is not None:
                     tab_widget = item_widget.layout().itemAt(1).widget()
                     tab_widget.setCurrentIndex(idx)
 
     def update_layout(self):
         old_layout = self.main_layout.itemAt(0)
         self.main_layout.removeItem(old_layout)
-        for p_preset_layout in [old_layout.itemAt(idx).layout() for idx in
-                                range(old_layout.count())]:
+        for p_preset_layout in [
+            old_layout.itemAt(idx).layout() for idx in range(old_layout.count())
+        ]:
             title_label = p_preset_layout.itemAt(0).widget()
             title_label.deleteLater()
             scroll_area = p_preset_layout.itemAt(1).widget()
             scroll_area.deleteLater()
         del old_layout
 
         self._setup_views()
 
     def change_columns(self, direction):
         # Set Column-Count
-        if direction == '+':
+        if direction == "+":
             self.column_count += 1
         else:
             self.column_count -= 1
 
         # Make sure, that at least one column is shown
         if self.column_count < 1:
             self.column_count = 1
 
-        self.column_label.setText(f'{self.column_count} Columns')
+        self.column_label.setText(f"{self.column_count} Columns")
         self.update_layout()
 
     def zoom_items(self, zoom):
         # Zoom-Labels
-        if zoom == '+':
+        if zoom == "+":
             self.zoom_factor += 10
-        elif zoom == '++':
+        elif zoom == "++":
             self.zoom_factor += 50
-        elif zoom == '-':
+        elif zoom == "-":
             self.zoom_factor -= 10
         else:
             self.zoom_factor -= 50
 
         # Make sure, that zoom is not smaller than 10%
         if self.zoom_factor < 10:
             self.zoom_factor = 10
 
-        self.zoom_label.setText(f'{self.zoom_factor} %')
+        self.zoom_label.setText(f"{self.zoom_factor} %")
         self.update_layout()
 
     def show_single_items(self, p_preset, obj_name):
         # Create dictionary similar to what you get from loading
         # to open a new viewer with just the selected items
         obj_items = [item.copy() for item in self.items[p_preset][obj_name]]
-        item_dict = {
-            'Default': {idx: [value] for idx, value in enumerate(obj_items)}}
+        item_dict = {"Default": {idx: [value] for idx, value in enumerate(obj_items)}}
         PlotViewer(self, item_dict, self.interactive, False)
 
     def closeEvent(self, event):
         if self.top_level:
             self.parent().show()
 
         event.accept()
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/tools.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from functools import partial
 
 from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (QComboBox, QDialog, QGridLayout,
-                             QHBoxLayout, QPushButton,
-                             QSizePolicy, QVBoxLayout)
+from PyQt5.QtWidgets import (
+    QComboBox,
+    QDialog,
+    QGridLayout,
+    QHBoxLayout,
+    QPushButton,
+    QSizePolicy,
+    QVBoxLayout,
+)
 
 from mne_pipeline_hd.gui.base_widgets import CheckList
-from mne_pipeline_hd.gui.gui_utils import (CodeEditor, MainConsoleWidget,
-                                           WorkerDialog, get_exception_tuple,
-                                           set_ratio_geometry)
+from mne_pipeline_hd.gui.gui_utils import (
+    CodeEditor,
+    MainConsoleWidget,
+    WorkerDialog,
+    get_exception_tuple,
+    set_ratio_geometry,
+)
 from mne_pipeline_hd.pipeline.loading import MEEG
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class HistoryDlg(QDialog):
     def __init__(self, dt):
         super().__init__(dt)
@@ -34,19 +42,19 @@
     def init_ui(self):
         layout = QVBoxLayout()
 
         self.checklist = CheckList(self.dt.history, self.checked)
 
         layout.addWidget(self.checklist)
 
-        add_bt = QPushButton('Add')
+        add_bt = QPushButton("Add")
         add_bt.clicked.connect(self.add_cmds)
         layout.addWidget(add_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt)
 
         self.setLayout(layout)
 
     def add_cmds(self):
         for item in self.checked:
@@ -62,46 +70,58 @@
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
 
         self.obj = current_object
         self.history = list()
 
-        self.default_t_globals = ['mw', 'main_window', 'ct', 'controller',
-                                  'pr', 'project', 'par', 'parameters']
-
-        self.t_globals = {'mw': self.mw,
-                          'main_window': self.mw,
-                          'ct': self.ct,
-                          'controller': self.ct,
-                          'pr': self.pr,
-                          'project': self.pr,
-                          'par': self.pr.parameters,
-                          'parameters': self.pr.parameters}
+        self.default_t_globals = [
+            "mw",
+            "main_window",
+            "ct",
+            "controller",
+            "pr",
+            "project",
+            "par",
+            "parameters",
+        ]
+
+        self.t_globals = {
+            "mw": self.mw,
+            "main_window": self.mw,
+            "ct": self.ct,
+            "controller": self.ct,
+            "pr": self.pr,
+            "project": self.pr,
+            "par": self.pr.parameters,
+            "parameters": self.pr.parameters,
+        }
 
         # Load the subject in globals if given in Class-Call
         if self.obj:
-            self.t_globals['obj'] = self.obj
+            self.t_globals["obj"] = self.obj
 
         self.bt_dict = {}
 
-        self.load_mapping = {'info': 'load_info',
-                             'raw': 'load_raw',
-                             'filtered': 'load_filtered',
-                             'events': 'load_events',
-                             'epochs': 'load_epochs',
-                             'evokeds': 'load_evokeds',
-                             'ica': 'load_ica',
-                             'tfr_epochs': 'load_power_tfr_epochs',
-                             'tfr_average': 'load_power_tfr_average',
-                             'trans': 'load_transformation',
-                             'forward': 'load_forward',
-                             'noise_cov': 'load_noise_covariance',
-                             'inv_op': 'load_inverse_operator',
-                             'stc': 'load_source_estimates'}
+        self.load_mapping = {
+            "info": "load_info",
+            "raw": "load_raw",
+            "filtered": "load_filtered",
+            "events": "load_events",
+            "epochs": "load_epochs",
+            "evokeds": "load_evokeds",
+            "ica": "load_ica",
+            "tfr_epochs": "load_power_tfr_epochs",
+            "tfr_average": "load_power_tfr_average",
+            "trans": "load_transformation",
+            "forward": "load_forward",
+            "noise_cov": "load_noise_covariance",
+            "inv_op": "load_inverse_operator",
+            "stc": "load_source_estimates",
+        }
 
         # sys.stdout.signal.text_written.connect(self.update_label)
 
         set_ratio_geometry(0.7, self)
 
         self.init_ui()
         self.show()
@@ -131,36 +151,40 @@
         self.layout.addLayout(bt_layout)
 
         self.displayw = MainConsoleWidget()
         self.layout.addWidget(self.displayw)
 
         self.sub_layout = QGridLayout()
         self.inputw = CodeEditor()
-        self.inputw.setSizePolicy(QSizePolicy(QSizePolicy.Preferred,
-                                              QSizePolicy.Maximum))
+        self.inputw.setSizePolicy(
+            QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
+        )
         self.sub_layout.addWidget(self.inputw, 0, 0, 3, 1)
 
-        self.start_bt = QPushButton('Start')
-        self.start_bt.setFont(QFont(QS().value('app_font'), 16))
-        self.start_bt.setSizePolicy(QSizePolicy(QSizePolicy.Maximum,
-                                                QSizePolicy.Preferred))
+        self.start_bt = QPushButton("Start")
+        self.start_bt.setFont(QFont(QS().value("app_font"), 16))
+        self.start_bt.setSizePolicy(
+            QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
+        )
         self.start_bt.clicked.connect(self.start_execution)
         self.sub_layout.addWidget(self.start_bt, 0, 1)
 
-        self.history_bt = QPushButton('History')
-        self.history_bt.setFont(QFont(QS().value('app_font'), 16))
-        self.history_bt.setSizePolicy(QSizePolicy(QSizePolicy.Maximum,
-                                                  QSizePolicy.Preferred))
+        self.history_bt = QPushButton("History")
+        self.history_bt.setFont(QFont(QS().value("app_font"), 16))
+        self.history_bt.setSizePolicy(
+            QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
+        )
         self.history_bt.clicked.connect(partial(HistoryDlg, self))
         self.sub_layout.addWidget(self.history_bt, 1, 1)
 
-        self.quit_bt = QPushButton('Close')
-        self.quit_bt.setFont(QFont(QS().value('app_font'), 16))
-        self.quit_bt.setSizePolicy(QSizePolicy(QSizePolicy.Maximum,
-                                               QSizePolicy.Preferred))
+        self.quit_bt = QPushButton("Close")
+        self.quit_bt.setFont(QFont(QS().value("app_font"), 16))
+        self.quit_bt.setSizePolicy(
+            QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Preferred)
+        )
         self.quit_bt.clicked.connect(self.close)
         self.sub_layout.addWidget(self.quit_bt, 2, 1)
 
         self.layout.addLayout(self.sub_layout)
 
         self.setLayout(self.layout)
 
@@ -170,70 +194,71 @@
         if self.obj is None:
             for bt_name in self.bt_dict:
                 self.bt_dict[bt_name].setEnabled(True)
 
         name = self.sub_cmbx.itemText(index)
         try:
             self.obj = MEEG(name, self.ct)
-        except:  # noqa: E722
+        except Exception:
             get_exception_tuple()
             # Return ComboBox to previous state
             if self.obj is None:
                 self.sub_cmbx.setCurrentIndex(-1)
             else:
                 self.sub_cmbx.setCurrentText(self.obj.name)
         else:
             # Reset globals to default
-            for key in [k for k in self.t_globals.keys()
-                        if k not in self.default_t_globals]:
+            for key in [
+                k for k in self.t_globals.keys() if k not in self.default_t_globals
+            ]:
                 self.t_globals.pop(key)
-            self.t_globals['obj'] = self.obj
-            self.displayw.insertHtml(
-                f'<b>Subject: {self.obj.name} loaded</b><br>')
+            self.t_globals["obj"] = self.obj
+            self.displayw.insertHtml(f"<b>Subject: {self.obj.name} loaded</b><br>")
             self.displayw.ensureCursorVisible()
 
     def load_bt_pressed(self, bt_name):
         worker_dialog = WorkerDialog(
-            self, self.start_load, title=f'Loading {bt_name}...',
-            bt_name=bt_name)
+            self, self.start_load, title=f"Loading {bt_name}...", bt_name=bt_name
+        )
         worker_dialog.thread_finished.connect(self.finished_handling)
 
     def finished_handling(self, result_msg):
         if isinstance(result_msg, str):
             self.displayw.insertHtml(result_msg)
             self.displayw.ensureCursorVisible()
 
     def start_load(self, bt_name):
         try:
             load_fn = getattr(self.obj, self.load_mapping[bt_name])
             self.t_globals[bt_name] = load_fn()
-        except (FileNotFoundError, OSError):
-            result_msg = \
-                f'<b><center>No file found for {bt_name}</center></b><br>'
+        except OSError:
+            result_msg = f"<b><center>No file found for {bt_name}</center></b><br>"
         else:
-            result_msg = \
-                f'<b><big><center>{bt_name} loaded ' \
-                f'(namespace = {bt_name})</center></big></b><br>'
+            result_msg = (
+                f"<b><big><center>{bt_name} loaded "
+                f"(namespace = {bt_name})</center></big></b><br>"
+            )
 
         return result_msg
 
     def start_execution(self):
         command = self.inputw.toPlainText()
-        command_html = command.replace('\n', '<br>')
+        command_html = command.replace("\n", "<br>")
         self.displayw.insertHtml(
-            f'<font color="blue"><b><i>{command_html}</i></b></font><br>')
+            f'<font color="blue"><b><i>{command_html}</i></b></font><br>'
+        )
         self.displayw.ensureCursorVisible()
         self.history.insert(0, command)
 
         try:
             print(eval(command, self.t_globals))
         except SyntaxError:
             try:
                 exec(command, self.t_globals)
-            except:  # noqa: E722
+            except Exception:
                 get_exception_tuple()
             else:
                 self.inputw.clear()
-        except:  # noqa: E722
+        except Exception:
             get_exception_tuple()
         else:
             self.inputw.clear()
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/gui/welcome_window.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/welcome_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from importlib import resources
 from os import listdir
 from os.path import isdir, join
 
 from PyQt5.QtCore import Qt
 from PyQt5.QtGui import QFont, QPixmap
-from PyQt5.QtWidgets import (QComboBox, QFileDialog, QGroupBox, QHBoxLayout,
-                             QLabel, QPushButton, QVBoxLayout,
-                             QWidget)
+from PyQt5.QtWidgets import (
+    QComboBox,
+    QFileDialog,
+    QGroupBox,
+    QHBoxLayout,
+    QLabel,
+    QPushButton,
+    QVBoxLayout,
+    QWidget,
+)
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.gui.base_widgets import SimpleList
-from mne_pipeline_hd.gui.gui_utils import (center, WorkerDialog,
-                                           get_user_input_string)
+from mne_pipeline_hd.gui.gui_utils import center, WorkerDialog, \
+    get_user_input_string
 from mne_pipeline_hd.gui.main_window import MainWindow
 from mne_pipeline_hd.pipeline.controller import Controller
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class WelcomeWindow(QWidget):
     def __init__(self, controller=None):
         super().__init__()
-        _object_refs['welcome_window'] = self
+        _object_refs["welcome_window"] = self
         if controller is None:
             try:
                 self.ct = Controller()
             except RuntimeError:
                 self.ct = None
         else:
             self.ct = controller
@@ -42,100 +47,101 @@
         self.update_widgets()
 
         self.show()
         center(self)
 
     def init_ui(self):
         layout = QVBoxLayout()
-        title_label = QLabel('Welcome to MNE-Pipeline!')
-        title_label.setFont(QFont(QS().value('app_font'), 20))
+        title_label = QLabel("Welcome to MNE-Pipeline!")
+        title_label.setFont(QFont(QS().value("app_font"), 20))
         layout.addWidget(title_label)
 
         image_label = QLabel()
-        with resources.path('mne_pipeline_hd.resource',
-                            'mne_pipeline_logo_evee_smaller.jpg') as img_path:
+        with resources.path(
+            "mne_pipeline_hd.resource", "mne_pipeline_logo_evee_smaller.jpg"
+        ) as img_path:
             image_label.setPixmap(QPixmap(str(img_path)))
         layout.addWidget(image_label)
 
         home_layout = QHBoxLayout()
         self.home_path_label = QLabel()
         home_layout.addWidget(self.home_path_label, stretch=4)
-        self.home_path_bt = QPushButton('Set Home-Folder')
+        self.home_path_bt = QPushButton("Set Home-Folder")
         self.home_path_bt.clicked.connect(self.set_home_path)
         home_layout.addWidget(self.home_path_bt, alignment=Qt.AlignRight)
         layout.addLayout(home_layout)
 
         project_layout = QHBoxLayout()
         self.project_label = QLabel()
         project_layout.addWidget(self.project_label)
         self.project_cmbx = QComboBox()
         self.project_cmbx.activated.connect(self.project_changed)
 
         project_layout.addWidget(self.project_cmbx)
-        self.add_pr_bt = QPushButton('Add Project')
+        self.add_pr_bt = QPushButton("Add Project")
         self.add_pr_bt.clicked.connect(self.add_project)
         project_layout.addWidget(self.add_pr_bt, alignment=Qt.AlignRight)
         layout.addLayout(project_layout)
 
-        self.edu_groupbox = QGroupBox('Education')
+        self.edu_groupbox = QGroupBox("Education")
         self.edu_groupbox.setCheckable(True)
-        self.edu_groupbox.setChecked(QS().value('education',
-                                                defaultValue=False))
+        self.edu_groupbox.setChecked(QS().value("education", defaultValue=False))
         self.edu_groupbox.toggled.connect(self.edu_toggled)
 
         edu_layout = QVBoxLayout()
-        self.edu_selection = SimpleList(title='Education')
+        self.edu_selection = SimpleList(title="Education")
         edu_layout.addWidget(self.edu_selection)
         self.edu_groupbox.setLayout(edu_layout)
         layout.addWidget(self.edu_groupbox)
 
         bt_layout = QHBoxLayout()
-        self.start_bt = QPushButton('Start')
-        self.start_bt.setFont(QFont(QS().value('app_font'), 20))
+        self.start_bt = QPushButton("Start")
+        self.start_bt.setFont(QFont(QS().value("app_font"), 20))
         self.start_bt.clicked.connect(self.init_main_window)
         bt_layout.addWidget(self.start_bt)
 
-        close_bt = QPushButton('Close')
+        close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
-        close_bt.setFont(QFont(QS().value('app_font'), 20))
+        close_bt.setFont(QFont(QS().value("app_font"), 20))
         bt_layout.addWidget(close_bt)
 
         layout.addLayout(bt_layout)
         self.setLayout(layout)
 
     def edu_toggled(self, value):
-        QS().setValue('education', value)
+        QS().setValue("education", value)
 
     def update_widgets(self):
         if self.ct is not None:
-            self.home_path_label.setText(f'{self.ct.home_path} selected.')
+            self.home_path_label.setText(f"{self.ct.home_path} selected.")
             self.add_pr_bt.setEnabled(True)
-            if hasattr(self.ct, 'projects'):
+            if hasattr(self.ct, "projects"):
                 self.project_cmbx.setEnabled(True)
                 self.project_cmbx.clear()
                 self.project_cmbx.addItems(self.ct.projects)
             if self.ct.pr is not None:
-                self.project_label.setText(f'{self.ct.pr.name} selected.')
+                self.project_label.setText(f"{self.ct.pr.name} selected.")
                 self.project_cmbx.setCurrentText(self.ct.pr.name)
 
             self.update_education_list()
             if self.ct.pr is not None:
                 self.start_bt.setEnabled(True)
         else:
             self.project_cmbx.setEnabled(False)
             self.add_pr_bt.setEnabled(False)
             self.start_bt.setEnabled(False)
-            self.home_path_label.setText('No Home-Path selected')
+            self.home_path_label.setText("No Home-Path selected")
 
     def set_home_path(self):
         if self.ct is not None:
             self.ct.save()
         loaded_home_path = QFileDialog.getExistingDirectory(
-            self, 'Select a folder as Home-Path')
-        if loaded_home_path != '':
+            self, "Select a folder as Home-Path"
+        )
+        if loaded_home_path != "":
             try:
                 self.ct = Controller(str(loaded_home_path))
             except RuntimeError as err:
                 self.home_path_label.setText(str(err))
                 self.start_bt.setEnabled(False)
                 self.project_cmbx.setEnabled(False)
                 self.add_pr_bt.setEnabled(False)
@@ -149,40 +155,41 @@
         if self.ct is not None:
             project = self.project_cmbx.itemText(project_idx)
             self.ct.change_project(project)
             self.update_widgets()
 
     def update_education_list(self):
         if self.ct is not None:
-            edu_path = join(self.ct.home_path, 'edu_programs')
+            edu_path = join(self.ct.home_path, "edu_programs")
             if isdir(edu_path):
                 self.edu_selection.replace_data(
-                    [f for f in listdir(edu_path) if f[-9:] == '-edu.json'])
+                    [f for f in listdir(edu_path) if f[-9:] == "-edu.json"]
+                )
 
     def add_project(self):
         if self.ct is not None:
             new_project = get_user_input_string(
-                'Please enter the name of a project!', 'Add Project')
+                "Please enter the name of a project!", "Add Project"
+            )
             if new_project is not None:
                 self.ct.change_project(new_project)
                 self.update_widgets()
 
     def init_main_window(self):
         if self.ct is not None:
-            edu_on = QS().value('education')
+            edu_on = QS().value("education")
             if edu_on:
                 self.ct.edu_program_name = self.edu_selection.get_current()
                 self.ct.load_edu()
 
             self.hide()
             MainWindow(self.ct)
 
     def closeEvent(self, event):
         if self.ct is not None:
-            WorkerDialog(self, self.ct.save, blocking=True,
-                         title='Saving Project!')
+            WorkerDialog(self, self.ct.save, blocking=True, title="Saving Project!")
         if self.edu_groupbox.isChecked():
-            QS().setValue('education', 1)
+            QS().setValue("education", 1)
         else:
-            QS().setValue('education', 0)
-        _object_refs['welcom_window'] = None
+            QS().setValue("education", 0)
+        _object_refs["welcom_window"] = None
         event.accept()
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/controller.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import json
 import logging
 import os
 import re
 import shutil
@@ -25,338 +23,360 @@
 from mne_pipeline_hd import functions
 from mne_pipeline_hd.gui.gui_utils import get_user_input_string
 from mne_pipeline_hd.pipeline.legacy import \
     transfer_file_params_to_single_subject
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 from mne_pipeline_hd.pipeline.project import Project
 
-home_dirs = ['custom_packages', 'freesurfer', 'projects']
-project_dirs = ['_pipeline_scripts', 'data', 'figures']
+home_dirs = ["custom_packages", "freesurfer", "projects"]
+project_dirs = ["_pipeline_scripts", "data", "figures"]
 
 
 class Controller:
-
-    def __init__(self, home_path=None, selected_project=None,
-                 edu_program_name=None):
+    def __init__(self, home_path=None, selected_project=None, edu_program_name=None):
         # Check Home-Path
         self.pr = None
         # Try to load home_path from QSettings
-        self.home_path = home_path or QS().value('home_path',
-                                                 defaultValue=None)
+        self.home_path = home_path or QS().value("home_path", defaultValue=None)
         self.settings = dict()
         if self.home_path is None:
-            raise RuntimeError('No Home-Path found!')
+            raise RuntimeError("No Home-Path found!")
 
         # Check if path exists
         elif not isdir(self.home_path):
-            raise RuntimeError(f'{self.home_path} not found!')
+            raise RuntimeError(f"{self.home_path} not found!")
 
         # Check, if path is writable
         elif not os.access(self.home_path, os.W_OK):
-            raise RuntimeError(f'{self.home_path} not writable!')
+            raise RuntimeError(f"{self.home_path} not writable!")
 
         # Initialize log-file
-        self.logging_path = join(self.home_path, '_pipeline.log')
-        file_handler = logging.FileHandler(self.logging_path, 'w')
+        self.logging_path = join(self.home_path, "_pipeline.log")
+        file_handler = logging.FileHandler(self.logging_path, "w")
         logging.getLogger().addHandler(file_handler)
 
-        logging.info(f'Home-Path: {self.home_path}')
-        QS().setValue('home_path', self.home_path)
+        logging.info(f"Home-Path: {self.home_path}")
+        QS().setValue("home_path", self.home_path)
         # Create subdirectories if not existing for a valid home_path
-        for subdir in [d for d in home_dirs if
-                       not isdir(join(self.home_path, d))]:
+        for subdir in [d for d in home_dirs if not isdir(join(self.home_path, d))]:
             os.mkdir(join(self.home_path, subdir))
 
         # Get Project-Folders (recognized by distinct sub-folders)
-        self.projects_path = join(self.home_path, 'projects')
-        self.projects = [p for p in listdir(self.projects_path)
-                         if all([isdir(join(self.projects_path, p, d))
-                                 for d in project_dirs])]
+        self.projects_path = join(self.home_path, "projects")
+        self.projects = [
+            p
+            for p in listdir(self.projects_path)
+            if all([isdir(join(self.projects_path, p, d)) for d in project_dirs])
+        ]
 
         # Initialize Subjects-Dir
-        self.subjects_dir = join(self.home_path, 'freesurfer')
+        self.subjects_dir = join(self.home_path, "freesurfer")
         mne.utils.set_config("SUBJECTS_DIR", self.subjects_dir, set_env=True)
 
         # Initialize folder for custom packages
-        self.custom_pkg_path = join(self.home_path, 'custom_packages')
+        self.custom_pkg_path = join(self.home_path, "custom_packages")
 
         # Initialize educational programs
         self.edu_program_name = edu_program_name
         self.edu_program = None
 
         # Load default settings
-        with resources.open_text('mne_pipeline_hd.resource',
-                                 'default_settings.json') as file:
+        with resources.open_text(
+            "mne_pipeline_hd.resource", "default_settings.json"
+        ) as file:
             self.default_settings = json.load(file)
 
         # Load settings (which are stored as .json-file in home_path)
         # settings=<everything, that's OS-independent>
         self.load_settings()
 
         self.all_modules = dict()
         self.all_pd_funcs = None
 
         # Pandas-DataFrame for contextual data of basic functions
         # (included with program)
-        with resources.path('mne_pipeline_hd.resource',
-                            'functions.csv') as pd_funcs_path:
-            self.pd_funcs = pd.read_csv(str(pd_funcs_path), sep=';',
-                                        index_col=0)
+        with resources.path(
+            "mne_pipeline_hd.resource", "functions.csv"
+        ) as pd_funcs_path:
+            self.pd_funcs = pd.read_csv(
+                str(pd_funcs_path),
+                sep=";",
+                index_col=0,
+                na_values=[""],
+                keep_default_na=False,
+            )
 
         # Pandas-DataFrame for contextual data of parameters
         # for basic functions (included with program)
-        with resources.path('mne_pipeline_hd.resource',
-                            'parameters.csv') as pd_params_path:
-            self.pd_params = pd.read_csv(str(pd_params_path), sep=';',
-                                         index_col=0)
+        with resources.path(
+            "mne_pipeline_hd.resource", "parameters.csv"
+        ) as pd_params_path:
+            self.pd_params = pd.read_csv(
+                str(pd_params_path),
+                sep=";",
+                index_col=0,
+                na_values=[""],
+                keep_default_na=False,
+            )
 
         # Import the basic- and custom-function-modules
         self.import_custom_modules()
 
         # Check Project
         if selected_project is None:
-            selected_project = self.settings['selected_project']
+            selected_project = self.settings["selected_project"]
 
         if selected_project is None:
             if len(self.projects) > 0:
                 selected_project = self.projects[0]
 
         # Initialize Project
         if selected_project is not None:
             self.change_project(selected_project)
 
     def load_settings(self):
         try:
-            with open(join(self.home_path,
-                           'mne_pipeline_hd-settings.json'), 'r') as file:
+            with open(
+                join(self.home_path, "mne_pipeline_hd-settings.json"), "r"
+            ) as file:
                 self.settings = json.load(file)
             # Account for settings, which were not saved
             # but exist in default_settings
-            for setting in [s for s in self.default_settings['settings']
-                            if s not in self.settings]:
-                self.settings[setting] = \
-                    self.default_settings['settings'][setting]
+            for setting in [
+                s for s in self.default_settings["settings"] if s not in self.settings
+            ]:
+                self.settings[setting] = self.default_settings["settings"][setting]
         except FileNotFoundError:
-            self.settings = self.default_settings['settings']
+            self.settings = self.default_settings["settings"]
         else:
             # Check integrity of Settings-Keys
             s_keys = set(self.settings.keys())
-            default_keys = set(self.default_settings['settings'])
+            default_keys = set(self.default_settings["settings"])
             # Remove additional (old) keys not appearing in default-settings
             for setting in s_keys - default_keys:
                 self.settings.pop(setting)
             # Add new keys from default-settings
             # which are not present in settings
             for setting in default_keys - s_keys:
-                self.settings[setting] = \
-                    self.default_settings['settings'][setting]
+                self.settings[setting] = self.default_settings["settings"][setting]
 
         # Check integrity of QSettings-Keys
         QS().sync()
         qs_keys = set(QS().childKeys())
-        qdefault_keys = set(self.default_settings['qsettings'])
+        qdefault_keys = set(self.default_settings["qsettings"])
         # Remove additional (old) keys not appearing in default-settings
         for qsetting in qs_keys - qdefault_keys:
             QS().remove(qsetting)
         # Add new keys from default-settings which are not present in QSettings
         for qsetting in qdefault_keys - qs_keys:
-            QS().setValue(qsetting,
-                          self.default_settings['qsettings'][qsetting])
+            QS().setValue(qsetting, self.default_settings["qsettings"][qsetting])
 
     def save_settings(self):
         try:
-            with open(join(self.home_path,
-                           'mne_pipeline_hd-settings.json'), 'w') as file:
+            with open(
+                join(self.home_path, "mne_pipeline_hd-settings.json"), "w"
+            ) as file:
                 json.dump(self.settings, file, indent=4)
         except FileNotFoundError:
-            print('Settings could not be saved!')
+            print("Settings could not be saved!")
 
         # Sync QSettings with other instances
         QS().sync()
 
     def get_setting(self, setting):
         try:
             value = self.settings[setting]
         except KeyError:
-            value = self.default_settings['settings'][setting]
+            value = self.default_settings["settings"][setting]
 
         return value
 
     def change_project(self, new_project):
         self.pr = Project(self, new_project)
-        self.settings['selected_project'] = new_project
+        self.settings["selected_project"] = new_project
         if new_project not in self.projects:
             self.projects.append(new_project)
-        logging.info(f'Selected-Project: {self.pr.name}')
+        logging.info(f"Selected-Project: {self.pr.name}")
         # Legacy
         transfer_file_params_to_single_subject(self)
 
         return self.pr
 
     def remove_project(self, project):
         self.projects.remove(project)
         if self.pr.name == project:
             if len(self.projects) > 0:
                 new_project = self.projects[0]
             else:
                 new_project = get_user_input_string(
-                    'Please enter the name of a new project!',
-                    'Add Project', force=True)
+                    "Please enter the name of a new project!", "Add Project", force=True
+                )
             self.change_project(new_project)
 
         # Remove Project-Folder
         try:
             shutil.rmtree(join(self.projects_path, project))
         except OSError as error:
             print(error)
             logging.warning(
-                f'The folder of {project} can\'t be deleted '
-                f'and has to be deleted manually!')
-
-    def copy_parameters_between_projects(self, from_name, from_p_preset,
-                                         to_name, to_p_preset):
+                f"The folder of {project} can't be deleted "
+                f"and has to be deleted manually!"
+            )
+
+    def copy_parameters_between_projects(
+        self, from_name, from_p_preset, to_name, to_p_preset
+    ):
         from_project = Project(self, from_name)
         if to_name == self.pr.name:
             to_project = self.pr
         else:
             to_project = Project(self, to_name)
-        to_project.parameters[to_p_preset] = \
-            from_project.parameters[from_p_preset]
+        to_project.parameters[to_p_preset] = from_project.parameters[from_p_preset]
         to_project.save()
 
     def save(self, worker_signals=None):
         if self.pr is not None:
             # Save Project
             self.pr.save(worker_signals)
-            self.settings['selected_project'] = self.pr.name
+            self.settings["selected_project"] = self.pr.name
 
         self.save_settings()
 
     def load_edu(self):
         if self.edu_program_name is not None:
-            edu_path = join(self.home_path, 'edu_programs',
-                            self.edu_program_name)
-            with open(edu_path, 'r') as file:
+            edu_path = join(self.home_path, "edu_programs", self.edu_program_name)
+            with open(edu_path, "r") as file:
                 self.edu_program = json.load(file)
 
             self.all_pd_funcs = self.pd_funcs.copy()
             # Exclude functions which are not selected
             self.pd_funcs = self.pd_funcs.loc[
-                self.pd_funcs.index.isin(self.edu_program['functions'])]
+                self.pd_funcs.index.isin(self.edu_program["functions"])
+            ]
 
             # Change the Project-Scripts-Path to a new folder
             # to store the Education-Project-Scripts separately
-            self.pr.pscripts_path = \
-                join(self.pr.project_path,
-                     f'_pipeline_scripts{self.edu_program["name"]}')
+            self.pr.pscripts_path = join(
+                self.pr.project_path, f'_pipeline_scripts{self.edu_program["name"]}'
+            )
             if not isdir(self.pr.pscripts_path):
                 os.mkdir(self.pr.pscripts_path)
             self.pr.init_pipeline_scripts()
 
             # Exclude MEEG
             self.pr._all_meeg = self.pr.all_meeg.copy()
-            self.pr.all_meeg = [meeg for meeg in self.pr.all_meeg if
-                                meeg in self.edu_program['meeg']]
+            self.pr.all_meeg = [
+                meeg for meeg in self.pr.all_meeg if meeg in self.edu_program["meeg"]
+            ]
 
             # Exclude FSMRI
             self.pr._all_fsmri = self.pr.all_fsmri.copy()
-            self.pr.all_fsmri = [meeg for meeg in self.pr.all_meeg if
-                                 meeg in self.edu_program['meeg']]
+            self.pr.all_fsmri = [
+                meeg for meeg in self.pr.all_meeg if meeg in self.edu_program["meeg"]
+            ]
 
     def import_custom_modules(self):
         """
         Load all modules in functions and custom_functions
         """
 
         # Load basic-modules
         # Add functions to sys.path
         sys.path.insert(0, str(Path(functions.__file__).parent))
-        basic_functions_list = [x for x in dir(functions) if '__' not in x]
-        self.all_modules['basic'] = list()
+        basic_functions_list = [x for x in dir(functions) if "__" not in x]
+        self.all_modules["basic"] = list()
         for module_name in basic_functions_list:
-            self.all_modules['basic'].append(module_name)
+            self.all_modules["basic"].append(module_name)
 
         # Load custom_modules
-        pd_functions_pattern = r'.*_functions\.csv'
-        pd_parameters_pattern = r'.*_parameters\.csv'
-        custom_module_pattern = r'(.+)(\.py)$'
-        for directory in [d for d in os.scandir(self.custom_pkg_path) if
-                          not d.name.startswith('.')]:
+        pd_functions_pattern = r".*_functions\.csv"
+        pd_parameters_pattern = r".*_parameters\.csv"
+        custom_module_pattern = r"(.+)(\.py)$"
+        for directory in [
+            d for d in os.scandir(self.custom_pkg_path) if not d.name.startswith(".")
+        ]:
             pkg_name = directory.name
             pkg_path = directory.path
-            file_dict = {'functions': None, 'parameters': None,
-                         'modules': list()}
-            for file_name in [f for f in listdir(pkg_path)
-                              if not f.startswith(('.', '_'))]:
-                functions_match = \
-                    re.match(pd_functions_pattern, file_name)
-                parameters_match = \
-                    re.match(pd_parameters_pattern, file_name)
-                custom_module_match = \
-                    re.match(custom_module_pattern, file_name)
+            file_dict = {"functions": None, "parameters": None, "modules": list()}
+            for file_name in [
+                f for f in listdir(pkg_path) if not f.startswith((".", "_"))
+            ]:
+                functions_match = re.match(pd_functions_pattern, file_name)
+                parameters_match = re.match(pd_parameters_pattern, file_name)
+                custom_module_match = re.match(custom_module_pattern, file_name)
                 if functions_match:
-                    file_dict['functions'] = join(pkg_path, file_name)
+                    file_dict["functions"] = join(pkg_path, file_name)
                 elif parameters_match:
-                    file_dict['parameters'] = join(pkg_path, file_name)
-                elif custom_module_match \
-                        and custom_module_match.group(1) != '__init__':
-                    file_dict['modules'].append(custom_module_match)
+                    file_dict["parameters"] = join(pkg_path, file_name)
+                elif custom_module_match and custom_module_match.group(1) != "__init__":
+                    file_dict["modules"].append(custom_module_match)
 
             # Check, that there is a whole set for a custom-module
             # (module-file, functions, parameters)
-            if all([value is not None or value != []
-                    for value in file_dict.values()]):
+            if all([value is not None or value != [] for value in file_dict.values()]):
                 self.all_modules[pkg_name] = list()
-                functions_path = file_dict['functions']
-                parameters_path = file_dict['parameters']
+                functions_path = file_dict["functions"]
+                parameters_path = file_dict["parameters"]
                 correct_count = 0
-                for module_match in file_dict['modules']:
+                for module_match in file_dict["modules"]:
                     module_name = module_match.group(1)
                     # Add pkg-path to sys.path
                     sys.path.insert(0, pkg_path)
                     try:
                         import_module(module_name)
-                    except:  # noqa: E722
+                    except Exception:
                         traceback.print_exc()
                     else:
                         correct_count += 1
                         # Add Module to dictionary
                         self.all_modules[pkg_name].append(module_name)
 
                 # Make sure, that every module in modules
                 # is imported without error
                 # (otherwise don't append to pd_funcs and pd_params)
-                if len(file_dict['modules']) == correct_count:
+                if len(file_dict["modules"]) == correct_count:
                     try:
-                        read_pd_funcs = pd.read_csv(functions_path,
-                                                    sep=';', index_col=0)
-                        read_pd_params = pd.read_csv(parameters_path,
-                                                     sep=';', index_col=0)
-                    except:  # noqa: E722
+                        read_pd_funcs = pd.read_csv(
+                            functions_path,
+                            sep=";",
+                            index_col=0,
+                            na_values=[""],
+                            keep_default_na=False,
+                        )
+                        read_pd_params = pd.read_csv(
+                            parameters_path,
+                            sep=";",
+                            index_col=0,
+                            na_values=[""],
+                            keep_default_na=False,
+                        )
+                    except Exception:
                         traceback.print_exc()
                     else:
                         # Add pkg_name here (would be redundant
                         # in read_pd_funcs of each custom-package)
-                        read_pd_funcs['pkg_name'] = pkg_name
+                        read_pd_funcs["pkg_name"] = pkg_name
 
                         # Check, that there are no duplicates
                         pd_funcs_to_append = read_pd_funcs.loc[
-                            ~read_pd_funcs.index.isin(self.pd_funcs.index)]
-                        self.pd_funcs = pd.concat([self.pd_funcs,
-                                                   pd_funcs_to_append])
+                            ~read_pd_funcs.index.isin(self.pd_funcs.index)
+                        ]
+                        self.pd_funcs = pd.concat([self.pd_funcs, pd_funcs_to_append])
                         pd_params_to_append = read_pd_params.loc[
-                            ~read_pd_params.index.isin(self.pd_params.index)]
-                        self.pd_params = pd.concat([self.pd_params,
-                                                    pd_params_to_append])
+                            ~read_pd_params.index.isin(self.pd_params.index)
+                        ]
+                        self.pd_params = pd.concat(
+                            [self.pd_params, pd_params_to_append]
+                        )
 
             else:
-                missing_files = [key for key in file_dict
-                                 if file_dict[key] is None]
-                logging.warning(f'Files for import of {pkg_name} '
-                                f'are missing: {missing_files}')
+                missing_files = [key for key in file_dict if file_dict[key] is None]
+                logging.warning(
+                    f"Files for import of {pkg_name} " f"are missing: {missing_files}"
+                )
 
     def reload_modules(self):
         for pkg_name in self.all_modules:
             for module_name in self.all_modules[pkg_name]:
                 module = import_module(module_name)
                 try:
                     reload(module)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/function_utils.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/function_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,121 +1,120 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 import io
 import logging
 import sys
 from collections import OrderedDict
 from importlib import import_module
 from multiprocessing import Pipe
 
-from PyQt5.QtCore import (QThreadPool, QRunnable, pyqtSlot,
-                          QObject, pyqtSignal)
-from PyQt5.QtWidgets import (QAbstractItemView)
-
-from mne_pipeline_hd.gui.gui_utils import (get_exception_tuple,
-                                           ExceptionTuple, Worker)
-from mne_pipeline_hd.pipeline.loading import (BaseLoading, FSMRI, Group, MEEG)
+from PyQt5.QtCore import QThreadPool, QRunnable, pyqtSlot, QObject, pyqtSignal
+from PyQt5.QtWidgets import QAbstractItemView
+
+from mne_pipeline_hd.gui.gui_utils import get_exception_tuple, ExceptionTuple, \
+    Worker
+from mne_pipeline_hd.pipeline.loading import BaseLoading, FSMRI, Group, MEEG
 from mne_pipeline_hd.pipeline.pipeline_utils import shutdown, ismac, QS
 
 
 def get_func(func_name, obj):
     # Get module- and package-name, has to specified in pd_funcs
     # (which imports from functions.csv or the <custom_package>.csv)
-    module_name = obj.ct.pd_funcs.loc[func_name, 'module']
+    module_name = obj.ct.pd_funcs.loc[func_name, "module"]
     module = import_module(module_name)
     func = getattr(module, func_name)
 
     return func
 
 
 def get_arguments(func, obj):
     keyword_arguments = {}
     project_attributes = vars(obj.pr)
 
     # Get arguments from function signature
     arg_names = list(inspect.signature(func).parameters)
 
     # Remove args/kwargs
-    if 'args' in arg_names:
-        arg_names.remove('args')
-    if 'kwargs' in arg_names:
-        arg_names.remove('kwargs')
+    if "args" in arg_names:
+        arg_names.remove("args")
+    if "kwargs" in arg_names:
+        arg_names.remove("kwargs")
 
     # Get the values for parameter-names
     for arg_name in arg_names:
-        if arg_name == 'ct':
-            keyword_arguments.update({'ct': obj.ct})
-        elif arg_name == 'controller':
-            keyword_arguments.update({'controller': obj.ct})
-        elif arg_name == 'pr':
-            keyword_arguments.update({'pr': obj.pr})
-        elif arg_name == 'project':
-            keyword_arguments.update({'project': obj.pr})
-        elif arg_name == 'meeg':
-            keyword_arguments.update({'meeg': obj})
-        elif arg_name == 'fsmri':
-            keyword_arguments.update({'fsmri': obj})
-        elif arg_name == 'group':
-            keyword_arguments.update({'group': obj})
+        if arg_name == "ct":
+            keyword_arguments.update({"ct": obj.ct})
+        elif arg_name == "controller":
+            keyword_arguments.update({"controller": obj.ct})
+        elif arg_name == "pr":
+            keyword_arguments.update({"pr": obj.pr})
+        elif arg_name == "project":
+            keyword_arguments.update({"project": obj.pr})
+        elif arg_name == "meeg":
+            keyword_arguments.update({"meeg": obj})
+        elif arg_name == "fsmri":
+            keyword_arguments.update({"fsmri": obj})
+        elif arg_name == "group":
+            keyword_arguments.update({"group": obj})
         elif arg_name in project_attributes:
             keyword_arguments.update({arg_name: project_attributes[arg_name]})
         elif arg_name in obj.pr.parameters[obj.pr.p_preset]:
-            keyword_arguments.update({arg_name: obj.pr.parameters[
-                obj.pr.p_preset][arg_name]})
+            keyword_arguments.update(
+                {arg_name: obj.pr.parameters[obj.pr.p_preset][arg_name]}
+            )
         elif arg_name in obj.ct.settings:
             keyword_arguments.update({arg_name: obj.ct.settings[arg_name]})
         elif arg_name in QS().childKeys():
             keyword_arguments.update({arg_name: QS().value(arg_name)})
         else:
-            raise RuntimeError(f'{arg_name} could not be found '
-                               f'in Subject, Project or Parameters')
+            raise RuntimeError(
+                f"{arg_name} could not be found " f"in Subject, Project or Parameters"
+            )
 
     # Add additional keyword-arguments if added for function by user
     if func.__name__ in obj.pr.add_kwargs:
         for kwarg in obj.pr.add_kwargs[func.__name__]:
             keyword_arguments[kwarg] = obj.pr.add_kwargs[func.__name__][kwarg]
 
     return keyword_arguments
 
 
 class StreamManager:
     def __init__(self, pipe):
         self.pipe_busy = False
-        self.stdout_sender = StreamSender(self, 'stdout', pipe)
-        self.stderr_sender = StreamSender(self, 'stderr', pipe)
+        self.stdout_sender = StreamSender(self, "stdout", pipe)
+        self.stderr_sender = StreamSender(self, "stderr", pipe)
 
 
 class StreamSender(io.TextIOBase):
     def __init__(self, manager, kind, pipe):
         super().__init__()
         self.manager = manager
         self.kind = kind
-        if kind == 'stdout':
+        if kind == "stdout":
             self.original_stream = sys.__stdout__
         else:
             self.original_stream = sys.__stderr__
         self.pipe = pipe
 
     def write(self, text):
         # Still send output to the command-line
         self.original_stream.write(text)
         # Wait until pipe is free
         while self.manager.pipe_busy:
             pass
         self.manager.pipe_busy = True
-        if text[:1] == '\r':
-            kind = 'progress'
+        if text[:1] == "\r":
+            kind = "progress"
         else:
             kind = self.kind
         self.pipe.send((text, kind))
         self.manager.pipe_busy = False
 
 
 class StreamRcvSignals(QObject):
@@ -134,30 +133,30 @@
     def run(self):
         while True:
             try:
                 text, kind = self.pipe.recv()
             except EOFError:
                 break
             else:
-                if kind == 'stdout':
+                if kind == "stdout":
                     self.signals.stdout_received.emit(text)
-                elif kind == 'stderr':
+                elif kind == "stderr":
                     self.signals.stderr_received.emit(text)
                 else:
                     self.signals.progress_received.emit(text)
 
 
 def run_func(func, keywargs, pipe=None):
     if pipe is not None:
         stream_manager = StreamManager(pipe)
         sys.stdout = stream_manager.stdout_sender
         sys.stderr = stream_manager.stderr_sender
     try:
         return func(**keywargs)
-    except:  # noqa: E722
+    except Exception:
         return get_exception_tuple(is_mp=pipe is not None)
 
 
 class RunController:
     def __init__(self, controller):
         self.ct = controller
 
@@ -171,135 +170,142 @@
         self.current_func = None
         self.prog_count = 0
 
         self.init_lists()
 
     def init_lists(self):
         # Lists dividing the
-        self.meeg_funcs = self.ct.pd_funcs[
-            self.ct.pd_funcs['target'] == 'MEEG']
-        self.fsmri_funcs = self.ct.pd_funcs[
-            self.ct.pd_funcs['target'] == 'FSMRI']
-        self.group_funcs = self.ct.pd_funcs[
-            self.ct.pd_funcs['target'] == 'Group']
-        self.other_funcs = self.ct.pd_funcs[
-            self.ct.pd_funcs['target'] == 'Other']
+        self.meeg_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "MEEG"]
+        self.fsmri_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "FSMRI"]
+        self.group_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "Group"]
+        self.other_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "Other"]
 
         # Lists of selected functions divided into object-types
         # (MEEG, FSMRI, ...)
-        self.sel_meeg_funcs = [ff for ff in self.meeg_funcs.index
-                               if ff in self.ct.pr.sel_functions]
-        self.sel_fsmri_funcs = [mf for mf in self.fsmri_funcs.index if
-                                mf in self.ct.pr.sel_functions]
-        self.sel_group_funcs = [gf for gf in self.group_funcs.index if
-                                gf in self.ct.pr.sel_functions]
-        self.sel_other_funcs = [of for of in self.other_funcs.index if
-                                of in self.ct.pr.sel_functions]
+        self.sel_meeg_funcs = [
+            ff for ff in self.meeg_funcs.index if ff in self.ct.pr.sel_functions
+        ]
+        self.sel_fsmri_funcs = [
+            mf for mf in self.fsmri_funcs.index if mf in self.ct.pr.sel_functions
+        ]
+        self.sel_group_funcs = [
+            gf for gf in self.group_funcs.index if gf in self.ct.pr.sel_functions
+        ]
+        self.sel_other_funcs = [
+            of for of in self.other_funcs.index if of in self.ct.pr.sel_functions
+        ]
 
         # Get a dict with all objects paired with their functions
         # and their type-definition. Give all objects and functions in
         # all_objects the status 1 (which means pending)
         if len(self.ct.pr.sel_fsmri) * len(self.sel_fsmri_funcs) != 0:
             for fsmri in self.ct.pr.sel_fsmri:
                 self.all_objects[fsmri] = {
-                    'type': 'FSMRI',
-                    'functions': {x: 1 for x in self.sel_fsmri_funcs},
-                    'status': 1}
+                    "type": "FSMRI",
+                    "functions": {x: 1 for x in self.sel_fsmri_funcs},
+                    "status": 1,
+                }
                 for fsmri_func in self.sel_fsmri_funcs:
                     self.all_steps.append((fsmri, fsmri_func))
 
         if len(self.ct.pr.sel_meeg) * len(self.sel_meeg_funcs) != 0:
             for meeg in self.ct.pr.sel_meeg:
                 self.all_objects[meeg] = {
-                    'type': 'MEEG',
-                    'functions': {x: 1 for x in self.sel_meeg_funcs},
-                    'status': 1}
+                    "type": "MEEG",
+                    "functions": {x: 1 for x in self.sel_meeg_funcs},
+                    "status": 1,
+                }
                 for meeg_func in self.sel_meeg_funcs:
                     self.all_steps.append((meeg, meeg_func))
 
         if len(self.ct.pr.sel_groups) * len(self.sel_group_funcs) != 0:
             for group in self.ct.pr.sel_groups:
                 self.all_objects[group] = {
-                    'type': 'Group',
-                    'functions': {x: 1 for x in self.sel_group_funcs},
-                    'status': 1}
+                    "type": "Group",
+                    "functions": {x: 1 for x in self.sel_group_funcs},
+                    "status": 1,
+                }
                 for group_func in self.sel_group_funcs:
                     self.all_steps.append((group, group_func))
 
         if len(self.sel_other_funcs) != 0:
             # blank object-name for other functions
-            self.all_objects[''] = {
-                'type': 'Other',
-                'functions': {x: 1 for x in self.sel_other_funcs},
-                'status': 1}
+            self.all_objects[""] = {
+                "type": "Other",
+                "functions": {x: 1 for x in self.sel_other_funcs},
+                "status": 1,
+            }
             for other_func in self.sel_other_funcs:
-                self.all_steps.append(('', other_func))
+                self.all_steps.append(("", other_func))
 
     def mark_current_items(self, status):
         # Mark current object with status
-        self.all_objects[self.current_object.name]['status'] = status
+        self.all_objects[self.current_object.name]["status"] = status
         # Mark current function with status
-        self.all_objects[self.current_object.name]['functions'][
-            self.current_func] = status
+        self.all_objects[self.current_object.name]["functions"][
+            self.current_func
+        ] = status
 
     def get_object(self):
-        self.current_type = self.all_objects[self.current_obj_name]['type']
+        self.current_type = self.all_objects[self.current_obj_name]["type"]
 
         # Load object if the preceding object is not the same
-        if not self.current_object \
-                or self.current_object.name != self.current_obj_name:
-            if self.current_type == 'FSMRI':
+        if not self.current_object or self.current_object.name != self.current_obj_name:
+            if self.current_type == "FSMRI":
                 self.current_object = FSMRI(self.current_obj_name, self.ct)
                 self.loaded_fsmri = self.current_object
 
-            elif self.current_type == 'MEEG':
+            elif self.current_type == "MEEG":
                 # Avoid reloading of same MRI-Subject for multiple files
                 # (with the same MRI-Subject)
-                if self.current_obj_name in self.ct.pr.meeg_to_fsmri \
-                        and self.loaded_fsmri \
-                        and self.loaded_fsmri.name == \
-                        self.ct.pr.meeg_to_fsmri[self.current_obj_name]:
-                    self.current_object = MEEG(self.current_obj_name, self.ct,
-                                               fsmri=self.loaded_fsmri)
+                if (
+                    self.current_obj_name in self.ct.pr.meeg_to_fsmri
+                    and self.loaded_fsmri
+                    and self.loaded_fsmri.name
+                    == self.ct.pr.meeg_to_fsmri[self.current_obj_name]
+                ):
+                    self.current_object = MEEG(
+                        self.current_obj_name, self.ct, fsmri=self.loaded_fsmri
+                    )
                 else:
                     self.current_object = MEEG(self.current_obj_name, self.ct)
                 self.loaded_fsmri = self.current_object.fsmri
 
-            elif self.current_type == 'Group':
+            elif self.current_type == "Group":
                 self.current_object = Group(self.current_obj_name, self.ct)
 
-            elif self.current_type == 'Other':
-                self.current_object = BaseLoading(self.current_obj_name,
-                                                  self.ct)
+            elif self.current_type == "Other":
+                self.current_object = BaseLoading(self.current_obj_name, self.ct)
 
     def process_finished(self, result):
         # ToDo: tqdm-progressbar for headless-mode
         self.prog_count += 1
         self.start()
 
     def finished(self):
         pass
 
     def prepare_start(self):
         # Take first step of all_steps until there are no steps left.
         if len(self.all_steps) > 0:
             # Getting information as encoded in init_lists
             self.current_obj_name, self.current_func = self.all_steps.pop(0)
-            logging.debug(f'Running {self.current_func} for '
-                          f'{self.current_obj_name}')
+            logging.debug(
+                f"Running {self.current_func} for " f"{self.current_obj_name}"
+            )
             # Get current object
             self.get_object()
 
             # Mark current object and current function
             self.mark_current_items(2)
 
             # Run function in Multiprocessing-Pool
             kwds = dict()
-            kwds['func'] = get_func(self.current_func, self.current_object)
-            kwds['keywargs'] = get_arguments(kwds['func'], self.current_object)
+            kwds["func"] = get_func(self.current_func, self.current_object)
+            kwds["keywargs"] = get_arguments(kwds["func"], self.current_object)
 
             return kwds
 
         else:
             self.finished()
 
     def start(self):
@@ -320,122 +326,134 @@
         self.error_count = 0
         self.is_prog_text = False
         self.paused = False
 
     def mark_current_items(self, status):
         super().mark_current_items(status)
         obj_idx = list(self.all_objects.keys()).index(self.current_object.name)
-        func_idx = list(self.all_objects[self.current_object.name]
-                        ['functions'].keys()).index(self.current_func)
+        func_idx = list(
+            self.all_objects[self.current_object.name]["functions"].keys()
+        ).index(self.current_func)
         # Notify Object-Model of change
         self.rd.object_model.layoutChanged.emit()
         # Scroll to current object
         self.rd.object_view.scrollTo(
             self.rd.object_model.createIndex(obj_idx, 0),
-            QAbstractItemView.PositionAtCenter)
+            QAbstractItemView.PositionAtCenter,
+        )
         # Notify Function-Model of change
         self.rd.func_model.layoutChanged.emit()
         # Scroll to current function
         self.rd.func_view.scrollTo(
             self.rd.func_model.createIndex(func_idx, 0),
-            QAbstractItemView.PositionAtCenter)
+            QAbstractItemView.PositionAtCenter,
+        )
 
     def get_object(self):
         old_obj_name = self.current_obj_name
         super().get_object()
         # Print Headline for object if new
         if old_obj_name != self.current_obj_name:
             self.rd.console_widget.write_html(
-                f'<br><h1>{self.current_obj_name}</h1><br>')
+                f"<br><h1>{self.current_obj_name}</h1><br>"
+            )
         # Load functions for object into func_model
         # (which displays functions in func_view)
-        self.current_all_funcs = self.all_objects[
-            self.current_obj_name]['functions']
+        self.current_all_funcs = self.all_objects[self.current_obj_name]["functions"]
         self.rd.func_model._data = self.current_all_funcs
         self.rd.func_model.layoutChanged.emit()
 
         # Print Headline for function
-        self.rd.console_widget.write_html(f'<h2>{self.current_func}</h2><br>')
+        self.rd.console_widget.write_html(f"<h2>{self.current_func}</h2><br>")
 
     def process_finished(self, result):
         self.prog_count += 1
         self.rd.pgbar.setValue(self.prog_count)
         self.mark_current_items(0)
         # Process
         if self.paused:
-            self.rd.console_widget.write_html('<b><big>Paused</big></b><br>')
+            self.rd.console_widget.write_html("<b><big>Paused</big></b><br>")
             # Enable/Disable Buttons
             self.rd.continue_bt.setEnabled(True)
             self.rd.pause_bt.setEnabled(False)
             self.rd.restart_bt.setEnabled(True)
             self.rd.close_bt.setEnabled(True)
         else:
             if isinstance(result, ExceptionTuple):
-                error_cause = f'{self.error_count}: ' \
-                              f'{self.current_object.name} ' \
-                              f'<- {self.current_func}'
+                error_cause = (
+                    f"{self.error_count}: "
+                    f"{self.current_object.name} "
+                    f"<- {self.current_func}"
+                )
                 self.errors[error_cause] = (result, self.error_count)
                 # Update Error-Widget
                 self.rd.error_widget.replace_data(list(self.errors.keys()))
 
                 # Insert Error-Number into console-widget as an anchor
                 # for later inspection
                 self.rd.console_widget.write_html(
-                    f'<a name=\"{self.error_count}\" href={self.error_count}>'
-                    f'<i>Error No.{self.error_count}</i><br></a>')
+                    f'<a name="{self.error_count}" href={self.error_count}>'
+                    f"<i>Error No.{self.error_count}</i><br></a>"
+                )
                 # Increase Error-Count by one
                 self.error_count += 1
 
             # Continue with next object
             self.start()
 
     def finished(self):
-        self.rd.console_widget.write_html('<b><big>Finished</big></b><br>')
+        self.rd.console_widget.write_html("<b><big>Finished</big></b><br>")
         # Enable/Disable Buttons
         self.rd.continue_bt.setEnabled(False)
         self.rd.pause_bt.setEnabled(False)
         self.rd.restart_bt.setEnabled(True)
         self.rd.close_bt.setEnabled(True)
 
-        if self.ct.get_setting('shutdown'):
+        if self.ct.get_setting("shutdown"):
             self.ct.save()
             shutdown()
 
     def start(self):
         kwds = self.prepare_start()
         if kwds:
             # Plot functions with interactive plots currently can't
             # run in a separate thread, so they
             #  excuted in the main thread
-            ismayavi = self.ct.pd_funcs.loc[self.current_func, 'mayavi']
-            ismpl = self.ct.pd_funcs.loc[self.current_func, 'matplotlib']
-            show_plots = self.ct.get_setting('show_plots')
-            use_qthread = QS().value('use_qthread')
-            if ismayavi \
-                    or (ismpl and show_plots and use_qthread) \
-                    or (ismpl and not show_plots and use_qthread and ismac):
-                logging.info('Starting in Main-Thread.')
+            ismayavi = self.ct.pd_funcs.loc[self.current_func, "mayavi"]
+            ismpl = self.ct.pd_funcs.loc[self.current_func, "matplotlib"]
+            show_plots = self.ct.get_setting("show_plots")
+            use_qthread = QS().value("use_qthread")
+            if (
+                ismayavi
+                or (ismpl and show_plots and use_qthread)
+                or (ismpl and not show_plots and use_qthread and ismac)
+            ):
+                logging.info("Starting in Main-Thread.")
                 result = run_func(**kwds)
                 self.process_finished(result)
 
-            elif QS().value('use_qthread'):
-                logging.info('Starting in separate Thread.')
+            elif QS().value("use_qthread"):
+                logging.info("Starting in separate Thread.")
                 worker = Worker(function=run_func, **kwds)
                 worker.signals.error.connect(self.process_finished)
                 worker.signals.finished.connect(self.process_finished)
                 QThreadPool.globalInstance().start(worker)
 
             else:
-                logging.info('Starting in process from multiprocessing.')
+                logging.info("Starting in process from multiprocessing.")
                 recv_pipe, send_pipe = Pipe(False)
-                kwds['pipe'] = send_pipe
+                kwds["pipe"] = send_pipe
                 stream_rcv = StreamReceiver(recv_pipe)
                 stream_rcv.signals.stdout_received.connect(
-                    self.rd.console_widget.write_stdout)
+                    self.rd.console_widget.write_stdout
+                )
                 stream_rcv.signals.stderr_received.connect(
-                    self.rd.console_widget.write_stderr)
+                    self.rd.console_widget.write_stderr
+                )
                 stream_rcv.signals.progress_received.connect(
-                    self.rd.console_widget.write_progress)
+                    self.rd.console_widget.write_progress
+                )
                 QThreadPool.globalInstance().start(stream_rcv)
                 # ToDO: MP
-                self.pool.apply_async(func=run_func, kwds=kwds,
-                                      callback=self.process_finished)
+                self.pool.apply_async(
+                    func=run_func, kwds=kwds, callback=self.process_finished
+                )
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/loading.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/loading.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from __future__ import print_function
 
 import functools
 import inspect
 import itertools
@@ -21,148 +19,158 @@
 from os import listdir, makedirs, remove
 from os.path import exists, getsize, isdir, isfile, join
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import mne
 import numpy as np
-# ==============================================================================
+
+# =============================================================================
 # LOADING FUNCTIONS
-# ==============================================================================
+# =============================================================================
 from tqdm import tqdm
 
 from mne_pipeline_hd.pipeline.pipeline_utils import (
-    TypedJSONEncoder, type_json_hook, QS, _test_run)
-
-sample_paths = {'raw': 'sample_audvis_raw.fif',
-                'erm': 'ernoise_raw.fif',
-                'events': 'sample_audvis_raw-eve.fif',
-                'trans': 'sample_audvis_raw-trans.fif'}
+    TypedJSONEncoder,
+    type_json_hook,
+    QS,
+    _test_run,
+)
+
+sample_paths = {
+    "raw": "sample_audvis_raw.fif",
+    "erm": "ernoise_raw.fif",
+    "events": "sample_audvis_raw-eve.fif",
+    "trans": "sample_audvis_raw-trans.fif",
+}
 
 
 def _get_data_type_from_func(self, func, method):
     # Get matching data-type from IO-Dict
     func_name = func.__name__
     data_type = None
     for dt in self.io_dict:
         io_func = self.io_dict[dt][method]
-        if getattr(io_func, '__name__', None) == func_name:
+        if getattr(io_func, "__name__", None) == func_name:
             data_type = dt
             break
     if data_type is None:
-        raise RuntimeError(f'No datatype for loading-function '
-                           f'"{func_name}"!')
+        raise RuntimeError(f"No datatype for loading-function {func_name}!")
 
     return data_type
 
 
 def load_decorator(load_func):
     @functools.wraps(load_func)
     def load_wrapper(self, *args, **kwargs):
         # Get matching data-type from IO-Dict
-        data_type = _get_data_type_from_func(self, load_func, 'load')
-        print(f'Loading {data_type} for {self.name}')
+        data_type = _get_data_type_from_func(self, load_func, "load")
+        print(f"Loading {data_type} for {self.name}")
 
         if data_type in self.data_dict:
             data = self.data_dict[data_type]
         else:
             # Todo: Dependencies!
             try:
                 data = load_func(self, *args, **kwargs)
-            except (FileNotFoundError, OSError) as err:
-                deprc_path = self.deprecated_paths.get(data_type, '')
+            except OSError as err:
+                deprc_path = self.deprecated_paths.get(data_type, "")
                 if isfile(deprc_path):
-                    new_path = self.io_dict[data_type]['path']
-                    self.io_dict[data_type]['path'] = deprc_path
+                    new_path = self.io_dict[data_type]["path"]
+                    self.io_dict[data_type]["path"] = deprc_path
                     data = load_func(self, *args, **kwargs)
-                    self.io_dict[data_type]['path'] = new_path
-                    logging.info(f'Deprecated path: Saving file for '
-                                 f'{data_type} in updated path...')
+                    self.io_dict[data_type]["path"] = new_path
+                    logging.info(
+                        f"Deprecated path: Saving file for "
+                        f"{data_type} in updated path..."
+                    )
                     # Save data with new path
-                    save_func = self.io_dict[data_type]['save']
+                    save_func = self.io_dict[data_type]["save"]
                     # Does only support save-functions with no extra args
                     save_func(self, data)
                     # Remove deprecated path
                     os.remove(deprc_path)
 
-                elif self.p_preset != 'Default':
-                    print(f'No File for {data_type} from {self.name}'
-                          f' with Parameter-Preset={self.p_preset} found,'
-                          f' trying Default')
+                elif self.p_preset != "Default":
+                    print(
+                        f"No File for {data_type} from {self.name}"
+                        f" with Parameter-Preset={self.p_preset} found,"
+                        f" trying Default"
+                    )
 
                     actual_p_preset = self.p_preset
-                    self.p_preset = 'Default'
+                    self.p_preset = "Default"
                     self.init_paths()
 
                     data = load_func(*args, **kwargs)
 
                     self.p_preset = actual_p_preset
                     self.init_paths()
                 else:
                     raise err
 
         # Save data in data-dict for machines with big RAM
-        if not QS().value('save_ram'):
+        if not QS().value("save_ram"):
             self.data_dict[data_type] = data
 
         return data
 
     return load_wrapper
 
 
 def save_decorator(save_func):
     @functools.wraps(save_func)
     def save_wrapper(self, *args, **kwargs):
         # Get matching data-type from IO-Dict
-        data_type = _get_data_type_from_func(self, save_func, 'save')
+        data_type = _get_data_type_from_func(self, save_func, "save")
 
         # Get data-object
         if len(args) > 1:
             data = args[1]
         elif len(kwargs) > 0:
             data = kwargs[list(kwargs.keys())[0]]
         else:
             data = None
 
         # Make sure, that parent-directory exists
         paths = self._return_path_list(data_type)
         for path in [p for p in paths if not isdir(Path(p).parent)]:
             makedirs(Path(path).parent, exist_ok=True)
 
-        print(f'Saving {data_type} for {self.name}')
+        print(f"Saving {data_type} for {self.name}")
         save_func(self, *args, **kwargs)
 
         # Save data in data-dict for machines with big RAM
-        if not QS().value('save_ram'):
+        if not QS().value("save_ram"):
             self.data_dict[data_type] = data
 
         # Save File-Parameters
         paths = self._return_path_list(data_type)
         for path in paths:
             self.save_file_params(path)
 
     return save_wrapper
 
 
 class BaseLoading:
-    """ Base-Class for Sub (The current File/MRI-File/Grand-Average-Group,
-     which is executed)"""
+    """Base-Class for Sub (The current File/MRI-File/Grand-Average-Group,
+    which is executed)"""
 
     def __init__(self, name, controller):
         # Basic Attributes (partly taking parameters or main-win-attributes
         # for easier access)
         self.name = name
         self.ct = controller
         self.pr = controller.pr
         self.p_preset = self.pr.p_preset
         self.subjects_dir = self.ct.subjects_dir
-        self.save_plots = self.ct.get_setting('save_plots')
+        self.save_plots = self.ct.get_setting("save_plots")
         self.figures_path = self.pr.figures_path
-        self.img_format = self.ct.get_setting('img_format')
-        self.dpi = self.ct.get_setting('dpi')
+        self.img_format = self.ct.get_setting("img_format")
+        self.dpi = self.ct.get_setting("dpi")
 
         self.data_dict = dict()
         self.existing_paths = dict()
 
         if name is not None:
             self.init_parameters()
             self.init_attributes()
@@ -182,149 +190,155 @@
     def init_attributes(self):
         """Initialization of additional attributes, should be overridden
         in inherited classes"""
         pass
 
     def init_paths(self):
         """Initialization of all paths and the io_dict, should be overridden
-         in inherited classes"""
+        in inherited classes"""
         self.save_dir = None
         self.io_dict = dict()
         self.deprecated_paths = dict()
 
     def _return_path_list(self, data_type):
-        paths = self.io_dict[data_type]['path']
+        paths = self.io_dict[data_type]["path"]
         # Convert paths to list
         if not isinstance(paths, list):
             # from string
             if isinstance(paths, str):
                 paths = [paths]
             elif isinstance(paths, dict):
                 # from string in dictionary
                 paths = list(paths.values())
                 if len(paths) > 0:
                     # from nested list in dictionary
                     if isinstance(paths[0], list):
                         paths = list(itertools.chain.from_iterable(paths))
                     # from nested dictionary in dictionary
                     elif isinstance(paths[0], dict):
-                        paths = list(itertools.chain.from_iterable(
-                            [d.values() for d in paths]))
+                        paths = list(
+                            itertools.chain.from_iterable([d.values() for d in paths])
+                        )
 
         return paths
 
     def load_file_parameter_file(self):
-        self.file_parameters_path = join(self.save_dir,
-                                         f'_{self.name}_file_parameters.json')
+        self.file_parameters_path = join(
+            self.save_dir, f"_{self.name}_file_parameters.json"
+        )
         try:
-            with open(self.file_parameters_path, 'r') as file:
-                self.file_parameters = json.load(file,
-                                                 object_hook=type_json_hook)
+            with open(self.file_parameters_path, "r") as file:
+                self.file_parameters = json.load(file, object_hook=type_json_hook)
         except (json.JSONDecodeError, FileNotFoundError):
             self.file_parameters = dict()
 
     def save_file_parameter_file(self):
         # Save File-Parameters file
-        with open(self.file_parameters_path, 'w') as file:
-            json.dump(self.file_parameters, file, cls=TypedJSONEncoder,
-                      indent=4)
+        with open(self.file_parameters_path, "w") as file:
+            json.dump(self.file_parameters, file, cls=TypedJSONEncoder, indent=4)
 
     def save_file_params(self, path):
-
         # Check existence of path and append appendices for hemispheres
         if not isfile(path):
-            if isfile(path + '-lh.stc'):
-                paths = [path + '-lh.stc', path + '-rh.stc']
+            if isfile(path + "-lh.stc"):
+                paths = [path + "-lh.stc", path + "-rh.stc"]
             else:
                 paths = list()
         else:
             paths = [path]
 
         for path in paths:
             file_name = Path(path).name
 
             if file_name not in self.file_parameters:
                 self.file_parameters[file_name] = dict()
             # Get the name of the calling function (assuming it is 2 Frames
             # above when running in pipeline)
             function = inspect.stack()[2][3]
-            self.file_parameters[file_name]['FUNCTION'] = function
+            self.file_parameters[file_name]["FUNCTION"] = function
 
             if function in self.ct.pd_funcs.index:
-                critical_params_str = self.ct.pd_funcs.loc[
-                    function, 'func_args']
+                critical_params_str = self.ct.pd_funcs.loc[function, "func_args"]
                 # Make sure there are no spaces left
-                critical_params_str = critical_params_str.replace(' ', '')
-                critical_params = critical_params_str.split(',')
+                critical_params_str = critical_params_str.replace(" ", "")
+                critical_params = critical_params_str.split(",")
 
                 # Add critical parameters
                 for p_name in [p for p in self.pa if p in critical_params]:
                     self.file_parameters[file_name][p_name] = self.pa[p_name]
 
-            self.file_parameters[file_name]['NAME'] = self.name
+            self.file_parameters[file_name]["NAME"] = self.name
 
-            self.file_parameters[file_name]['TIME'] = str(datetime.now())
+            self.file_parameters[file_name]["TIME"] = str(datetime.now())
 
-            self.file_parameters[file_name]['SIZE'] = getsize(path)
+            self.file_parameters[file_name]["SIZE"] = getsize(path)
 
-            self.file_parameters[file_name]['P_PRESET'] = self.p_preset
+            self.file_parameters[file_name]["P_PRESET"] = self.p_preset
 
         self.save_file_parameter_file()
 
     def clean_file_parameters(self):
         remove_files = list()
         n_remove_params = 0
         for file_name in self.file_parameters:
-
             # Can be changed to only relative path (12.02.2021)
             if not isfile(join(self.save_dir, file_name)):
                 remove_files.append(file_name)
 
             # Remove lists (can be removed soon 12.02.2021)
-            if isinstance(self.file_parameters[file_name]['FUNCTION'], list):
-                self.file_parameters[file_name]['FUNCTION'] = \
-                    self.file_parameters[file_name]['FUNCTION'][0]
-            if isinstance(self.file_parameters[file_name]['TIME'], list):
-                self.file_parameters[file_name]['TIME'] = \
-                    self.file_parameters[file_name]['TIME'][0]
+            if isinstance(self.file_parameters[file_name]["FUNCTION"], list):
+                self.file_parameters[file_name]["FUNCTION"] = self.file_parameters[
+                    file_name
+                ]["FUNCTION"][0]
+            if isinstance(self.file_parameters[file_name]["TIME"], list):
+                self.file_parameters[file_name]["TIME"] = self.file_parameters[
+                    file_name
+                ]["TIME"][0]
 
-            function = self.file_parameters[file_name]['FUNCTION']
+            function = self.file_parameters[file_name]["FUNCTION"]
             # ToDo: Why is there sometimes <module> as FUNCTION?
-            if function == '<module>' \
-                    or function not in self.ct.pd_funcs.index:
+            if function == "<module>" or function not in self.ct.pd_funcs.index:
                 pass
             else:
                 remove_params = list()
-                critical_params_str = self.ct.pd_funcs.loc[
-                    function, 'func_args']
+                critical_params_str = self.ct.pd_funcs.loc[function, "func_args"]
                 # Make sure there are no spaces left
-                critical_params_str = critical_params_str.replace(' ', '')
-                critical_params = critical_params_str.split(',')
-                critical_params += ['FUNCTION', 'NAME', 'TIME', 'SIZE',
-                                    'P_PRESET']
+                critical_params_str = critical_params_str.replace(" ", "")
+                critical_params = critical_params_str.split(",")
+                critical_params += ["FUNCTION", "NAME", "TIME", "SIZE", "P_PRESET"]
 
                 for param in self.file_parameters[file_name]:
                     if param not in critical_params:
                         remove_params.append(param)
 
                 for param in remove_params:
                     self.file_parameters[file_name].pop(param)
 
                 n_remove_params += len(remove_params)
 
         for file_name in remove_files:
             self.file_parameters.pop(file_name)
-        print(f'Removed {len(remove_files)} Files '
-              f'and {n_remove_params} Parameters.')
+        print(
+            f"Removed {len(remove_files)} Files " f"and {n_remove_params} Parameters."
+        )
         self.save_file_parameter_file()
 
     # Todo: Type recognition
-    def plot_save(self, plot_name, subfolder=None, trial=None, idx=None,
-                  matplotlib_figure=None, brain=None, brain_movie_kwargs=None,
-                  dpi=None, img_format=None):
+    def plot_save(
+        self,
+        plot_name,
+        subfolder=None,
+        trial=None,
+        idx=None,
+        matplotlib_figure=None,
+        brain=None,
+        brain_movie_kwargs=None,
+        dpi=None,
+        img_format=None,
+    ):
         """
         Save a plot with this method either by letting the figure be detected
          by the backend (pyplot, mayavi) or by
         supplying the figure directly.
 
         Parameters
         ----------
@@ -377,15 +391,15 @@
                 base_name_sequence.insert(1, trial)
             if subfolder:
                 base_name_sequence.append(subfolder)
             if idx is not None:
                 base_name_sequence.append(str(idx))
 
             # Join name-parts together with "--" and append the image-format
-            file_name = '--'.join(base_name_sequence)
+            file_name = "--".join(base_name_sequence)
             file_name += self.img_format
 
             save_path = join(dir_path, file_name)
             # Get the plot-function and the save the path to the image
             calling_func = inspect.stack()[1][3]
 
             # Check if required keys are in the dictionary-levels
@@ -393,93 +407,95 @@
                 self.plot_files[calling_func] = list()
 
             if matplotlib_figure:
                 if isinstance(matplotlib_figure, list):
                     for ix, figure in enumerate(matplotlib_figure):
                         # Insert additional index in front of image-format
                         # (easier with removesuffix when moving to 3.9)
-                        idx_file_name = \
-                            f'{file_name[:-len(self.img_format)]}' \
-                            f'--{ix}{self.img_format}'
+                        idx_file_name = (
+                            f"{file_name[:-len(self.img_format)]}"
+                            f"--{ix}{self.img_format}"
+                        )
                         idx_file_path = join(dir_path, idx_file_name)
                         figure.savefig(idx_file_path)
-                        print(f'figure: {idx_file_path} has been saved')
+                        print(f"figure: {idx_file_path} has been saved")
                         # Only store relative path to be compatible across OS
                         plot_files_save_path = os.path.relpath(
-                            idx_file_path, self.figures_path)
+                            idx_file_path, self.figures_path
+                        )
                         # Add Plot-Save-Path to plot_files
                         # if not already contained
-                        if plot_files_save_path \
-                                not in self.plot_files[calling_func]:
-                            self.plot_files[calling_func].append(
-                                plot_files_save_path)
+                        if plot_files_save_path not in self.plot_files[calling_func]:
+                            self.plot_files[calling_func].append(plot_files_save_path)
                 else:
                     matplotlib_figure.savefig(save_path, dpi=dpi)
             elif brain:
                 if brain_movie_kwargs is not None:
-                    time_dilation = brain_movie_kwargs['stc_animation_dilat']
-                    tmin, tmax = brain_movie_kwargs['stc_animation_span']
-                    brain.save_movie(save_path, time_dilation=time_dilation,
-                                     tmin=tmin, tmax=tmax)
+                    time_dilation = brain_movie_kwargs["stc_animation_dilat"]
+                    tmin, tmax = brain_movie_kwargs["stc_animation_span"]
+                    brain.save_movie(
+                        save_path, time_dilation=time_dilation, tmin=tmin, tmax=tmax
+                    )
                 else:
                     brain.save_image(save_path)
             else:
                 plt.savefig(save_path, dpi=dpi)
-            print(f'figure: {save_path} has been saved')
+            print(f"figure: {save_path} has been saved")
 
             if not isinstance(matplotlib_figure, list):
                 # Only store relative path to be compatible across OS
-                plot_files_save_path = os.path.relpath(save_path,
-                                                       self.figures_path)
+                plot_files_save_path = os.path.relpath(save_path, self.figures_path)
                 # Add Plot-Save-Path to plot_files if not already contained
                 if plot_files_save_path not in self.plot_files[calling_func]:
                     self.plot_files[calling_func].append(plot_files_save_path)
         else:
             print('Not saving plots; set "save_plots" to "True" to save')
 
     def load_json(self, file_name, default=None):
-        file_path = join(self.save_dir,
-                         f'{self.name}_{self.p_preset}_{file_name}.json')
+        file_path = join(self.save_dir, f"{self.name}_{self.p_preset}_{file_name}.json")
         try:
-            with open(file_path, 'r') as file:
+            with open(file_path, "r") as file:
                 data = json.load(file, object_hook=type_json_hook)
         except json.JSONDecodeError:
-            print(f'{file_path} could not be loaded')
+            print(f"{file_path} could not be loaded")
             data = default
         except FileNotFoundError:
-            print(f'{file_path} could not be found')
+            print(f"{file_path} could not be found")
             data = default
 
         return data
 
     def save_json(self, file_name, data):
         # If file-ending is supplied, remove it to avoid doubling
-        if file_name[-5:] == '.json':
+        if file_name[-5:] == ".json":
             file_name = file_name[:-5]
-        file_path = join(self.save_dir,
-                         f'{self.name}_{self.p_preset}_{file_name}.json')
+        file_path = join(self.save_dir, f"{self.name}_{self.p_preset}_{file_name}.json")
         try:
-            with open(file_path, 'w') as file:
+            with open(file_path, "w") as file:
                 json.dump(data, file, cls=TypedJSONEncoder, indent=4)
         except json.JSONDecodeError:
-            print(f'{file_path} could not be saved')
+            print(f"{file_path} could not be saved")
 
         self.save_file_params(file_path)
 
     def get_existing_paths(self):
         """Get existing paths and add the mapped File-Type
-         to existing_paths (set)"""
+        to existing_paths (set)"""
         self.existing_paths.clear()
         for data_type in self.io_dict:
             paths = self._return_path_list(data_type)
             if paths:
-                self.existing_paths[data_type] = [p for p in paths if
-                                                  isfile(p) or isdir(p)
-                                                  or isfile(p + '-lh.stc')
-                                                  or isfile(p + '-rh.stc')]
+                self.existing_paths[data_type] = [
+                    p
+                    for p in paths
+                    if isfile(p)
+                    or isdir(p)
+                    or isfile(p + "-lh.stc")
+                    or isfile(p + "-rh.stc")
+                ]
             else:
                 self.existing_paths[data_type] = list()
 
     def remove_path(self, data_type):
         # Remove path specified by path_type (which is the name
         # mapped to the path in self.paths_dict)
         # Dependent on Paramter-Preset
@@ -488,346 +504,416 @@
             p_name = Path(p).name
             # Remove from file-parameters
             try:
                 self.file_parameters.pop(p_name)
             except KeyError:
                 # Accounting for Source-Estimate naming-conventions
                 try:
-                    p_name_lh = p_name + '-lh.stc'
-                    p_name_rh = p_name + '-rh.stc'
+                    p_name_lh = p_name + "-lh.stc"
+                    p_name_rh = p_name + "-rh.stc"
                     for pn in [p_name_lh, p_name_rh]:
                         self.file_parameters.pop(pn)
                 except KeyError:
-                    print(f'{Path(p).name} not in file-parameters')
+                    print(f"{Path(p).name} not in file-parameters")
             try:
                 remove(p)
             except FileNotFoundError:
                 # Accounting for Source-Estimate naming-conventions
                 try:
-                    p_lh = p + '-lh.stc'
-                    p_rh = p + '-rh.stc'
+                    p_lh = p + "-lh.stc"
+                    p_rh = p + "-rh.stc"
                     for ps in [p_lh, p_rh]:
                         os.remove(ps)
                 except FileNotFoundError:
-                    print(f'{p} was not found')
+                    print(f"{p} was not found")
             except IsADirectoryError:
                 try:
                     shutil.rmtree(p)
                 except OSError as err:
-                    print(f'{p} could not be removed due to {err}')
+                    print(f"{p} could not be removed due to {err}")
             except OSError as err:
-                print(f'{p} could not be removed due to {err}')
+                print(f"{p} could not be removed due to {err}")
 
 
 class MEEG(BaseLoading):
-    """ Class for File-Data in File-Loop"""
+    """Class for File-Data in File-Loop"""
 
     def __init__(self, name, controller, fsmri=None, suppress_warnings=True):
         self.fsmri = fsmri
         self.suppress_warnings = suppress_warnings
         super().__init__(name, controller)
 
-        if name == '_sample_':
+        if name == "_sample_":
             self.init_sample()
 
     def init_attributes(self):
         """Initialize additional attributes for MEEG"""
         # The assigned Empty-Room-Measurement if existing
         if self.name not in self.pr.meeg_to_erm:
             self.erm = None
             if not self.suppress_warnings:
                 print(
-                    f'No Empty-Room-Measurement assigned for {self.name},'
-                    f' defaulting to "None"')
+                    f"No Empty-Room-Measurement assigned for {self.name},"
+                    f' defaulting to "None"'
+                )
         else:
             # Transition from 'None' to None (placed 30.01.2021,
             # can be removed soon)
-            if self.pr.meeg_to_erm[self.name] == 'None':
+            if self.pr.meeg_to_erm[self.name] == "None":
                 self.pr.meeg_to_erm[self.name] = None
             self.erm = self.pr.meeg_to_erm[self.name]
 
         # The assigned Freesurfer-MRI(already as FSMRI-Class)
         if self.name in self.pr.meeg_to_fsmri:
-            if self.fsmri \
-                    and self.fsmri.name == self.pr.meeg_to_fsmri[self.name]:
+            if self.fsmri and self.fsmri.name == self.pr.meeg_to_fsmri[self.name]:
                 pass
             else:
                 self.fsmri = FSMRI(self.pr.meeg_to_fsmri[self.name], self.ct)
         else:
             self.fsmri = FSMRI(None, self.ct)
             if not self.suppress_warnings:
                 print(
-                    f'No Freesurfer-MRI-Subject assigned for {self.name},'
-                    f' defaulting to "None"')
+                    f"No Freesurfer-MRI-Subject assigned for {self.name},"
+                    f' defaulting to "None"'
+                )
 
         # The assigned bad-channels
         if self.name not in self.pr.meeg_bad_channels:
             self.bad_channels = list()
             if not self.suppress_warnings:
                 print(
-                    f'No bad channels assigned for {self.name},'
-                    f' defaulting to empty list')
+                    f"No bad channels assigned for {self.name},"
+                    f" defaulting to empty list"
+                )
         else:
             self.bad_channels = self.pr.meeg_bad_channels[self.name]
 
         # The selected trials from the event-id
         if self.name not in self.pr.sel_event_id:
             self.sel_trials = list()
             if not self.suppress_warnings:
                 print(
-                    f'No Trials selected for {self.name},'
-                    f' defaulting to empty list')
+                    f"No Trials selected for {self.name}," f" defaulting to empty list"
+                )
         else:
             self.sel_trials = self.pr.sel_event_id[self.name]
 
         # The assigned event-id
         if self.name not in self.pr.meeg_event_id:
             self.event_id = dict()
             if not self.suppress_warnings:
                 print(
-                    f'No EventID assigned for {self.name},'
-                    f' defaulting to empty dictionary')
+                    f"No EventID assigned for {self.name},"
+                    f" defaulting to empty dictionary"
+                )
         else:
             # Only inlcude event-ids which are selected
             self.event_id = {
-                key: value for key, value
-                in self.pr.meeg_event_id[self.name].items()
-                if any([k in self.sel_trials for k in key.split('/')])
+                key: value
+                for key, value in self.pr.meeg_event_id[self.name].items()
+                if any([k in self.sel_trials for k in key.split("/")])
             }
 
     def init_paths(self):
         """Load Paths as attributes
-         (depending on which Parameter-Preset is selected)"""
+        (depending on which Parameter-Preset is selected)"""
 
         # Main save directory
         self.save_dir = join(self.pr.data_path, self.name)
         if not isdir(self.save_dir):
             os.mkdir(self.save_dir)
 
         # Data-Paths
-        self.raw_path = join(self.save_dir, f'{self.name}-raw.fif')
+        self.raw_path = join(self.save_dir, f"{self.name}-raw.fif")
         self.raw_filtered_path = join(
-            self.save_dir, f'{self.name}_{self.p_preset}-filtered-raw.fif')
+            self.save_dir, f"{self.name}_{self.p_preset}-filtered-raw.fif"
+        )
         if self.erm:
-            self.erm_path = join(self.pr.data_path, self.erm,
-                                 f'{self.erm}-raw.fif')
+            self.erm_path = join(self.pr.data_path, self.erm, f"{self.erm}-raw.fif")
             self.old_erm_processed_path = join(
-                self.pr.data_path, self.erm,
-                f'{self.erm}_{self.p_preset}-raw.fif')
+                self.pr.data_path, self.erm, f"{self.erm}_{self.p_preset}-raw.fif"
+            )
             self.erm_processed_path = join(
-                self.pr.data_path, self.erm,
-                f'{self.erm}-{self.name}_{self.p_preset}-processed-raw.fif')
+                self.pr.data_path,
+                self.erm,
+                f"{self.erm}-{self.name}_{self.p_preset}-processed-raw.fif",
+            )
         else:
             self.erm_path = None
             self.erm_processed_path = None
-        self.events_path = join(self.save_dir,
-                                f'{self.name}_{self.p_preset}-eve.fif')
-        self.epochs_path = join(self.save_dir,
-                                f'{self.name}_{self.p_preset}-epo.fif')
-        self.reject_log_path = join(self.save_dir,
-                                    f'{self.name}_{self.p_preset}-arlog.py')
-        self.ica_path = join(self.save_dir,
-                             f'{self.name}_{self.p_preset}-ica.fif')
-        self.eog_epochs_path = join(self.save_dir,
-                                    f'{self.name}_{self.p_preset}-eog-epo.fif')
-        self.ecg_epochs_path = join(self.save_dir,
-                                    f'{self.name}_{self.p_preset}-ecg-epo.fif')
-        self.evokeds_path = join(self.save_dir,
-                                 f'{self.name}_{self.p_preset}-ave.fif')
+        self.events_path = join(self.save_dir, f"{self.name}_{self.p_preset}-eve.fif")
+        self.epochs_path = join(self.save_dir, f"{self.name}_{self.p_preset}-epo.fif")
+        self.reject_log_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-arlog.py"
+        )
+        self.ica_path = join(self.save_dir, f"{self.name}_{self.p_preset}-ica.fif")
+        self.eog_epochs_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-eog-epo.fif"
+        )
+        self.ecg_epochs_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-ecg-epo.fif"
+        )
+        self.evokeds_path = join(self.save_dir, f"{self.name}_{self.p_preset}-ave.fif")
         self.power_tfr_epochs_path = join(
             self.save_dir,
-            f'{self.name}_{self.p_preset}_'
-            f'#{self.pa["tfr_method"]}-epo-pw-tfr.h5')
+            f"{self.name}_{self.p_preset}_" f'#{self.pa["tfr_method"]}-epo-pw-tfr.h5',
+        )
         self.itc_tfr_epochs_path = join(
             self.save_dir,
-            f'{self.name}_{self.p_preset}_'
-            f'{self.pa["tfr_method"]}-epo-itc-tfr.h5')
+            f"{self.name}_{self.p_preset}_" f'{self.pa["tfr_method"]}-epo-itc-tfr.h5',
+        )
         self.power_tfr_average_path = join(
             self.save_dir,
-            f'{self.name}_{self.p_preset}_'
-            f'{self.pa["tfr_method"]}-ave-pw-tfr.h5')
+            f"{self.name}_{self.p_preset}_" f'{self.pa["tfr_method"]}-ave-pw-tfr.h5',
+        )
         self.itc_tfr_average_path = join(
             self.save_dir,
-            f'{self.name}_{self.p_preset}_'
-            f'{self.pa["tfr_method"]}-ave-itc-tfr.h5')
-        self.trans_path = join(self.save_dir, f'{self.fsmri.name}-trans.fif')
-        self.forward_path = join(self.save_dir,
-                                 f'{self.name}_{self.p_preset}-fwd.fif')
+            f"{self.name}_{self.p_preset}_" f'{self.pa["tfr_method"]}-ave-itc-tfr.h5',
+        )
+        self.trans_path = join(self.save_dir, f"{self.fsmri.name}-trans.fif")
+        self.forward_path = join(self.save_dir, f"{self.name}_{self.p_preset}-fwd.fif")
         self.source_morph_path = join(
-            self.save_dir, f'{self.name}--to--{self.pa["morph_to"]}_'
-                           f'{self.pa["src_spacing"]}-morph.h5')
-        self.calm_cov_path = join(self.save_dir,
-                                  f'{self.name}_{self.p_preset}-calm-cov.fif')
-        self.erm_cov_path = join(self.save_dir,
-                                 f'{self.name}_{self.p_preset}-erm-cov.fif')
+            self.save_dir,
+            f'{self.name}--to--{self.pa["morph_to"]}_'
+            f'{self.pa["src_spacing"]}-morph.h5',
+        )
+        self.calm_cov_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-calm-cov.fif"
+        )
+        self.erm_cov_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-erm-cov.fif"
+        )
         self.noise_covariance_path = join(
-            self.save_dir, f'{self.name}_{self.p_preset}-cov.fif')
-        self.inverse_path = join(
-            self.save_dir, f'{self.name}_{self.p_preset}-inv.fif')
-        self.stc_paths = {trial: join(
-            self.save_dir, f'{self.name}_{trial}_{self.p_preset}-stc')
-            for trial in self.sel_trials}
+            self.save_dir, f"{self.name}_{self.p_preset}-cov.fif"
+        )
+        self.inverse_path = join(self.save_dir, f"{self.name}_{self.p_preset}-inv.fif")
+        self.stc_paths = {
+            trial: join(self.save_dir, f"{self.name}_{trial}_{self.p_preset}-stc")
+            for trial in self.sel_trials
+        }
         self.morphed_stc_paths = {
-            trial: join(self.save_dir,
-                        f'{self.name}_{trial}_{self.p_preset}-morphed')
-            for trial in self.sel_trials}
-        self.ecd_paths = {trial: {dip: join(
-            self.save_dir, 'ecd_dipoles',
-            f'{self.name}_{trial}_{self.p_preset}_{dip}-ecd-dip.dip')
-            for dip in self.pa['ecd_times']}
-            for trial in self.sel_trials}
+            trial: join(self.save_dir, f"{self.name}_{trial}_{self.p_preset}-morphed")
+            for trial in self.sel_trials
+        }
+        self.ecd_paths = {
+            trial: {
+                dip: join(
+                    self.save_dir,
+                    "ecd_dipoles",
+                    f"{self.name}_{trial}_{self.p_preset}_{dip}-ecd-dip.dip",
+                )
+                for dip in self.pa["ecd_times"]
+            }
+            for trial in self.sel_trials
+        }
         self.ltc_paths = {
-            trial: {label: join(
-                self.save_dir, 'label_time_course',
-                f'{self.name}_{trial}_{self.p_preset}_{label}-ltc.npy')
-                for label in self.pa['target_labels']}
-            for trial in self.sel_trials}
-        self.con_paths = {trial: {con_method: join(
-            self.save_dir,
-            f'{self.name}_{trial}_{self.p_preset}_{con_method}-con.npy')
-            for con_method in self.pa['con_methods']}
-            for trial in self.sel_trials}
+            trial: {
+                label: join(
+                    self.save_dir,
+                    "label_time_course",
+                    f"{self.name}_{trial}_{self.p_preset}_{label}-ltc.npy",
+                )
+                for label in self.pa["target_labels"]
+            }
+            for trial in self.sel_trials
+        }
+        self.con_paths = {
+            trial: {
+                con_method: join(
+                    self.save_dir,
+                    f"{self.name}_{trial}_{self.p_preset}_{con_method}-con.npy",
+                )
+                for con_method in self.pa["con_methods"]
+            }
+            for trial in self.sel_trials
+        }
 
         # This dictionary contains entries for each data-type
         # which is loaded to/saved from disk
-        self.io_dict = {'raw': {'path': self.raw_path,
-                                'load': self.load_raw,
-                                'save': self.save_raw},
-                        'raw_filtered': {'path': self.raw_filtered_path,
-                                         'load': self.load_filtered,
-                                         'save': self.save_filtered},
-                        'erm': {'path': self.erm_path,
-                                'load': self.load_erm,
-                                'save': None},
-                        'erm_filtered': {'path': self.erm_processed_path,
-                                         'load': self.load_erm_processed,
-                                         'save': self.save_erm_processed},
-                        'events': {'path': self.events_path,
-                                   'load': self.load_events,
-                                   'save': self.save_events},
-                        'epochs': {'path': self.epochs_path,
-                                   'load': self.load_epochs,
-                                   'save': self.save_epochs},
-                        'reject_log': {'path': self.reject_log_path,
-                                       'load': self.load_reject_log,
-                                       'save': self.save_reject_log},
-                        'ica': {'path': self.ica_path,
-                                'load': self.load_ica,
-                                'save': self.save_ica},
-                        'epochs_eog': {'path': self.eog_epochs_path,
-                                       'load': self.load_eog_epochs,
-                                       'save': self.save_eog_epochs},
-                        'epochs_ecg': {'path': self.ecg_epochs_path,
-                                       'load': self.load_ecg_epochs,
-                                       'save': self.save_ecg_epochs},
-                        'evoked': {'path': self.evokeds_path,
-                                   'load': self.load_evokeds,
-                                   'save': self.save_evokeds},
-                        'tf_power_epochs': {
-                            'path': self.power_tfr_epochs_path,
-                            'load': self.load_power_tfr_epochs,
-                            'save': self.save_power_tfr_epochs},
-                        'tf_itc_epochs': {'path': self.itc_tfr_epochs_path,
-                                          'load': self.load_itc_tfr_epochs,
-                                          'save': self.save_itc_tfr_epochs},
-                        'tf_power_average': {
-                            'path': self.power_tfr_average_path,
-                            'load': self.load_power_tfr_average,
-                            'save': self.save_power_tfr_average},
-                        'tf_itc_average': {'path': self.itc_tfr_average_path,
-                                           'load': self.load_itc_tfr_average,
-                                           'save': self.save_itc_tfr_average},
-                        'trans': {'path': self.trans_path,
-                                  'load': self.load_transformation,
-                                  'save': None},
-                        'forward': {'path': self.forward_path,
-                                    'load': self.load_forward,
-                                    'save': self.save_forward},
-                        'morph': {'path': self.source_morph_path,
-                                  'load': self.load_source_morph,
-                                  'save': self.save_source_morph},
-                        'noise_cov': {'path': self.noise_covariance_path,
-                                      'load': self.load_noise_covariance,
-                                      'save': self.save_noise_covariance},
-                        'inverse': {'path': self.inverse_path,
-                                    'load': self.load_inverse_operator,
-                                    'save': self.save_inverse_operator},
-                        'stcs': {'path': self.stc_paths,
-                                 'load': self.load_source_estimates,
-                                 'save': self.save_source_estimates},
-                        'stcs_morphed': {
-                            'path': self.morphed_stc_paths,
-                            'load': self.load_morphed_source_estimates,
-                            'save': self.save_morphed_source_estimates},
-                        'ecd': {'path': self.ecd_paths,
-                                'load': self.load_ecd,
-                                'save': self.save_ecd},
-                        'ltc': {'path': self.ltc_paths,
-                                'load': self.load_ltc,
-                                'save': self.save_ltc},
-                        'src_con': {'path': self.con_paths,
-                                    'load': self.load_connectivity,
-                                    'save': self.save_connectivity}}
-
-        self.deprecated_paths = {'stcs': {trial: join(
-            self.save_dir, f'{self.name}_{trial}_{self.p_preset}')
-            for trial in self.sel_trials}}
+        self.io_dict = {
+            "raw": {
+                "path": self.raw_path,
+                "load": self.load_raw,
+                "save": self.save_raw,
+            },
+            "raw_filtered": {
+                "path": self.raw_filtered_path,
+                "load": self.load_filtered,
+                "save": self.save_filtered,
+            },
+            "erm": {"path": self.erm_path, "load": self.load_erm, "save": None},
+            "erm_filtered": {
+                "path": self.erm_processed_path,
+                "load": self.load_erm_processed,
+                "save": self.save_erm_processed,
+            },
+            "events": {
+                "path": self.events_path,
+                "load": self.load_events,
+                "save": self.save_events,
+            },
+            "epochs": {
+                "path": self.epochs_path,
+                "load": self.load_epochs,
+                "save": self.save_epochs,
+            },
+            "reject_log": {
+                "path": self.reject_log_path,
+                "load": self.load_reject_log,
+                "save": self.save_reject_log,
+            },
+            "ica": {
+                "path": self.ica_path,
+                "load": self.load_ica,
+                "save": self.save_ica,
+            },
+            "epochs_eog": {
+                "path": self.eog_epochs_path,
+                "load": self.load_eog_epochs,
+                "save": self.save_eog_epochs,
+            },
+            "epochs_ecg": {
+                "path": self.ecg_epochs_path,
+                "load": self.load_ecg_epochs,
+                "save": self.save_ecg_epochs,
+            },
+            "evoked": {
+                "path": self.evokeds_path,
+                "load": self.load_evokeds,
+                "save": self.save_evokeds,
+            },
+            "tf_power_epochs": {
+                "path": self.power_tfr_epochs_path,
+                "load": self.load_power_tfr_epochs,
+                "save": self.save_power_tfr_epochs,
+            },
+            "tf_itc_epochs": {
+                "path": self.itc_tfr_epochs_path,
+                "load": self.load_itc_tfr_epochs,
+                "save": self.save_itc_tfr_epochs,
+            },
+            "tf_power_average": {
+                "path": self.power_tfr_average_path,
+                "load": self.load_power_tfr_average,
+                "save": self.save_power_tfr_average,
+            },
+            "tf_itc_average": {
+                "path": self.itc_tfr_average_path,
+                "load": self.load_itc_tfr_average,
+                "save": self.save_itc_tfr_average,
+            },
+            "trans": {
+                "path": self.trans_path,
+                "load": self.load_transformation,
+                "save": None,
+            },
+            "forward": {
+                "path": self.forward_path,
+                "load": self.load_forward,
+                "save": self.save_forward,
+            },
+            "morph": {
+                "path": self.source_morph_path,
+                "load": self.load_source_morph,
+                "save": self.save_source_morph,
+            },
+            "noise_cov": {
+                "path": self.noise_covariance_path,
+                "load": self.load_noise_covariance,
+                "save": self.save_noise_covariance,
+            },
+            "inverse": {
+                "path": self.inverse_path,
+                "load": self.load_inverse_operator,
+                "save": self.save_inverse_operator,
+            },
+            "stcs": {
+                "path": self.stc_paths,
+                "load": self.load_source_estimates,
+                "save": self.save_source_estimates,
+            },
+            "stcs_morphed": {
+                "path": self.morphed_stc_paths,
+                "load": self.load_morphed_source_estimates,
+                "save": self.save_morphed_source_estimates,
+            },
+            "ecd": {
+                "path": self.ecd_paths,
+                "load": self.load_ecd,
+                "save": self.save_ecd,
+            },
+            "ltc": {
+                "path": self.ltc_paths,
+                "load": self.load_ltc,
+                "save": self.save_ltc,
+            },
+            "src_con": {
+                "path": self.con_paths,
+                "load": self.load_connectivity,
+                "save": self.save_connectivity,
+            },
+        }
+
+        self.deprecated_paths = {
+            "stcs": {
+                trial: join(self.save_dir, f"{self.name}_{trial}_{self.p_preset}")
+                for trial in self.sel_trials
+            }
+        }
 
     def init_sample(self):
         # Add _sample_ to project and update attributes
-        self.pr.all_erm.append('ernoise')
-        self.erm = 'ernoise'
+        self.pr.all_erm.append("ernoise")
+        self.erm = "ernoise"
         self.pr.meeg_to_erm[self.name] = self.erm
         self.init_paths()
 
         # Load sample
-        test_data_folder = join(mne.datasets.sample.data_path(), 'MEG',
-                                'sample')
+        test_data_folder = join(mne.datasets.sample.data_path(), "MEG", "sample")
         test_file_dict = sample_paths
 
         for data_type in test_file_dict:
             test_file_name = test_file_dict[data_type]
             test_file_path = join(test_data_folder, test_file_name)
-            file_path = self.io_dict[data_type]['path']
+            file_path = self.io_dict[data_type]["path"]
 
             if isfile(test_file_path) and not isfile(file_path):
-                print(f'Copying {data_type} from sample-dataset...')
+                print(f"Copying {data_type} from sample-dataset...")
                 folder = Path(file_path).parent
                 if not isdir(folder):
                     os.mkdir(folder)
                 shutil.copy2(test_file_path, file_path)
-                print('Done!')
+                print("Done!")
 
-        self.bad_channels = self.load_info()['bads']
+        self.bad_channels = self.load_info()["bads"]
         self.pr.meeg_bad_channels[self.name] = self.bad_channels
 
     def rename(self, new_name):
         # Stor old name
         old_name = self.name
         all_old_paths = dict()
         for data_type in self.io_dict:
             all_old_paths[data_type] = self._return_path_list(data_type)
 
         # Update paths
         self.name = new_name
         self.init_paths()
 
-        self.pr.all_meeg = [new_name if n == old_name else n for n in
-                            self.pr.all_meeg]
+        self.pr.all_meeg = [new_name if n == old_name else n for n in self.pr.all_meeg]
         if old_name in self.pr.sel_meeg:
-            self.pr.sel_meeg = [new_name if n == old_name else n for n in
-                                self.pr.sel_meeg]
+            self.pr.sel_meeg = [
+                new_name if n == old_name else n for n in self.pr.sel_meeg
+            ]
 
         # Update entries in dictionaries
         # ToDo: Rename Plot-Files
         # ToDo: Rename File-Parameters
         self.pr.meeg_to_erm[self.name] = self.pr.meeg_to_erm.pop(old_name)
         self.pr.meeg_to_fsmri[self.name] = self.pr.meeg_to_fsmri.pop(old_name)
-        self.pr.meeg_bad_channels[self.name] = self.pr.meeg_bad_channels.pop(
-            old_name)
+        self.pr.meeg_bad_channels[self.name] = self.pr.meeg_bad_channels.pop(old_name)
         self.pr.meeg_event_id[self.name] = self.pr.meeg_event_id.pop(old_name)
         self.pr.sel_event_id[self.name] = self.pr.sel_event_id.pop(old_name)
         self.init_attributes()
 
         # Rename old paths to new paths
         for data_type in self.io_dict:
             new_paths = self._return_path_list(data_type)
@@ -842,77 +928,76 @@
 
     def load_info(self):
         return mne.io.read_info(self.raw_path)
 
     @load_decorator
     def load_raw(self):
         raw = mne.io.read_raw_fif(self.raw_path, preload=True)
-        raw.info['bads'] = [bc for bc in self.bad_channels if
-                            bc in raw.ch_names]
+        raw.info["bads"] = [bc for bc in self.bad_channels if bc in raw.ch_names]
         return raw
 
     @save_decorator
     def save_raw(self, raw):
         raw.save(self.raw_path, fmt=raw.orig_format, overwrite=True)
 
     @load_decorator
     def load_filtered(self):
         raw = mne.io.read_raw_fif(self.raw_filtered_path, preload=True)
-        raw.info['bads'] = [bc for bc in self.bad_channels if
-                            bc in raw.ch_names]
+        raw.info["bads"] = [bc for bc in self.bad_channels if bc in raw.ch_names]
         return raw
 
     @save_decorator
     def save_filtered(self, raw_filtered):
-        raw_filtered.save(self.raw_filtered_path, fmt=raw_filtered.orig_format,
-                          overwrite=True)
+        raw_filtered.save(
+            self.raw_filtered_path, fmt=raw_filtered.orig_format, overwrite=True
+        )
 
     @load_decorator
     def load_erm(self):
         erm_raw = mne.io.read_raw_fif(self.erm_path, preload=True)
-        if self.erm in self.pr.meeg_bad_channels:
-            erm_raw.info['bads'] = self.pr.meeg_bad_channels[self.erm]
         return erm_raw
 
     @load_decorator
     def load_erm_processed(self):
         if isfile(self.old_erm_processed_path):
             os.remove(self.old_erm_processed_path)
         return mne.io.read_raw_fif(self.erm_processed_path, preload=True)
 
     @save_decorator
     def save_erm_processed(self, erm_filtered):
-        erm_filtered.save(self.erm_processed_path,
-                          fmt=erm_filtered.orig_format, overwrite=True)
+        erm_filtered.save(
+            self.erm_processed_path, fmt=erm_filtered.orig_format, overwrite=True
+        )
 
     @load_decorator
     def load_events(self):
         return mne.read_events(self.events_path)
 
     @save_decorator
     def save_events(self, events):
-        mne.event.write_events(self.events_path, events, overwrite=True)
+        mne.write_events(self.events_path, events, overwrite=True)
 
     @load_decorator
     def load_epochs(self):
-        return mne.read_epochs(self.epochs_path, proj=self.pa['apply_proj'],
-                               preload=True)
+        return mne.read_epochs(
+            self.epochs_path, proj=self.pa["apply_proj"], preload=True
+        )
 
     @save_decorator
     def save_epochs(self, epochs):
         epochs.save(self.epochs_path, overwrite=True)
 
     @load_decorator
     def load_reject_log(self):
-        with open(self.reject_log_path, 'rb') as file:
+        with open(self.reject_log_path, "rb") as file:
             return pickle.load(file)
 
     @save_decorator
     def save_reject_log(self, reject_log):
-        with open(self.reject_log_path, 'wb') as file:
+        with open(self.reject_log_path, "wb") as file:
             pickle.dump(reject_log, file)
 
     @load_decorator
     def load_ica(self):
         ica = mne.preprocessing.read_ica(self.ica_path)
         # Change ica.exclude to indices stored in ica_exclude.py
         # for this MEEG-Object
@@ -938,63 +1023,63 @@
 
     @save_decorator
     def save_ecg_epochs(self, ecg_epochs):
         ecg_epochs.save(self.ecg_epochs_path, overwrite=True)
 
     @load_decorator
     def load_evokeds(self):
-        return mne.read_evokeds(self.evokeds_path, proj=self.pa['apply_proj'])
+        return mne.read_evokeds(self.evokeds_path, proj=self.pa["apply_proj"])
 
     @save_decorator
     def save_evokeds(self, evokeds):
         mne.evoked.write_evokeds(self.evokeds_path, evokeds, overwrite=True)
 
     @load_decorator
     def load_power_tfr_epochs(self):
         return mne.time_frequency.read_tfrs(self.power_tfr_epochs_path)
 
     @save_decorator
     def save_power_tfr_epochs(self, powers):
-        mne.time_frequency.write_tfrs(self.power_tfr_epochs_path, powers,
-                                      overwrite=True)
+        mne.time_frequency.write_tfrs(
+            self.power_tfr_epochs_path, powers, overwrite=True
+        )
 
     @load_decorator
     def load_itc_tfr_epochs(self):
         return mne.time_frequency.read_tfrs(self.itc_tfr_epochs_path)
 
     @save_decorator
     def save_itc_tfr_epochs(self, itcs):
-        mne.time_frequency.write_tfrs(self.itc_tfr_epochs_path, itcs,
-                                      overwrite=True)
+        mne.time_frequency.write_tfrs(self.itc_tfr_epochs_path, itcs, overwrite=True)
 
     @load_decorator
     def load_power_tfr_average(self):
         return mne.time_frequency.read_tfrs(self.power_tfr_average_path)
 
     @save_decorator
     def save_power_tfr_average(self, powers):
-        mne.time_frequency.write_tfrs(self.power_tfr_average_path, powers,
-                                      overwrite=True)
+        mne.time_frequency.write_tfrs(
+            self.power_tfr_average_path, powers, overwrite=True
+        )
 
     @load_decorator
     def load_itc_tfr_average(self):
         return mne.time_frequency.read_tfrs(self.itc_tfr_average_path)
 
     @save_decorator
     def save_itc_tfr_average(self, itcs):
-        mne.time_frequency.write_tfrs(self.itc_tfr_average_path, itcs,
-                                      overwrite=True)
+        mne.time_frequency.write_tfrs(self.itc_tfr_average_path, itcs, overwrite=True)
 
     @load_decorator
     def load_transformation(self):
         return mne.read_trans(self.trans_path)
 
     @load_decorator
     def load_forward(self):
-        return mne.read_forward_solution(self.forward_path, verbose='WARNING')
+        return mne.read_forward_solution(self.forward_path, verbose="WARNING")
 
     @save_decorator
     def save_forward(self, forward):
         mne.write_forward_solution(self.forward_path, forward, overwrite=True)
 
     @load_decorator
     def load_source_morph(self):
@@ -1006,135 +1091,140 @@
 
     @load_decorator
     def load_noise_covariance(self):
         return mne.read_cov(self.noise_covariance_path)
 
     @save_decorator
     def save_noise_covariance(self, noise_cov):
-        mne.cov.write_cov(self.noise_covariance_path, noise_cov,
-                          overwrite=True)
+        mne.cov.write_cov(self.noise_covariance_path, noise_cov, overwrite=True)
 
     @load_decorator
     def load_inverse_operator(self):
-        return mne.minimum_norm.read_inverse_operator(self.inverse_path,
-                                                      verbose='WARNING')
+        return mne.minimum_norm.read_inverse_operator(
+            self.inverse_path, verbose="WARNING"
+        )
 
     @save_decorator
     def save_inverse_operator(self, inverse):
-        mne.minimum_norm.write_inverse_operator(self.inverse_path, inverse,
-                                                overwrite=True)
+        mne.minimum_norm.write_inverse_operator(
+            self.inverse_path, inverse, overwrite=True
+        )
 
     @load_decorator
     def load_source_estimates(self):
         stcs = dict()
         for trial in self.stc_paths:
             stcs[trial] = mne.source_estimate.read_source_estimate(
-                self.stc_paths[trial])
+                self.stc_paths[trial]
+            )
 
         return stcs
 
     @save_decorator
     def save_source_estimates(self, stcs):
         for trial in stcs:
-            stcs[trial].save(self.stc_paths[trial])
+            stcs[trial].save(self.stc_paths[trial], overwrite=True)
 
     @load_decorator
     def load_morphed_source_estimates(self):
         morphed_stcs = dict()
         for trial in self.morphed_stc_paths:
             morphed_stcs[trial] = mne.source_estimate.read_source_estimate(
-                self.morphed_stc_paths[trial])
+                self.morphed_stc_paths[trial]
+            )
 
         return morphed_stcs
 
     @save_decorator
     def save_morphed_source_estimates(self, morphed_stcs):
         for trial in morphed_stcs:
-            morphed_stcs[trial].save(self.morphed_stc_paths[trial],
-                                     overwrite=True)
+            morphed_stcs[trial].save(self.morphed_stc_paths[trial], overwrite=True)
 
     def load_mixn_dipoles(self):
         mixn_dips = dict()
         for trial in self.sel_trials:
             idx = 0
             dip_list = list()
-            for idx in range(
-                    len(listdir(join(self.save_dir, 'mixn_dipoles')))):
-                mixn_dip_path = join(self.save_dir, 'mixn_dipoles',
-                                     f'{self.name}_{trial}_'
-                                     f'{self.p_preset}-mixn-dip{idx}.dip')
+            for idx in range(len(listdir(join(self.save_dir, "mixn_dipoles")))):
+                mixn_dip_path = join(
+                    self.save_dir,
+                    "mixn_dipoles",
+                    f"{self.name}_{trial}_" f"{self.p_preset}-mixn-dip{idx}.dip",
+                )
                 dip_list.append(mne.read_dipole(mixn_dip_path))
                 idx += 1
             mixn_dips[trial] = dip_list
-            print(f'{idx + 1} dipoles read for {self.name}-{trial}')
+            print(f"{idx + 1} dipoles read for {self.name}-{trial}")
 
         return mixn_dips
 
     def save_mixn_dipoles(self, mixn_dips):
         # Remove old dipoles
-        if not exists(join(self.save_dir, 'mixn_dipoles')):
-            makedirs(join(self.save_dir, 'mixn_dipoles'))
-        old_dipoles = listdir(join(self.save_dir, 'mixn_dipoles'))
+        if not exists(join(self.save_dir, "mixn_dipoles")):
+            makedirs(join(self.save_dir, "mixn_dipoles"))
+        old_dipoles = listdir(join(self.save_dir, "mixn_dipoles"))
         for file in old_dipoles:
-            remove(join(self.save_dir, 'mixn_dipoles', file))
+            remove(join(self.save_dir, "mixn_dipoles", file))
 
         for trial in mixn_dips:
             for idx, dip in enumerate(mixn_dips[trial]):
-                mxn_dip_path = join(self.save_dir, 'mixn_dipoles',
-                                    f'{self.name}_{trial}_'
-                                    f'{self.p_preset}-mixn-dip{idx}.dip')
+                mxn_dip_path = join(
+                    self.save_dir,
+                    "mixn_dipoles",
+                    f"{self.name}_{trial}_" f"{self.p_preset}-mixn-dip{idx}.dip",
+                )
                 dip.save(mxn_dip_path, overwrite=True)
 
     def load_mixn_source_estimates(self):
         mixn_stcs = dict()
         for trial in self.sel_trials:
-            mx_stc_path = join(self.save_dir,
-                               f'{self.name}_{trial}_{self.p_preset}-mixn')
+            mx_stc_path = join(
+                self.save_dir, f"{self.name}_{trial}_{self.p_preset}-mixn"
+            )
             mx_stc = mne.source_estimate.read_source_estimate(mx_stc_path)
             mixn_stcs.update({trial: mx_stc})
 
         return mixn_stcs
 
     def save_mixn_source_estimates(self, stcs):
         for trial in stcs:
-            stc_path = join(self.save_dir,
-                            f'{self.name}_{trial}_{self.p_preset}-mixn')
-            stcs[trial].save(stc_path)
+            stc_path = join(self.save_dir, f"{self.name}_{trial}_{self.p_preset}-mixn")
+            stcs[trial].save(stc_path, overwrite=True)
 
     @load_decorator
     def load_ecd(self):
         ecd_dipoles = dict()
         for trial in self.ecd_paths:
             ecd_dipoles[trial] = dict()
             for dip in self.ecd_paths[trial]:
-                ecd_dipoles[trial][dip] = mne.read_dipole(
-                    self.ecd_paths[trial][dip])
+                ecd_dipoles[trial][dip] = mne.read_dipole(self.ecd_paths[trial][dip])
 
         return ecd_dipoles
 
     @save_decorator
     def save_ecd(self, ecd_dips):
         for trial in ecd_dips:
             for dip in ecd_dips[trial]:
-                ecd_dips[trial][dip].save(self.ecd_paths[trial][dip],
-                                          overwrite=True)
+                ecd_dips[trial][dip].save(self.ecd_paths[trial][dip], overwrite=True)
 
     @load_decorator
     def load_ltc(self):
         ltcs = dict()
         for trial in self.sel_trials:
             ltcs[trial] = dict()
             for label in self.ltc_paths[trial]:
                 ltc_path = self.ltc_paths[trial][label]
                 if isfile(ltc_path):
                     ltcs[trial][label] = np.load(ltc_path)
                 else:
-                    raise FileNotFoundError(f'No Label-Time-Course found '
-                                            f'for trial {trial} '
-                                            f'in label {label}!')
+                    raise FileNotFoundError(
+                        f"No Label-Time-Course found "
+                        f"for trial {trial} "
+                        f"in label {label}!"
+                    )
 
         return ltcs
 
     @save_decorator
     def save_ltc(self, ltcs):
         for trial in ltcs:
             for label in ltcs[trial]:
@@ -1142,142 +1232,162 @@
 
     @load_decorator
     def load_connectivity(self):
         con_dict = dict()
         for trial in self.con_paths:
             con_dict[trial] = dict()
             for con_method in self.con_paths[trial]:
-                con_dict[trial][con_method] = np.load(
-                    self.con_paths[trial][con_method])
+                con_dict[trial][con_method] = np.load(self.con_paths[trial][con_method])
 
         return con_dict
 
     @save_decorator
     def save_connectivity(self, con_dict):
         for trial in con_dict:
             for con_method in con_dict[trial]:
-                np.save(self.con_paths[trial][con_method],
-                        con_dict[trial][con_method])
+                np.save(self.con_paths[trial][con_method], con_dict[trial][con_method])
 
 
 class FSMRI(BaseLoading):
-    def __init__(self, name, controller):
-        if name == 'fsaverage':
+    def __init__(self, name, controller, load_labels=False):
+        if name == "fsaverage" and not isfile(
+            join(controller.subjects_dir, "fsaverage/mri/T1.mgz")
+        ):
             if _test_run():
-                test_data_folder = join(mne.datasets.sample.data_path(),
-                                        'subjects',
-                                        'fsaverage')
-                shutil.copytree(test_data_folder,
-                                join(controller.subjects_dir, name))
+                test_data_folder = join(
+                    mne.datasets.sample.data_path(), "subjects", "fsaverage"
+                )
+                shutil.copytree(test_data_folder, join(controller.subjects_dir, name))
             else:
                 try:
-                    logging.info('Downloading fsaverage...')
-                    mne.datasets.fetch_fsaverage(
-                        subjects_dir=controller.subjects_dir)
+                    logging.info("Downloading fsaverage...")
+                    mne.datasets.fetch_fsaverage(subjects_dir=controller.subjects_dir)
                 # Not working on macOS for mne<=0.24
                 except ValueError:
-                    logging.warning('fsaverage could not be downloaded!')
+                    logging.warning("fsaverage could not be downloaded!")
 
+        self.load_labels = load_labels
         super().__init__(name, controller)
 
     def init_attributes(self):
         """Initialize additional attributes for FSMRI"""
-        self.fs_path = QS().value('fs_path')
-        self.mne_path = QS().value('mne_path')
+        self.fs_path = QS().value("fs_path")
+        self.mne_path = QS().value("mne_path")
 
         # Initialize Parcellations and Labels
-        self.parcellations = self._get_available_parc()
-        self.labels = self._get_available_labels()
+        if self.load_labels:
+            self.parcellations = self._get_available_parc()
+            self.labels = self._get_available_labels()
+        else:
+            self.parcellations = None
+            self.labels = None
 
     def init_paths(self):
         # Main Path
         self.save_dir = join(self.subjects_dir, self.name)
 
         # Data-Paths
         self.src_path = join(
-            self.save_dir, 'bem',
-            f'{self.name}_{self.p_preset}_{self.pa["src_spacing"]}-src.fif')
+            self.save_dir,
+            "bem",
+            f'{self.name}_{self.p_preset}_{self.pa["src_spacing"]}-src.fif',
+        )
         self.bem_model_path = join(
-            self.save_dir, 'bem',
-            f'{self.name}_{self.p_preset}-bem.fif')
+            self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem.fif"
+        )
         self.bem_solution_path = join(
-            self.save_dir, 'bem',
-            f'{self.name}_{self.p_preset}-bem-sol.fif')
+            self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem-sol.fif"
+        )
         self.vol_src_path = join(
-            self.save_dir, 'bem',
-            f'{self.name}_{self.p_preset}-vol-src.fif')
+            self.save_dir, "bem", f"{self.name}_{self.p_preset}-vol-src.fif"
+        )
 
         # This dictionary contains entries for each data-type
         # which is loaded to/saved from disk
         self.io_dict = {
-            'src': {'path': self.src_path,
-                    'load': self.load_source_space,
-                    'save': self.save_source_space},
-            'bem_model': {'path': self.bem_model_path,
-                          'load': self.load_bem_model,
-                          'save': self.save_bem_model},
-            'bem_solution': {'path': self.bem_solution_path,
-                             'load': self.load_bem_solution,
-                             'save': self.save_bem_solution},
-            'volume_src': {'path': self.vol_src_path,
-                           'load': self.load_volume_source_space,
-                           'save': self.save_volume_source_space}
+            "src": {
+                "path": self.src_path,
+                "load": self.load_source_space,
+                "save": self.save_source_space,
+            },
+            "bem_model": {
+                "path": self.bem_model_path,
+                "load": self.load_bem_model,
+                "save": self.save_bem_model,
+            },
+            "bem_solution": {
+                "path": self.bem_solution_path,
+                "load": self.load_bem_solution,
+                "save": self.save_bem_solution,
+            },
+            "volume_src": {
+                "path": self.vol_src_path,
+                "load": self.load_volume_source_space,
+                "save": self.save_volume_source_space,
+            },
         }
 
         self.deprecated_paths = {
-            'src': join(self.save_dir, 'bem',
-                        f'{self.name}_{self.pa["src_spacing"]}-src.fif'),
-            'bem_model': join(self.save_dir, 'bem',
-                              f'{self.name}-bem.fif'),
-            'bem_solution': join(self.save_dir, 'bem',
-                                 f'{self.name}-bem-sol.fif'),
-            'volume_src': join(self.save_dir, 'bem',
-                               f'{self.name}-vol-src.fif')
+            "src": join(
+                self.save_dir, "bem", f'{self.name}_{self.pa["src_spacing"]}-src.fif'
+            ),
+            "bem_model": join(self.save_dir, "bem", f"{self.name}-bem.fif"),
+            "bem_solution": join(self.save_dir, "bem", f"{self.name}-bem-sol.fif"),
+            "volume_src": join(self.save_dir, "bem", f"{self.name}-vol-src.fif"),
         }
 
     def _get_available_parc(self):
-        annot_dir = join(self.subjects_dir, self.name, 'label')
+        annot_dir = join(self.subjects_dir, self.name, "label")
         try:
             files = os.listdir(annot_dir)
-            annotations = [file[3:-6] for file in files
-                           if file[-6:] == '.annot']
+            annotations = [file[3:-6] for file in files if file[-6:] == ".annot"]
         except FileNotFoundError:
             annotations = list()
 
         return annotations
 
     def _get_available_labels(self):
         labels = dict()
-        label_dir = join(self.subjects_dir, self.name, 'label')
+        labels["Other"] = list()
+        label_dir = join(self.subjects_dir, self.name, "label")
         try:
             files = os.listdir(label_dir)
-            labels['Other'] = list()
             for label_path in tqdm(
-                    [str(lp) for lp in files if lp[-6:] == '.label'],
-                    desc='Loading labels...',
-                    ascii=True):
-                label = mne.read_label(join(label_dir, label_path),
-                                       self.name)
-                labels['Other'].append(label)
+                [str(lp) for lp in files if lp[-6:] == ".label"],
+                desc="Loading labels...",
+                ascii=True,
+            ):
+                label = mne.read_label(join(label_dir, label_path), self.name)
+                labels["Other"].append(label)
         except FileNotFoundError:
-            logging.warning(f'No label directory found for {self.name}!')
+            logging.warning(f"No label directory found for {self.name}!")
 
-        for parcellation in tqdm(self.parcellations,
-                                 desc='Loading parcellations...',
-                                 ascii=True):
-            labels[parcellation] = mne.read_labels_from_annot(
-                self.name, parcellation, subjects_dir=self.subjects_dir,
-                verbose='warning'
-            )
+        if self.parcellations is None:
+            self.parcellations = self._get_available_parc()
+
+        for parcellation in tqdm(
+            self.parcellations, desc="Loading parcellations...", ascii=True
+        ):
+            try:
+                labels[parcellation] = mne.read_labels_from_annot(
+                    self.name,
+                    parcellation,
+                    subjects_dir=self.subjects_dir,
+                    verbose="warning",
+                )
+            except RuntimeError:
+                print(f"Parcellation {parcellation} could not be loaded!")
 
         return labels
 
     def get_labels(self, target_labels):
         labels = list()
-        if hasattr(self, 'labels'):
+        if target_labels is not None:
+            if self.labels is None:
+                self.labels = self._get_available_labels()
             for label_list in self.labels.values():
                 labels += [lb for lb in label_list if lb.name in target_labels]
 
         return labels
 
     ###########################################################################
     # Load- & Save-Methods
@@ -1300,16 +1410,15 @@
 
     @load_decorator
     def load_bem_solution(self):
         return mne.read_bem_solution(self.bem_solution_path)
 
     @save_decorator
     def save_bem_solution(self, bem_solution):
-        mne.write_bem_solution(self.bem_solution_path, bem_solution,
-                               overwrite=True)
+        mne.write_bem_solution(self.bem_solution_path, bem_solution, overwrite=True)
 
     @load_decorator
     def load_volume_source_space(self):
         return mne.read_source_spaces(self.vol_src_path)
 
     @save_decorator
     def save_volume_source_space(self, vol_src):
@@ -1323,131 +1432,163 @@
 
     def init_attributes(self):
         """Initialize additional attributes for Group"""
         if self.name not in self.pr.all_groups:
             self.group_list = []
             if not self.suppress_warnings:
                 print(
-                    f'No objects assigned for {self.name},'
-                    f' defaulting to empty list')
+                    f"No objects assigned for {self.name}," f" defaulting to empty list"
+                )
         else:
             self.group_list = self.pr.all_groups[self.name]
 
         # The assigned event-id
         self.event_id = dict()
-        for group_item in [gi for gi in self.group_list if
-                           gi in self.ct.pr.meeg_event_id]:
-            self.event_id = {**self.event_id,
-                             **self.ct.pr.meeg_event_id[group_item]}
+        for group_item in [
+            gi for gi in self.group_list if gi in self.ct.pr.meeg_event_id
+        ]:
+            self.event_id = {**self.event_id, **self.ct.pr.meeg_event_id[group_item]}
 
         # The selected trials from the event-id
         self.sel_trials = set()
-        for group_item in [gi for gi in self.group_list if
-                           gi in self.ct.pr.sel_event_id]:
-            self.sel_trials = self.sel_trials | set(
-                self.ct.pr.sel_event_id[group_item])
+        for group_item in [
+            gi for gi in self.group_list if gi in self.ct.pr.sel_event_id
+        ]:
+            self.sel_trials = self.sel_trials | set(self.ct.pr.sel_event_id[group_item])
 
         # The fsmri where all group members are morphed to
-        self.fsmri = FSMRI(self.pa['morph_to'], self.ct)
+        self.fsmri = FSMRI(self.pa["morph_to"], self.ct)
 
     def init_paths(self):
         # Main Path
         self.save_dir = self.pr.save_dir_averages
         if not isdir(self.save_dir):
             os.mkdir(self.save_dir)
 
         # Data Paths
-        self.ga_evokeds_paths = {trial: join(self.save_dir, 'evokeds',
-                                             f'{self.name}_{trial}_'
-                                             f'{self.p_preset}-ave.fif')
-                                 for trial in self.sel_trials}
-        self.ga_tfr_paths = {trial: join(self.save_dir, 'time-frequency',
-                                         f'{self.name}_{trial}_'
-                                         f'{self.p_preset}-tfr.h5')
-                             for trial in self.sel_trials}
-        self.ga_stc_paths = {trial: join(self.save_dir, 'source-estimates',
-                                         f'{self.name}_{trial}_'
-                                         f'{self.p_preset}')
-                             for trial in self.sel_trials}
+        self.ga_evokeds_paths = {
+            trial: join(
+                self.save_dir,
+                "evokeds",
+                f"{self.name}_{trial}_" f"{self.p_preset}-ave.fif",
+            )
+            for trial in self.sel_trials
+        }
+        self.ga_tfr_paths = {
+            trial: join(
+                self.save_dir,
+                "time-frequency",
+                f"{self.name}_{trial}_" f"{self.p_preset}-tfr.h5",
+            )
+            for trial in self.sel_trials
+        }
+        self.ga_stc_paths = {
+            trial: join(
+                self.save_dir,
+                "source-estimates",
+                f"{self.name}_{trial}_" f"{self.p_preset}",
+            )
+            for trial in self.sel_trials
+        }
         self.ga_ltc_paths = {
-            trial: {label: join(self.save_dir, 'label-time-courses',
-                                f'{self.name}_{trial}_'
-                                f'{self.p_preset}_{label}.npy')
-                    for label in self.pa['target_labels']}
-            for trial in self.sel_trials}
+            trial: {
+                label: join(
+                    self.save_dir,
+                    "label-time-courses",
+                    f"{self.name}_{trial}_" f"{self.p_preset}_{label}.npy",
+                )
+                for label in self.pa["target_labels"]
+            }
+            for trial in self.sel_trials
+        }
         self.ga_con_paths = {
-            trial: {con_method: join(self.save_dir, 'connectivity',
-                                     f'{self.name}_{trial}_'
-                                     f'{self.p_preset}_{con_method}.npy')
-                    for con_method in self.pa['con_methods']}
-            for trial in self.sel_trials}
+            trial: {
+                con_method: join(
+                    self.save_dir,
+                    "connectivity",
+                    f"{self.name}_{trial}_" f"{self.p_preset}_{con_method}.npy",
+                )
+                for con_method in self.pa["con_methods"]
+            }
+            for trial in self.sel_trials
+        }
 
         # This dictionary contains entries for each data-type
         # which is loaded to/saved from disk
-        self.io_dict = {'grand_avg_evoked': {'path': self.ga_evokeds_paths,
-                                             'load': self.load_ga_evokeds,
-                                             'save': self.save_ga_evokeds},
-                        'grand_avg_tfr': {'path': self.ga_tfr_paths,
-                                          'load': self.load_ga_tfr,
-                                          'save': self.save_ga_tfr},
-                        'grand_avg_stc': {'path': self.ga_stc_paths,
-                                          'load': self.load_ga_stc,
-                                          'save': self.save_ga_stc},
-                        'grand_avg_ltc': {'path': self.ga_ltc_paths,
-                                          'load': self.load_ga_ltc,
-                                          'save': self.save_ga_ltc},
-                        'grand_avg_src_con': {
-                            'path': self.ga_con_paths,
-                            'load': self.load_ga_con,
-                            'save': self.save_ga_con}}
+        self.io_dict = {
+            "grand_avg_evoked": {
+                "path": self.ga_evokeds_paths,
+                "load": self.load_ga_evokeds,
+                "save": self.save_ga_evokeds,
+            },
+            "grand_avg_tfr": {
+                "path": self.ga_tfr_paths,
+                "load": self.load_ga_tfr,
+                "save": self.save_ga_tfr,
+            },
+            "grand_avg_stc": {
+                "path": self.ga_stc_paths,
+                "load": self.load_ga_stc,
+                "save": self.save_ga_stc,
+            },
+            "grand_avg_ltc": {
+                "path": self.ga_ltc_paths,
+                "load": self.load_ga_ltc,
+                "save": self.save_ga_ltc,
+            },
+            "grand_avg_src_con": {
+                "path": self.ga_con_paths,
+                "load": self.load_ga_con,
+                "save": self.save_ga_con,
+            },
+        }
 
         self.deprecated_paths = {}
 
     ###########################################################################
     # Load- & Save-Methods
     ###########################################################################
-    def load_items(self, obj_type='MEEG', data_type=None):
+    def load_items(self, obj_type="MEEG", data_type=None):
         """Returns a generator for group items."""
         for obj_name in self.group_list:
-            if obj_type == 'MEEG':
+            if obj_type == "MEEG":
                 obj = MEEG(obj_name, self.ct)
-            elif obj_type == 'FSMRI':
+            elif obj_type == "FSMRI":
                 obj = FSMRI(obj_name, self.ct)
             else:
-                logging.error(f'The object-type {obj_type} is not valid!')
+                logging.error(f"The object-type {obj_type} is not valid!")
                 continue
             if data_type is None:
                 yield obj
             elif data_type in obj.io_dict:
-                data = obj.io_dict[data_type]['load']()
-                yield data
+                data = obj.io_dict[data_type]["load"]()
+                yield data, obj
             else:
-                logging.error(f'{data_type} is not valid for {obj_type}')
+                logging.error(f"{data_type} is not valid for {obj_type}")
 
     @load_decorator
     def load_ga_evokeds(self):
         ga_evokeds = dict()
         for trial in self.sel_trials:
-            ga_evokeds[trial] = mne.read_evokeds(
-                self.ga_evokeds_paths[trial])[0]
+            ga_evokeds[trial] = mne.read_evokeds(self.ga_evokeds_paths[trial])[0]
 
         return ga_evokeds
 
     @save_decorator
     def save_ga_evokeds(self, ga_evokeds):
         for trial in ga_evokeds:
-            mne.evoked.write_evokeds(self.ga_evokeds_paths[trial],
-                                     ga_evokeds[trial])
+            mne.evoked.write_evokeds(
+                self.ga_evokeds_paths[trial], ga_evokeds[trial], overwrite=True
+            )
 
     @load_decorator
     def load_ga_tfr(self):
         ga_tfr = dict()
         for trial in self.sel_trials:
-            ga_tfr[trial] = \
-                mne.time_frequency.read_tfrs(self.ga_tfr_paths[trial])[0]
+            ga_tfr[trial] = mne.time_frequency.read_tfrs(self.ga_tfr_paths[trial])[0]
 
         return ga_tfr
 
     @save_decorator
     def save_ga_tfr(self, ga_tfr):
         for trial in ga_tfr:
             ga_tfr[trial].save(self.ga_tfr_paths[trial], overwrite=True)
@@ -1459,15 +1600,15 @@
             ga_stcs[trial] = mne.read_source_estimate(self.ga_stc_paths[trial])
 
         return ga_stcs
 
     @save_decorator
     def save_ga_stc(self, ga_stcs):
         for trial in ga_stcs:
-            ga_stcs[trial].save(self.ga_stc_paths[trial])
+            ga_stcs[trial].save(self.ga_stc_paths[trial], overwrite=True)
 
     @load_decorator
     def load_ga_ltc(self):
         ga_ltc = dict()
         for trial in self.ga_ltc_paths:
             ga_ltc[trial] = dict()
             for label in self.ga_ltc_paths[trial]:
@@ -1484,17 +1625,17 @@
     @load_decorator
     def load_ga_con(self):
         ga_connect = dict()
         for trial in self.ga_con_paths:
             ga_connect[trial] = {}
             for con_method in self.ga_con_paths[trial]:
                 ga_connect[trial][con_method] = np.load(
-                    self.ga_con_paths[trial][con_method])
+                    self.ga_con_paths[trial][con_method]
+                )
 
         return ga_connect
 
     @save_decorator
     def save_ga_con(self, ga_con):
         for trial in ga_con:
             for con_method in ga_con[trial]:
-                np.save(self.ga_con_paths[trial][con_method],
-                        ga_con[trial][con_method])
+                np.save(self.ga_con_paths[trial][con_method], ga_con[trial][con_method])
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/pipeline_utils.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/pipeline_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 import json
 import logging
 import os
 import sys
@@ -18,61 +16,61 @@
 from importlib import resources
 from os.path import join, isfile
 from pathlib import Path
 
 import numpy as np
 import psutil
 
-datetime_format = '%d.%m.%Y %H:%M:%S'
+datetime_format = "%d.%m.%Y %H:%M:%S"
 
 ismac = sys.platform.startswith("darwin")
 iswin = sys.platform.startswith("win32")
 islin = not ismac and not iswin
 
 
 def encode_tuples(input_dict):
     """Encode tuples in a dictionary, because JSON does not recognize them
     (CAVE: input_dict is changed in place)"""
     for key, value in input_dict.items():
         if isinstance(value, dict):
             encode_tuples(value)
         else:
             if isinstance(value, tuple):
-                input_dict[key] = {'tuple_type': value}
+                input_dict[key] = {"tuple_type": value}
 
 
 class TypedJSONEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.integer):
             return int(obj)
         elif isinstance(obj, np.floating):
             return float(obj)
         elif isinstance(obj, np.ndarray):
-            return {'numpy_array': obj.tolist()}
+            return {"numpy_array": obj.tolist()}
         elif isinstance(obj, datetime):
-            return {'datetime': obj.strftime(datetime_format)}
+            return {"datetime": obj.strftime(datetime_format)}
         elif isinstance(obj, set):
-            return {'set_type': list(obj)}
+            return {"set_type": list(obj)}
         else:
             return json.JSONEncoder.default(self, obj)
 
 
 def type_json_hook(obj):
-    if 'numpy_int' in obj.keys():
-        return obj['numpy_int']
-    elif 'numpy_float' in obj.keys():
-        return obj['numpy_float']
-    elif 'numpy_array' in obj.keys():
-        return np.asarray(obj['numpy_array'])
-    elif 'datetime' in obj.keys():
-        return datetime.strptime(obj['datetime'], datetime_format)
-    elif 'tuple_type' in obj.keys():
-        return tuple(obj['tuple_type'])
-    elif 'set_type' in obj.keys():
-        return set(obj['set_type'])
+    if "numpy_int" in obj.keys():
+        return obj["numpy_int"]
+    elif "numpy_float" in obj.keys():
+        return obj["numpy_float"]
+    elif "numpy_array" in obj.keys():
+        return np.asarray(obj["numpy_array"])
+    elif "datetime" in obj.keys():
+        return datetime.strptime(obj["datetime"], datetime_format)
+    elif "tuple_type" in obj.keys():
+        return tuple(obj["tuple_type"])
+    elif "set_type" in obj.keys():
+        return set(obj["set_type"])
     else:
         return obj
 
 
 def compare_filep(obj, path, target_parameters=None, verbose=True):
     """Compare the parameters of the previous run to the current
     parameters for the given path
@@ -100,61 +98,65 @@
 
     result_dict = dict()
     file_name = Path(path).name
     # Try to get the parameters relevant for the last function,
     # which altered the data at path
     try:
         # The last entry in FUNCTION should be the most recent
-        function = obj.file_parameters[file_name]['FUNCTION']
-        critical_params_str = obj.ct.pd_funcs.loc[function, 'func_args']
+        function = obj.file_parameters[file_name]["FUNCTION"]
+        critical_params_str = obj.ct.pd_funcs.loc[function, "func_args"]
         # Make sure there are no spaces left
-        critical_params_str = critical_params_str.replace(' ', '')
-        if ',' in critical_params_str:
-            critical_params = critical_params_str.split(',')
+        critical_params_str = critical_params_str.replace(" ", "")
+        if "," in critical_params_str:
+            critical_params = critical_params_str.split(",")
         else:
             critical_params = [critical_params_str]
     except KeyError:
         critical_params = list()
         function = None
 
     if not target_parameters:
         target_parameters = obj.pa.keys()
     for param in target_parameters:
         try:
             previous_value = obj.file_parameters[file_name][param]
             current_value = obj.pa[param]
 
             if str(previous_value) == str(current_value):
-                result_dict[param] = 'equal'
+                result_dict[param] = "equal"
                 if verbose:
-                    print(f'{param} equal for {file_name}')
+                    print(f"{param} equal for {file_name}")
             else:
                 if param in critical_params:
                     result_dict[param] = (previous_value, current_value, True)
                     if verbose:
                         print(
-                            f'{param} changed from {previous_value} to '
-                            f'{current_value} for {file_name} '
-                            f'and is probably crucial for {function}')
+                            f"{param} changed from {previous_value} to "
+                            f"{current_value} for {file_name} "
+                            f"and is probably crucial for {function}"
+                        )
                 else:
                     result_dict[param] = (previous_value, current_value, False)
                     if verbose:
                         print(
-                            f'{param} changed from {previous_value} to '
-                            f'{current_value} for {file_name}')
+                            f"{param} changed from {previous_value} to "
+                            f"{current_value} for {file_name}"
+                        )
         except KeyError:
-            result_dict[param] = 'missing'
+            result_dict[param] = "missing"
             if verbose:
-                print(f'{param} is missing in records for {file_name}')
+                print(f"{param} is missing in records for {file_name}")
 
-    if obj.ct.settings['overwrite']:
-        result_dict[param] = 'overwrite'
+    if obj.ct.settings["overwrite"]:
+        result_dict[param] = "overwrite"
         if verbose:
-            print(f'{file_name} will be overwritten anyway'
-                  f' because Overwrite=True (Settings)')
+            print(
+                f"{file_name} will be overwritten anyway"
+                f" because Overwrite=True (Settings)"
+            )
 
     return result_dict
 
 
 def check_kwargs(kwargs, function):
     kwargs = kwargs.copy()
 
@@ -165,15 +167,15 @@
 
     return kwargs
 
 
 def count_dict_keys(d, max_level=None):
     """Count the number of keys of a nested dictionary"""
     keys = 0
-    for key, value in d.items():
+    for value in d.values():
         if isinstance(value, dict):
             if max_level is None:
                 keys += count_dict_keys(value)
             elif max_level > 1:
                 keys += count_dict_keys(value, max_level - 1)
             else:
                 keys += 1
@@ -181,73 +183,78 @@
             keys += 1
 
     return keys
 
 
 def shutdown():
     if iswin:
-        os.system('shutdown /s')
+        os.system("shutdown /s")
     if islin:
-        os.system('sudo shutdown now')
+        os.system("sudo shutdown now")
     if ismac:
-        os.system('sudo shutdown -h now')
+        os.system("sudo shutdown -h now")
 
 
 def restart_program():
     """Restarts the current program, with file objects and descriptors
-       cleanup."""
-    logging.info('Restarting')
+    cleanup."""
+    logging.info("Restarting")
     try:
         p = psutil.Process(os.getpid())
         for handler in p.open_files() + p.connections():
             os.close(handler.fd)
     except Exception as e:
         logging.error(e)
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
 
 def _get_func_param_kwargs(func, params):
-    kwargs = {kwarg: params[kwarg] if kwarg in params else None
-              for kwarg in inspect.signature(func).parameters}
+    kwargs = {
+        kwarg: params[kwarg] if kwarg in params else None
+        for kwarg in inspect.signature(func).parameters
+    }
 
     return kwargs
 
 
 class BaseSettings:
     def __init__(self):
         # Load default settings
-        with resources.open_text('mne_pipeline_hd.resource',
-                                 'default_settings.json') as file:
-            self.default_qsettings = json.load(file)['qsettings']
+        with resources.open_text(
+            "mne_pipeline_hd.resource", "default_settings.json"
+        ) as file:
+            self.default_qsettings = json.load(file)["qsettings"]
 
     def get_default(self, name):
         if name in self.default_qsettings:
             return self.default_qsettings[name]
         else:
-            raise RuntimeError(f'{name} not in default_settings.json! '
-                               f'Please add it or fix the bug.')
+            raise RuntimeError(
+                f"{name} not in default_settings.json! "
+                f"Please add it or fix the bug."
+            )
 
 
 class QSettingsDummy(BaseSettings):
     def __init__(self):
         super().__init__()
 
-        self.settings_path = join(Path.home(), '.mnephd_settings.json')
+        self.settings_path = join(Path.home(), ".mnephd_settings.json")
 
     def _load_settings(self):
         if isfile(self.settings_path):
-            with open(self.settings_path, 'r') as file:
+            with open(self.settings_path, "r") as file:
                 self.settings = json.load(file)
         else:
             self.settings = deepcopy(self.default_qsettings)
 
     def _write_settings(self):
-        with open(self.settings_path, 'w') as file:
+        with open(self.settings_path, "w") as file:
             json.dump(self.settings, file)
 
     def value(self, setting, defaultValue=None):
         self._load_settings()
         if setting in self.settings:
             return self.settings[setting]
 
@@ -296,17 +303,17 @@
 
     class QS(QSettingsDummy):
         def __init__(self):
             super().__init__()
 
 
 def _set_test_run():
-    os.environ['TEST_RUN'] = 'True'
+    os.environ["TEST_RUN"] = "True"
 
 
 def _test_run():
-    if 'TEST_RUN' in os.environ:
+    if "TEST_RUN" in os.environ:
         return True
 
 
 def _run_from_script():
-    return '__main__.py' in sys.argv[0]
+    return "__main__.py" in sys.argv[0]
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/plot_utils.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/plot_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import functools
 
 from mne_pipeline_hd.gui.plot_widgets import show_plot_manager
 
 
 def pipeline_plot(plot_func):
     @functools.wraps(plot_func)
     def func_wrapper(*args, **kwargs):
-        obj = [kwargs.get(kw, None) for kw in ['meeg', 'fsmri', 'group']
-               if kwargs.get(kw, None) is not None][0]
-        use_plot_manager = obj.ct.settings['use_plot_manager']
-        if use_plot_manager and 'show_plots' in kwargs:
-            kwargs['show_plots'] = False
+        obj = [
+            kwargs.get(kw, None)
+            for kw in ["meeg", "fsmri", "group"]
+            if kwargs.get(kw, None) is not None
+        ][0]
+        use_plot_manager = obj.ct.settings["use_plot_manager"]
+        if use_plot_manager and "show_plots" in kwargs:
+            kwargs["show_plots"] = False
         plot = plot_func(*args, **kwargs)
         if use_plot_manager and plot is not None:
             if not isinstance(plot, list):
                 plot = [plot]
             plot_manager = show_plot_manager()
             plot_manager.add_plot(plot, obj.name, plot_func.__name__)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/pipeline/project.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import json
 import logging
 import os
 import shutil
 from ast import literal_eval
@@ -18,17 +16,20 @@
 from pathlib import Path
 
 import mne
 import numpy as np
 
 from mne_pipeline_hd.pipeline.legacy import renamed_parameters
 from mne_pipeline_hd.pipeline.loading import MEEG, FSMRI, Group
-from mne_pipeline_hd.pipeline.pipeline_utils import TypedJSONEncoder, \
-    count_dict_keys, \
-    encode_tuples, type_json_hook
+from mne_pipeline_hd.pipeline.pipeline_utils import (
+    TypedJSONEncoder,
+    count_dict_keys,
+    encode_tuples,
+    type_json_hook,
+)
 
 
 class Project:
     """
     A class with attributes for all the paths, file-lists/dicts
     and parameters of the selected project
     """
@@ -42,37 +43,40 @@
         self.init_pipeline_scripts()
         self.load()
         self.save()
         # ToDo: MacOs weird folders added (.DSStore)
         # self.check_data()
 
     def init_main_paths(self):
-
         # Main folder of project
         self.project_path = join(self.ct.projects_path, self.name)
         # Folder to store the data
-        self.data_path = join(self.project_path, 'data')
+        self.data_path = join(self.project_path, "data")
         # Folder to store the figures (with an additional subfolder
         # for each parameter-preset)
-        self.figures_path = join(self.project_path, 'figures')
+        self.figures_path = join(self.project_path, "figures")
         # A dedicated folder to store grand-average data
-        self.save_dir_averages = join(self.data_path, 'grand_averages')
+        self.save_dir_averages = join(self.data_path, "grand_averages")
         # A folder to store all pipeline-scripts as .json-files
-        self.pscripts_path = join(self.project_path, '_pipeline_scripts')
+        self.pscripts_path = join(self.project_path, "_pipeline_scripts")
 
-        self.main_paths = [self.ct.subjects_dir, self.data_path,
-                           self.save_dir_averages,
-                           self.pscripts_path, self.ct.custom_pkg_path,
-                           self.figures_path]
+        self.main_paths = [
+            self.ct.subjects_dir,
+            self.data_path,
+            self.save_dir_averages,
+            self.pscripts_path,
+            self.ct.custom_pkg_path,
+            self.figures_path,
+        ]
 
         # Create or check existence of main_paths
         for path in self.main_paths:
             if not exists(path):
                 makedirs(path)
-                logging.debug(f'{path} created')
+                logging.debug(f"{path} created")
 
     def init_attributes(self):
         # Stores the names of all MEG/EEG-Files
         self.all_meeg = list()
         # Stores selected MEG/EEG-Files
         self.sel_meeg = list()
         # Stores Bad-Channels for each MEG/EEG-File
@@ -103,102 +107,105 @@
         # Stores functions and if they are selected
         self.sel_functions = list()
         # Stores additional keyword-arguments for functions by function-name
         self.add_kwargs = dict()
         # Stores parameters for each Parameter-Preset
         self.parameters = dict()
         # Parameter-Preset
-        self.p_preset = 'Default'
+        self.p_preset = "Default"
 
         # Attributes, which have their own special function for loading
-        self.special_loads = ['parameters', 'p_preset']
+        self.special_loads = ["parameters", "p_preset"]
 
     def init_pipeline_scripts(self):
         # Initiate Project-Lists and Dicts
-        self.all_meeg_path = join(self.pscripts_path,
-                                  f'all_meeg_{self.name}.json')
-        self.sel_meeg_path = join(self.pscripts_path,
-                                  f'selected_meeg_{self.name}.json')
+        self.all_meeg_path = join(self.pscripts_path, f"all_meeg_{self.name}.json")
+        self.sel_meeg_path = join(self.pscripts_path, f"selected_meeg_{self.name}.json")
         self.meeg_bad_channels_path = join(
-            self.pscripts_path, f'meeg_bad_channels_{self.name}.json')
-        self.meeg_event_id_path = join(self.pscripts_path,
-                                       f'meeg_event_id_{self.name}.json')
-        self.sel_event_id_path = join(self.pscripts_path,
-                                      f'selected_event_ids_{self.name}.json')
-        self.all_erm_path = join(self.pscripts_path,
-                                 f'all_erm_{self.name}.json')
-        self.meeg_to_erm_path = join(self.pscripts_path,
-                                     f'meeg_to_erm_{self.name}.json')
-        self.all_fsmri_path = join(self.pscripts_path,
-                                   f'all_fsmri_{self.name}.json')
-        self.sel_fsmri_path = join(self.pscripts_path,
-                                   f'selected_fsmri_{self.name}.json')
-        self.meeg_to_fsmri_path = join(self.pscripts_path,
-                                       f'meeg_to_fsmri_{self.name}.json')
-        self.ica_exclude_path = join(self.pscripts_path,
-                                     f'ica_exclude_{self.name}.json')
-        self.all_groups_path = join(self.pscripts_path,
-                                    f'all_groups_{self.name}.json')
-        self.sel_groups_path = join(self.pscripts_path,
-                                    f'selected_groups_{self.name}.json')
-        self.plot_files_path = join(self.pscripts_path,
-                                    f'plot_files_{self.name}.json')
-        self.sel_functions_path = join(self.pscripts_path,
-                                       f'selected_functions_{self.name}.json')
-        self.add_kwargs_path = join(self.pscripts_path,
-                                    f'additional_kwargs_{self.name}.json')
-        self.parameters_path = join(self.pscripts_path,
-                                    f'parameters_{self.name}.json')
-        self.sel_p_preset_path = join(self.pscripts_path,
-                                      f'sel_p_preset_{self.name}.json')
+            self.pscripts_path, f"meeg_bad_channels_{self.name}.json"
+        )
+        self.meeg_event_id_path = join(
+            self.pscripts_path, f"meeg_event_id_{self.name}.json"
+        )
+        self.sel_event_id_path = join(
+            self.pscripts_path, f"selected_event_ids_{self.name}.json"
+        )
+        self.all_erm_path = join(self.pscripts_path, f"all_erm_{self.name}.json")
+        self.meeg_to_erm_path = join(
+            self.pscripts_path, f"meeg_to_erm_{self.name}.json"
+        )
+        self.all_fsmri_path = join(self.pscripts_path, f"all_fsmri_{self.name}.json")
+        self.sel_fsmri_path = join(
+            self.pscripts_path, f"selected_fsmri_{self.name}.json"
+        )
+        self.meeg_to_fsmri_path = join(
+            self.pscripts_path, f"meeg_to_fsmri_{self.name}.json"
+        )
+        self.ica_exclude_path = join(
+            self.pscripts_path, f"ica_exclude_{self.name}.json"
+        )
+        self.all_groups_path = join(self.pscripts_path, f"all_groups_{self.name}.json")
+        self.sel_groups_path = join(
+            self.pscripts_path, f"selected_groups_{self.name}.json"
+        )
+        self.plot_files_path = join(self.pscripts_path, f"plot_files_{self.name}.json")
+        self.sel_functions_path = join(
+            self.pscripts_path, f"selected_functions_{self.name}.json"
+        )
+        self.add_kwargs_path = join(
+            self.pscripts_path, f"additional_kwargs_{self.name}.json"
+        )
+        self.parameters_path = join(self.pscripts_path, f"parameters_{self.name}.json")
+        self.sel_p_preset_path = join(
+            self.pscripts_path, f"sel_p_preset_{self.name}.json"
+        )
 
         # Map the paths to their attribute in the Project-Class
         self.path_to_attribute = {
-            self.all_meeg_path: 'all_meeg',
-            self.sel_meeg_path: 'sel_meeg',
-            self.meeg_bad_channels_path: 'meeg_bad_channels',
-            self.meeg_event_id_path: 'meeg_event_id',
-            self.sel_event_id_path: 'sel_event_id',
-            self.all_erm_path: 'all_erm',
-            self.meeg_to_erm_path: 'meeg_to_erm',
-            self.all_fsmri_path: 'all_fsmri',
-            self.sel_fsmri_path: 'sel_fsmri',
-            self.meeg_to_fsmri_path: 'meeg_to_fsmri',
-            self.ica_exclude_path: 'ica_exclude',
-            self.all_groups_path: 'all_groups',
-            self.sel_groups_path: 'sel_groups',
-            self.plot_files_path: 'plot_files',
-            self.sel_functions_path: 'sel_functions',
-            self.add_kwargs_path: 'add_kwargs',
-            self.parameters_path: 'parameters',
-            self.sel_p_preset_path: 'p_preset'}
+            self.all_meeg_path: "all_meeg",
+            self.sel_meeg_path: "sel_meeg",
+            self.meeg_bad_channels_path: "meeg_bad_channels",
+            self.meeg_event_id_path: "meeg_event_id",
+            self.sel_event_id_path: "sel_event_id",
+            self.all_erm_path: "all_erm",
+            self.meeg_to_erm_path: "meeg_to_erm",
+            self.all_fsmri_path: "all_fsmri",
+            self.sel_fsmri_path: "sel_fsmri",
+            self.meeg_to_fsmri_path: "meeg_to_fsmri",
+            self.ica_exclude_path: "ica_exclude",
+            self.all_groups_path: "all_groups",
+            self.sel_groups_path: "sel_groups",
+            self.plot_files_path: "plot_files",
+            self.sel_functions_path: "sel_functions",
+            self.add_kwargs_path: "add_kwargs",
+            self.parameters_path: "parameters",
+            self.sel_p_preset_path: "p_preset",
+        }
 
     def load_lists(self):
         # Old Paths to allow transition (22.11.2020)
-        self.old_all_meeg_path = join(self.pscripts_path, 'file_list.json')
-        self.old_sel_meeg_path = join(self.pscripts_path,
-                                      'selected_files.json')
-        self.old_meeg_bad_channels_path = join(self.pscripts_path,
-                                               'bad_channels_dict.json')
-        self.old_meeg_event_id_path = join(self.pscripts_path,
-                                           'event_id_dict.json')
-        self.old_sel_event_id_path = join(self.pscripts_path,
-                                          'selected_evid_labels.json')
-        self.old_all_erm_path = join(self.pscripts_path, 'erm_list.json')
-        self.old_meeg_to_erm_path = join(self.pscripts_path, 'erm_dict.json')
-        self.old_all_fsmri_path = join(self.pscripts_path, 'mri_sub_list.json')
-        self.old_sel_fsmri_path = join(self.pscripts_path,
-                                       'selected_mri_files.json')
-        self.old_meeg_to_fsmri_path = join(self.pscripts_path, 'sub_dict.json')
-        self.old_all_groups_path = join(self.pscripts_path,
-                                        'grand_avg_dict.json')
-        self.old_sel_groups_path = join(self.pscripts_path,
-                                        'selected_grand_average_groups.json')
-        self.old_sel_funcs_path = join(self.pscripts_path,
-                                       'selected_funcs.json')
+        self.old_all_meeg_path = join(self.pscripts_path, "file_list.json")
+        self.old_sel_meeg_path = join(self.pscripts_path, "selected_files.json")
+        self.old_meeg_bad_channels_path = join(
+            self.pscripts_path, "bad_channels_dict.json"
+        )
+        self.old_meeg_event_id_path = join(self.pscripts_path, "event_id_dict.json")
+        self.old_sel_event_id_path = join(
+            self.pscripts_path, "selected_evid_labels.json"
+        )
+        self.old_all_erm_path = join(self.pscripts_path, "erm_list.json")
+        self.old_meeg_to_erm_path = join(self.pscripts_path, "erm_dict.json")
+        self.old_all_fsmri_path = join(self.pscripts_path, "mri_sub_list.json")
+        self.old_sel_fsmri_path = join(self.pscripts_path, "selected_mri_files.json")
+        self.old_meeg_to_fsmri_path = join(self.pscripts_path, "sub_dict.json")
+        self.old_all_groups_path = join(self.pscripts_path, "grand_avg_dict.json")
+        self.old_sel_groups_path = join(
+            self.pscripts_path, "selected_grand_average_groups.json"
+        )
+        self.old_sel_funcs_path = join(self.pscripts_path, "selected_funcs.json")
 
         # Old Paths to allow transition (22.11.2020)
         self.old_paths = {
             self.all_meeg_path: self.old_all_meeg_path,
             self.sel_meeg_path: self.old_sel_meeg_path,
             self.meeg_bad_channels_path: self.old_meeg_bad_channels_path,
             self.meeg_event_id_path: self.old_meeg_event_id_path,
@@ -206,150 +213,162 @@
             self.all_erm_path: self.old_all_erm_path,
             self.meeg_to_erm_path: self.old_meeg_to_erm_path,
             self.all_fsmri_path: self.old_all_fsmri_path,
             self.sel_fsmri_path: self.old_sel_fsmri_path,
             self.meeg_to_fsmri_path: self.old_meeg_to_fsmri_path,
             self.all_groups_path: self.old_all_groups_path,
             self.sel_groups_path: self.old_sel_groups_path,
-            self.sel_functions_path: self.old_sel_funcs_path}
+            self.sel_functions_path: self.old_sel_funcs_path,
+        }
 
-        for path in [p for p in self.path_to_attribute if
-                     self.path_to_attribute[p] not in self.special_loads]:
+        for path in [
+            p
+            for p in self.path_to_attribute
+            if self.path_to_attribute[p] not in self.special_loads
+        ]:
             attribute_name = self.path_to_attribute[path]
             try:
-                with open(path, 'r') as file:
-                    loaded_attribute = json.load(file,
-                                                 object_hook=type_json_hook)
+                with open(path, "r") as file:
+                    loaded_attribute = json.load(file, object_hook=type_json_hook)
                     # Make sure, that loaded object has same type
                     # as default from __init__
-                    if isinstance(loaded_attribute,
-                                  type(getattr(self, attribute_name))):
+                    if isinstance(
+                        loaded_attribute, type(getattr(self, attribute_name))
+                    ):
                         setattr(self, attribute_name, loaded_attribute)
             # Either empty file or no file, leaving default from __init__
             except (json.JSONDecodeError, FileNotFoundError):
                 # Old Paths to allow transition (22.11.2020)
                 try:
-                    with open(self.old_paths[path], 'r') as file:
-                        setattr(self, attribute_name,
-                                json.load(file, object_hook=type_json_hook))
+                    with open(self.old_paths[path], "r") as file:
+                        setattr(
+                            self,
+                            attribute_name,
+                            json.load(file, object_hook=type_json_hook),
+                        )
                 except (json.JSONDecodeError, FileNotFoundError, KeyError):
                     pass
 
     def load_parameters(self):
         try:
-            with open(join(self.pscripts_path, f'parameters_{self.name}.json'),
-                      'r') as read_file:
-                loaded_parameters = json.load(read_file,
-                                              object_hook=type_json_hook)
+            with open(
+                join(self.pscripts_path, f"parameters_{self.name}.json"), "r"
+            ) as read_file:
+                loaded_parameters = json.load(read_file, object_hook=type_json_hook)
 
                 for p_preset in loaded_parameters:
                     # Make sure, that only parameters,
                     # which exist in pd_params are loaded
-                    for param in [p for p in loaded_parameters[p_preset] if
-                                  p not in self.ct.pd_params.index]:
-                        if '_exp' not in param:
+                    for param in [
+                        p
+                        for p in loaded_parameters[p_preset]
+                        if p not in self.ct.pd_params.index
+                    ]:
+                        if "_exp" not in param:
                             loaded_parameters[p_preset].pop(param)
 
                     # Add parameters, which exist in resource/parameters.csv,
                     # but not in loaded-parameters
                     # (e.g. added with custom-module)
-                    for param in [p for p in self.ct.pd_params.index if
-                                  p not in loaded_parameters[p_preset]]:
+                    for param in [
+                        p
+                        for p in self.ct.pd_params.index
+                        if p not in loaded_parameters[p_preset]
+                    ]:
                         try:
                             eval_param = literal_eval(
-                                self.ct.pd_params.loc[param, 'default'])
+                                self.ct.pd_params.loc[param, "default"]
+                            )
                         except (ValueError, SyntaxError, NameError):
                             # Allow parameters to be defined by functions
                             # e.g. by numpy, etc.
-                            is_func_gui = self.ct.pd_params.loc[
-                                              param, 'gui_type'] == 'FuncGui'
+                            is_func_gui = (
+                                self.ct.pd_params.loc[param, "gui_type"] == "FuncGui"
+                            )
                             if is_func_gui:
-                                default_string = \
-                                    self.ct.pd_params.loc[param, 'default']
-                                eval_param = eval(default_string, {'np': np})
-                                exp_name = param + '_exp'
+                                default_string = self.ct.pd_params.loc[param, "default"]
+                                eval_param = eval(default_string, {"np": np})
+                                exp_name = param + "_exp"
                                 loaded_parameters[p_preset].update(
-                                    {exp_name: default_string})
+                                    {exp_name: default_string}
+                                )
                             else:
-                                eval_param = self.ct.pd_params.loc[
-                                    param, 'default']
+                                eval_param = self.ct.pd_params.loc[param, "default"]
                         loaded_parameters[p_preset].update({param: eval_param})
                     # Change renamed legacy parameters
                     for param, value in loaded_parameters[p_preset].items():
                         if param in renamed_parameters:
                             if value in renamed_parameters[param]:
-                                loaded_parameters[p_preset][param] = \
-                                    renamed_parameters[param][value]
+                                loaded_parameters[p_preset][param] = renamed_parameters[
+                                    param
+                                ][value]
 
                 self.parameters = loaded_parameters
         except (FileNotFoundError, json.decoder.JSONDecodeError):
             self.load_default_parameters()
 
     def load_default_param(self, param_name):
-        string_param = self.ct.pd_params.loc[param_name, 'default']
+        string_param = self.ct.pd_params.loc[param_name, "default"]
         try:
-            self.parameters[self.p_preset][param_name] = literal_eval(
-                string_param)
+            self.parameters[self.p_preset][param_name] = literal_eval(string_param)
         except (ValueError, SyntaxError):
             # Allow parameters to be defined by functions e.g. by numpy, etc.
-            if self.ct.pd_params.loc[param_name, 'gui_type'] == 'FuncGui':
-                self.parameters[self.p_preset][param_name] = \
-                    eval(string_param, {'np': np})
-                exp_name = param_name + '_exp'
+            if self.ct.pd_params.loc[param_name, "gui_type"] == "FuncGui":
+                self.parameters[self.p_preset][param_name] = eval(
+                    string_param, {"np": np}
+                )
+                exp_name = param_name + "_exp"
                 self.parameters[self.p_preset][exp_name] = string_param
             else:
                 self.parameters[self.p_preset][param_name] = string_param
 
     def load_default_parameters(self):
         # Empty the dict for current Parameter-Preset
         self.parameters[self.p_preset] = dict()
         for param_name in self.ct.pd_params.index:
             self.load_default_param(param_name)
 
     def load_last_p_preset(self):
         try:
-            with open(self.sel_p_preset_path, 'r') as read_file:
+            with open(self.sel_p_preset_path, "r") as read_file:
                 self.p_preset = json.load(read_file)
                 # If parameter-preset not in Parameters,
                 # load first Parameter-Key(=Parameter-Preset)
                 if self.p_preset not in self.parameters:
                     self.p_preset = list(self.parameters.keys())[0]
         except (FileNotFoundError, json.decoder.JSONDecodeError):
             self.p_preset = list(self.parameters.keys())[0]
 
     def load(self):
         self.load_lists()
         self.load_parameters()
         self.load_last_p_preset()
 
     def save(self, worker_signals=None):
-
         if worker_signals:
             worker_signals.pgbar_max.emit(len(self.path_to_attribute))
 
         for idx, path in enumerate(self.path_to_attribute):
             if worker_signals:
                 worker_signals.pgbar_n.emit(idx)
-                worker_signals.pgbar_text.emit(
-                    f'Saving {self.path_to_attribute[path]}')
+                worker_signals.pgbar_text.emit(f"Saving {self.path_to_attribute[path]}")
 
             attribute = getattr(self, self.path_to_attribute[path], None)
 
             # Make sure the tuples are encoded correctly
             if isinstance(attribute, dict):
                 attribute = deepcopy(attribute)
                 encode_tuples(attribute)
 
             try:
-                with open(path, 'w') as file:
+                with open(path, "w") as file:
                     json.dump(attribute, file, cls=TypedJSONEncoder, indent=4)
 
             except json.JSONDecodeError as err:
-                print(f'There is a problem with path:\n'
-                      f'{err}')
+                print(f"There is a problem with path:\n" f"{err}")
 
     def add_meeg(self, name, file_path=None, is_erm=False):
         if is_erm:
             # Organize Empty-Room-FIles
             self.all_erm.append(name)
         else:
             # Organize other files
@@ -358,161 +377,165 @@
         # Copy sub_files to destination (with MEEG-Class
         # to also include raw into file_parameters)
         meeg = MEEG(name, self.ct)
 
         if file_path is not None:
             # Get bad-channels from raw-file
             raw = mne.io.read_raw(file_path, preload=True)
-            loaded_bads = raw.info['bads']
+            loaded_bads = raw.info["bads"]
             if len(loaded_bads) > 0:
-                self.meeg_bad_channels[name] = raw.info['bads']
+                self.meeg_bad_channels[name] = raw.info["bads"]
 
             meeg.save_raw(raw)
 
         return meeg
 
     def remove_meeg(self, remove_files):
         for meeg in self.sel_meeg:
             try:
                 # Remove MEEG from Lists/Dictionaries
                 self.all_meeg.remove(meeg)
             except ValueError:
-                logging.warning(f'{meeg} already removed!')
+                logging.warning(f"{meeg} already removed!")
             self.meeg_to_erm.pop(meeg, None)
             self.meeg_to_fsmri.pop(meeg, None)
             self.meeg_bad_channels.pop(meeg, None)
             self.meeg_event_id.pop(meeg, None)
             if remove_files:
                 try:
                     remove_path = join(self.data_path, meeg)
                     shutil.rmtree(remove_path)
-                    print(f'Succesful removed {remove_path}')
+                    print(f"Succesful removed {remove_path}")
                 except FileNotFoundError:
-                    print(join(self.data_path, meeg) + ' not found!')
+                    print(join(self.data_path, meeg) + " not found!")
         self.sel_meeg.clear()
 
     def add_fsmri(self, name, src_dir=None):
         self.all_fsmri.append(name)
         # Initialize FSMRI
         fsmri = FSMRI(name, self.ct)
         if src_dir is not None:
             dst_dir = join(self.ct.subjects_dir, name)
             if not isdir(dst_dir):
-                print(f'Copying Folder from {src_dir}...')
+                print(f"Copying Folder from {src_dir}...")
                 try:
                     shutil.copytree(src_dir, dst_dir)
                 # surfaces with .H and .K at the end can't be copied
                 except shutil.Error:
                     pass
-                print(f'Finished Copying to {dst_dir}')
+                print(f"Finished Copying to {dst_dir}")
             else:
-                print(f'{dst_dir} already exists')
+                print(f"{dst_dir} already exists")
 
         return fsmri
 
     def remove_fsmri(self, remove_files):
         for fsmri in self.sel_fsmri:
             try:
                 self.all_fsmri.remove(fsmri)
             except ValueError:
-                logging.warning(f'{fsmri} already deleted!')
+                logging.warning(f"{fsmri} already deleted!")
             if remove_files:
                 try:
                     shutil.rmtree(join(self.ct.subjects_dir, fsmri))
                 except FileNotFoundError:
-                    print(join(self.ct.subjects_dir, fsmri) + ' not found!')
+                    print(join(self.ct.subjects_dir, fsmri) + " not found!")
         self.sel_fsmri.clear()
 
     def add_group(self):
         pass
 
     def remove_group(self):
         pass
 
     def check_data(self):
-
-        missing_objects = [x for x in listdir(self.data_path)
-                           if x != 'grand_averages' and x not in self.all_meeg
-                           and x not in self.all_erm]
+        missing_objects = [
+            x
+            for x in listdir(self.data_path)
+            if x != "grand_averages"
+            and x not in self.all_meeg
+            and x not in self.all_erm
+        ]
 
         for obj in missing_objects:
             self.all_meeg.append(obj)
 
         # Get Freesurfer-folders (with 'surf'-folder)
         # from subjects_dir (excluding .files for Mac)
-        read_dir = sorted([f for f in os.listdir(self.ct.subjects_dir) if
-                           not f.startswith('.')],
-                          key=str.lower)
-        self.all_fsmri = [fsmri for fsmri in read_dir if
-                          exists(join(self.ct.subjects_dir, fsmri, 'surf'))]
+        read_dir = sorted(
+            [f for f in os.listdir(self.ct.subjects_dir) if not f.startswith(".")],
+            key=str.lower,
+        )
+        self.all_fsmri = [
+            fsmri
+            for fsmri in read_dir
+            if exists(join(self.ct.subjects_dir, fsmri, "surf"))
+        ]
 
         self.save()
 
     def clean_file_parameters(self, worker_signals=None):
         if worker_signals is not None:
             worker_signals.pgbar_max.emit(
-                len(self.all_meeg) + len(self.all_fsmri) +
-                len(self.all_groups.keys()))
+                len(self.all_meeg) + len(self.all_fsmri) + len(self.all_groups.keys())
+            )
         count = 0
 
         for meeg in self.all_meeg:
             meeg = MEEG(meeg, self.ct)
-            worker_signals.pgbar_text.emit(
-                f'Cleaning File-Parameters for {meeg}')
+            worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {meeg}")
             meeg.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print('Cleaning was canceled by the user!')
+                    print("Cleaning was canceled by the user!")
                     return
 
         for fsmri in self.all_fsmri:
             fsmri = FSMRI(fsmri, self.ct)
-            worker_signals.pgbar_text.emit(
-                f'Cleaning File-Parameters for {fsmri}')
+            worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {fsmri}")
             fsmri.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print('Cleaning was canceled by the user!')
+                    print("Cleaning was canceled by the user!")
                     return
 
         for group in self.all_groups:
             group = Group(group, self.ct)
-            worker_signals.pgbar_text.emit(
-                f'Cleaning File-Parameters for {group}')
+            worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {group}")
             group.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print('Cleaning was canceled by the user!')
+                    print("Cleaning was canceled by the user!")
                     return
 
     def clean_plot_files(self, worker_signals=None):
         all_image_paths = list()
         # Remove object-keys which no longer exist
         remove_obj = list()
         n_remove_ppreset = 0
         n_remove_funcs = 0
 
         if worker_signals is not None:
-            worker_signals.pgbar_max.emit(
-                count_dict_keys(self.plot_files, max_level=3))
+            worker_signals.pgbar_max.emit(count_dict_keys(self.plot_files, max_level=3))
         key_count = 0
 
         for obj_key in self.plot_files:
             key_count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(key_count)
 
-            if obj_key not in self.all_meeg + self.all_erm + \
-                    self.all_fsmri + list(self.all_groups.keys()):
+            if obj_key not in self.all_meeg + self.all_erm + self.all_fsmri + list(
+                self.all_groups.keys()
+            ):
                 remove_obj.append(obj_key)
             else:
                 # Remove Parameter-Presets which no longer exist
                 remove_p_preset = list()
                 for p_preset in self.plot_files[obj_key]:
                     key_count += 1
                     if worker_signals is not None:
@@ -530,83 +553,86 @@
                         remove_funcs = list()
                         for func in self.plot_files[obj_key][p_preset]:
                             key_count += 1
                             if worker_signals is not None:
                                 worker_signals.pgbar_n.emit(key_count)
 
                             # Cancel if canceled
-                            if worker_signals is not None \
-                                    and worker_signals.was_canceled:
-                                print('Cleaning was canceled by user')
+                            if (
+                                worker_signals is not None
+                                and worker_signals.was_canceled
+                            ):
+                                print("Cleaning was canceled by user")
                                 return
 
                             if func not in self.ct.pd_funcs.index:
                                 remove_funcs.append(func)
                             else:
                                 # Remove image-paths which no longer exist
-                                for rel_image_path in \
-                                        self.plot_files[obj_key][p_preset][
-                                            func]:
-                                    image_path = Path(join(self.figures_path,
-                                                           rel_image_path))
-                                    if not isfile(
-                                            image_path) or self.figures_path \
-                                            in rel_image_path:
-                                        self.plot_files[obj_key][p_preset][
-                                            func].remove(
-                                            rel_image_path)
+                                for rel_image_path in self.plot_files[obj_key][
+                                    p_preset
+                                ][func]:
+                                    image_path = Path(
+                                        join(self.figures_path, rel_image_path)
+                                    )
+                                    if (
+                                        not isfile(image_path)
+                                        or self.figures_path in rel_image_path
+                                    ):
+                                        self.plot_files[obj_key][p_preset][func].remove(
+                                            rel_image_path
+                                        )
                                     else:
                                         all_image_paths.append(str(image_path))
-                                if len(self.plot_files[obj_key][p_preset][
-                                           func]) == 0:
+                                if len(self.plot_files[obj_key][p_preset][func]) == 0:
                                     # Keys can't be dropped from dictionary
                                     # during iteration
                                     remove_funcs.append(func)
 
                         for remove_func_key in remove_funcs:
-                            self.plot_files[obj_key][p_preset].pop(
-                                remove_func_key)
+                            self.plot_files[obj_key][p_preset].pop(remove_func_key)
                         n_remove_funcs += len(remove_funcs)
 
                 for remove_preset_key in remove_p_preset:
                     self.plot_files[obj_key].pop(remove_preset_key)
                 n_remove_ppreset += len(remove_p_preset)
 
             print(
-                f'Removed {n_remove_ppreset} Parameter-Presets and '
-                f'{n_remove_funcs} from {obj_key}')
+                f"Removed {n_remove_ppreset} Parameter-Presets and "
+                f"{n_remove_funcs} from {obj_key}"
+            )
 
         for remove_key in remove_obj:
             self.plot_files.pop(remove_key)
-        print(f'Removed {len(remove_obj)} Objects from Plot-Files')
+        print(f"Removed {len(remove_obj)} Objects from Plot-Files")
 
         # Remove image-files, which aren't listed in plot_files.
         free_space = 0
-        print('Removing unregistered images...')
+        print("Removing unregistered images...")
         n_removed_images = 0
         for root, _, files in os.walk(self.figures_path):
             files = [join(root, f) for f in files]
-            for file_path in [fp for fp in files if
-                              str(Path(fp)) not in all_image_paths]:
+            for file_path in [
+                fp for fp in files if str(Path(fp)) not in all_image_paths
+            ]:
                 free_space += getsize(file_path)
                 n_removed_images += 1
                 os.remove(file_path)
-        print(f'Removed {n_removed_images} images')
+        print(f"Removed {n_removed_images} images")
 
         # Remove empty folders (loop until all empty folders are removed)
-        print('Removing empty folders...')
+        print("Removing empty folders...")
         n_removed_folders = 0
         folder_loop = True
         # Redo the file-walk because folders can get empty
         # by deleting folders inside
         while folder_loop:
             folder_loop = False
             for root, folders, _ in os.walk(self.figures_path):
                 folders = [join(root, fd) for fd in folders]
-                for folder in [fdp for fdp in folders if
-                               len(listdir(fdp)) == 0]:
+                for folder in [fdp for fdp in folders if len(listdir(fdp)) == 0]:
                     os.rmdir(folder)
                     n_removed_folders += 1
                     folder_loop = True
-        print(f'Removed {n_removed_folders} folders')
+        print(f"Removed {n_removed_folders} folders")
 
-        print(f'{round(free_space / (1024 ** 2), 2)} MB of space was freed!')
+        print(f"{round(free_space / (1024 ** 2), 2)} MB of space was freed!")
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/default_settings.json` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/default_settings.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'qsettings'": "{'app_style': 'auto'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "qsettings": {
         "app_font": "AnyStyle",
         "app_font_size": 10,
-        "app_style": "Fusion",
+        "app_style": "auto",
         "education": 0,
         "enable_cuda": 0,
         "fs_path": "",
         "gui": true,
         "home_path": "",
         "log_level": 20,
         "mne_path": "",
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/functions.csv` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/functions.csv`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,14 @@
 plot_src_connectivity;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,target_labels,con_fmin,con_fmax,show_plots
 plot_grand_avg_evokeds;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
 plot_grand_avg_tfr;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
 plot_grand_avg_stc;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
 plot_grand_avg_stc_anim;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation,stc_animation_span,stc_animation_dilat
 plot_grand_average_stc_interactive;;Group;Plot;Grand-Average;True;True;;plot;basic;group,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
 plot_grand_avg_ltc;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
-plot_grand_avg_connect;;Group;Plot;Grand-Average;True;False;;plot;basic;group,con_fmin,con_fmax,target_labels,morph_to,show_plots
+plot_grand_avg_connect;;Group;Plot;Grand-Average;True;False;;plot;basic;group,con_fmin,con_fmax,target_labels,morph_to,show_plots,connectivity_vmin,connectivity_vmax
 plot_ica_components;Plot ICA-Components;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
 plot_ica_sources;Plot ICA-Sources;MEEG;Plot;ICA;True;False;;operations;basic;meeg,ica_source_data,show_plots
 plot_ica_overlay;Plot ICA-Overlay;MEEG;Plot;ICA;True;False;;operations;basic;meeg,ica_overlay_data,show_plots
 plot_ica_properties;Plot ICA-Properties;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
 plot_ica_scores;Plot ICA-Scores;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
 print_info;Print Info;MEEG;Plot;Raw;False;False;;operations;basic;meeg
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/license.txt` & `mne-pipeline-hd-0.3.3a0/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 BSD 3-Clause License
 
-Copyright (c) 2019-2021, Martin Schulz
+Copyright (c) 2019-2023, authors of mne-pipeline-hd
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
+1.  Redistributions of source code must retain the above copyright notice, this
+    list of conditions and the following disclaimer.
 
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
+2.  Redistributions in binary form must reproduce the above copyright notice,
+    this list of conditions and the following disclaimer in the documentation
+    and/or other materials provided with the distribution.
+
+3.  Neither the name of the copyright holder nor the names of its
+    contributors may be used to endorse or promote products derived from
+    this software without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_license.txt` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_license.txt`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/resource/parameters.csv` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/parameters.csv`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ;alias;group;default;unit;description;gui_type;gui_args
 ch_types;Channel-Types;Preprocessing;['mag', 'grad', 'eeg', 'stim', 'eog', 'ecg'];;Specify Channel-Types used in data;CheckListGui;{'options': ['mag', 'grad', 'eeg', 'stim', 'eog', 'ecg', 'emg', 'ref_meg', 'misc', 'resp', 'chpi', 'exci', 'ias', 'syst', 'seeg', 'dipole', 'gof', 'bio', 'ecog', 'fnirs', 'csd']}
 ch_names;Channel-Names;Preprocessing;'all';;Specify Channel-Names to use in data (set all for all depending on what you have selected as channel-types);MultiTypeGui;{'type_selection': True, 'types': ['str', 'list']}
 ref_channels;;Preprocessing;'average';;Set the kind of eeg-reference, look at documentation of mne.set_eeg_reference();MultiTypeGui;{'type_selection': True, 'types': ['str', 'list']}
-highpass;Highpass-Cutoff;Filtering;1;Hz;Highpass-Filter;SliderGui;{'min_val': 0, 'max_val': 100, 'step': 1, 'none_select': True}
-lowpass;Lowpass-Cutoff;Filtering;100;Hz;Lowpass-Filter;SliderGui;{'min_val': 0, 'max_val': 100, 'step': 1, 'none_select': True}
+highpass;Highpass-Cutoff;Filtering;1;Hz;Highpass-Filter;SliderGui;{'min_val': 0, 'max_val': 100, 'step': 0.1, 'none_select': True}
+lowpass;Lowpass-Cutoff;Filtering;100;Hz;Lowpass-Filter;SliderGui;{'min_val': 0, 'max_val': 100, 'step': 0.1, 'none_select': True}
 filter_target;;Filtering;'raw';;The target for Filtering (experimental when other than raw);ComboGui;{'options': ['raw', 'epochs', 'evoked']}
 filter_length;;Filtering;auto;;;MultiTypeGui;{'type_selection': True, 'types': ['str', 'int']}
 l_trans_bandwidth;;Filtering;auto;;;MultiTypeGui;{'type_selection': True, 'types': ['str', 'float']}
 h_trans_bandwidth;;Filtering;auto;;;MultiTypeGui;{'type_selection': True, 'types': ['str', 'float']}
 filter_method;;Filtering;fir;;;StringGui;
 iir_params;;Filtering;None;;;DictGui;{'none_select': True}
 fir_phase;;Filtering;zero;;;StringGui;
 fir_window;;Filtering;hamming;;;StringGui;
 fir_design;;Filtering;firwin;;;StringGui;
 skip_by_annotation;;Filtering;['edge', 'bad_acq_skip'];;;ListGui;
 fir_pad;;Filtering;reflect_limited;;;StringGui;
 erm_t_limit;;Preprocessing;300;s;Limits Empty-Room-Measurement-Length[s];IntGui;{'none_select': True, 'min_val':0, 'max_val': 10000}
 stim_channels;Stimulation-Channels;events;['STI 001'];;Stimulation Channel(s);ListGui;
-min_duration;Minimum Duration;events;0.002;s;Minimum-Duration for events;FloatGui;{'min_val': 0, 'step': 0.001}
+min_duration;Minimum Duration;events;0.002;s;Minimum-Duration for events;FloatGui;{'min_val': 0, 'step': 0.001, 'decimals': 3}
 shortest_event;Shortest Event;events;2;sample;Shortest possible Event;IntGui;{'min_val': 0}
 adjust_timeline_by_msec;Adjust Time;events;0;ms;custom delay to stimulus in ms;IntGui;{'min_val':-10000, 'max_val': 10000}
 t_epoch;Epoch-Timeframe;epochs;(-0.5,1.5);s;start and end of epoch;TupleGui;
 baseline;Baseline-Timeframe;epochs;(-0.5,0);s;start and end of baseline;TupleGui;{'max_val': 0, 'none_select': True}
 apply_proj;Apply Projections;epochs;True;;If to apply the projections (if present);BoolGui;
 bad_interpolation;Bad-Channel-Interpolation;Preprocessing;None;;Choose where to apply bad-channels-interpolation;ComboGui;{'none_select': True, 'options': ['raw_filtered', 'epochs', 'evoked']}
 reject_by_annotation;;epochs;True;;If to reject by Annotations;BoolGui;
@@ -29,42 +29,42 @@
 n_interpolates;;epochs;np.array([1, 4, 32]);;p-values for autoreject;FuncGui;
 consensus_percs;;epochs;np.linspace(0, 1.0, 11);;k-values for autoreject;FuncGui;
 overwrite_ar;Overwrite Autoreject(Threshold);epochs;False;;if to calculate new threshold or use the previously calculated;BoolGui;
 reject;;epochs;{'mag':3000e-15, 'grad':3000e-13, 'eeg':100e-6, 'eog':200e-6};;Chose reject-thresholds if not reject with autoreject_threshold;DictGui;{'none_select': True}
 flat;;epochs;{'mag': 1e-15, 'grad':1e-13, 'eeg': 1e-6};;Chose flat-thresholds;DictGui;{'none_select': True}
 decim;;epochs;1;;Downsampling-Factor for epochs;IntGui;
 ica_method;ICA-Method;ICA;fastica;;The method for calculating ICA;ComboGui;{'options': ['fastica', 'infomax', 'picard']}
-ica_fitto;Fit ICA to: ;ICA;'raw_filtered';;The data to fit the ICA to;ComboGui;{'options': ['raw', 'raw_filtered', 'epochs']}
+ica_fitto;Fit ICA to:;ICA;'raw_filtered';;The data to fit the ICA to;ComboGui;{'options': ['raw', 'raw_filtered', 'epochs']}
 n_components;;ICA;25;;The number of components for ICA;IntGui;
 max_pca_components;;ICA;None;;;IntGui;{'none_select': True}
 n_pca_components;;ICA;None;;;IntGui;{'none_select': True}
 ica_noise_cov;Use Noise-Covariance;ICA;False;;If to use a noise-covariance for pre-whitening;BoolGui;
 ica_remove_proj;Remove projections;ICA;False;;If to remove projections from the data before fitting;BoolGui;
 ica_reject;Reject-Parameters;ICA;{'mag':3000e-15, 'grad':3000e-13, 'eeg':100e-6, 'eog':200e-6};;Reject-Parameters for ICA;DictGui;{'none_select': True}
 ica_autoreject;Autoreject;ICA;False;;If to use Autoreject for ICA;BoolGui;
 ica_eog;Use EOG;ICA;False;;If to use EOG-Channels for automatic selection of components;BoolGui;
 eog_channel;;ICA;None;;Set Vertical EOG-Channel;StringGui;
 ica_ecg;Use ECG;ICA;False;;If to use automatic ECG-detection either by ECG-Channel (if provided) or by an artificial ECG-Channel;BoolGui;
 ecg_channel;;ICA;None;;Set ECG-Channel;StringGui;{'none_select': True}
-tfr_freqs;;Time-Frequency;np.arange(7,40,3) ;Hz;Select the frequencies of interest (Array/List);FuncGui;
+tfr_freqs;;Time-Frequency;np.arange(7,40,3);Hz;Select the frequencies of interest (Array/List);FuncGui;
 tfr_method;;Time-Frequency;morlet;;Choose the method to calculate Time-Frequency-Data;ComboGui;{'options': ['morlet', 'multitaper', 'stockwell']}
 tfr_n_cycles;n_cycles;Time-Frequency;np.arange(7,40,3) / 2;;Select the number of cycles for each frequency;FuncGui;
 tfr_average;;Time-Frequency;True;;If to take the average of the Time-Frequency across observations;BoolGui;
 tfr_use_fft;use_fft;Time-Frequency;False;;If to use fft based convolution;BoolGui;
 tfr_baseline;;Time-Frequency;None;;Check to apply the entered baseline;TupleGui;{'none_select': True}
 tfr_baseline_mode;;Time-Frequency;mean;;Select the mode for baseline-application (if enabled);ComboGui;{'options':['mean', 'ratio', 'logratio', 'percent', 'zscore', 'zlogratio']}
 multitaper_bandwidth;;Time-Frequency;4.0;;;FloatGui;
 stockwell_width;;Time-Frequency;1.0;;;FloatGui;
 bem_spacing;;Forward;4;;See the MNE-Documentation for further details;IntGui;
 bem_conductivity;BEM Conductivity;Forward;[0.3, 0.006, 0.3];;The conductivities for each shell of the bem-model, contain only one element for a one-layer model and three elements for a three-layer model;ListGui;
 src_spacing;;Forward;ico5;;See the MNE-Documentation for further details;StringGui;
 vol_src_spacing;;Forward;5.0;;Spacing between sources in 3D-Grid;FloatGui;
 surface;;Forward;white;;Surface for computing the Source-Space;ComboGui;{'options': ['white', 'pial']}
 noise_cov_mode;Noise-Covariance Mode;Preprocessing;'Empty-Room';;Select the origin of the Noise-Covariance;ComboGui;{'options': ['Empty-Room', 'epochs']}
-noise_cov_method;Noise-Covariance Method;Preprocessing;empirical;;Select the method for computing the Noise-Covariance;ComboGui;{'options': ['shrunk', 'diagonal_fixed', 'empirical', 'factor_analysis']}
+noise_cov_method;Noise-Covariance Method;Preprocessing;empirical;;Select the method for computing the Noise-Covariance;ComboGui;{'options': ['auto', 'empirical', 'diagonal_fixed', 'shrunk', 'oas', 'ledoit_wolf', 'factor_analysis', 'shrinkage', 'pca']}
 inverse_method;Inverse-Method;Inverse;MNE;;Choose the Inverse-Method for Source-Estimate;ComboGui;{'options': ['MNE', 'dSPM', 'sLORETA', 'eLORETA']}
 pick_ori;Dipole-Orientation;Inverse;None;;Choose the Dipole-Orientation for Source-Estimate;ComboGui;{'options': [None, 'normal', 'vector']}
 lambda2;;Inverse;1.0 / 3.0 ** 2;;lambda2 for Source-Estimate;FuncGui;
 stc_surface;;Inverse;inflated;;Select the surface type for Source Estimate Plots;ComboGui;{'options':['inflated', 'white', 'pial']}
 stc_hemi;;Inverse;'split';;Select the hemispheres for Source Estimate Plots;ComboGui;{'options':['lh', 'rh', 'both', 'split']}
 stc_views;;Inverse;['med', 'lat'];;Select the views for Source Estimate Plots;MultiTypeGui;{'type_selection': True, 'types': ['str', 'list']}
 stc_time;;Inverse;0;;Initial time for Source Estimate Plots;FloatGui;
@@ -89,8 +89,10 @@
 ica_overlay_data;;ICA;Evokeds;;Which data to plot in overlay-plot from ICA;ComboGui;{'options':['raw', 'raw_filtered', 'evoked', 'evoked (EOG)', 'evoked (ECG)']}
 plot_sensors_kind;;Plot;'topomap';;The kind of plot for plot_sensors;ComboGui;{'options':['topomap', '3d', 'select']}
 erm_ssp_duration;;Preprocessing;1;s;The time-chunk to use for ssp;IntGui;
 erm_n_grad;;Preprocessing;2;;The number of projections for Gradiometer;IntGui;
 erm_n_mag;;Preprocessing;2;;The number of projections for Magnetometer;IntGui;
 erm_n_eeg;;Preprocessing;0;;The number of projections for EEG;IntGui;
 ga_interpolate_bads;;Grand-Average;True;;If to interpolate bad channels for the Grand-Average;BoolGui;
-ga_drop_bads;;Grand-Average;True;;If to drop bad channels for the Grand-Average;BoolGui;
+ga_drop_bads;;Grand-Average;True;;If to drop bad channels for the Grand-Average;BoolGui;
+connectivity_vmin;;Connectivity;None;;Minimum value for colormap;FloatGui;{'step': 0.01, 'none_select':True}
+connectivity_vmax;;Connectivity;None;;Maximum value for colormap;FloatGui;{'step': 0.01, 'none_select':True}
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_concurrent.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_concurrent.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 # def test_blocking_worker_dialog(qtbot):
 #     def _test_func():
 #         time.sleep(2)
 #         print('Finished Test-Func')
 #
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_controller.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import io
 
 from mne_pipeline_hd.pipeline.controller import Controller
 
-controller_attributes = ['home_path', 'projects', 'pr', 'projects_path',
-                         'subjects_dir']
+controller_attributes = ["home_path", "projects", "pr", "projects_path", "subjects_dir"]
 
 
 def test_init(tmpdir):
     ct = Controller(tmpdir)
 
     for ca in controller_attributes:
         assert hasattr(ct, ca)
 
 
 def _check_project(ct, project_name):
     assert ct.pr.name == project_name
     assert project_name in ct.projects
-    assert ct.settings['selected_project'] == project_name
+    assert ct.settings["selected_project"] == project_name
 
 
 def test_project_management(tmpdir, monkeypatch):
-    ct = Controller(tmpdir, 'test1')
+    ct = Controller(tmpdir, "test1")
 
     # Initialize with "test1"
-    assert hasattr(ct, 'pr')
-    _check_project(ct, 'test1')
+    assert hasattr(ct, "pr")
+    _check_project(ct, "test1")
 
     # Remove project "test1"
     # Add monkeypatch for stdin to pass input for "test2"
-    monkeypatch.setattr('sys.stdin', io.StringIO('test2'))
-    ct.remove_project('test1')
-    _check_project(ct, 'test2')
+    monkeypatch.setattr("sys.stdin", io.StringIO("test2"))
+    ct.remove_project("test1")
+    _check_project(ct, "test2")
 
     # Add two projects "test3" and "test4"
-    ct.change_project('test3')
-    _check_project(ct, 'test3')
-    ct.change_project('test4')
-    _check_project(ct, 'test4')
+    ct.change_project("test3")
+    _check_project(ct, "test3")
+    ct.change_project("test4")
+    _check_project(ct, "test4")
 
     # Change back to existing project
-    ct.change_project('test3')
-    _check_project(ct, 'test3')
+    ct.change_project("test3")
+    _check_project(ct, "test3")
 
     assert len(ct.projects) == 3
 
     # Remove non-selected project
-    ct.remove_project('test2')
-    _check_project(ct, 'test3')
+    ct.remove_project("test2")
+    _check_project(ct, "test3")
 
     assert len(ct.projects) == 2
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_functions.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 # from mne_pipeline_hd.pipeline.function_utils import RunController
 # from mne_pipeline_hd.pipeline.loading import MEEG
 #
 #
 # def test_all_functions(controller):
 #     controller.pr.sel_functions = list(controller.pd_funcs.index)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_param_guis.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_param_guis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,99 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 import inspect
 import sys
 from ast import literal_eval
 
 import pytest
-from PyQt5.QtWidgets import QVBoxLayout, QGridLayout, QPushButton, QLineEdit, \
-    QDialog, QApplication, QWidget, QHBoxLayout, QComboBox
+from PyQt5.QtWidgets import (
+    QVBoxLayout,
+    QGridLayout,
+    QPushButton,
+    QLineEdit,
+    QDialog,
+    QApplication,
+    QWidget,
+    QHBoxLayout,
+    QComboBox,
+)
 from numpy.testing import assert_allclose
 
 from mne_pipeline_hd.gui import parameter_widgets
 from mne_pipeline_hd.gui.base_widgets import SimpleDict
 from mne_pipeline_hd.gui.parameter_widgets import Param, _eval_param
 
-parameters = {'IntGui': 1,
-              'FloatGui': 5.3,
-              'StringGui': 'postcentral-lh',
-              'MultiTypeGui': 42,
-              'FuncGui': 'np.arange(10) * np.pi',
-              'BoolGui': True,
-              'TupleGui': (45, 6),
-              'ComboGui': 'a',
-              'ListGui': [1, 454.33, 'postcentral-lh', 5],
-              'CheckListGui': ['postcentral-lh'],
-              'DictGui': {'A': 'B',
-                          'C': 58.144,
-                          3: [1, 2, 3, 4],
-                          'D': {'A': 1, 'B': 2}},
-              'SliderGui': 5,
-              'ColorGui': {'C': '#98765432',
-                           '3': '#97867564'}}
-
-alternative_parameters = {'IntGui': 5,
-                          'FloatGui': 8.45,
-                          'StringGui': 'precentral-lh',
-                          'MultiTypeGui': 32,
-                          'FuncGui': 'np.ones((2,3))',
-                          'BoolGui': False,
-                          'TupleGui': (2, 23),
-                          'ComboGui': 'b',
-                          'ListGui': [33, 2234.33, 'precentral-lh', 3],
-                          'CheckListGui': ['precentral-lh'],
-                          'DictGui': {'B': 'V',
-                                      'e': 11.333,
-                                      5: [65, 3, 11],
-                                      'F': {'C': 1, 'D': 2}},
-                          'SliderGui': 2,
-                          'ColorGui': {'A': '#12345678',
-                                       'B': '#13243546'}}
-
-gui_kwargs = {'none_select': True,
-              'min_val': -40,
-              'max_val': 100,
-              'step': 0.5,
-              'return_integer': False,
-              'param_unit': 'ms',
-              'options': {'a': 'A', 'b': 'B', 'c': 'C'},
-              'keys': 'DictGui'}
+parameters = {
+    "IntGui": 1,
+    "FloatGui": 5.3,
+    "StringGui": "postcentral-lh",
+    "MultiTypeGui": 42,
+    "FuncGui": "np.arange(10) * np.pi",
+    "BoolGui": True,
+    "TupleGui": (45, 6),
+    "ComboGui": "a",
+    "ListGui": [1, 454.33, "postcentral-lh", 5],
+    "CheckListGui": ["postcentral-lh"],
+    "DictGui": {"A": "B", "C": 58.144, 3: [1, 2, 3, 4], "D": {"A": 1, "B": 2}},
+    "SliderGui": 5,
+    "ColorGui": {"C": "#98765432", "3": "#97867564"},
+}
+
+alternative_parameters = {
+    "IntGui": 5,
+    "FloatGui": 8.45,
+    "StringGui": "precentral-lh",
+    "MultiTypeGui": 32,
+    "FuncGui": "np.ones((2,3))",
+    "BoolGui": False,
+    "TupleGui": (2, 23),
+    "ComboGui": "b",
+    "ListGui": [33, 2234.33, "precentral-lh", 3],
+    "CheckListGui": ["precentral-lh"],
+    "DictGui": {"B": "V", "e": 11.333, 5: [65, 3, 11], "F": {"C": 1, "D": 2}},
+    "SliderGui": 2,
+    "ColorGui": {"A": "#12345678", "B": "#13243546"},
+}
+
+gui_kwargs = {
+    "none_select": True,
+    "min_val": -40,
+    "max_val": 100,
+    "step": 0.5,
+    "return_integer": False,
+    "param_unit": "ms",
+    "options": {"a": "A", "b": "B", "c": "C"},
+    "keys": "DictGui",
+}
 
 
 def _check_param(gui, gui_name, alternative=False):
     if alternative:
         value = alternative_parameters[gui_name]
     else:
         value = parameters[gui_name]
 
-    if gui_name == 'FuncGui':
+    if gui_name == "FuncGui":
         value = _eval_param(value)
         assert_allclose(gui.get_value(), value)
     else:
         assert gui.get_value() == value
 
 
-@pytest.mark.parametrize('gui_name', list(parameters.keys()))
+@pytest.mark.parametrize("gui_name", list(parameters.keys()))
 def test_basic_param_guis(qtbot, gui_name):
     gui_class = getattr(parameter_widgets, gui_name)
-    gui_parameters = \
-        list(inspect.signature(gui_class).parameters) + \
-        list(inspect.signature(Param).parameters)
-    kwargs = {key: value for key, value in gui_kwargs.items()
-              if key in gui_parameters}
+    gui_parameters = list(inspect.signature(gui_class).parameters) + list(
+        inspect.signature(Param).parameters
+    )
+    kwargs = {key: value for key, value in gui_kwargs.items() if key in gui_parameters}
     gui = gui_class(data=parameters, name=gui_name, **kwargs)
     qtbot.addWidget(gui)
 
     # Check if value is correct
     _check_param(gui, gui_name)
 
     # Check if value changes correctly
@@ -103,56 +107,57 @@
     assert not gui.group_box.isChecked()
 
     # Uncheck groupbox
     gui.group_box.setChecked(True)
     parameters[gui_name] = new_param
     _check_param(gui, gui_name, alternative=True)
 
-    if 'max_val' in gui_parameters:
-        if gui_name == 'TupleGui':
+    if "max_val" in gui_parameters:
+        if gui_name == "TupleGui":
             value = (1000, 1000)
             neg_value = (-1000, -1000)
-            max_val = (kwargs['max_val'], kwargs['max_val'])
-            min_val = (kwargs['min_val'], kwargs['min_val'])
+            max_val = (kwargs["max_val"], kwargs["max_val"])
+            min_val = (kwargs["min_val"], kwargs["min_val"])
         else:
             value = 1000
             neg_value = -1000
-            max_val = kwargs['max_val']
-            min_val = kwargs['min_val']
+            max_val = kwargs["max_val"]
+            min_val = kwargs["min_val"]
         gui.set_param(value)
         assert parameters[gui_name] == max_val
         # less than min
         gui.set_param(neg_value)
         assert parameters[gui_name] == min_val
 
-    if 'return_integer' in gui_parameters:
+    if "return_integer" in gui_parameters:
         gui.return_integer = True
         gui.set_param(True)
         assert gui.get_value() == 1
 
-    if gui_name == 'ComboGui':
+    if gui_name == "ComboGui":
         # Don't set values which are not in options
         with pytest.raises(KeyError):
-            gui.set_param('d')
+            gui.set_param("d")
 
-    if gui_name == 'MultiTypeGui':
+    if gui_name == "MultiTypeGui":
         for gui_type, gui_name in gui.gui_types.items():
             gui.set_param(parameters[gui_name])
             assert gui.get_value() == parameters[gui_name]
             assert type(gui.get_value()).__name__ == gui_type
-        kwargs['type_selection'] = True
-        kwargs['type_kwargs'] = dict()
+        kwargs["type_selection"] = True
+        kwargs["type_kwargs"] = dict()
         for gui_name in gui.gui_types.values():
             type_class = getattr(parameter_widgets, gui_name)
-            gui_parameters = \
-                list(inspect.signature(type_class).parameters) + \
-                list(inspect.signature(Param).parameters)
-            t_kwargs = {key: value for key, value in gui_kwargs.items()
-                        if key in gui_parameters}
-            kwargs['type_kwargs'][gui_name] = t_kwargs
+            gui_parameters = list(inspect.signature(type_class).parameters) + list(
+                inspect.signature(Param).parameters
+            )
+            t_kwargs = {
+                key: value for key, value in gui_kwargs.items() if key in gui_parameters
+            }
+            kwargs["type_kwargs"][gui_name] = t_kwargs
         gui = gui_class(data=parameters, name=gui_name, **kwargs)
         for gui_type, gui_name in gui.gui_types.items():
             type_idx = gui.types.index(gui_type)
             gui.change_type(type_idx)
             gui.set_param(parameters[gui_name])
             assert gui.get_value() == parameters[gui_name]
             assert type(gui.get_value()).__name__ == gui_type
@@ -172,40 +177,40 @@
         max_cols = 4
         set_none_select = True
         set_groupbox_layout = False
         set_alias = False
 
         for idx, gui_nm in enumerate(gui_kwargs):
             kw_args = gui_kwargs[gui_nm]
-            kw_args['data'] = parameters
-            kw_args['name'] = gui_nm
-            kw_args['none_select'] = set_none_select
-            kw_args['groupbox_layout'] = set_groupbox_layout
+            kw_args["data"] = parameters
+            kw_args["name"] = gui_nm
+            kw_args["none_select"] = set_none_select
+            kw_args["groupbox_layout"] = set_groupbox_layout
             if set_alias:
-                kw_args['alias'] = gui_nm + '-alias'
-            kw_args['description'] = gui_nm + '-description'
+                kw_args["alias"] = gui_nm + "-alias"
+            kw_args["description"] = gui_nm + "-description"
             gui = getattr(parameter_widgets, gui_nm)(**kw_args)
             grid_layout.addWidget(gui, idx // max_cols, idx % max_cols)
             self.gui_dict[gui_nm] = gui
 
         test_layout.addLayout(grid_layout)
 
         set_layout = QHBoxLayout()
         self.gui_cmbx = QComboBox()
         self.gui_cmbx.addItems(self.gui_dict.keys())
         set_layout.addWidget(self.gui_cmbx)
 
         self.set_le = QLineEdit()
         set_layout.addWidget(self.set_le)
 
-        set_bt = QPushButton('Set')
+        set_bt = QPushButton("Set")
         set_bt.clicked.connect(self.set_param)
         set_layout.addWidget(set_bt)
 
-        show_bt = QPushButton('Show Parameters')
+        show_bt = QPushButton("Show Parameters")
         show_bt.clicked.connect(self.show_parameters)
         set_layout.addWidget(show_bt)
 
         test_layout.addLayout(set_layout)
 
         self.setLayout(test_layout)
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd/tests/test_qsettings.py` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_qsettings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf-8 -*-
 """
-Pipeline-GUI for Analysis with MNE-Python
-@author: Martin Schulz
-@email: dev@earthman-music.de
-@github: https://github.com/marsipu/mne-pipeline-hd
-License: GPL-3.0
+Authors: Martin Schulz <dev@mgschulz.de>
+License: BSD 3-Clause
+Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import json
 from importlib import resources
 
 from PyQt5.QtCore import QSettings
 
 
 def test_qsettings_types(qtbot):
     """Test if QSettings keep types on all operating systems."""
-    with resources.open_text('mne_pipeline_hd.resource',
-                             'default_settings.json') as file:
-        default_qsettings = json.load(file)['qsettings']
+    with resources.open_text(
+        "mne_pipeline_hd.resource", "default_settings.json"
+    ) as file:
+        default_qsettings = json.load(file)["qsettings"]
 
     for v in default_qsettings:
         QSettings().setValue(v, default_qsettings[v])
 
     for v in default_qsettings:
         value = QSettings().value(v)
         if value is not None:
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/PKG-INFO` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,124 @@
 Metadata-Version: 2.1
 Name: mne-pipeline-hd
-Version: 0.3.2a0
-Summary: A pipeline-GUI for brain-data analysis with MNE-Python
-Home-page: https://github.com/marsipu/mne-pipeline-hd
-Author: Martin Schulz
-Author-email: dev@earthman-music.de
-License: BSD (3-clause)
+Version: 0.3.3a0
+Summary: A Pipeline-GUI for MNE-Python from MEG-Lab Heidelberg
+Author-email: Martin Schulz <dev@mgschulz.de>
+License: BSD-3-Clause
+Project-URL: Homepage, https://github.com/marsipu/mne-pipeline-hd
+Project-URL: Repository, https://github.com/marsipu/mne-pipeline-hd.git
+Keywords: mne-python,meg,eeg,pipeline,gui,heidelberg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.txt
 
 # mne-pipeline-hd
-### A [MNE-Python](https://mne.tools/stable/index.html) Pipeline-GUI for MEG-Lab Heidelberg
-###### inspired by: [Andersen L.M. 2018](https://doi.org/10.3389/fnins.2018.00006)
+
+### A Pipeline-GUI for [MNE-Python](https://mne.tools/stable/index.html)  from MEG-Lab Heidelberg
 
 ![mne-pipeline-hd Logo](mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg)
 
 ## Installation
-1. Install MNE-python as instructed on the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
-I would recommend to install in a separate conda environment with:
-`conda env create -n mne_p -f environment.yml`
+
+1. Install MNE-python as instructed on
+   the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
+   I would recommend to install in a separate conda environment with:
+   `conda env create -n mne_p -f environment.yml`
 2. `conda activate mne_p`
 3. `pip install https://github.com/marsipu/mne-pipeline-hd/zipball/main`
 
 ## Update
 
-Just
-run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
-again or use the update-funtion from within the programm (in Settings-Menu).
+Run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
+for an update to the development version
+or `pip install --upgrade mne-pipeline-hd` for the latest release.
 
 ## Start
+
 Run `mne_pipeline_hd` in your mne_pipeline-environment (`conda activate mne_p`)
 
 **or**
 
-run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom, etc.
+run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom,
+etc.
 
-***When using the pipeline and its functions bear in mind that the pipeline is still in development!
-The basic functions supplied are just a suggestion and you should verify before usage if they do what you need.
-They are also partly still adjusted to specific requirements which may not apply to all data.***
+***When using the pipeline and its functions bear in mind that the pipeline is
+still in development!
+The basic functions supplied are just a suggestion and you should verify before
+usage if they do what you need.
+They are also partly still adjusted to specific requirements which may not
+apply to all data.***
 
 ## Bug-Report/Feature-Request
-Please report bugs on GitHub as an issue or to me (dev@earthman-music.de) directly.
+
+Please report bugs on GitHub as an issue or to me (dev@earthman-music.de)
+directly.
 And if you got ideas on how to improve the pipeline or some feature-requests,
 you are welcome to open an issue too or send an e-mail (dev@earthman-music.de)
 
 ## Contribute and build your own functions/fix bugs
+
 I you want to help by contributing, I would be very happy:
 
 You need a [GitHub-Account](https://github.com/)
-and should have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed.
+and should
+have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
+installed.
 
 1. Fork this repository on GitHub
 2. Move to the folder where you want to clone to
 3. Clone **your forked repository** with git from a
    terminal: `git clone <url you get from the green clone-button from your forked repository on GitHub>`
 4. Add upstream to git for
    updates: `git remote add upstream git://github.com/marsipu/mne-pipeline-hd.git`
 5. Install development version with pip: `pip install -e ./`
 6. Create a branch for changes: `git checkout -b <branch-name>`
 7. Commit changes: `git commit -am "<your commit message>"`
 8. Push changes to your forked repository on GitHub: `git push`
 9. Make "New pull request" from your new feature branch
 
-You can always [write me](mailto:dev@earthman-music.de), if you have questions about the contribution-process 
+You can always [write me](mailto:dev@earthman-music.de), if you have questions
+about the contribution-process
 or about the program-structure.
 
 ## Acknowledgments
-This Pipeline is build on top of [MNE-Python](https://mne.tools/stable/index.html)
-> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck, L. Parkkonen, M. Hämäläinen,
-> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1 February 2014, Pages 446-460, ISSN 1053-8119,
+
+This Pipeline is build on top
+of [MNE-Python](https://mne.tools/stable/index.html)
+> A. Gramfort, M. Luessi, E. Larson, D. Engemann, D. Strohmeier, C. Brodbeck,
+> L. Parkkonen, M. Hämäläinen,
+> MNE software for processing MEG and EEG data, NeuroImage, Volume 86, 1
+> February 2014, Pages 446-460, ISSN 1053-8119,
 > [DOI](https://doi.org/10.1016/j.neuroimage.2013.10.027)
 
-It was inspired by a pipeline from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
-> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile Stimulation Paradigm: A Pipeline for
-> Reproducibility at Every Step of Processing, Going from Individual Sensor Space Representations to an across-Group
-> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi: 10.3389/fnins.2018.00006. PMID: 29403349;
+It was inspired by a pipeline
+from [Lau M. Andersen](https://doi.org/10.3389/fnins.2018.00006)
+> Andersen LM. Group Analysis in MNE-Python of Evoked Responses from a Tactile
+> Stimulation Paradigm: A Pipeline for
+> Reproducibility at Every Step of Processing, Going from Individual Sensor
+> Space Representations to an across-Group
+> Source Space Representation. Front Neurosci. 2018 Jan 22;12:6. doi:
+> 10.3389/fnins.2018.00006. PMID: 29403349;
 > PMCID: PMC5786561.
 
-This program also integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
-> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre Gramfort. 2017.
-> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage, 159, 417-429.
+This program also
+integrates [autoreject](https://doi.org/10.1016/j.neuroimage.2017.06.030)
+> Mainak Jas, Denis Engemann, Yousra Bekhti, Federico Raimondo, and Alexandre
+> Gramfort. 2017.
+> “Autoreject: Automated artifact rejection for MEG and EEG data”. NeuroImage,
+> 159, 417-429.
 
-Many ideas and basics for GUI-Programming where taken from [LearnPyQt](https://www.learnpyqt.com/) and numerous
+Many ideas and basics for GUI-Programming where taken
+from [LearnPyQt](https://www.learnpyqt.com/) and numerous
 stackoverflow-questions/solutions.
 
-The development is financially supported by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
+The development is financially supported
+by [Heidelberg University](https://www.uni-heidelberg.de/de/forschung/forschungsprofil/fields-of-focus/field-of-focus-i).
 
-Thank you to the members of my laboratory (especially my supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271)) for their feedback and testing in the early stages of development.
+Thank you to the members of my laboratory (especially my
+supervisor [Andre Rupp](https://www.klinikum.uni-heidelberg.de/personen/pd-dr-phil-andre-rupp-271))
+for their feedback and testing in the early stages of development.
```

### Comparing `mne-pipeline-hd-0.3.2a0/mne_pipeline_hd.egg-info/SOURCES.txt` & `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+requirements.txt
 mne_pipeline_hd/__init__.py
 mne_pipeline_hd/__main__.py
 mne_pipeline_hd/_version.py
 mne_pipeline_hd/conftest.py
 mne_pipeline_hd.egg-info/PKG-INFO
 mne_pipeline_hd.egg-info/SOURCES.txt
 mne_pipeline_hd.egg-info/dependency_links.txt
@@ -47,14 +48,15 @@
 mne_pipeline_hd/resource/mne_license.txt
 mne_pipeline_hd/resource/mne_pipeline_icon_dark.png
 mne_pipeline_hd/resource/mne_pipeline_icon_light.png
 mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg
 mne_pipeline_hd/resource/parameters.csv
 mne_pipeline_hd/tests/__init__.py
 mne_pipeline_hd/tests/_test_utils.py
+mne_pipeline_hd/tests/test_app.py
 mne_pipeline_hd/tests/test_concurrent.py
 mne_pipeline_hd/tests/test_controller.py
 mne_pipeline_hd/tests/test_functions.py
 mne_pipeline_hd/tests/test_loading.py
 mne_pipeline_hd/tests/test_main_window.py
 mne_pipeline_hd/tests/test_param_guis.py
 mne_pipeline_hd/tests/test_project.py
```

