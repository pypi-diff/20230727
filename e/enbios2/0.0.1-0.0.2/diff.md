# Comparing `tmp/enbios2-0.0.1.tar.gz` & `tmp/enbios2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enbios2-0.0.1.tar", last modified: Thu Jul 27 15:59:28 2023, max compression
+gzip compressed data, was "enbios2-0.0.2.tar", last modified: Thu Jul 27 16:57:33 2023, max compression
```

## Comparing `enbios2-0.0.1.tar` & `enbios2-0.0.2.tar`

### file list

```diff
@@ -1,106 +1,100 @@
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.053024 enbios2-0.0.1/
--rw-rw-r--   0 ram       (1001) ram       (1001)     1302 2023-07-11 09:20:15.000000 enbios2-0.0.1/LICENSE
--rw-rw-r--   0 ram       (1001) ram       (1001)     1183 2023-07-27 15:59:28.053024 enbios2-0.0.1/PKG-INFO
--rw-rw-r--   0 ram       (1001) ram       (1001)      942 2023-07-27 06:32:38.000000 enbios2-0.0.1/README.md
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.037024 enbios2-0.0.1/enbios2/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/__init__.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.041024 enbios2-0.0.1/enbios2/analyse/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/analyse/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6369 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/analyse/callipope_ana.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      425 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/analyse/const.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4981 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/analyse/experiment_exporter.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      561 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/analyse/util.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    14944 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/analyse/vizprevexperiment.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.041024 enbios2-0.0.1/enbios2/base/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/base/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      615 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/base/databases.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2243 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/base/db_fields.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6094 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/base/db_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    22348 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/base/experiment.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     5141 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/base/experiment_io.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      798 2023-07-13 10:46:47.000000 enbios2-0.0.1/enbios2/base/unit_registry.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.041024 enbios2-0.0.1/enbios2/bw2/
--rw-rw-r--   0 ram       (1001) ram       (1001)       49 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/bw2/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2917 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/bw2/bw_autoimporter.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1921 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/bw2/experiment_multiLCA.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1185 2023-07-11 09:20:15.000000 enbios2-0.0.1/enbios2/bw2/extract_from_xml.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4221 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/bw2/project_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4959 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/bw2/util.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      508 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/const.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.041024 enbios2-0.0.1/enbios2/demos/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/demos/__init__.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.041024 enbios2-0.0.1/enbios2/dev/
--rw-rw-r--   0 ram       (1001) ram       (1001)      529 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/dev/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      585 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/dev/create_experiment_schema.py
--rw-rw-r--   0 ram       (1001) ram       (1001)       71 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/dev/pull_docs.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.045024 enbios2-0.0.1/enbios2/ecoinvent/
--rw-rw-r--   0 ram       (1001) ram       (1001)       58 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/ecoinvent/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     7885 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/ecoinvent/ecoinvent_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     8217 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1663 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/ecoinvent/spatial.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.045024 enbios2-0.0.1/enbios2/enbios_extend/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/enbios_extend/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    13099 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/enbios_extend/bw_lci2nis.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.045024 enbios2-0.0.1/enbios2/enbios_extend/nis/
--rw-rw-r--   0 ram       (1001) ram       (1001)      696 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/enbios_extend/nis/_1_lci_to_nis.py
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/enbios_extend/nis/__init__.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/experiment/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3541 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/activity_search.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     6925 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/ai_lcia.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/experiment/bw2/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/bw2/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      333 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/bw2/non_linear_methods.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3678 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/bw2sigma.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1094 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/bw_manipulation.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3462 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/characterizations.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      232 2023-07-11 21:09:47.000000 enbios2-0.0.1/enbios2/experiment/class_static_me.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1954 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/comp_numba.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1764 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/create_networkx.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     7578 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/dot2bw.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     8238 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/fast_tree.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/experiment/gnn/
--rw-rw-r--   0 ram       (1001) ram       (1001)     2409 2023-07-14 23:13:54.000000 enbios2-0.0.1/enbios2/experiment/gnn/base.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/experiment/my_numba/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/my_numba/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      811 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/my_numba/simple.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    12309 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/promt_toolkit_checker.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/schema_builder.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3342 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/spold2json.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      977 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/starcoder.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4012 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/sum_hierarchy.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     4241 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/tree_transformer.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      346 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/experiment/util.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/generic/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/generic/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3065 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/generic/enbios2_logging.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     3003 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/generic/files.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.049024 enbios2-0.0.1/enbios2/generic/tree/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/generic/tree/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    27164 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/generic/tree/basic_tree.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     2852 2023-07-27 06:31:58.000000 enbios2-0.0.1/enbios2/generic/util.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.053024 enbios2-0.0.1/enbios2/models/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/models/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1256 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/models/bw_project_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)    11014 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/models/experiment_models.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      378 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/models/prepare.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.053024 enbios2-0.0.1/enbios2/plot/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/plot/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1440 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/plot/sanky1.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.053024 enbios2-0.0.1/enbios2/plotting/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/plotting/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1599 2023-07-27 06:32:38.000000 enbios2-0.0.1/enbios2/plotting/plot_experiment.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      273 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/settings.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.053024 enbios2-0.0.1/enbios2/test/
--rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/test/__init__.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      338 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/test/conftest.py
--rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/test/master_index.py
--rw-rw-r--   0 ram       (1001) ram       (1001)     1444 2023-07-11 08:36:40.000000 enbios2-0.0.1/enbios2/test/test_dot2bw.py
-drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 15:59:28.037024 enbios2-0.0.1/enbios2.egg-info/
--rw-rw-r--   0 ram       (1001) ram       (1001)     1183 2023-07-27 15:59:28.000000 enbios2-0.0.1/enbios2.egg-info/PKG-INFO
--rw-rw-r--   0 ram       (1001) ram       (1001)     2543 2023-07-27 15:59:28.000000 enbios2-0.0.1/enbios2.egg-info/SOURCES.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)        1 2023-07-27 15:59:28.000000 enbios2-0.0.1/enbios2.egg-info/dependency_links.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)      110 2023-07-27 15:59:28.000000 enbios2-0.0.1/enbios2.egg-info/requires.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)        8 2023-07-27 15:59:28.000000 enbios2-0.0.1/enbios2.egg-info/top_level.txt
--rw-rw-r--   0 ram       (1001) ram       (1001)      744 2023-07-27 15:59:20.000000 enbios2-0.0.1/pyproject.toml
--rw-rw-r--   0 ram       (1001) ram       (1001)       38 2023-07-27 15:59:28.053024 enbios2-0.0.1/setup.cfg
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1302 2023-07-11 09:20:15.000000 enbios2-0.0.2/LICENSE
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1164 2023-07-27 16:57:33.250920 enbios2-0.0.2/PKG-INFO
+-rw-rw-r--   0 ram       (1001) ram       (1001)      943 2023-07-27 16:04:30.000000 enbios2-0.0.2/README.md
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.234920 enbios2-0.0.2/enbios2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/__init__.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.238920 enbios2-0.0.2/enbios2/analyse/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/analyse/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6369 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/analyse/callipope_ana.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      425 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/analyse/const.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4981 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/analyse/experiment_exporter.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      561 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/analyse/util.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    14944 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/analyse/vizprevexperiment.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.238920 enbios2-0.0.2/enbios2/base/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/base/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      615 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/base/databases.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2243 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/base/db_fields.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6094 2023-07-27 06:31:58.000000 enbios2-0.0.2/enbios2/base/db_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    22348 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/base/experiment.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     5141 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/base/experiment_io.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      798 2023-07-13 10:46:47.000000 enbios2-0.0.2/enbios2/base/unit_registry.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.238920 enbios2-0.0.2/enbios2/bw2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)       49 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/bw2/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2917 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/bw2/bw_autoimporter.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1921 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/bw2/experiment_multiLCA.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1185 2023-07-11 09:20:15.000000 enbios2-0.0.2/enbios2/bw2/extract_from_xml.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4187 2023-07-27 16:26:05.000000 enbios2-0.0.2/enbios2/bw2/project_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4959 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/bw2/util.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      508 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/const.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.238920 enbios2-0.0.2/enbios2/demos/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/demos/__init__.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.242920 enbios2-0.0.2/enbios2/dev/
+-rw-rw-r--   0 ram       (1001) ram       (1001)      529 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/dev/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      585 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/dev/create_experiment_schema.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)       71 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/dev/pull_docs.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.242920 enbios2-0.0.2/enbios2/ecoinvent/
+-rw-rw-r--   0 ram       (1001) ram       (1001)       58 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/ecoinvent/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     7885 2023-07-27 06:31:58.000000 enbios2-0.0.2/enbios2/ecoinvent/ecoinvent_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     8217 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1663 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/ecoinvent/spatial.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.246920 enbios2-0.0.2/enbios2/experiment/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3541 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/activity_search.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     6925 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/ai_lcia.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.246920 enbios2-0.0.2/enbios2/experiment/bw2/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/bw2/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      333 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/bw2/non_linear_methods.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3678 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/bw2sigma.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1094 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/bw_manipulation.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3462 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/characterizations.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      232 2023-07-11 21:09:47.000000 enbios2-0.0.2/enbios2/experiment/class_static_me.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1954 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/comp_numba.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1764 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/create_networkx.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     7578 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/dot2bw.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     8238 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/fast_tree.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.246920 enbios2-0.0.2/enbios2/experiment/gnn/
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2409 2023-07-14 23:13:54.000000 enbios2-0.0.2/enbios2/experiment/gnn/base.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.246920 enbios2-0.0.2/enbios2/experiment/my_numba/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/my_numba/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      811 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/my_numba/simple.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    12309 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/promt_toolkit_checker.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/schema_builder.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3342 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/spold2json.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      977 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/starcoder.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4012 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/sum_hierarchy.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     4241 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/tree_transformer.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      346 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/experiment/util.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.246920 enbios2-0.0.2/enbios2/generic/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/generic/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3065 2023-07-27 06:31:58.000000 enbios2-0.0.2/enbios2/generic/enbios2_logging.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     3033 2023-07-27 16:22:19.000000 enbios2-0.0.2/enbios2/generic/files.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/enbios2/generic/tree/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/generic/tree/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    27164 2023-07-27 06:31:58.000000 enbios2-0.0.2/enbios2/generic/tree/basic_tree.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2852 2023-07-27 06:31:58.000000 enbios2-0.0.2/enbios2/generic/util.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/enbios2/models/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/models/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1256 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/models/bw_project_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)    11014 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/models/experiment_models.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      378 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/models/prepare.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/enbios2/plot/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/plot/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1440 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/plot/sanky1.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/enbios2/plotting/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/plotting/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1599 2023-07-27 06:32:38.000000 enbios2-0.0.2/enbios2/plotting/plot_experiment.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      273 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/settings.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.250920 enbios2-0.0.2/enbios2/test/
+-rw-rw-r--   0 ram       (1001) ram       (1001)        0 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/test/__init__.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      338 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/test/conftest.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)      593 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/test/master_index.py
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1444 2023-07-11 08:36:40.000000 enbios2-0.0.2/enbios2/test/test_dot2bw.py
+drwxrwxr-x   0 ram       (1001) ram       (1001)        0 2023-07-27 16:57:33.234920 enbios2-0.0.2/enbios2.egg-info/
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1164 2023-07-27 16:57:33.000000 enbios2-0.0.2/enbios2.egg-info/PKG-INFO
+-rw-rw-r--   0 ram       (1001) ram       (1001)     2392 2023-07-27 16:57:33.000000 enbios2-0.0.2/enbios2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)        1 2023-07-27 16:57:33.000000 enbios2-0.0.2/enbios2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1034 2023-07-27 16:57:33.000000 enbios2-0.0.2/enbios2.egg-info/requires.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)        8 2023-07-27 16:57:33.000000 enbios2-0.0.2/enbios2.egg-info/top_level.txt
+-rw-rw-r--   0 ram       (1001) ram       (1001)     1583 2023-07-27 16:57:26.000000 enbios2-0.0.2/pyproject.toml
+-rw-rw-r--   0 ram       (1001) ram       (1001)       38 2023-07-27 16:57:33.254920 enbios2-0.0.2/setup.cfg
```

### Comparing `enbios2-0.0.1/LICENSE` & `enbios2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/PKG-INFO` & `enbios2-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: enbios2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-# enbios2
+# Enbios 2
 
 This a ground up new implementation of enbios.
 
 Compared to the original version of enbios, this version is more flexible does not make it's own LCA calculations, but
 uses brightway2 for that.
 
 The main functionality of enbios2 is currently to run experiments, which are described a set of (brightway) activities a
```

### Comparing `enbios2-0.0.1/README.md` & `enbios2-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# enbios2
+# Enbios 2
 
 This a ground up new implementation of enbios.
 
 Compared to the original version of enbios, this version is more flexible does not make it's own LCA calculations, but
 uses brightway2 for that.
 
 The main functionality of enbios2 is currently to run experiments, which are described a set of (brightway) activities a
```

### Comparing `enbios2-0.0.1/enbios2/analyse/callipope_ana.py` & `enbios2-0.0.2/enbios2/analyse/callipope_ana.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/analyse/experiment_exporter.py` & `enbios2-0.0.2/enbios2/analyse/experiment_exporter.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/analyse/util.py` & `enbios2-0.0.2/enbios2/analyse/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/analyse/vizprevexperiment.py` & `enbios2-0.0.2/enbios2/analyse/vizprevexperiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/databases.py` & `enbios2-0.0.2/enbios2/base/databases.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/db_fields.py` & `enbios2-0.0.2/enbios2/base/db_fields.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/db_models.py` & `enbios2-0.0.2/enbios2/base/db_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/experiment.py` & `enbios2-0.0.2/enbios2/base/experiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/experiment_io.py` & `enbios2-0.0.2/enbios2/base/experiment_io.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/base/unit_registry.py` & `enbios2-0.0.2/enbios2/base/unit_registry.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/bw2/bw_autoimporter.py` & `enbios2-0.0.2/enbios2/bw2/bw_autoimporter.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/bw2/experiment_multiLCA.py` & `enbios2-0.0.2/enbios2/bw2/experiment_multiLCA.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/bw2/extract_from_xml.py` & `enbios2-0.0.2/enbios2/bw2/extract_from_xml.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/bw2/project_index.py` & `enbios2-0.0.2/enbios2/bw2/project_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 This helps with the problem of different bw project names on different machines
 """
 from typing import Optional
 
 import bw2data
 import yaml
 from bw2data.backends import SQLiteBackend
-from peewee import SqliteDatabase
 
 from enbios2.base.databases import init_databases
 from enbios2.base.db_models import BWProjectIndex, EcoinventDataset
 from enbios2.ecoinvent.ecoinvent_index import get_ecoinvent_dataset_index
 from enbios2.generic.enbios2_logging import get_logger
 
 projects = bw2data.projects
```

### Comparing `enbios2-0.0.1/enbios2/bw2/util.py` & `enbios2-0.0.2/enbios2/bw2/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/dev/__init__.py` & `enbios2-0.0.2/enbios2/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/dev/create_experiment_schema.py` & `enbios2-0.0.2/enbios2/dev/create_experiment_schema.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/ecoinvent/ecoinvent_index.py` & `enbios2-0.0.2/enbios2/ecoinvent/ecoinvent_index.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py` & `enbios2-0.0.2/enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/ecoinvent/spatial.py` & `enbios2-0.0.2/enbios2/ecoinvent/spatial.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/activity_search.py` & `enbios2-0.0.2/enbios2/experiment/activity_search.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/ai_lcia.py` & `enbios2-0.0.2/enbios2/experiment/ai_lcia.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/bw2sigma.py` & `enbios2-0.0.2/enbios2/experiment/bw2sigma.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/bw_manipulation.py` & `enbios2-0.0.2/enbios2/experiment/bw_manipulation.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/characterizations.py` & `enbios2-0.0.2/enbios2/experiment/characterizations.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/comp_numba.py` & `enbios2-0.0.2/enbios2/experiment/comp_numba.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/create_networkx.py` & `enbios2-0.0.2/enbios2/experiment/create_networkx.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/dot2bw.py` & `enbios2-0.0.2/enbios2/experiment/dot2bw.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/fast_tree.py` & `enbios2-0.0.2/enbios2/experiment/fast_tree.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/gnn/base.py` & `enbios2-0.0.2/enbios2/experiment/gnn/base.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/my_numba/simple.py` & `enbios2-0.0.2/enbios2/experiment/my_numba/simple.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/promt_toolkit_checker.py` & `enbios2-0.0.2/enbios2/experiment/promt_toolkit_checker.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/schema_builder.py` & `enbios2-0.0.2/enbios2/experiment/schema_builder.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/spold2json.py` & `enbios2-0.0.2/enbios2/experiment/spold2json.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/starcoder.py` & `enbios2-0.0.2/enbios2/experiment/starcoder.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/sum_hierarchy.py` & `enbios2-0.0.2/enbios2/experiment/sum_hierarchy.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/experiment/tree_transformer.py` & `enbios2-0.0.2/enbios2/experiment/tree_transformer.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/generic/enbios2_logging.py` & `enbios2-0.0.2/enbios2/generic/enbios2_logging.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/generic/files.py` & `enbios2-0.0.2/enbios2/generic/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from csv import DictReader
 from pathlib import Path
 from typing import Generator, Optional
 
 import openpyxl
+import xmltodict as xmltodict
 
 import yaml
 
 from enbios2.const import BASE_DATA_PATH
 from enbios2.generic.enbios2_logging import get_logger
 
 logger = get_logger(__file__)
```

### Comparing `enbios2-0.0.1/enbios2/generic/tree/basic_tree.py` & `enbios2-0.0.2/enbios2/generic/tree/basic_tree.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/generic/util.py` & `enbios2-0.0.2/enbios2/generic/util.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/models/bw_project_models.py` & `enbios2-0.0.2/enbios2/models/bw_project_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/models/experiment_models.py` & `enbios2-0.0.2/enbios2/models/experiment_models.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/plot/sanky1.py` & `enbios2-0.0.2/enbios2/plot/sanky1.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/plotting/plot_experiment.py` & `enbios2-0.0.2/enbios2/plotting/plot_experiment.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/test/master_index.py` & `enbios2-0.0.2/enbios2/test/master_index.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2/test/test_dot2bw.py` & `enbios2-0.0.2/enbios2/test/test_dot2bw.py`

 * *Files identical despite different names*

### Comparing `enbios2-0.0.1/enbios2.egg-info/PKG-INFO` & `enbios2-0.0.2/enbios2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: enbios2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Enbios 2
 Author: Ramin Soleymani
 License: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
-# enbios2
+# Enbios 2
 
 This a ground up new implementation of enbios.
 
 Compared to the original version of enbios, this version is more flexible does not make it's own LCA calculations, but
 uses brightway2 for that.
 
 The main functionality of enbios2 is currently to run experiments, which are described a set of (brightway) activities a
```

### Comparing `enbios2-0.0.1/enbios2.egg-info/SOURCES.txt` & `enbios2-0.0.2/enbios2.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -32,18 +32,14 @@
 enbios2/dev/__init__.py
 enbios2/dev/create_experiment_schema.py
 enbios2/dev/pull_docs.py
 enbios2/ecoinvent/__init__.py
 enbios2/ecoinvent/ecoinvent_index.py
 enbios2/ecoinvent/ecoinvent_resolved_dataset_db.py
 enbios2/ecoinvent/spatial.py
-enbios2/enbios_extend/__init__.py
-enbios2/enbios_extend/bw_lci2nis.py
-enbios2/enbios_extend/nis/_1_lci_to_nis.py
-enbios2/enbios_extend/nis/__init__.py
 enbios2/experiment/__init__.py
 enbios2/experiment/activity_search.py
 enbios2/experiment/ai_lcia.py
 enbios2/experiment/bw2sigma.py
 enbios2/experiment/bw_manipulation.py
 enbios2/experiment/characterizations.py
 enbios2/experiment/class_static_me.py
```

