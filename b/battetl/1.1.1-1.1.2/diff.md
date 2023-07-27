# Comparing `tmp/battetl-1.1.1.tar.gz` & `tmp/battetl-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.1.1.tar", last modified: Tue Jul 11 22:26:33 2023, max compression
+gzip compressed data, was "battetl-1.1.2.tar", last modified: Thu Jul 27 01:59:39 2023, max compression
```

## Comparing `battetl-1.1.1.tar` & `battetl-1.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.686521 battetl-1.1.1/
--rw-r--r--   0 Benjamin   (502) staff       (20)     1066 2023-07-10 18:08:18.000000 battetl-1.1.1/LICENSE
--rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 22:26:33.685912 battetl-1.1.1/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)    15958 2023-07-11 18:30:14.000000 battetl-1.1.1/README.md
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.674062 battetl-1.1.1/battetl/
--rw-r--r--   0 Benjamin   (502) staff       (20)     7528 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/BattETL.py
--rw-r--r--   0 Benjamin   (502) staff       (20)      155 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     6971 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/battetl_quick.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     9627 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/constants.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.678755 battetl-1.1.1/battetl/extract/
--rw-r--r--   0 Benjamin   (502) staff       (20)    26584 2023-07-11 22:24:08.000000 battetl-1.1.1/battetl/extract/Extractor.py
--rw-r--r--   0 Benjamin   (502) staff       (20)       33 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/extract/__init__.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.683109 battetl-1.1.1/battetl/load/
--rw-r--r--   0 Benjamin   (502) staff       (20)    39804 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/Loader.py
--rw-r--r--   0 Benjamin   (502) staff       (20)      115 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     7341 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/batt_db_test_helper.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     3201 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/load/quick_loader.py
--rw-r--r--   0 Benjamin   (502) staff       (20)     1677 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/logger.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.685073 battetl-1.1.1/battetl/transform/
--rw-r--r--   0 Benjamin   (502) staff       (20)    29382 2023-07-11 22:24:08.000000 battetl-1.1.1/battetl/transform/Transformer.py
--rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-07-10 18:08:18.000000 battetl-1.1.1/battetl/transform/__init__.py
--rw-r--r--   0 Benjamin   (502) staff       (20)    13584 2023-07-11 18:30:14.000000 battetl-1.1.1/battetl/utils.py
-drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 22:26:33.676650 battetl-1.1.1/battetl.egg-info/
--rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/PKG-INFO
--rw-r--r--   0 Benjamin   (502) staff       (20)      533 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/SOURCES.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/dependency_links.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)      171 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/requires.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)        8 2023-07-11 22:26:33.000000 battetl-1.1.1/battetl.egg-info/top_level.txt
--rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-07-11 22:26:33.686728 battetl-1.1.1/setup.cfg
--rw-r--r--   0 Benjamin   (502) staff       (20)      886 2023-07-11 22:24:08.000000 battetl-1.1.1/setup.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.970594 battetl-1.1.2/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     6350 2023-07-27 01:56:07.000000 battetl-1.1.2/LICENSE
+-rw-r--r--   0 Benjamin   (502) staff       (20)    18801 2023-07-27 01:59:39.970069 battetl-1.1.2/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)    18250 2023-07-27 01:56:07.000000 battetl-1.1.2/README.md
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.961476 battetl-1.1.2/battetl/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7528 2023-07-10 18:08:18.000000 battetl-1.1.2/battetl/BattETL.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      155 2023-07-11 22:48:05.000000 battetl-1.1.2/battetl/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7449 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/battetl_quick.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     9882 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/constants.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.964939 battetl-1.1.2/battetl/extract/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    29524 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/extract/Extractor.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       33 2023-07-10 18:08:18.000000 battetl-1.1.2/battetl/extract/__init__.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.967888 battetl-1.1.2/battetl/load/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    39804 2023-07-11 22:48:05.000000 battetl-1.1.2/battetl/load/Loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      115 2023-07-11 22:48:05.000000 battetl-1.1.2/battetl/load/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7341 2023-07-10 18:08:18.000000 battetl-1.1.2/battetl/load/batt_db_test_helper.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     3262 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/load/quick_loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     1677 2023-07-10 18:08:18.000000 battetl-1.1.2/battetl/logger.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.969053 battetl-1.1.2/battetl/transform/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    31961 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/transform/Transformer.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-07-10 18:08:18.000000 battetl-1.1.2/battetl/transform/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)    14558 2023-07-27 01:56:07.000000 battetl-1.1.2/battetl/utils.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-27 01:59:39.963688 battetl-1.1.2/battetl.egg-info/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    18801 2023-07-27 01:59:39.000000 battetl-1.1.2/battetl.egg-info/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)      533 2023-07-27 01:59:39.000000 battetl-1.1.2/battetl.egg-info/SOURCES.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-07-27 01:59:39.000000 battetl-1.1.2/battetl.egg-info/dependency_links.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)      171 2023-07-27 01:59:39.000000 battetl-1.1.2/battetl.egg-info/requires.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        8 2023-07-27 01:59:39.000000 battetl-1.1.2/battetl.egg-info/top_level.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-07-27 01:59:39.970706 battetl-1.1.2/setup.cfg
+-rw-r--r--   0 Benjamin   (502) staff       (20)      886 2023-07-27 01:56:07.000000 battetl-1.1.2/setup.py
```

### Comparing `battetl-1.1.1/PKG-INFO` & `battetl-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
 
 # BattETL
 
@@ -26,20 +26,21 @@
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
   - [Quick Mode](#quick-mode)
+    - [Unstructured data](#unstructured-data)
   - [Config File](#config-file)
   - [Env File](#env-file)
   - [Data Export Requirements](#data-export-requirements)
     - [Maccor](#maccor)
     - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
+- [BattETL Process Overview](#battetl-process-overview)
   - [System Diagram](#system-diagram)
   - [Transformer](#transformer)
   - [Extractor](#extractor)
   - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
@@ -136,14 +137,78 @@
 
 ```bash
 python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
 ```
 
 This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
 
+#### Unstructured data
+
+Quick mode also supports importing battery test data not generated by an Arbin or Maccor cycler, henceforth referred to as "unstructured data". When handling unstructured data it is necessary to include a third command line argument, `file_meta.json` that will be used to define how the data should be imported and to rename column to conform to names expected by the database. An example file_meta is given below:
+
+```JSON
+{
+    "pandas_read_csv_args" : {
+        "delimiter":",",
+        "index_col": false
+    }, 
+    "voltage_mv" : 
+    {
+        "column_name":"volt",
+        "scaling_factor":1
+    },
+    "current_ma" : 
+    {
+        "column_name":"curr",
+        "scaling_factor":1
+    },
+    "test_time_s" :
+    {
+        "column_name":"time",
+        "scaling_factor":1
+    },
+    "cycle" :
+    {
+        "column_name":"cycl"
+    }
+}
+```
+
+The `pandas_read_csv_args` object holds any function arguments that should be passed to [`pandas.read_csv()`](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html) to correctly import the data as a pandas dataframe.
+
+All the the other objects have the following format:
+
+```JSON
+{
+    "new_column_name" : 
+    {
+        "column_name" : "existing_column_name",
+        "scaling_factor": 1
+    }
+}
+```
+
+Where:
+
+- `new_column_name` is the new name of the column that should be set in the dataframe, e.g. `voltage_mv`
+- `existing_column_name` is the existing column name that should be changed to the `new_column_name`
+- `scaling_factor` *optional* provides an optional multiplicative scaling to use to scale the column value ot the desired units. 
+
+A few notes:
+
+- Column decoders must be included for `voltage_mv`, `current_ma`, and `test_time_s` or `recorded_datetime` so as to match the database schema. 
+- Any column can be transformed, even it is to a name that does not exist in the database schema.
+- Any column name does that does not exist in the `test_data` table will be loaded in the `other_details` column
+
+So, the command to run unstructured data would like the following:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" file_meta="file_meta.json" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
 ### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
```

### Comparing `battetl-1.1.1/README.md` & `battetl-1.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
   - [Quick Mode](#quick-mode)
+    - [Unstructured data](#unstructured-data)
   - [Config File](#config-file)
   - [Env File](#env-file)
   - [Data Export Requirements](#data-export-requirements)
     - [Maccor](#maccor)
     - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
+- [BattETL Process Overview](#battetl-process-overview)
   - [System Diagram](#system-diagram)
   - [Transformer](#transformer)
   - [Extractor](#extractor)
   - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
@@ -121,14 +122,78 @@
 
 ```bash
 python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
 ```
 
 This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
 
+#### Unstructured data
+
+Quick mode also supports importing battery test data not generated by an Arbin or Maccor cycler, henceforth referred to as "unstructured data". When handling unstructured data it is necessary to include a third command line argument, `file_meta.json` that will be used to define how the data should be imported and to rename column to conform to names expected by the database. An example file_meta is given below:
+
+```JSON
+{
+    "pandas_read_csv_args" : {
+        "delimiter":",",
+        "index_col": false
+    }, 
+    "voltage_mv" : 
+    {
+        "column_name":"volt",
+        "scaling_factor":1
+    },
+    "current_ma" : 
+    {
+        "column_name":"curr",
+        "scaling_factor":1
+    },
+    "test_time_s" :
+    {
+        "column_name":"time",
+        "scaling_factor":1
+    },
+    "cycle" :
+    {
+        "column_name":"cycl"
+    }
+}
+```
+
+The `pandas_read_csv_args` object holds any function arguments that should be passed to [`pandas.read_csv()`](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html) to correctly import the data as a pandas dataframe.
+
+All the the other objects have the following format:
+
+```JSON
+{
+    "new_column_name" : 
+    {
+        "column_name" : "existing_column_name",
+        "scaling_factor": 1
+    }
+}
+```
+
+Where:
+
+- `new_column_name` is the new name of the column that should be set in the dataframe, e.g. `voltage_mv`
+- `existing_column_name` is the existing column name that should be changed to the `new_column_name`
+- `scaling_factor` *optional* provides an optional multiplicative scaling to use to scale the column value ot the desired units. 
+
+A few notes:
+
+- Column decoders must be included for `voltage_mv`, `current_ma`, and `test_time_s` or `recorded_datetime` so as to match the database schema. 
+- Any column can be transformed, even it is to a name that does not exist in the database schema.
+- Any column name does that does not exist in the `test_data` table will be loaded in the `other_details` column
+
+So, the command to run unstructured data would like the following:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" file_meta="file_meta.json" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
 ### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
```

### Comparing `battetl-1.1.1/battetl/BattETL.py` & `battetl-1.1.2/battetl/BattETL.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.1/battetl/battetl_quick.py` & `battetl-1.1.2/battetl/battetl_quick.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 import os
 import re
 import sys
+import json
 import subprocess
 import pandas as pd
 
 from battetl import logger
 from battetl.extract import Extractor
 from battetl.transform import Transformer
 from battetl.load import QuickLoader
 
 
-def battetl_quick(file_name: str) -> pd.DataFrame:
+def battetl_quick(file_path: str, file_meta = None) -> pd.DataFrame:
     '''
     The BattETL Quick Mode. Extracts test data or cycle stats from a file, transforms it,
     and loads it to the database.
 
     Parameters
     ----------
-    file_name : str
+    file_path : str
         Name of the file to be processed.
+    file_meta : dict
+        A dictionary used to decode unstructured data.
 
     Returns
     -------
     pd.DataFrame
         The test data or cycle stats that was loaded to the database.
     '''
 
     extractor = Extractor()
     try:
-        extractor.data_from_files([file_name])
+        extractor.data_from_files([file_path], file_meta)
         raw_test_data = extractor.raw_test_data
         raw_cycle_stats = extractor.raw_cycle_stats
     except Exception as e:
         logger.error('Failed to extract test data', exc_info=True)
 
     transformer = Transformer()
     test_data = pd.DataFrame()
     cycle_stats = pd.DataFrame()
     if not raw_test_data.empty:
         try:
-            transformer.transform_test_data(raw_test_data)
+            transformer.transform_test_data(raw_test_data, file_meta)
             test_data = transformer.test_data
         except Exception as e:
             logger.error('Failed to transform test data', exc_info=True)
     elif not raw_cycle_stats.empty:
         try:
             transformer.transform_cycle_stats(raw_cycle_stats)
             cycle_stats = transformer.cycle_stats
         except Exception as e:
             logger.error('Failed to transform cycle stats', exc_info=True)
 
-    loader = QuickLoader(file_name)
+    loader = QuickLoader(file_path)
     if not test_data.empty:
         try:
             loader.load_test_data(test_data)
             logger.info(
-                f'**** Data successfully loaded to test_data table under test_name {file_name} ****')
+                f'**** Data successfully loaded to test_data table under test_name {file_path} ****')
         except Exception as e:
             logger.error('Failed to load test data', exc_info=True)
     elif not cycle_stats.empty:
         try:
             loader.load_cycle_stats(cycle_stats)
             logger.info(
-                f'**** Data successfully loaded to test_data_cycle_stats table under test_name {file_name} ****')
+                f'**** Data successfully loaded to test_data_cycle_stats table under test_name {file_path} ****')
         except Exception as e:
             logger.error('Failed to load cycle stats', exc_info=True)
 
     if not test_data.empty:
         return test_data
     elif not cycle_stats.empty:
         return cycle_stats
@@ -175,30 +178,40 @@
 
 if __name__ == '__main__':
     n = len(sys.argv)
     print("num arguments" + str(n))
     if n < 3:
         print("Not enough arguments passed! Exiting!")
         sys.exit()
-    elif n > 3:
+    elif n > 4:
         print("Too many arguments passed! Exiting!")
         sys.exit()
     else:
         for i in range(1, n):
             arg = str(sys.argv[i])
             if arg.startswith('file='):
-                file_name = re.split('file=', arg)[-1]
+                file_path = re.split('file=', arg)[-1]
             elif arg.startswith('db_url='):
                 db_url = re.split('db_url=', arg)[-1]
+            elif arg.startswith('file_meta='):
+                file_meta_path = re.split('file_meta=', arg)[-1]
             else:
                 print("Unknown argument " + arg + "! Exiting!")
                 sys.exit()
 
-    if not os.path.isfile(file_name):
-        print("File path " + file_name + " does not exist! Exiting!")
+    if not os.path.isfile(file_path):
+        print("File path " + file_path + " does not exist! Exiting!")
+        sys.exit()
+
+    file_meta = None
+    if os.path.isfile(file_meta_path):
+        with open(file_meta_path) as file:
+            file_meta = json.load(file)
+    else:
+        print("Invalid path for file_meta! Exiting!")
         sys.exit()
 
     # Assumes a db_url format of:
     # "postgres://YourUserName:YourPassword@YourHostname:Port/YourDatabaseName"
     split_list = re.split('//', db_url)[-1].split(':')
     username = split_list[0]
     password, hostname = split_list[1].split("@")
@@ -229,8 +242,8 @@
         sys.exit()
 
     clone_battdb(battdb_folder)
     docker_result = run_docker_compose(battdb_folder)
     logger.info(docker_result.stdout)
     logger.info(docker_result.stderr)
 
-    battetl_quick(file_name)
+    battetl_quick(file_path, file_meta)
```

### Comparing `battetl-1.1.1/battetl/constants.py` & `battetl-1.1.2/battetl/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,7 +281,19 @@
         'T1_Max': 'maccor_charge_thermocouple_max_c',
         'T1_Start.1': 'maccor_discharge_thermocouple_start_c',
         'T1_End.1': 'maccor_discharge_thermocouple_end_c',
         'T1_Min.1': 'maccor_discharge_thermocouple_min_c',
         'T1_Max.1': 'maccor_discharge_thermocouple_max_c',
         'ACR': 'acr_ohm',
     }
+ 
+    COLUMNS_UNSTRUCTURED_TEST_DATA = {
+        'voltage_mv',
+        'current_ma',
+        'time_s',
+        'other_details',
+    }
+    UNSTRUCTURED_DATA_REQUIRED_KEYS = {
+        'voltage_mv',
+        'current_ma',
+        'pandas_read_csv_args'
+    }
```

### Comparing `battetl-1.1.1/battetl/extract/Extractor.py` & `battetl-1.1.2/battetl/extract/Extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,31 +23,42 @@
 
         self.schedule = {
             'schedule': DashOrderedDict(),
             'file_name': '',
             'steps': {'chg': [], 'dsg': [], 'rst': []}
         }
 
-    def data_from_files(self, paths: list[str]):
+    def data_from_files(self, paths: list[str], file_meta: dict = None) -> pd.DataFrame:
         """
         Extracts multiple test data files into a single pandas DataFrame.
         If only a single data file exists then it only extracts that data.
 
         Parameters
         ----------
         paths : list[str]
             Relative or absolute paths to the target data files.
+        file_meta : dict, optional
+            Dictionary containing the user defined column names for the test data. The default is None.
+        Returns
+        -------
+        pd.DataFrame
+            A pandas DataFrame containing the test data.
         """
         if type(paths) != list:
             raise TypeError('Input paths is not list')
 
         logger.info(f'Total {len(paths)} files')
 
         for path in paths:
-            self.__data_from_file(path)
+            if file_meta:
+                self.__unstructured_data_from_file(
+                    path=path,
+                    file_meta=file_meta)
+            else:
+                self.__data_from_file(path=path)
 
         logger.info('Extract success')
 
     def schedule_from_files(self, paths: list[str]) -> dict:
         """
         Reads Arbin schedules and associated files or Maccor procedures and associated 
         files from the passed paths list and saves them together in a nested dictionary.
@@ -76,14 +87,83 @@
                 break
             elif i == (len(paths)-1):
                 logger.error(
                     'Unable to identify schedule type from paths: ' + str(paths))
 
         return self.schedule
 
+    def schedule_from_files(self, paths: list[str]) -> dict:
+        """
+        Reads Arbin schedules and associated files or Maccor procedures and associated 
+        files from the passed paths list and saves them together in a nested dictionary.
+
+        Parameters
+        ----------
+        paths : list[str]
+            Relative or absolute paths to the Maccor schedule and associated files
+        """
+        if type(paths) != list:
+            raise TypeError('Input paths is not list')
+
+        logger.info(f'Total {len(paths)} files')
+
+        for i, path in enumerate(paths):
+            if path.endswith('.000'):
+                logger.info("Processing procedure files for Maccor")
+                self.schedule['schedule'] = self.__maccor_procedure_from_files(
+                    paths)
+                break
+            elif path.endswith('.sdu') or path.endswith('.sdx'):
+                logger.info("Processing schedule files for Arbin")
+                self.schedule['schedule'] = self.__arbin_schedule_from_files(
+                    paths)
+
+                break
+            elif i == (len(paths)-1):
+                logger.error(
+                    'Unable to identify schedule type from paths: ' + str(paths))
+
+        return self.schedule
+
+    def __unstructured_data_from_file(self, path: str, file_meta: dict) -> pd.DataFrame:
+        """
+        Reads unstructured data from the passed file path and returns it as a pandas DataFrame.
+        Parameters
+        ----------
+        path : str
+            Relative or absolute path to the datafile.
+        file_meta : dict
+            Dictionary containing the meta data for the file.
+        Returns
+        -------
+        df : pandas.DataFrame
+            A pandas DataFrame containing the data file.
+        """
+        logger.info(f'Load file path: {path}')
+        logger.info(f'Unstructured data from file. File meta: {file_meta}')
+        if not os.path.exists(path):
+            raise FileNotFoundError(f'Unable to load file {path}')
+
+        # Check file_meta contains all required keys
+        Utils.validate_file_meta(file_meta)
+
+        df = pd.read_csv(path, **file_meta['pandas_read_csv_args'])
+
+        self.raw_test_data = pd.concat(
+            [
+                self.raw_test_data,
+                df
+            ],
+            ignore_index=True
+        )
+        logger.debug(
+            f'Update raw_test_data. Total rows: {self.raw_test_data.shape[0]}')
+
+        return df
+
     def __maccor_procedure_from_files(self, paths: list[str]) -> DashOrderedDict:
         """
         Reads the Maccor procedure and associated files from the passed file path list.
         Returns all files a dictionaries in a single nested DashOrderedDict. Supported files to 
         include in paths list are Maccor procedures (.000) (required),  FastWave (*.MWF)  
         and frequency response analyzer (*.FRA) files.
```

### Comparing `battetl-1.1.1/battetl/load/Loader.py` & `battetl-1.1.2/battetl/load/Loader.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.1/battetl/load/batt_db_test_helper.py` & `battetl-1.1.2/battetl/load/batt_db_test_helper.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.1/battetl/load/quick_loader.py` & `battetl-1.1.2/battetl/load/quick_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import pandas as pd
 import json
+import os
+import copy
 from .Loader import Loader
 from battetl import logger
 
 
 class QuickLoader(Loader):
 
-    def __init__(self, file_name):
+    def __init__(self, file_path):
 
         # The config needed by the BattETL parent class
-        self._file_name = file_name
+        self._file_name = os.path.basename(file_path)
         config = {
             "meta_data": {
                 "test_meta": {
-                    "test_name": file_name,
+                    "test_name": copy.deepcopy(self._file_name),
                     "channel": "0"
                 },
                 "cell": {
                     "manufacturer_sn": "NA"
                 },
                 "cell_meta": {
                     "manufacturer": "NA",
```

### Comparing `battetl-1.1.1/battetl/logger.py` & `battetl-1.1.2/battetl/logger.py`

 * *Files identical despite different names*

### Comparing `battetl-1.1.1/battetl/transform/Transformer.py` & `battetl-1.1.2/battetl/transform/Transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,45 +37,47 @@
             logger.info('User defined transform_test_data function found')
         if self.user_transform_cycle_stats:
             logger.info('User defined transform_cycle_stats function found')
 
         self.test_data = pd.DataFrame(dtype=object)
         self.cycle_stats = pd.DataFrame(dtype=object)
 
-    def transform_test_data(self, data: pd.DataFrame) -> pd.DataFrame:
+    def transform_test_data(self, data: pd.DataFrame, file_meta: dict = None) -> pd.DataFrame:
         """
         Transforms test data to conform to BattETL naming and data conventions
 
         Parameters
         ----------
         data : pandas.DataFrame
             The input DataFrame
         schedule_steps : dict
             A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and 
             rest (key->'rst') steps from the schedule used to generate the data. Used to calculate
-            cycle level statistics (e.g. CV charge time.)
-
+            cycle level statistics (e.g. CV charge time.)s
+        file_meta : dict, optional
+            Dictionary containing the user defined column names for the test data. The default is None.
         Returns
         -------
         df : pandas.DataFrame
             The transformed output DataFrame
         """
         logger.info('Transform test data')
 
         df = data.copy()
         df = Utils.drop_unnamed_columns(df)
         df = Utils.drop_empty_rows(df)
 
         cycleMake, dataType = Utils.get_cycle_make(df.columns)
         logger.info(f'Cycle make: {cycleMake}. Data type: {dataType}')
 
-        if cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_TEST_DATA:
+        if file_meta:
+            df = self.__transform_unstructured_data(df, file_meta)
+        elif cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_TEST_DATA:
             df = self.__transform_arbin_test_data(df)
-
-        if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_TEST_DATA:
+        elif cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_TEST_DATA:
             df = self.__transform_maccor_test_data(df)
 
         df = self.__consolidate_temps(df)
 
         # Apply user defined transformation
         if self.user_transform_test_data:
             df = self.user_transform_test_data(df)
@@ -115,14 +117,64 @@
         # Apply user defined transformation
         if self.user_transform_cycle_stats:
             df = self.user_transform_cycle_stats(df)
 
         self.cycle_stats = df.astype(object)
         return df
 
+    def __transform_unstructured_data(self, df: pd.DataFrame, file_meta: dict) -> pd.DataFrame:
+        """
+        Transforms unstructured data with file_meta to conform to BattETL naming and data conventions
+        1. Rename columns
+        2. Concert units
+        4. Convert data type
+        5. Sort data
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+        file_meta : dict
+            Dictionary containing the meta data for the file.
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        logger.info('Transform unstructured data')
+
+        # Check user defined column names exist
+        if not file_meta.get('voltage_mv'):
+            raise ValueError(
+                f'Voltage column name does not exist: `voltage_mv`')
+        if not file_meta.get('current_ma'):
+            raise ValueError(
+                f'Current column name does not exist: `current_ma`')
+        if not file_meta.get('test_time_s') or file_meta.get('recorded_datetime'):
+            raise ValueError(
+                f'Required to have either `test_time_s` or `recorded_datetime` column!')
+
+        # Remove the `pandas_read_csv_args` dictionary if it is there
+        file_meta.pop("pandas_read_csv_args", None)
+
+        # Rename columns
+        columns_mappings = {}
+        for column in file_meta:
+            columns_mappings[file_meta[column]['column_name']] = column
+        df = Utils.rename_df_columns(df, columnsMapping=columns_mappings)
+
+        # Apply any transformations
+        for column in file_meta:
+            if file_meta.get(column).get('scaling_factor'):
+                df[column] = df[column] * \
+                    file_meta.get(column).get('scaling_factor')
+
+        df = self.__convert_data_type(df)
+
+        return df
+
     def __transform_arbin_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Transforms Arbin test data to conform to BattETL naming and data conventions
         1. Rename columns
         2. Convert to milli
         3. Convert datetime
         4. Convert data type
@@ -314,43 +366,47 @@
             A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and rest (key->'rst') steps.
 
         Returns
         -------
         df : pd.DataFrame
             A pandas DataFrame with harmonized capacity/energy values across cyclers.
         """
-
-        if 'maccor_capacity_mah' in df:
-            df['charge_capacity_mah'] = df[df.step.isin(
-                steps['chg'])].maccor_capacity_mah
-            df['discharge_capacity_mah'] = df[df.step.isin(
-                steps['dsg'])].maccor_capacity_mah
-        if 'maccor_energy_mwh' in df:
-            df['charge_energy_mwh'] = df[df.step.isin(
-                steps['chg'])].maccor_energy_mwh
-            df['discharge_energy_mwh'] = df[df.step.isin(
-                steps['dsg'])].maccor_energy_mwh
-            # log rows and columns that be modified
-            logger.debug(
-                f'Harmonized capacity/energy values for Maccor cyclers. Modified {len(df)} rows and 4 columns.')
-            logger.debug(
-                'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
-        elif 'arbin_charge_capacity_mah' in df:
+        
+        if 'arbin_charge_capacity_mah' in df:
             df['charge_capacity_mah'] = df[df.step.isin(
                 steps['chg'])].arbin_charge_capacity_mah
             df['charge_energy_mwh'] = df[df.step.isin(
                 steps['chg'])].arbin_charge_energy_mwh
             df['discharge_capacity_mah'] = df[df.step.isin(
                 steps['dsg'])].arbin_discharge_capacity_mah
             df['discharge_energy_mwh'] = df[df.step.isin(
                 steps['dsg'])].arbin_discharge_energy_mwh
             logger.debug(
                 f'Harmonized capacity/energy values for Arbin cyclers. Modified {len(df)} rows and 4 columns.')
             logger.debug(
                 'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
+        elif 'maccor_capacity_mah' in df:
+            df['charge_capacity_mah'] = df[df.step.isin(
+                steps['chg'])].maccor_capacity_mah
+            df['discharge_capacity_mah'] = df[df.step.isin(
+                steps['dsg'])].maccor_capacity_mah  
+            if 'maccor_energy_mwh' in df:
+                df['charge_energy_mwh'] = df[df.step.isin(
+                    steps['chg'])].maccor_energy_mwh
+                df['discharge_energy_mwh'] = df[df.step.isin(
+                    steps['dsg'])].maccor_energy_mwh
+                logger.debug(
+                    f'Harmonized capacity/energy values for Maccor cyclers. Modified {len(df)} rows and 4 columns.')
+                logger.debug(
+                    'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
+            else:
+                logger.debug(
+                    f'Harmonized capacity values for Maccor cyclers. Modified {len(df)} rows and 2 columns.')
+                logger.debug(
+                    'Added columns: charge_capacity_mah, discharge_capacity_mah')
         else:
             logger.warning("No capacity columns were found to refactor!")
 
         return df
 
     def calc_cycle_stats(self, steps: dict, cv_voltage_threshold_mv: float = None, cell_thermocouple: int = None) -> pd.DataFrame:
         """
@@ -609,18 +665,21 @@
             if step_slice.empty:
                 continue
 
             if ez_df.empty:
                 ez_df[time_col] = step_slice['test_time_s'] - \
                     step_slice['test_time_s'].iloc[0]
                 ez_df[volt_col] = step_slice['voltage_mv']
-                ez_df[eng_col] = step_slice[eng_col] - \
-                    step_slice[eng_col].iloc[0]
                 ez_df[cap_col] = step_slice[cap_col] - \
                     step_slice[cap_col].iloc[0]
+
+                if eng_col in step_slice.columns:
+                    ez_df[eng_col] = step_slice[eng_col] - \
+                        step_slice[eng_col].iloc[0]
+
                 if step_type == 'charge' and cv_voltage_thresh_mv is not None:
                     # if ez_df is empty, we're at beginning of a cycle and cap/step time should be reset to zero
                     # TODO: add documentation for this
                     delta_time = step_slice['step_time_s'] - \
                         step_slice['step_time_s'].shift(1, fill_value=0)
                     ez_df[cc_time] = np.where(
                         step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
@@ -639,28 +698,33 @@
                 # This catches if capacity was reset after each step. Modifies test_data DF in place.
                 if step_slice[cap_col].iloc[0] < ez_df[cap_col].iloc[-1]:
                     current_cycle = cycle_df.cycle.iloc[0]
                     self.test_data.loc[
                         (self.test_data.cycle == current_cycle) &
                         (self.test_data.step == step),
                         cap_col] += ez_df[cap_col]
-                    self.test_data.loc[
-                        (self.test_data.cycle == current_cycle) &
-                        (self.test_data.step == step),
-                        eng_col] += ez_df[eng_col]
                     step_slice[cap_col] += ez_df[cap_col].iloc[-1]
-                    step_slice[eng_col] += ez_df[eng_col].iloc[-1]
+
+                    if eng_col in self.test_data.columns:
+                        self.test_data.loc[
+                            (self.test_data.cycle == current_cycle) &
+                            (self.test_data.step == step),
+                            eng_col] += ez_df[eng_col]
+                        step_slice[eng_col] += ez_df[eng_col].iloc[-1]
+
                 if not ez_df.empty:
                     # keeps running time across steps. ignoring time between steps
                     step_df[time_col] = (
                         step_slice['test_time_s'] - step_slice['test_time_s'].iloc[0]) + ez_df[time_col].iloc[-1]
                 # step_slice is updated with above updates to test_data because it's a slice, not copy, of test_data
                 step_df[volt_col] = step_slice[volt_col]
                 step_df[cap_col] = step_slice[cap_col]
-                step_df[eng_col] = step_slice[eng_col]
+                if eng_col in step_slice.columns:
+                    step_df[eng_col] = step_slice[eng_col]
+
                 if step_type == 'charge' and cv_voltage_thresh_mv is not None:
                     # calculate the delta time/cap for each step, sum the deltas in calc_stats() to get cycle time/cap
                     delta_time = step_slice['step_time_s'] - \
                         step_slice['step_time_s'].shift(1, fill_value=0)
                     step_df[cc_time] = np.where(
                         step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
                     step_df[cv_time] = np.where(
@@ -692,8 +756,8 @@
         '''
         thermocouple_cols = [
             col for col in df.columns if re.search('thermocouple_\d+_c', col)]
 
         df['thermocouple_temps_c'] = df.apply(
             lambda row: [row[col] for col in thermocouple_cols], axis=1)
 
-        return df
+        return df
```

### Comparing `battetl-1.1.1/battetl/utils.py` & `battetl-1.1.2/battetl/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -407,14 +407,49 @@
         Returns
         -------
         float
         '''
         if isinstance(value, str):
             return float(value.replace(',', ''))
         return value
+    
+    def validate_file_meta(file_meta: dict) -> bool:
+        """
+        Validate file_meta
+        Parameters
+        ----------
+        file_meta : dict
+            Dictionary containing the meta data for the file.
+            For example:
+            ```json
+            {
+                "voltage_mv" : 
+                {
+                    "column_name":"volt",
+                    "scaling_factor":1,
+                },
+                "current_ma" : 
+                {
+                    "column_name":"curr",
+                    "scaling_factor":1,
+                },
+            }
+            ```
+        Returns
+        -------
+        bool
+            True if valid
+        """
+        # Check file_meta contains all required keys
+        for key in Constants.UNSTRUCTURED_DATA_REQUIRED_KEYS:
+            if key not in file_meta:
+                raise ValueError(
+                    f'file_meta does not contain required key: {key}')
+
+        return True
 
 
 class DashOrderedDict(OrderedDict):
     """
     Pulled from BEEP:
     https://github.com/TRI-AMDD/beep/blob/master/beep/utils/__init__.py
```

### Comparing `battetl-1.1.1/battetl.egg-info/PKG-INFO` & `battetl-1.1.2/battetl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: battetl
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python module for extracting, transforming, and loading battery data to a database.
 Home-page: https://github.com/BattGenie/battetl
 Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
 Author-email: info@battgenie.life
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.11
+Requires-Python: >=3.9, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
 
 # BattETL
 
@@ -26,20 +26,21 @@
 - [Motivation](#motivation)
 - [Video Guides](#video-guides)
 - [Installation](#installation)
   - [Requirements](#requirements)
   - [Installation Instructions](#installation-instructions)
 - [Usage](#usage)
   - [Quick Mode](#quick-mode)
+    - [Unstructured data](#unstructured-data)
   - [Config File](#config-file)
   - [Env File](#env-file)
   - [Data Export Requirements](#data-export-requirements)
     - [Maccor](#maccor)
     - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
+- [BattETL Process Overview](#battetl-process-overview)
   - [System Diagram](#system-diagram)
   - [Transformer](#transformer)
   - [Extractor](#extractor)
   - [Loader](#loader)
 - [Testing](#testing)
 - [Troubleshooting](#troubleshooting)
 
@@ -136,14 +137,78 @@
 
 ```bash
 python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
 ```
 
 This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
 
+#### Unstructured data
+
+Quick mode also supports importing battery test data not generated by an Arbin or Maccor cycler, henceforth referred to as "unstructured data". When handling unstructured data it is necessary to include a third command line argument, `file_meta.json` that will be used to define how the data should be imported and to rename column to conform to names expected by the database. An example file_meta is given below:
+
+```JSON
+{
+    "pandas_read_csv_args" : {
+        "delimiter":",",
+        "index_col": false
+    }, 
+    "voltage_mv" : 
+    {
+        "column_name":"volt",
+        "scaling_factor":1
+    },
+    "current_ma" : 
+    {
+        "column_name":"curr",
+        "scaling_factor":1
+    },
+    "test_time_s" :
+    {
+        "column_name":"time",
+        "scaling_factor":1
+    },
+    "cycle" :
+    {
+        "column_name":"cycl"
+    }
+}
+```
+
+The `pandas_read_csv_args` object holds any function arguments that should be passed to [`pandas.read_csv()`](https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html) to correctly import the data as a pandas dataframe.
+
+All the the other objects have the following format:
+
+```JSON
+{
+    "new_column_name" : 
+    {
+        "column_name" : "existing_column_name",
+        "scaling_factor": 1
+    }
+}
+```
+
+Where:
+
+- `new_column_name` is the new name of the column that should be set in the dataframe, e.g. `voltage_mv`
+- `existing_column_name` is the existing column name that should be changed to the `new_column_name`
+- `scaling_factor` *optional* provides an optional multiplicative scaling to use to scale the column value ot the desired units. 
+
+A few notes:
+
+- Column decoders must be included for `voltage_mv`, `current_ma`, and `test_time_s` or `recorded_datetime` so as to match the database schema. 
+- Any column can be transformed, even it is to a name that does not exist in the database schema.
+- Any column name does that does not exist in the `test_data` table will be loaded in the `other_details` column
+
+So, the command to run unstructured data would like the following:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" file_meta="file_meta.json" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
 ### Config File
 
 To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
 
 ```json
 {
     "timezone": "America/Los_Angeles",
```

### Comparing `battetl-1.1.1/battetl.egg-info/SOURCES.txt` & `battetl-1.1.2/battetl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `battetl-1.1.1/setup.py` & `battetl-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="battetl",
-    version="1.1.1",
+    version="1.1.2",
     author="Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak",
     author_email="info@battgenie.life",
     description="A Python module for extracting, transforming, and loading battery data to a database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BattGenie/battetl",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9, <3.11',
+    python_requires='>=3.9, <3.12',
     license='MIT',
 )
```

