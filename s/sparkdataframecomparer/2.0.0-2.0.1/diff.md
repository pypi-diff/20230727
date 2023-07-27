# Comparing `tmp/sparkdataframecomparer-2.0.0.tar.gz` & `tmp/sparkdataframecomparer-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparkdataframecomparer-2.0.0.tar", last modified: Thu Jul 27 02:02:32 2023, max compression
+gzip compressed data, was "sparkdataframecomparer-2.0.1.tar", last modified: Thu Jul 27 03:31:52 2023, max compression
```

## Comparing `sparkdataframecomparer-2.0.0.tar` & `sparkdataframecomparer-2.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 02:02:31.000000 sparkdataframecomparer-2.0.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/list_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparison_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/sparjk_data_frame_comparer_generic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:02:32.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 02:01:02.000000 sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail_with_func_path_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.652758 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16637 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/schema_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/schema_comparison_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/sparjk_data_frame_comparer_generic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/spark_data_frame_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/spark_data_frame_comparer/spark_data_frame_comparer_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.652758 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 03:31:52.000000 sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.652758 sparkdataframecomparer-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.652758 sparkdataframecomparer-2.0.1/tests/schema_comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.656758 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.656758 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18831 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_complex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/tests/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/tests/simple/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/tests/simple_fail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple_fail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:31:52.660758 sparkdataframecomparer-2.0.1/tests/simple_fail/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple_fail/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple_fail/test_simple_fail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-27 03:30:31.000000 sparkdataframecomparer-2.0.1/tests/simple_fail/test_simple_fail_with_func_path_modifier.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sparkdataframecomparer-2.0.0/LICENSE` & `sparkdataframecomparer-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/PKG-INFO` & `sparkdataframecomparer-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdataframecomparer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Deep Comparer for Spark Data Frames
 Home-page: https://github.com/imranq2/sparkdataframecomparer
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkdataframecomparer-2.0.0/README.md` & `sparkdataframecomparer-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/setup.py` & `sparkdataframecomparer-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/schema_comparer.py` & `sparkdataframecomparer-2.0.1/spark_data_frame_comparer/schema_comparer.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer.py` & `sparkdataframecomparer-2.0.1/spark_data_frame_comparer/spark_data_frame_comparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         if result_value is None and expected_value is None:
             return error_count, []
         if result_value is None or expected_value is None:
             return error_count + 1, [
                 f"Expected array in row:{row_num}, col:{column_num} to be {expected_value} "
                 f"but actual is {result_value}"
             ]
-        array_item: Row
+
         for array_item_index in range(0, len(result_value)):
             element_type: DataType = data_type_for_column.elementType
             result_array_item = result_value[array_item_index]
             if len(expected_value) < array_item_index + 1:
                 return error_count + 1, [
                     f"Expected row:{row_num}, col:{column_num} has only {len(expected_value)} "
                     f"items but Actual has > {array_item_index + 1}"
```

### Comparing `sparkdataframecomparer-2.0.0/spark_data_frame_comparer/spark_data_frame_comparer_exception.py` & `sparkdataframecomparer-2.0.1/spark_data_frame_comparer/spark_data_frame_comparer_exception.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/PKG-INFO` & `sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkdataframecomparer
-Version: 2.0.0
+Version: 2.0.1
 Summary: Deep Comparer for Spark Data Frames
 Home-page: https://github.com/imranq2/sparkdataframecomparer
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkdataframecomparer-2.0.0/sparkdataframecomparer.egg-info/SOURCES.txt` & `sparkdataframecomparer-2.0.1/sparkdataframecomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/conftest.py` & `sparkdataframecomparer-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_fail.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_array_to_array_allow_missing_nullable_properties_pass.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_simple.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/matches/test_schema_comparer_struct_to_struct_nullable_parent_recursive.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_array_to_array.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_complex.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_complex.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_simple.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py` & `sparkdataframecomparer-2.0.1/tests/schema_comparer/not_matches/test_schema_comparer_struct_to_struct.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/simple/test_simple.py` & `sparkdataframecomparer-2.0.1/tests/simple/test_simple.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail.py` & `sparkdataframecomparer-2.0.1/tests/simple_fail/test_simple_fail.py`

 * *Files identical despite different names*

### Comparing `sparkdataframecomparer-2.0.0/tests/simple_fail/test_simple_fail_with_func_path_modifier.py` & `sparkdataframecomparer-2.0.1/tests/simple_fail/test_simple_fail_with_func_path_modifier.py`

 * *Files identical despite different names*

