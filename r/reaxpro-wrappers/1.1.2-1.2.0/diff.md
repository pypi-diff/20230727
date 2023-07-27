# Comparing `tmp/reaxpro-wrappers-1.1.2.tar.gz` & `tmp/reaxpro-wrappers-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxpro-wrappers-1.1.2.tar", last modified: Wed Jul 26 12:52:24 2023, max compression
+gzip compressed data, was "reaxpro-wrappers-1.2.0.tar", last modified: Thu Jul 27 10:26:28 2023, max compression
```

## Comparing `reaxpro-wrappers-1.1.2.tar` & `reaxpro-wrappers-1.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/dictionaries/ams/
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/ams/energy_landscape.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/dictionaries/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/defaults/defaults_AMS.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/dictionaries/energies/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/energies/gas_energies.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/lattice_input.dat
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state1.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state2.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state3.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state4.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state5.xyz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/models/ams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/ams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/ams/energy_landscape_refinement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/models/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/settings/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.812551 reaxpro-wrappers-1.1.2/osp/models/zacros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/zacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49078 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/models/zacros/co_pyzacros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/osp/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/tools/graph_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/tools/io_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    77148 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/tools/mapping_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/tools/set_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/osp/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/osp/wrappers/simams/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/wrappers/simams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/wrappers/simams/simams_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/osp/wrappers/simzacros/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/wrappers/simzacros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/osp/wrappers/simzacros/simzacros_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 12:52:24.000000 reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:24.816552 reaxpro-wrappers-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/tests/test_energy_landscape_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/tests/test_pyzacros_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-26 12:52:06.000000 reaxpro-wrappers-1.1.2/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/ams/energy_landscape.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/defaults_AMS.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/energies/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/energies/gas_energies.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/lattice_input.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state1.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state2.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state3.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state4.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state5.xyz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.395790 reaxpro-wrappers-1.2.0/osp/models/ams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/ams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/ams/energy_landscape_refinement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/settings/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/models/zacros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/zacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49183 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/models/zacros/co_pyzacros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/graph_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27318 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/io_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77122 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/mapping_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/tools/set_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/simams/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simams/simams_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/simzacros_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-27 10:26:28.000000 reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-27 10:26:28.403791 reaxpro-wrappers-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 10:26:28.399791 reaxpro-wrappers-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_energy_landscape_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_pyzacros_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-27 10:26:11.000000 reaxpro-wrappers-1.2.0/tests/test_tools.py
```

### Comparing `reaxpro-wrappers-1.1.2/LICENSE` & `reaxpro-wrappers-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/PKG-INFO` & `reaxpro-wrappers-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.1.2
+Version: 1.2.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.1.2/README.md` & `reaxpro-wrappers-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json` & `reaxpro-wrappers-1.2.0/osp/dictionaries/ams/Ziff-Gulari-Barshad-model-variants.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/ams/energy_landscape.json` & `reaxpro-wrappers-1.2.0/osp/dictionaries/ams/energy_landscape.json`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/defaults/defaults_AMS.yaml` & `reaxpro-wrappers-1.2.0/osp/dictionaries/defaults/defaults_AMS.yaml`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/lattice_input.dat` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/lattice_input.dat`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state1.xyz` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state1.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state2.xyz` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state2.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state3.xyz` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state3.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state4.xyz` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state4.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/dictionaries/example_data/state5.xyz` & `reaxpro-wrappers-1.2.0/osp/dictionaries/example_data/state5.xyz`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/models/ams/energy_landscape_refinement.py` & `reaxpro-wrappers-1.2.0/osp/models/ams/energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/models/settings/general.py` & `reaxpro-wrappers-1.2.0/osp/models/settings/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/models/utils/general.py` & `reaxpro-wrappers-1.2.0/osp/models/utils/general.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/models/zacros/co_pyzacros.py` & `reaxpro-wrappers-1.2.0/osp/models/zacros/co_pyzacros.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from pathlib import Path
 import tempfile
 from typing import TYPE_CHECKING, List, Union, Optional
 from uuid import UUID
 import warnings
 
-from arcp import arcp_random
+from arcp import arcp_random, arcp_name
 from pydantic import AnyUrl, BaseModel, Field, root_validator, confloat, conlist, conint
 from pydantic.dataclasses import dataclass
 from urllib.parse import quote, urlencode
 
 
 from osp.core.cuds import Cuds
 from osp.core.namespaces import emmo, crystallography
@@ -561,15 +561,15 @@
 
     def __post_init_post_parse__(self):
         with CoreSession() as session:
 
             calculation = emmo.MesoscopicCalculation()
             calculation.add(*self._make_model(), rel=emmo.hasInput)
 
-        file = tempfile.NamedTemporaryFile(suffix=".ttl")
+        file = tempfile.NamedTemporaryFile(suffix=".ttl", delete=False)
         export_cuds(session, file.name)
         self._file = file.name
         try:
             self._uuid = get_upload(file)
         except Exception as error:
             self._uuid = None
             message = message = f"The graph of the model could not be stored at the minio-instance: {error.args}"
@@ -834,24 +834,25 @@
         step_float = emmo.Real(hasNumericalData=self.simulation_input.wall_time, iri=iri)
         cuds_object.add(step_float, rel=emmo.hasPart)
 
         return cuds_object
 
     def _make_lattice(self) -> Cuds:
         """Creates CUDS graph for the lattice input"""
-        xyz_file = str(self.lattice_input.xyz_file)
+        xyz_file = self.lattice_input.xyz_file
         if isinstance(xyz_file, UUID):
-            xyz_file = get_download(xyz_file, as_file=True)
+            return crystallography.UnitCell(uid=xyz_file)
         elif isinstance(xyz_file, AnyUrl):
-            xyz_file = _download_file(xyz_file, as_file=True)
-
-        iri = self._make_arcp("lattice_input", query=dict(jsonpath=[[xyz_file]]))
-        cuds_object = crystallography.UnitCell(iri=iri)
-
-        return cuds_object
+            return crystallography.UnitCell(iri=str(xyz_file))
+        elif isinstance(xyz_file, Path):
+            if not "file:" in str(xyz_file):
+                iri = f"file://{xyz_file.as_posix()}"
+            else:
+                iri = xyz_file.as_posix()
+            return crystallography.UnitCell(iri=iri)
 
     def _make_energetics(self) -> "List[Cuds]":
         """Creates CUDS graph for the energy cluster input"""
 
         cuds_list = []
 
         for cluster in self.energetics_input:
```

### Comparing `reaxpro-wrappers-1.1.2/osp/tools/graph_functions.py` & `reaxpro-wrappers-1.2.0/osp/tools/graph_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/tools/io_functions.py` & `reaxpro-wrappers-1.2.0/osp/tools/io_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/tools/mapping_functions.py` & `reaxpro-wrappers-1.2.0/osp/tools/mapping_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1660,15 +1660,15 @@
                     search.find_relationships(find_rel=emmo.INVERSE_OF_hasTemporalLast,
                                               root=search_simulation[0],
                                               consider_rel=emmo.hasTemporalLast)
                 add_AMSenergy_to_object(engine.children[2], last_calculation[0])
 
             tarball = map_tarball(engine, last_calculation[0])
 
-    elif isinstance(engine, pz.ZacrosResults):
+    elif isinstance(engine, pz.ZacrosJob):
         search_calculation = search.find_cuds_objects_by_oclass(
                                    emmo.MesoscopicCalculation, root_cuds_object,
                                    rel=cuba.relationship)
         tarball = map_tarball(engine, search_calculation[0])
 
     else:
         raise_error(file=os.path.basename(__file__), function=map_results.__name__,
@@ -1806,18 +1806,16 @@
     :engine: Job PLAMS /Multijob PLAMS object for AMS calculations, str: for Zacros calculation
 
     :param root_cuds_object: CUDS Calculation to add results to.
 
     :return str: file system path to tarball
    """
 
-    path = "plams_workdir/"
-
     tar = tempfile.NamedTemporaryFile().name
-    shutil.make_archive(tar, "tar", path)
+    shutil.make_archive(tar, "tar", engine.path)
     tar_file = f"{tar}.tar"
 
     print(f"Job output dumped to {tar_file}")
 
     iri = arcp_random(tar_file)
     string = emmo.String(iri=iri)
     root_cuds_object.add(string, rel=emmo.hasOutput)
```

### Comparing `reaxpro-wrappers-1.1.2/osp/tools/set_functions.py` & `reaxpro-wrappers-1.2.0/osp/tools/set_functions.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/wrappers/simams/simams_session.py` & `reaxpro-wrappers-1.2.0/osp/wrappers/simams/simams_session.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/osp/wrappers/simzacros/simzacros_session.py` & `reaxpro-wrappers-1.2.0/osp/wrappers/simzacros/simzacros_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Describe Zacros Session class."""
 from osp.core.namespaces import emmo, crystallography, cuba
 from osp.core.session import SimWrapperSession
 from osp.core.cuds import Cuds
 from osp.tools.io_functions import raise_error
 from osp.tools.mapping_functions import map_function, map_results
 from osp.core.utils import simple_search as search
+from osp.models.utils.general import get_download
 import scm.pyzacros as pz
 import os
 # from osp.core.utils import pretty_print
 
 
 class SimzacrosSession(SimWrapperSession):
     """Describe Zacros Session class."""
@@ -33,15 +34,15 @@
         """
 
         (pz_settings, pz_lattice, pz_mechanism, pz_cluster_expansion) = \
             map_function(self, root_cuds_object, self.engine)
         pz_job = pz.ZacrosJob(settings=pz_settings, lattice=pz_lattice,
                               mechanism=pz_mechanism, cluster_expansion=pz_cluster_expansion)
         results = pz_job.run()
-        self._tarball = map_results(results, root_cuds_object)
+        self._tarball = map_results(pz_job, root_cuds_object)
 
         # Attributes to easily access (syntactic) info from results.
         self.get_reaction_network = results.get_reaction_network()
         self.provided_quantities_names = results.provided_quantities_names()
         self.provided_quantities = results.provided_quantities()
         self.number_of_lattice_sites = results.number_of_lattice_sites()
         self.gas_species_names = results.gas_species_names()
@@ -107,21 +108,23 @@
         if len(search_calculation) > 1:
             raise_error(file=os.path.basename(__file__),
                         function="_apply_added method",
                         type='NameError',
                         message='More than one crystallography.UnitCell defined'
                         ' in the Wrapper object.')
         if search_lattice:
-            if "jsonpath" in search_lattice[0].iri:
-                # lattice loaded from json dict:
-                self.lattice = "./" + \
-                    str(search_lattice[0].iri).replace("%2F", "/").split("jsonpath=")[1]
+            lattice = search_lattice.pop()
+            if "file://" in str(lattice.iri):
+                split = str(lattice.iri).split("file://")
+                self.lattice = split[-1]
             else:
-                # lattice loaded from semantic-based script:
-                self.lattice = search_lattice[0].iri[49:]
+                self.lattice = get_download(str(lattice.uid), as_file=True)
+        else:
+            # lattice loaded from semantic-based script:
+            self.lattice = search_lattice[0].iri[49:]
 
         # Cluster
         search_cluster = \
             search.find_cuds_objects_by_oclass(emmo.ClusterExpansion,
                                                self.calculation, emmo.hasInput)
         if search_cluster:
             self.cluster = search_cluster
```

### Comparing `reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/PKG-INFO` & `reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reaxpro-wrappers
-Version: 1.1.2
+Version: 1.2.0
 Summary: The wrapper of AMS and Zacros drivers for SimPhoNy
 Home-page: https://www.esciencecenter.nl/
 Author: Netherlands eScience Center, Fraunhofer IWM
 Keywords: simphony,cuds,AMS,zacros,SCM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `reaxpro-wrappers-1.1.2/reaxpro_wrappers.egg-info/SOURCES.txt` & `reaxpro-wrappers-1.2.0/reaxpro_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/setup.cfg` & `reaxpro-wrappers-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = reaxpro-wrappers
 author = Netherlands eScience Center, Fraunhofer IWM
 url = https://www.esciencecenter.nl/
-version = v1.1.2
+version = v1.2.0
 description = The wrapper of AMS and Zacros drivers for SimPhoNy
 keywords = simphony, cuds, AMS, zacros, SCM
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `reaxpro-wrappers-1.1.2/setup.py` & `reaxpro-wrappers-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/tests/test_energy_landscape_refinement.py` & `reaxpro-wrappers-1.2.0/tests/test_energy_landscape_refinement.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/tests/test_examples.py` & `reaxpro-wrappers-1.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/tests/test_pyzacros_model.py` & `reaxpro-wrappers-1.2.0/tests/test_pyzacros_model.py`

 * *Files identical despite different names*

### Comparing `reaxpro-wrappers-1.1.2/tests/test_tools.py` & `reaxpro-wrappers-1.2.0/tests/test_tools.py`

 * *Files identical despite different names*

