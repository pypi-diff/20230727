# Comparing `tmp/ricco-1.1.2.tar.gz` & `tmp/ricco-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricco-1.1.2.tar", last modified: Mon Jul 24 07:56:07 2023, max compression
+gzip compressed data, was "ricco-1.2.0.tar", last modified: Thu Jul 27 09:11:15 2023, max compression
```

## Comparing `ricco-1.1.2.tar` & `ricco-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 07:56:07.241949 ricco-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-24 07:55:57.000000 ricco-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 07:56:07.245949 ricco-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-24 07:55:57.000000 ricco-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.237949 ricco-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/geocode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/amap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/geocode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/geocode/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/area_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/city_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/epsg_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/resource/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/address_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/building_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/coord_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22210 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/id_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/topology_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-07-24 07:55:57.000000 ricco-1.1.2/src/ricco/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 07:56:07.241949 ricco-1.1.2/src/ricco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 07:56:07.000000 ricco-1.1.2/src/ricco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.971664 ricco-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 09:11:15.971664 ricco-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 09:11:04.000000 ricco-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 09:11:15.971664 ricco-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-27 09:11:04.000000 ricco-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/geocode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/amap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/area_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/city_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/epsg_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.971664 ricco-1.2.0/src/ricco/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/building_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/coord_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/id_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/topology_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/top_level.txt
```

### Comparing `ricco-1.1.2/PKG-INFO` & `ricco-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.1.2
+Version: 1.2.0
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.1.2/setup.py` & `ricco-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/__init__.py` & `ricco-1.2.0/src/ricco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 
 from .etl import file
 from .etl import load
 from .etl import transformer
 from .etl.extract import rdf
 from .etl.transformer import expand_dict
 from .etl.transformer import table2dict
```

### Comparing `ricco-1.1.2/src/ricco/etl/extract.py` & `ricco-1.2.0/src/ricco/etl/extract.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/etl/file.py` & `ricco-1.2.0/src/ricco/etl/file.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/etl/load.py` & `ricco-1.2.0/src/ricco/etl/load.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/etl/stat.py` & `ricco-1.2.0/src/ricco/etl/stat.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/etl/transformer.py` & `ricco-1.2.0/src/ricco/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/geocode/amap.py` & `ricco-1.2.0/src/ricco/geocode/amap.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/geocode/baidu.py` & `ricco-1.2.0/src/ricco/geocode/baidu.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/geocode/geocode.py` & `ricco-1.2.0/src/ricco/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/geocode/util.py` & `ricco-1.2.0/src/ricco/geocode/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/local.py` & `ricco-1.2.0/src/ricco/local.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/resource/area_code.py` & `ricco-1.2.0/src/ricco/resource/area_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/resource/city_id.py` & `ricco-1.2.0/src/ricco/resource/city_id.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/resource/epsg_code.py` & `ricco-1.2.0/src/ricco/resource/epsg_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/resource/names.py` & `ricco-1.2.0/src/ricco/resource/names.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/resource/phone_number.py` & `ricco-1.2.0/src/ricco/resource/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/address_tools.py` & `ricco-1.2.0/src/ricco/util/address_tools.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/assertion.py` & `ricco-1.2.0/src/ricco/util/assertion.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/building_address.py` & `ricco-1.2.0/src/ricco/util/building_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import warnings
 
-from .geom import mark_tags_v2
+from ..geometry.df import mark_tags_v2
 from .strings import drop_repeat_string
 from .util import union_str
 
 
 def make_building_address(
     df,
     *,
```

### Comparing `ricco-1.1.2/src/ricco/util/coord_trans.py` & `ricco-1.2.0/src/ricco/util/coord_trans.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,16 +362,16 @@
   坐标批量转换工具geometry
 
   :param df_org: 输入的dataframe，必须要有geometry列
   :param srs_from: 当前坐标系，可选'wgs84', 'bd09', 'gcj02'
   :param srs_to: 要转的坐标系，可选'wgs84', 'bd09', 'gcj02'
   :return:
   """
-  from .geom import wkb_dumps
-  from .geom import wkb_loads
+  from ..geometry.util import wkb_dumps
+  from ..geometry.util import wkb_loads
   if 'geometry' not in df_org.columns:
     raise KeyError('必须有geometry列')
   df_org['geometry'] = df_org['geometry'].apply(
       lambda x: wkb_dumps(
           coord_transform_geometry(wkb_loads(x, hex=True),
                                    srs_from,
                                    srs_to),
```

### Comparing `ricco-1.1.2/src/ricco/util/decorator.py` & `ricco-1.2.0/src/ricco/util/decorator.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/docx.py` & `ricco-1.2.0/src/ricco/util/docx.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/dt.py` & `ricco-1.2.0/src/ricco/util/dt.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/geom.py` & `ricco-1.2.0/src/ricco/geometry/df.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,319 +1,82 @@
-import json
 import logging
 import warnings
 from typing import List
 from typing import Union
 
-import geojson
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-from shapely import wkb
-from shapely import wkt
-from shapely.errors import GeometryTypeError
 from shapely.errors import ShapelyDeprecationWarning
-from shapely.errors import WKBReadingError
-from shapely.geometry import MultiLineString
-from shapely.geometry import MultiPolygon
 from shapely.geometry import Point
 from shapely.geometry import Polygon
-from shapely.geometry import shape
-from shapely.geos import WKTReadingError
-from simplejson.errors import JSONDecodeError
 from tqdm import tqdm
 
+from ..util.decorator import geom_progress
 from ..util.util import ensure_list
 from ..util.util import first_notnull_value
-from ..util.util import is_empty
 from ..util.util import not_empty
-from .decorator import geom_progress
+from .util import get_epsg
+from .util import get_epsg_by_lng
+from .util import get_inner_point
+from .util import infer_geom_format
+from .util import wkb_dumps
+from .util import wkb_loads
+from .util import wkt_dumps
+from .util import wkt_loads
 
 warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
 
 
-class GeomFormat:
-  wkb = 'wkb'
-  wkt = 'wkt'
-  shapely = 'shapely'
-  geojson = 'geojson'
-  unknown = 'unknown'
-
-
-def crs_sh2000():
-  """测绘院（上海2000）crs信息"""
-  from ..resource.crs import CRS_SH2000
-  return CRS_SH2000
-
-
-def get_epsg_by_lng(lng):
-  """通过经度获取epsg代码"""
-  lng_epsg_mapping = {
-    # 中央经线和epsg代码的对应关系
-    75: 4534, 78: 4535, 81: 4536, 84: 4537, 87: 4538,
-    90: 4539, 93: 4540, 96: 4541, 99: 4542,
-    102: 4543, 105: 4544, 108: 4545, 111: 4546,
-    114: 4547, 117: 4548, 120: 4549, 123: 4550,
-    126: 4551, 129: 4552, 132: 4553, 135: 4554,
-  }
-  lng = np.median(lng)
-  key = min(lng_epsg_mapping.keys(), key=lambda x: abs(x - lng))
-  return lng_epsg_mapping.get(key)
-
-
-def get_lng_by_city(city: str):
-  from ..resource.epsg_code import CITY_POINT
-  if city in CITY_POINT.keys():
-    return CITY_POINT[city]['lng']
-  else:
-    city += '市'
-    if city in CITY_POINT.keys():
-      return CITY_POINT[city]['lng']
-    else:
-      warnings.warn(f'请补充{city}的epsg信息，默认返回经度120')
-      return 120
-
-
-def get_epsg(city: str):
-  """根据城市查询epsg代码，用于投影"""
-  return get_epsg_by_lng(get_lng_by_city(city))
-
-
 def projection(
     gdf: gpd.GeoDataFrame,
     epsg: int = None,
     city: str = None):
   """投影变换"""
   if not epsg:
-    if city:
-      epsg = get_epsg(city)
-    else:
-      lngs = gdf['geometry'].centroid.x.tolist()
-      epsg = get_epsg_by_lng(lngs)
+    epsg = get_epsg(city) if city else get_epsg_by_lng(
+        gdf['geometry'].centroid.x.tolist()
+    )
   return gdf.to_crs(epsg=epsg)
 
 
-def projection_lnglat(lnglat, crs_from, crs_to):
-  from pyproj import Transformer
-  transformer = Transformer.from_crs(crs_from, crs_to)
-  return transformer.transform(xx=lnglat[1], yy=lnglat[0])
-
-
-def wkb_loads(x, hex=True):
-  warnings.filterwarnings('ignore',
-                          'Geometry column does not contain geometry.',
-                          UserWarning)
-
-  if is_empty(x):
-    return
-
-  try:
-    return wkb.loads(x, hex=hex)
-  except (AttributeError, WKBReadingError) as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def wkb_dumps(x, hex=True, srid=4326) -> (str, None):
-  if is_empty(x):
-    return
-
-  try:
-    return wkb.dumps(x, hex=hex, srid=srid)
-  except AttributeError as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def wkt_loads(x):
-  if is_empty(x):
-    return
-  try:
-    return wkt.loads(x)
-  except (AttributeError, WKTReadingError, TypeError) as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def wkt_dumps(x) -> (str, None):
-  if is_empty(x):
-    return
-  try:
-    return wkt.dumps(x)
-  except AttributeError as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def geojson_loads(x):
-  """geojson文本形式转为shapely格式"""
-  if is_empty(x):
-    return
-  try:
-    geom = shape(geojson.loads(x))
-    if geom.is_empty:
-      return
-    return geom
-  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError) as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def geojson_dumps(x) -> (str, None):
-  """shapely转为geojson文本格式"""
-  if is_empty(x):
-    return
-  try:
-    geom = geojson.Feature(geometry=x)
-    return json.dumps(geom.geometry)
-  except TypeError as e:
-    warnings.warn(f'{e}, 【{x}】')
-    return
-
-
-def is_shapely(x, na=False) -> bool:
-  """判断是否为shapely格式"""
-  from ..resource.geometry import GeomTypeSet
-  if pd.isna(x):
-    return na
-  if type(x) in GeomTypeSet:
-    return True
-  else:
-    return False
-
-
-def is_wkb(x, na=False) -> bool:
-  """判断是否为wkb格式"""
-  if not isinstance(x, str):
-    return False
-  if pd.isna(x):
-    return na
-  try:
-    wkb.loads(x, hex=True)
-    return True
-  except WKBReadingError:
-    return False
-
-
-def is_wkt(x, na=False) -> bool:
-  """判断是否为wkt格式"""
-  if not isinstance(x, str):
-    return False
-  if pd.isna(x):
-    return na
-  try:
-    wkt.loads(x)
-    return True
-  except WKTReadingError:
-    return False
-
-
-def is_geojson(x, na=False) -> bool:
-  """判断是否为geojson格式"""
-  if not isinstance(x, (str, dict)):
-    return False
-  if pd.isna(x):
-    return na
-  try:
-    if shape(geojson.loads(x)).is_empty:
-      return False
-    return True
-  except (JSONDecodeError, AttributeError, GeometryTypeError, TypeError):
-    return False
-
-
-def infer_geom_format(x):
-  """推断geometry格式"""
-  if is_shapely(x):
-    return GeomFormat.shapely
-  if is_wkb(x):
-    return GeomFormat.wkb
-  if is_wkt(x):
-    return GeomFormat.wkt
-  if is_geojson(x):
-    return GeomFormat.geojson
-  return GeomFormat.unknown
-
-
-def ensure_multi_geom(geom):
-  """将LineString和Polygon转为multi格式"""
-  if geom.geom_type == 'LineString':
-    return MultiLineString([geom])
-  if geom.geom_type == 'Polygon':
-    return MultiPolygon([geom])
-  return geom
-
-
-def multiline2multipolygon(multiline_shapely):
-  """multiline转为multipolygon，直接首尾相连"""
-  coords = []
-  for line in multiline_shapely:
-    lngs = line.xy[0]
-    lats = line.xy[1]
-    for i in range(len(lngs)):
-      lng, lat = lngs[i], lats[i]
-      point = Point((lng, lat))
-      if len(coords) >= 1:
-        if point != coords[-1]:
-          coords.append(point)
-      else:
-        coords.append(point)
-  try:
-    return MultiPolygon([Polygon(coords)])
-  except ValueError as e:
-    warnings.warn(f'{e}，{multiline_shapely}')
-    return
-
-
-def get_inner_point(polygon: Polygon, within=True):
-  """返回面内的一个点，默认返回中心点，当中心点不在面内则返回面内一个点"""
-  if is_empty(polygon):
-    return
-  point = polygon.centroid
-  if not polygon.is_valid:
-    polygon = polygon.buffer(0.000001)
-  if polygon.contains(point) or not within:
-    return point
-  return polygon.representative_point()
-
-
 @geom_progress
-def geom_wkb2shapely(df, geometry='geometry',
-                     epsg_code: int = 4326) -> gpd.GeoDataFrame:
+def wkb2shapely(df, geometry='geometry',
+                epsg_code: int = 4326) -> gpd.GeoDataFrame:
   df = df.copy()
   df[geometry] = df[geometry].progress_apply(wkb_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
 @geom_progress
-def geom_shapely2wkb(df, geometry='geometry'):
+def shapely2wkb(df, geometry='geometry'):
   df[geometry] = df[geometry].progress_apply(wkb_dumps)
   return df
 
 
 @geom_progress
-def geom_wkt2shapely(df, geometry='geometry',
-                     epsg_code: int = 4326) -> gpd.GeoDataFrame:
+def wkt2shapely(df, geometry='geometry',
+                epsg_code: int = 4326) -> gpd.GeoDataFrame:
   df[geometry] = df[geometry].progress_apply(wkt_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
 @geom_progress
-def geom_shapely2wkt(df, geometry='geometry'):
+def shapely2wkt(df, geometry='geometry'):
   df[geometry] = df[geometry].progress_apply(wkt_dumps)
   return df
 
 
 @geom_progress
-def geom_lnglat2shapely(df,
-                        lng='lng',
-                        lat='lat',
-                        geometry='geometry',
-                        delete=True,
-                        epsg_code: int = 4326) -> gpd.GeoDataFrame:
+def lnglat2shapely(df,
+                   lng='lng',
+                   lat='lat',
+                   geometry='geometry',
+                   delete=True,
+                   epsg_code: int = 4326) -> gpd.GeoDataFrame:
   from pandas.errors import SettingWithCopyWarning
   warnings.filterwarnings('ignore', category=SettingWithCopyWarning)
 
   df[geometry] = df.progress_apply(
       lambda d: Point((d[lng], d[lat]))
       if not_empty(d[lng]) and not_empty(d[lat])
       else None,
@@ -322,17 +85,17 @@
   df = gpd.GeoDataFrame(df, crs=epsg_code)
   if delete:
     del df[lng], df[lat]
   return df
 
 
 @geom_progress
-def geom_shapely2lnglat(df, geometry='geometry',
-                        lng='lng', lat='lat',
-                        within=False, delete=False):
+def shapely2lnglat(df, geometry='geometry',
+                   lng='lng', lat='lat',
+                   within=False, delete=False):
   """
   shapely格式提取中心点转为经纬度。
   within: 范围的点是否再面内，默认False，直接返回中心点；
   当为True时，不在面内的中心点将用一个在面内的点代替
   """
 
   def get_xy(x):
@@ -345,85 +108,126 @@
       axis=1
   )
   if delete:
     del df[geometry]
   return df
 
 
-def geom_wkb2lnglat(df, geometry='geometry', delete=False, within=False):
+def wkb2lnglat(df, geometry='geometry', delete=False, within=False):
   """geometry转经纬度，求中心点经纬度"""
-  df = geom_wkb2shapely(df, geometry=geometry)
-  df = geom_shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
+  df = wkb2shapely(df, geometry=geometry)
+  df = shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
   if not delete:
-    df = geom_shapely2wkb(df, geometry=geometry)
+    df = shapely2wkb(df, geometry=geometry)
   return df
 
 
-def geom_lnglat2wkb(df,
-                    lng='lng',
-                    lat='lat',
-                    geometry='geometry',
-                    delete=False, code=4326):
+def lnglat2wkb(df,
+               lng='lng',
+               lat='lat',
+               geometry='geometry',
+               delete=False, code=4326):
   """经纬度转wkb格式的geometry"""
-  df = geom_lnglat2shapely(
+  df = lnglat2shapely(
       df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
   )
-  df = geom_shapely2wkb(df, geometry=geometry)
+  df = shapely2wkb(df, geometry=geometry)
   if not delete:
     df = df.rename(columns={'lng': lng, 'lat': lat})
   return df
 
 
-def geom_wkt2lnglat(df, geometry='geometry', delete=False, within=False):
+def wkt2lnglat(df, geometry='geometry', delete=False, within=False):
   """geometry转经纬度，求中心点经纬度"""
-  df = geom_wkt2shapely(df, geometry=geometry)
-  df = geom_shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
+  df = wkt2shapely(df, geometry=geometry)
+  df = shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
   if not delete:
-    df = geom_shapely2wkt(df, geometry=geometry)
+    df = shapely2wkt(df, geometry=geometry)
   return df
 
 
-def geom_lnglat2wkt(df,
-                    lng='lng',
-                    lat='lat',
-                    geometry='geometry',
-                    delete=False, code=4326):
+def lnglat2wkt(df,
+               lng='lng',
+               lat='lat',
+               geometry='geometry',
+               delete=False, code=4326):
   """经纬度转wkb格式的geometry"""
-  df = geom_lnglat2shapely(
+  df = lnglat2shapely(
       df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
   )
-  df = geom_shapely2wkt(df, geometry=geometry)
+  df = shapely2wkt(df, geometry=geometry)
   if not delete:
     df = df.rename(columns={'lng': lng, 'lat': lat})
   return df
 
 
-def geom_wkb2wkt(df, geometry='geometry', epsg_code: int = 4326):
+def wkb2wkt(df, geometry='geometry', epsg_code: int = 4326):
   """wkb转wkt"""
-  df = geom_wkb2shapely(df, geometry=geometry, epsg_code=epsg_code)
-  return geom_shapely2wkt(df, geometry=geometry)
+  df = wkb2shapely(df, geometry=geometry, epsg_code=epsg_code)
+  return shapely2wkt(df, geometry=geometry)
 
 
-def geom_wkt2wkb(df, geometry='geometry', epsg_code: int = 4326):
+def wkt2wkb(df, geometry='geometry', epsg_code: int = 4326):
   """wkb转wkt"""
-  df = geom_wkt2shapely(df, geometry=geometry, epsg_code=epsg_code)
-  return geom_shapely2wkb(df, geometry=geometry)
+  df = wkt2shapely(df, geometry=geometry, epsg_code=epsg_code)
+  return shapely2wkb(df, geometry=geometry)
+
+
+def auto2shapely(df, geometry='geometry'):
+  geom = first_notnull_value(df[geometry])
+  geom_format = infer_geom_format(geom)
+  if geom_format == 'wkb':
+    return wkb2shapely(df, geometry=geometry)
+  elif geom_format == 'wkt':
+    return wkt2shapely(df, geometry=geometry)
+  elif geom_format == 'shapely':
+    return gpd.GeoDataFrame(df, geometry=geometry)
+  else:
+    raise TypeError('未知的地理格式，支持wkb,wkt,shapely三种格式')
+
+
+def shapely2x(df, geometry_format: str):
+  """将shapely转为指定的格式"""
+  if geometry_format == 'wkb':
+    return shapely2wkb(df)
+  elif geometry_format == 'wkt':
+    return shapely2wkt(df)
+  elif geometry_format == 'shapely':
+    return df
+  else:
+    raise ValueError('不支持的geometry格式')
+
+
+def distance_min(geometry, gdf: gpd.GeoDataFrame) -> float:
+  """
+  计算单个geometry到数据集gdf中元素的最短距离
+  Args:
+    geometry: 单个geometry，shapely格式
+    gdf: 数据集，GeoDataFrame格式
+  """
+  return gdf.distance(geometry).min()
+
+
+@geom_progress
+def distance_gdf(df: gpd.GeoDataFrame, df_target: gpd.GeoDataFrame, c_dst: str):
+  """计算一个数据集中的每个元素到另一个数据集之间的最短距离"""
+  df[c_dst] = df['geometry'].progress_apply(
+      lambda p: distance_min(p, df_target) if not_empty(p) else np.nan
+  )
+  return df
 
 
-def geom_split_grids(df: gpd.GeoDataFrame, step: int, city: str = None):
+def split_grids(df: gpd.GeoDataFrame, step: int, city: str = None):
   """
   根据所给边界划分固定边长的栅格
 
   Args:
       df: 边界文件，GeoDataFrame格式
       step: 栅格边长，单位：米
       city: 所属城市，用于投影
-
-  Returns:
-
   """
 
   def get_xxyy(df):
     bounds_dict = df.bounds.T.to_dict()[0]
     minx = bounds_dict['minx']
     miny = bounds_dict['miny']
     maxx = bounds_dict['maxx']
@@ -444,15 +248,15 @@
     B = get_lnglat(df, i, j + 1)
     C = get_lnglat(df, i + 1, j + 1)
     D = get_lnglat(df, i + 1, j)
     return Polygon((A, B, C, D, A))
 
   # 融合
   if not isinstance(df, gpd.GeoDataFrame):
-    df = geom_wkb2shapely(df)
+    df = wkb2shapely(df)
   df = df[['geometry']].dissolve()
 
   # 投影，获取实际的距离
   df_p = projection(df, city=city)
 
   # 分别获取投影前和投影后的点位及边长信息
   xy_o, xy_p = get_xxyy(df), get_xxyy(df_p)
@@ -481,15 +285,15 @@
   df_temp = pd.DataFrame({'i': i_l, 'j': j_l, 'lng': lng_l, 'lat': lat_l})
   # 删除末尾的格子，避免后面出现out of range
   df_res = df_temp.loc[
     (df_temp['i'] != x_num - 1) & (df_temp['j'] != y_num - 1),
     ['i', 'j']].reset_index(drop=True)
 
   # 组合坐标集并转为Polygon
-  tqdm.pandas(desc='lnglat2shapely')
+  tqdm.pandas(desc='lnglats2shapelyPolygon')
   df_res['geometry'] = df_res.progress_apply(
       lambda df: get_lnglat_sets(df_temp, df['i'], df['j']), axis=1)
 
   # 生成grid_id列
   df_res['grid_id'] = df_res['i'].astype(str) + '-' + df_res['j'].astype(str)
   del df_res['i'], df_res['j']
 
@@ -498,32 +302,18 @@
   df.crs = 'epsg:4326'
   df_res = gpd.sjoin(df_res,
                      df,
                      how='inner',
                      predicate='intersects').drop('index_right', axis=1)
 
   # 将geometry转为wkb格式
-  tqdm.pandas(desc='shapely2wkb')
-  df_res['geometry'] = df_res['geometry'].progress_apply(wkb_dumps)
+  df_res = shapely2wkb(df_res)
   return df_res
 
 
-def ensure_gdf(df, geometry='geometry'):
-  geom = first_notnull_value(df[geometry])
-  geom_format = infer_geom_format(geom)
-  if geom_format == 'wkb':
-    return geom_wkb2shapely(df, geometry=geometry)
-  elif geom_format == 'wkt':
-    return geom_wkt2shapely(df, geometry=geometry)
-  elif geom_format == 'shapely':
-    return gpd.GeoDataFrame(df, geometry=geometry)
-  else:
-    raise TypeError('未知的地理格式，支持wkb,wkt,shapely三种格式')
-
-
 def mark_tags_v2(
     point_df: pd.DataFrame,
     polygon_df: pd.DataFrame,
     col_list: list = None,
     predicate='intersects',
     drop_geometry=False,
     geometry_format='wkb',
@@ -534,14 +324,15 @@
   Args:
       point_df: 点数据
       polygon_df: 面数据
       col_list: 面数据中要关联到结果中的列，若为空则全部关联
       predicate: 关联方法，默认'intersects'
       drop_geometry: 结果是否删除geometry，默认删除
       geometry_format: 输出的geometry格式，支持wkb,、wkt、shapely，默认wkb
+      warning_message: 是否输出警告信息
   """
   if not col_list:
     col_list = polygon_df.columns.to_list()
   else:
     col_list = ensure_list(col_list)
     polygon_df = polygon_df[[*col_list, 'geometry']]
 
@@ -549,28 +340,28 @@
     if c in point_df and c not in ['lng', 'lat', 'geometry']:
       c_n = f'{c}_origin'
       if warning_message:
         warnings.warn(f'点数据中存在面文件中待关联的列，已重命名：{c} --> {c_n}')
       point_df.rename(columns={c: c_n}, inplace=True)
 
   if 'geometry' in point_df:
-    point_df = ensure_gdf(point_df)
+    point_df = auto2shapely(point_df)
     geom = first_notnull_value(point_df['geometry'])
     if geom.geom_type not in ['point', 'Point']:
       if warning_message:
         warnings.warn('左侧数据实际非点数据，将自动提取中心点进行关联')
       point_df['geometry_backup'] = point_df['geometry']
-      point_df = geom_shapely2lnglat(point_df, within=True)
-      point_df = geom_lnglat2shapely(point_df, delete=False)
+      point_df = shapely2lnglat(point_df, within=True)
+      point_df = lnglat2shapely(point_df, delete=False)
   elif 'lng' in point_df and 'lat' in point_df:
-    point_df = geom_lnglat2shapely(point_df, delete=False)
+    point_df = lnglat2shapely(point_df, delete=False)
   else:
     raise KeyError('点文件中必须有经纬度或geometry')
 
-  polygon_df = ensure_gdf(polygon_df)
+  polygon_df = auto2shapely(polygon_df)
 
   point_df = gpd.sjoin(
       point_df,
       polygon_df,
       how='left',
       predicate=predicate,
   ).drop('index_right', axis=1)
@@ -578,66 +369,55 @@
   if 'geometry_backup' in point_df:
     del point_df['geometry']
     point_df.rename(columns={'geometry_backup': 'geometry'}, inplace=True)
 
   if drop_geometry:
     del point_df['geometry']
   else:
-    if geometry_format == 'wkb':
-      point_df = geom_shapely2wkb(point_df)
-    elif geometry_format == 'wkt':
-      point_df = geom_shapely2wkt(point_df)
-    elif geometry_format == 'shapely':
-      pass
-    else:
-      raise ValueError('不支持的geometry格式')
+    point_df = shapely2x(point_df, geometry_format)
 
   return pd.DataFrame(point_df)
 
 
-def ensure_lnglat(lnglat) -> tuple:
-  if isinstance(lnglat, (list, tuple)):
-    if all([isinstance(i, (float, int)) for i in lnglat]):
-      return lnglat
-    else:
-      raise TypeError('数据类型错误，经度和纬度都应该为数值型')
-  if is_shapely(lnglat):
-    geom = lnglat
-  elif is_wkt(lnglat):
-    geom = wkt_loads(lnglat)
-  elif is_wkb(lnglat):
-    geom = wkb_loads(lnglat)
-  elif is_geojson(lnglat):
-    geom = geojson_loads(lnglat)
-  else:
-    raise ValueError('未知的地理类型')
-  return (geom.x, geom.y)
-
-
-def distance(
-    p1: (tuple, str),
-    p2: (tuple, str),
-    city: str = None,
-    epsg_from: int = 4326,
-    epsg_to: (str, int) = None):
+def nearest_neighbor(
+    df: pd.DataFrame,
+    df_target: pd.DataFrame,
+    c_dst='min_distance',
+    epsg: int = None) -> pd.DataFrame:
   """
-  计算两个点（经度，纬度）之间的距离，单位：米
+  近邻分析，计算一个数据集中的元素到另一个数据集中全部元素的最短距离（单位：米）
+
   Args:
-    p1: 点位1，经纬度或geometry
-    p2: 点位2，经纬度或geometry
-    city: 所在城市，用于投影
-    epsg_from: epsg代码
-    epsg_to: 投影epsg代码
-  """
-  p1, p2 = ensure_lnglat(p1), ensure_lnglat(p2)
-  if not epsg_to:
-    epsg_to = get_epsg(city) if city else get_epsg_by_lng([p1[0], p2[0]])
-  p1 = projection_lnglat(p1, epsg_from, epsg_to)
-  p2 = projection_lnglat(p2, epsg_from, epsg_to)
-  return Point(p1).distance(Point(p2))
+    df:
+    df_target:
+    c_dst: 输出最短距离的列名
+    epsg: 对于跨时区或不在同一个城市的可以指定epsg code
+  """
+
+  def ensure_geometry(_df):
+    if 'geometry' in _df:
+      return auto2shapely(_df[['geometry']])[['geometry']]
+    elif 'lng' in _df and 'lat' in _df:
+      return lnglat2shapely(
+          _df[['lng', 'lat']],
+          delete=False)[['geometry']]
+    else:
+      raise KeyError('文件中必须有经纬度或geometry')
+
+  # 将两个数据集都转为shapely格式
+  df_left = ensure_geometry(df)
+  df_target = ensure_geometry(df_target)
+  # 投影
+  df_left = projection(df_left, epsg=epsg)
+  df_target = projection(df_target, epsg=epsg)
+  # 计算最短距离
+  df_left = distance_gdf(df_left, df_target, c_dst)
+  # 将距离合并到原来的数据集上
+  df = df.merge(df_left[[c_dst]], left_index=True, right_index=True, how='left')
+  return pd.DataFrame(df).sort_index()
 
 
 def buffer(df: pd.DataFrame, radius: Union[int, float],
            city: str = None,
            geo_type: str = 'point',
            geometry: str = 'geometry',
            buffer_geometry: str = 'buffer_geometry',
@@ -681,47 +461,36 @@
   if 'lng' in df and 'lat' in df:
     cols.extend(['lng', 'lat'])
   df_tmp = df[cols]
   df_tmp.rename(columns={geometry: 'geometry'}, inplace=True)
 
   if geo_type == 'point':
     if 'geometry' in df_tmp:
-      df_tmp = ensure_gdf(df_tmp)
+      df_tmp = auto2shapely(df_tmp)
       geom = first_notnull_value(df_tmp['geometry'])
       if geom.geom_type not in ['point', 'Point']:
         warnings.warn('数据实际非点数据，将自动提取中心点进行关联')
-        df_tmp = geom_shapely2lnglat(df_tmp)
-        df_tmp = geom_lnglat2shapely(df_tmp, delete=False)
+        df_tmp = shapely2lnglat(df_tmp)
+        df_tmp = lnglat2shapely(df_tmp, delete=False)
     elif 'lng' in df_tmp and 'lat' in df_tmp:
-      df_tmp = geom_lnglat2shapely(df_tmp, delete=False)
-
+      df_tmp = lnglat2shapely(df_tmp, delete=False)
     else:
       raise KeyError('点文件中必须有经纬度或geometry')
   elif geo_type == 'line' or geo_type == 'polygon':
-    df_tmp = ensure_gdf(df_tmp, geometry=geometry)
+    df_tmp = auto2shapely(df_tmp, geometry=geometry)
   else:
     raise ValueError('geo_type必须为point，line或polygon')
-  df_buffer = df_tmp[['geometry']]
 
+  df_buffer = df_tmp[['geometry']]
   df_buffer = projection(df_buffer, city=city)
   df_buffer['geometry'] = df_buffer.geometry.buffer(radius)
   df_buffer = projection(df_buffer, epsg=4326)
-  if geo_format == 'wkb':
-    tqdm.pandas(desc='shapely2wkb')
-    df_buffer['geometry'] = df_buffer['geometry'].progress_apply(wkb_dumps)
-  elif geo_format == 'wkt':
-    tqdm.pandas(desc='shapely2wkt')
-    df_buffer['geometry'] = df_buffer['geometry'].progress_apply(wkt_dumps)
-  elif geo_format == 'shapely':
-    pass
-  else:
-    raise ValueError('不支持的geometry格式')
+  df_buffer = shapely2x(df_buffer, geo_format)
   df_buffer.rename(columns={'geometry': buffer_geometry}, inplace=True)
   df = df.join(df_buffer, how='left')
-
   return df
 
 
 def spatial_agg(point_df: pd.DataFrame, polygon_df: pd.DataFrame,
                 by: Union[str, List[str]],
                 agg: dict,
                 polygon_geometry: str = 'geometry') -> pd.DataFrame:
```

### Comparing `ricco-1.1.2/src/ricco/util/id_number.py` & `ricco-1.2.0/src/ricco/util/id_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/os.py` & `ricco-1.2.0/src/ricco/util/os.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/phone_number.py` & `ricco-1.2.0/src/ricco/util/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/strings.py` & `ricco-1.2.0/src/ricco/util/strings.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/topology_check.py` & `ricco-1.2.0/src/ricco/util/topology_check.py`

 * *Files identical despite different names*

### Comparing `ricco-1.1.2/src/ricco/util/util.py` & `ricco-1.2.0/src/ricco/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     return now.year - birthday.year
   else:
     return now.year - birthday.year - 1
 
 
 def first_notnull_value(series):
   for v in series:
-    if pd.notna(v) or not v.is_empty:
+    if not_empty(v):
       return v
   warnings.warn('所有值均为空值')
   return None
 
 
 def pinyin(word: str) -> str:
   """将中文转换为汉语拼音"""
```

### Comparing `ricco-1.1.2/src/ricco.egg-info/PKG-INFO` & `ricco-1.2.0/src/ricco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.1.2
+Version: 1.2.0
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.1.2/src/ricco.egg-info/SOURCES.txt` & `ricco-1.2.0/src/ricco.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 src/ricco/etl/stat.py
 src/ricco/etl/transformer.py
 src/ricco/geocode/__init__.py
 src/ricco/geocode/amap.py
 src/ricco/geocode/baidu.py
 src/ricco/geocode/geocode.py
 src/ricco/geocode/util.py
+src/ricco/geometry/__init__.py
+src/ricco/geometry/df.py
+src/ricco/geometry/util.py
 src/ricco/resource/__init__.py
 src/ricco/resource/area_code.py
 src/ricco/resource/city_id.py
 src/ricco/resource/crs.py
 src/ricco/resource/epsg_code.py
 src/ricco/resource/geometry.py
 src/ricco/resource/names.py
```

