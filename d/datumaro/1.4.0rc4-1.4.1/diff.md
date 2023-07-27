# Comparing `tmp/datumaro-1.4.0rc4.tar.gz` & `tmp/datumaro-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.4.0rc4.tar", last modified: Thu Jul 20 08:13:36 2023, max compression
+gzip compressed data, was "datumaro-1.4.1.tar", last modified: Thu Jul 27 08:19:51 2023, max compression
```

## Comparing `datumaro-1.4.0rc4.tar` & `datumaro-1.4.1.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)   391964 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.632900 datumaro-1.4.0rc4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.636900 datumaro-1.4.0rc4/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29711 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    25867 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.636900 datumaro-1.4.0rc4/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.962949 datumaro-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)   391964 2023-07-27 08:19:39.000000 datumaro-1.4.1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-27 08:19:39.000000 datumaro-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 08:19:39.000000 datumaro-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-27 08:19:39.000000 datumaro-1.4.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-27 08:19:51.962949 datumaro-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-27 08:19:39.000000 datumaro-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-27 08:19:40.000000 datumaro-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-27 08:19:40.000000 datumaro-1.4.1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-27 08:19:40.000000 datumaro-1.4.1/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:19:51.962949 datumaro-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-07-27 08:19:40.000000 datumaro-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.910948 datumaro-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.918949 datumaro-1.4.1/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.922949 datumaro-1.4.1/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.922949 datumaro-1.4.1/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.922949 datumaro-1.4.1/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.922949 datumaro-1.4.1/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.926949 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.926949 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.926949 datumaro-1.4.1/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.926949 datumaro-1.4.1/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.926949 datumaro-1.4.1/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.930949 datumaro-1.4.1/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.930949 datumaro-1.4.1/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.930949 datumaro-1.4.1/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.930949 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29711 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25867 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.934949 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23596 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.942949 datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.946949 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.950949 datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.954949 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.958949 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.958949 datumaro-1.4.1/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.958949 datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.958949 datumaro-1.4.1/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.958949 datumaro-1.4.1/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.962949 datumaro-1.4.1/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 08:19:40.000000 datumaro-1.4.1/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:19:51.922949 datumaro-1.4.1/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 08:19:51.000000 datumaro-1.4.1/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.4.0rc4/3rd-party.txt` & `datumaro-1.4.1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/LICENSE` & `datumaro-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/PKG-INFO` & `datumaro-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc4
+Version: 1.4.1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc4/README.md` & `datumaro-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/pyproject.toml` & `datumaro-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/requirements-core.txt` & `datumaro-1.4.1/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/setup.py` & `datumaro-1.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def find_version(project_dir=None):
     if not project_dir:
         project_dir = osp.dirname(osp.abspath(__file__))
 
     file_path = osp.join(project_dir, "datumaro", "version.py")
 
-    with open(file_path, "r") as version_file:
+    with open(file_path, "r", encoding="utf-8") as version_file:
         version_text = version_file.read()
 
     # PEP440:
     # https://www.python.org/dev/peps/pep-0440/#appendix-b-parsing-version-strings-with-regular-expressions
     pep_regex = r"([1-9]\d*!)?(0|[1-9]\d*)(\.(0|[1-9]\d*))*((a|b|rc)(0|[1-9]\d*))?(\.post(0|[1-9]\d*))?(\.dev(0|[1-9]\d*))?"
     version_regex = r"__version__\s*=\s*.(" + pep_regex + ")."
     match = re.match(version_regex, version_text)
@@ -35,27 +35,27 @@
 
 
 CORE_REQUIREMENTS_FILE = "requirements-core.txt"
 DEFAULT_REQUIREMENTS_FILE = "requirements-default.txt"
 
 
 def parse_requirements(filename=CORE_REQUIREMENTS_FILE):
-    with open(filename) as fh:
+    with open(filename, "r", encoding="utf-8") as fh:
         return fh.readlines()
 
 
 CORE_REQUIREMENTS = parse_requirements(CORE_REQUIREMENTS_FILE)
 if strtobool(os.getenv("DATUMARO_HEADLESS", "0").lower()):
     CORE_REQUIREMENTS.append("opencv-python-headless")
 else:
     CORE_REQUIREMENTS.append("opencv-python")
 
 DEFAULT_REQUIREMENTS = parse_requirements(DEFAULT_REQUIREMENTS_FILE)
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 ext_modules = [
     Pybind11Extension(
         "datumaro._capi",
         ["src/datumaro/capi/pybind.cpp"],
         define_macros=[("VERSION_INFO", find_version("./src"))],
```

### Comparing `datumaro-1.4.0rc4/src/datumaro/__init__.py` & `datumaro-1.4.1/src/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/capi/pybind.cpp` & `datumaro-1.4.1/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/__main__.py` & `datumaro-1.4.1/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/__init__.py` & `datumaro-1.4.1/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/compare.py` & `datumaro-1.4.1/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/convert.py` & `datumaro-1.4.1/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.4.1/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/download.py` & `datumaro-1.4.1/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/explain.py` & `datumaro-1.4.1/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/explore.py` & `datumaro-1.4.1/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/filter.py` & `datumaro-1.4.1/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/generate.py` & `datumaro-1.4.1/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/info.py` & `datumaro-1.4.1/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/merge.py` & `datumaro-1.4.1/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/patch.py` & `datumaro-1.4.1/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/prune.py` & `datumaro-1.4.1/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.4.1/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/stats.py` & `datumaro-1.4.1/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/transform.py` & `datumaro-1.4.1/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/commands/validate.py` & `datumaro-1.4.1/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/contexts/model.py` & `datumaro-1.4.1/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.4.1/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/contexts/source.py` & `datumaro-1.4.1/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/contexts/util.py` & `datumaro-1.4.1/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/util/__init__.py` & `datumaro-1.4.1/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/util/compare.py` & `datumaro-1.4.1/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/cli/util/project.py` & `datumaro-1.4.1/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/abstracts/merger.py` & `datumaro-1.4.1/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.4.1/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/algorithms/rise.py` & `datumaro-1.4.1/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/annotation.py` & `datumaro-1.4.1/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/annotations/matcher.py` & `datumaro-1.4.1/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/annotations/merger.py` & `datumaro-1.4.1/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/cli_plugin.py` & `datumaro-1.4.1/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/comparator.py` & `datumaro-1.4.1/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/config.py` & `datumaro-1.4.1/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/config_model.py` & `datumaro-1.4.1/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/contexts/importer.py` & `datumaro-1.4.1/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/crypter.py` & `datumaro-1.4.1/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/dataset.py` & `datumaro-1.4.1/src/datumaro/components/dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/dataset_base.py` & `datumaro-1.4.1/src/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.4.1/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/dataset_storage.py` & `datumaro-1.4.1/src/datumaro/components/dataset_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/environment.py` & `datumaro-1.4.1/src/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/errors.py` & `datumaro-1.4.1/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/exporter.py` & `datumaro-1.4.1/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/extractor_tfds.py` & `datumaro-1.4.1/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/filter.py` & `datumaro-1.4.1/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/format_detection.py` & `datumaro-1.4.1/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/generator.py` & `datumaro-1.4.1/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.4.1/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/importer.py` & `datumaro-1.4.1/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/launcher.py` & `datumaro-1.4.1/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/lazy_plugin.py` & `datumaro-1.4.1/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/media.py` & `datumaro-1.4.1/src/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/media_manager.py` & `datumaro-1.4.1/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/__init__.py` & `datumaro-1.4.1/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/base.py` & `datumaro-1.4.1/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.4.1/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.4.1/src/datumaro/components/merge/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.4.1/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/merge/union_merge.py` & `datumaro-1.4.1/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/operations.py` & `datumaro-1.4.1/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/progress_reporting.py` & `datumaro-1.4.1/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/project.py` & `datumaro-1.4.1/src/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/shift_analyzer.py` & `datumaro-1.4.1/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/transformer.py` & `datumaro-1.4.1/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/validator.py` & `datumaro-1.4.1/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/components/visualizer.py` & `datumaro-1.4.1/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.4.1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -279,18 +279,23 @@
 
             yield item
             length += 1
 
         self._length = length
 
     def _parse_anns(self, img_info, ann_info, item):
-        if self._task is not CocoTask.panoptic:
-            self._load_annotations(ann_info, img_info, parsed_annotations=item.annotations)
-        else:
-            self._load_panoptic_ann(ann_info, parsed_annotations=item.annotations)
+        try:
+            if self._task is not CocoTask.panoptic:
+                self._load_annotations(ann_info, img_info, parsed_annotations=item.annotations)
+            else:
+                self._load_panoptic_ann(ann_info, parsed_annotations=item.annotations)
+        except Exception as e:
+            self._ctx.error_policy.report_annotation_error(
+                e, item_id=(ann_info.get("id", None), self._subset)
+            )
 
     def _load_items(self, json_data):
         pbar = self._ctx.progress_reporter
 
         def _gen_ann(info_lists):
             while info_lists:
                 yield info_lists.pop()
```

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,192 +119,203 @@
                 yield item_descs.pop()
 
         items = []
         for item_desc in pbar.iter(
             _gen(), desc=f"Importing '{self._subset}'", total=len(item_descs)
         ):
             item = self._parse_item(item_desc)
-            items.append(item)
+            if item is not None:
+                items.append(item)
 
         return items
 
-    def _parse_item(self, item_desc):
-        item_id = item_desc["id"]
-
-        media = None
-        image_info = item_desc.get("image")
-        if image_info:
-            image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
-            image_path = osp.join(self._images_dir, self._subset, image_filename)
-            if not osp.isfile(image_path):
-                # backward compatibility
-                old_image_path = osp.join(self._images_dir, image_filename)
-                if osp.isfile(old_image_path):
-                    image_path = old_image_path
-
-            media = Image.from_file(path=image_path, size=image_info.get("size"))
-            if self.media_type == MediaElement:
-                self.media_type = Image
-
-        pcd_info = item_desc.get("point_cloud")
-        if media and pcd_info:
-            raise MediaTypeError("Dataset cannot contain multiple media types")
-        if pcd_info:
-            pcd_path = pcd_info.get("path")
-            point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
-
-            related_images = None
-            ri_info = item_desc.get("related_images")
-            if ri_info:
-                related_images = [
-                    Image.from_file(
-                        size=ri.get("size"),
-                        path=osp.join(self._images_dir, self._subset, ri.get("path")),
-                    )
-                    for ri in ri_info
-                ]
-
-            media = PointCloud.from_file(path=point_cloud, extra_images=related_images)
-            if self.media_type == MediaElement:
-                self.media_type = PointCloud
-
-        media_desc = item_desc.get("media")
-        if not media and media_desc and media_desc.get("path"):
-            media = MediaElement(path=media_desc.get("path"))
+    def _parse_item(self, item_desc: Dict) -> Optional[DatasetItem]:
+        try:
+            item_id = item_desc["id"]
+
+            media = None
+            image_info = item_desc.get("image")
+            if image_info:
+                image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
+                image_path = osp.join(self._images_dir, self._subset, image_filename)
+                if not osp.isfile(image_path):
+                    # backward compatibility
+                    old_image_path = osp.join(self._images_dir, image_filename)
+                    if osp.isfile(old_image_path):
+                        image_path = old_image_path
+
+                media = Image.from_file(path=image_path, size=image_info.get("size"))
+                if self.media_type == MediaElement:
+                    self.media_type = Image
+
+            pcd_info = item_desc.get("point_cloud")
+            if media and pcd_info:
+                raise MediaTypeError("Dataset cannot contain multiple media types")
+            if pcd_info:
+                pcd_path = pcd_info.get("path")
+                point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
+
+                related_images = None
+                ri_info = item_desc.get("related_images")
+                if ri_info:
+                    related_images = [
+                        Image.from_file(
+                            size=ri.get("size"),
+                            path=osp.join(self._images_dir, self._subset, ri.get("path")),
+                        )
+                        for ri in ri_info
+                    ]
+
+                media = PointCloud.from_file(path=point_cloud, extra_images=related_images)
+                if self.media_type == MediaElement:
+                    self.media_type = PointCloud
+
+            media_desc = item_desc.get("media")
+            if not media and media_desc and media_desc.get("path"):
+                media = MediaElement(path=media_desc.get("path"))
+
+        except Exception as e:
+            self._ctx.error_policy.report_item_error(
+                e, item_id=(item_desc.get("id", None), self._subset)
+            )
+            return None
 
         annotations = self._load_annotations(item_desc)
 
-        item = DatasetItem(
+        return DatasetItem(
             id=item_id,
             subset=self._subset,
             annotations=annotations,
             media=media,
             attributes=item_desc.get("attr"),
         )
 
-        return item
-
-    @staticmethod
-    def _load_annotations(item):
-        parsed = item["annotations"]
+    def _load_annotations(self, item: Dict):
         loaded = []
 
-        for ann in parsed:
-            ann_id = ann.get("id")
-            ann_type = AnnotationType[ann["type"]]
-            attributes = ann.get("attributes")
-            group = ann.get("group")
-
-            label_id = ann.get("label_id")
-            z_order = ann.get("z_order")
-            points = ann.get("points")
-
-            if ann_type == AnnotationType.label:
-                loaded.append(Label(label=label_id, id=ann_id, attributes=attributes, group=group))
-
-            elif ann_type == AnnotationType.mask:
-                rle = ann["rle"]
-                rle["counts"] = rle["counts"].encode("ascii")
-                loaded.append(
-                    RleMask(
-                        rle=rle,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
-
-            elif ann_type == AnnotationType.polyline:
-                loaded.append(
-                    PolyLine(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
-
-            elif ann_type == AnnotationType.polygon:
-                loaded.append(
-                    Polygon(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
-
-            elif ann_type == AnnotationType.bbox:
-                x, y, w, h = ann["bbox"]
-                loaded.append(
-                    Bbox(
-                        x,
-                        y,
-                        w,
-                        h,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
-
-            elif ann_type == AnnotationType.points:
-                loaded.append(
-                    Points(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
+        for ann in item.get("annotations", []):
+            try:
+                ann_id = ann.get("id")
+                ann_type = AnnotationType[ann["type"]]
+                attributes = ann.get("attributes")
+                group = ann.get("group")
+
+                label_id = ann.get("label_id")
+                z_order = ann.get("z_order")
+                points = ann.get("points")
+
+                if ann_type == AnnotationType.label:
+                    loaded.append(
+                        Label(label=label_id, id=ann_id, attributes=attributes, group=group)
+                    )
+
+                elif ann_type == AnnotationType.mask:
+                    rle = ann["rle"]
+                    rle["counts"] = rle["counts"].encode("ascii")
+                    loaded.append(
+                        RleMask(
+                            rle=rle,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.polyline:
+                    loaded.append(
+                        PolyLine(
+                            points,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.polygon:
+                    loaded.append(
+                        Polygon(
+                            points,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.bbox:
+                    x, y, w, h = ann["bbox"]
+                    loaded.append(
+                        Bbox(
+                            x,
+                            y,
+                            w,
+                            h,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.points:
+                    loaded.append(
+                        Points(
+                            points,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.caption:
+                    caption = ann.get("caption")
+                    loaded.append(Caption(caption, id=ann_id, attributes=attributes, group=group))
+
+                elif ann_type == AnnotationType.cuboid_3d:
+                    loaded.append(
+                        Cuboid3d(
+                            ann.get("position"),
+                            ann.get("rotation"),
+                            ann.get("scale"),
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.ellipse:
+                    loaded.append(
+                        Ellipse(
+                            *points,
+                            label=label_id,
+                            id=ann_id,
+                            attributes=attributes,
+                            group=group,
+                            z_order=z_order,
+                        )
+                    )
+
+                elif ann_type == AnnotationType.hash_key:
+                    continue
+                else:
+                    raise NotImplementedError()
+            except Exception as e:
+                self._ctx.error_policy.report_annotation_error(
+                    e, item_id=(ann.get("id", None), self._subset)
                 )
 
-            elif ann_type == AnnotationType.caption:
-                caption = ann.get("caption")
-                loaded.append(Caption(caption, id=ann_id, attributes=attributes, group=group))
-
-            elif ann_type == AnnotationType.cuboid_3d:
-                loaded.append(
-                    Cuboid3d(
-                        ann.get("position"),
-                        ann.get("rotation"),
-                        ann.get("scale"),
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                    )
-                )
-
-            elif ann_type == AnnotationType.ellipse:
-                loaded.append(
-                    Ellipse(
-                        *points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
-
-            elif ann_type == AnnotationType.hash_key:
-                continue
-            else:
-                raise NotImplementedError()
-
         return loaded
 
     def __len__(self):
         return len(self.items)
 
     def __iter__(self):
         yield from self.items
```

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.4.1/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/explorer.py` & `datumaro-1.4.1/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.4.1/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.4.1/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/ndr.py` & `datumaro-1.4.1/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.4.1/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.4.1/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.4.1/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.4.1/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/specs.json` & `datumaro-1.4.1/src/datumaro/plugins/specs.json`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/specs.py` & `datumaro-1.4.1/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/splitter.py` & `datumaro-1.4.1/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.4.1/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.4.1/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.4.1/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.4.1/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.4.1/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/util.py` & `datumaro-1.4.1/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/transforms.py` & `datumaro-1.4.1/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/plugins/validators.py` & `datumaro-1.4.1/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/__init__.py` & `datumaro-1.4.1/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/annotation_util.py` & `datumaro-1.4.1/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/attrs_util.py` & `datumaro-1.4.1/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/definitions.py` & `datumaro-1.4.1/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/file_utils.py` & `datumaro-1.4.1/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/image.py` & `datumaro-1.4.1/src/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/image_cache.py` & `datumaro-1.4.1/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/log_utils.py` & `datumaro-1.4.1/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/mask_tools.py` & `datumaro-1.4.1/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/meta_file_util.py` & `datumaro-1.4.1/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/os_util.py` & `datumaro-1.4.1/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/pickle_util.py` & `datumaro-1.4.1/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/scope.py` & `datumaro-1.4.1/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/telemetry_stub.py` & `datumaro-1.4.1/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/telemetry_utils.py` & `datumaro-1.4.1/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro/util/tf_util.py` & `datumaro-1.4.1/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.4.1/src/datumaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc4
+Version: 1.4.1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc4/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.4.1/src/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc4/src/datumaro.egg-info/requires.txt` & `datumaro-1.4.1/src/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

