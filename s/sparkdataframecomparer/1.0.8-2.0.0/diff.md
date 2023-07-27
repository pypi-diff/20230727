# Comparing `tmp/sparkdataframecomparer-1.0.8.tar.gz` & `tmp/sparkdataframecomparer-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparkdataframecomparer-1.0.8.tar", last modified: Tue Jan  3 00:11:32 2023, max compression
+gzip compressed data, was "dist/sparkdataframecomparer-2.0.0.tar", last modified: Thu Jul 27 02:02:32 2023, max compression
```

## Comparing `sparkdataframecomparer-1.0.8.tar` & `sparkdataframecomparer-2.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/schema_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/schema_comparison_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/sparjk_data_frame_comparer_generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/spark_data_frame_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/spark_data_frame_comparer/spark_data_frame_comparer_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/simple/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-03 00:11:32.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/test_simple_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-01-03 00:10:08.000000 sparkdataframecomparer-1.0.8/tests/simple_fail/test_simple_fail_with_func_path_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 02:02:31.000000 sparkdataframecomparer-2.0.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparison_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/sparjk_data_frame_comparer_generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail_with_func_path_modifier.py
```

### Comparing `sparkdataframecomparer-1.0.8/LICENSE` & `sparkdataframecomparer-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/PKG-INFO` & `sparkdataframecomparer-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdataframecomparer
-Version: 1.0.8
+Version: 2.0.0
 Summary: Deep Comparer for Spark Data Frames
 Home-page: https://github.com/imranq2/sparkdataframecomparer
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkdataframecomparer-1.0.8/README.md` & `sparkdataframecomparer-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/setup.py` & `sparkdataframecomparer-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/spark_data_frame_comparer/schema_comparer.py` & `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparer.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/spark_data_frame_comparer/spark_data_frame_comparer.py` & `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/spark_data_frame_comparer/spark_data_frame_comparer_exception.py` & `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer_exception.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/PKG-INFO` & `sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdataframecomparer
-Version: 1.0.8
+Version: 2.0.0
 Summary: Deep Comparer for Spark Data Frames
 Home-page: https://github.com/imranq2/sparkdataframecomparer
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkdataframecomparer-1.0.8/sparkdataframecomparer.egg-info/SOURCES.txt` & `sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/conftest.py` & `sparkdataframecomparer-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_simple.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_complex.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_complex.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_simple.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py` & `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/simple/test_simple.py` & `sparkdataframecomparer-2.0.0/tests/simple/test_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/simple_fail/test_simple_fail.py` & `sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-1.0.8/tests/simple_fail/test_simple_fail_with_func_path_modifier.py` & `sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail_with_func_path_modifier.py`

 * *Files identical despite different names*

