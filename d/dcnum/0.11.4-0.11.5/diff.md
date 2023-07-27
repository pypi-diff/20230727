# Comparing `tmp/dcnum-0.11.4.tar.gz` & `tmp/dcnum-0.11.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.11.4.tar", last modified: Wed Jul 26 09:55:55 2023, max compression
+gzip compressed data, was "dcnum-0.11.5.tar", last modified: Thu Jul 27 12:54:01 2023, max compression
```

## Comparing `dcnum-0.11.4.tar` & `dcnum-0.11.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.851300 dcnum-0.11.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.835300 dcnum-0.11.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.839300 dcnum-0.11.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-26 09:55:46.000000 dcnum-0.11.4/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-26 09:55:46.000000 dcnum-0.11.4/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-26 09:55:46.000000 dcnum-0.11.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-26 09:55:46.000000 dcnum-0.11.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-26 09:55:46.000000 dcnum-0.11.4/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-26 09:55:46.000000 dcnum-0.11.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-26 09:55:55.851300 dcnum-0.11.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-26 09:55:46.000000 dcnum-0.11.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.839300 dcnum-0.11.4/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.847300 dcnum-0.11.4/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.847300 dcnum-0.11.4/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-26 09:55:46.000000 dcnum-0.11.4/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.843300 dcnum-0.11.4/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 09:55:55.000000 dcnum-0.11.4/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.847300 dcnum-0.11.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-26 09:55:46.000000 dcnum-0.11.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.847300 dcnum-0.11.4/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-26 09:55:46.000000 dcnum-0.11.4/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-26 09:55:46.000000 dcnum-0.11.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-26 09:55:46.000000 dcnum-0.11.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-26 09:55:46.000000 dcnum-0.11.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:55:55.851300 dcnum-0.11.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.851300 dcnum-0.11.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:55:55.851300 dcnum-0.11.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-26 09:55:46.000000 dcnum-0.11.4/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.578607 dcnum-0.11.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-27 12:53:52.000000 dcnum-0.11.5/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-27 12:53:52.000000 dcnum-0.11.5/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-27 12:53:52.000000 dcnum-0.11.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-27 12:53:52.000000 dcnum-0.11.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-27 12:53:52.000000 dcnum-0.11.5/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-27 12:53:52.000000 dcnum-0.11.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 12:54:01.586604 dcnum-0.11.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-27 12:53:52.000000 dcnum-0.11.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-27 12:53:52.000000 dcnum-0.11.5/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.582606 dcnum-0.11.5/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:54:01.000000 dcnum-0.11.5/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 12:53:52.000000 dcnum-0.11.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-27 12:53:52.000000 dcnum-0.11.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:54:01.586604 dcnum-0.11.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:54:01.586604 dcnum-0.11.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-27 12:53:52.000000 dcnum-0.11.5/tests/test_write_writer.py
```

### Comparing `dcnum-0.11.4/.github/workflows/check.yml` & `dcnum-0.11.5/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.5/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/.gitignore` & `dcnum-0.11.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/CHANGELOG` & `dcnum-0.11.5/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.11.5
+ - setup: fix bad package discovery
 0.11.4
  - fix: properly handle empty logs
 0.11.3
  - fix: make sure values in tables dictionary are one-dimensional
 0.11.2
  - meta: increment pipeline ID (texture feature computation)
  - fix: HDF5Data was not pickable
```

### Comparing `dcnum-0.11.4/LICENSE` & `dcnum-0.11.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/PKG-INFO` & `dcnum-0.11.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.4
+Version: 0.11.5
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.4/README.rst` & `dcnum-0.11.5/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.5/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_background/base.py` & `dcnum-0.11.5/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.5/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.5/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.5/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.5/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.5/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/gate.py` & `dcnum-0.11.5/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.5/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/meta/ppid.py` & `dcnum-0.11.5/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/read/cache.py` & `dcnum-0.11.5/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/read/hdf5_data.py` & `dcnum-0.11.5/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/segm/segm_thresh.py` & `dcnum-0.11.5/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/segm/segmenter.py` & `dcnum-0.11.5/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.5/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/segm/segmenter_gpu.py` & `dcnum-0.11.5/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.5/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.5/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.5/dcnum/write/queue_collector_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
             if len(cur_nevents) == 0:
                 self.logger.warning("Encountered empty nevents array!")
                 break
 
             # We have reached the writer threshold. This means the extractor
             # has analyzed at least `write_threshold` frames (not events).
-            self.logger.debug(f"Current frane: {cur_frame}")
+            self.logger.debug(f"Current frame: {cur_frame}")
 
             # Create an event stash
             stash = EventStash(
                 index_offset=cur_frame,
                 feat_nevents=cur_nevents
             )
```

### Comparing `dcnum-0.11.4/dcnum/write/writer.py` & `dcnum-0.11.5/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.5/dcnum.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.11.4
+Version: 0.11.5
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.11.4/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.5/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/docs/conf.py` & `dcnum-0.11.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/docs/extensions/github_changelog.py` & `dcnum-0.11.5/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/pyproject.toml` & `dcnum-0.11.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -36,13 +36,10 @@
 
 [project.urls]
 source = "https://github.com/DC-Analysis/dcnum"
 tracker = "https://github.com/DC-Analysis/dcnum/issues"
 documentation = "https://dcnum.readthedocs.io/en/stable/"
 changelog = "https://dcnum.readthedocs.io/en/stable/sec_changelog.html"
 
-[tool.setuptools.packages]
-find = {}
-
 [tool.setuptools_scm]
 write_to = "dcnum/_version.py"
 version_scheme = "post-release"
```

### Comparing `dcnum-0.11.4/tests/conftest.py` & `dcnum-0.11.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/helper_methods.py` & `dcnum-0.11.5/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.5/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_feat_brightness.py` & `dcnum-0.11.5/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_feat_haralick.py` & `dcnum-0.11.5/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_feat_moments_based.py` & `dcnum-0.11.5/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_ppid.py` & `dcnum-0.11.5/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_read_concat_hdf5.py` & `dcnum-0.11.5/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_read_hdf5.py` & `dcnum-0.11.5/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_segm_thresh.py` & `dcnum-0.11.5/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_segmenter.py` & `dcnum-0.11.5/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.5/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.11.4/tests/test_write_writer.py` & `dcnum-0.11.5/tests/test_write_writer.py`

 * *Files identical despite different names*

