# Comparing `tmp/voxio-1.0.0.tar.gz` & `tmp/voxio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxio-1.0.0.tar", max compression
+gzip compressed data, was "voxio-1.0.1.tar", max compression
```

## Comparing `voxio-1.0.0.tar` & `voxio-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1658 2023-03-25 07:28:26.601121 voxio-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      893 2023-03-25 07:20:06.435288 voxio-1.0.0/README.md
--rw-r--r--   0        0        0     1327 2023-07-27 04:49:24.462098 voxio-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 18:02:41.603087 voxio-1.0.0/voxio/__init__.py
--rw-r--r--   0        0        0      953 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/caching.py
--rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-1.0.0/voxio/clean/__init__.py
--rwxr-xr-x   0        0        0     1596 2023-07-27 04:35:37.202047 voxio-1.0.0/voxio/clean/single_big_obj_artifact_purge.py
--rw-r--r--   0        0        0     1592 2023-07-27 08:01:39.157450 voxio-1.0.0/voxio/cli/__init__.py
--rw-r--r--   0        0        0      144 2023-03-25 07:20:06.402289 voxio-1.0.0/voxio/cli/settings.py
--rw-r--r--   0        0        0      899 2023-07-27 04:47:18.387395 voxio-1.0.0/voxio/crop.py
--rw-r--r--   0        0        0     2248 2023-07-27 04:40:04.303418 voxio-1.0.0/voxio/read.py
--rw-r--r--   0        0        0        0 2023-03-19 15:27:51.685539 voxio-1.0.0/voxio/utils/__init__.py
--rw-r--r--   0        0        0     1601 2023-07-27 04:47:18.397395 voxio-1.0.0/voxio/utils/distance.py
--rw-r--r--   0        0        0     1466 2023-07-27 04:47:18.377395 voxio-1.0.0/voxio/utils/interpolate.py
--rw-r--r--   0        0        0     1370 2023-07-27 04:47:41.670340 voxio-1.0.0/voxio/utils/io.py
--rw-r--r--   0        0        0     1603 2023-07-27 04:51:53.495746 voxio-1.0.0/voxio/utils/misc.py
--rw-r--r--   0        0        0       29 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/utils/typings.py
--rw-r--r--   0        0        0      336 2023-07-27 04:26:59.572267 voxio-1.0.0/voxio/volume_info/__init__.py
--rw-r--r--   0        0        0     6101 2023-07-27 04:47:18.414395 voxio-1.0.0/voxio/volume_info/read.py
--rw-r--r--   0        0        0     7788 2023-07-27 04:51:53.615746 voxio-1.0.0/voxio/volume_info/volume_info.py
--rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-1.0.0/voxio/workflows/__init__.py
--rw-r--r--   0        0        0     9044 2023-07-27 04:53:54.110462 voxio-1.0.0/voxio/workflows/label_binary_image.py
--rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 voxio-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1658 2023-03-25 07:28:26.601121 voxio-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      893 2023-03-25 07:20:06.435288 voxio-1.0.1/README.md
+-rw-r--r--   0        0        0     1327 2023-07-27 15:06:51.422268 voxio-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 18:02:41.603087 voxio-1.0.1/voxio/__init__.py
+-rw-r--r--   0        0        0      953 2023-07-27 12:50:36.790204 voxio-1.0.1/voxio/caching.py
+-rw-r--r--   0        0        0        0 2023-03-25 07:20:06.396289 voxio-1.0.1/voxio/clean/__init__.py
+-rwxr-xr-x   0        0        0     1596 2023-07-27 12:50:56.030102 voxio-1.0.1/voxio/clean/single_big_obj_artifact_purge.py
+-rw-r--r--   0        0        0     1110 2023-07-27 13:17:46.441060 voxio-1.0.1/voxio/cli.py
+-rw-r--r--   0        0        0      899 2023-07-27 12:50:56.030102 voxio-1.0.1/voxio/crop.py
+-rw-r--r--   0        0        0     2248 2023-07-27 12:50:56.030102 voxio-1.0.1/voxio/read.py
+-rw-r--r--   0        0        0        0 2023-03-19 15:27:51.685539 voxio-1.0.1/voxio/utils/__init__.py
+-rw-r--r--   0        0        0     1601 2023-07-27 12:50:56.030102 voxio-1.0.1/voxio/utils/distance.py
+-rw-r--r--   0        0        0     1466 2023-07-27 12:50:56.030102 voxio-1.0.1/voxio/utils/interpolate.py
+-rw-r--r--   0        0        0     3972 2023-07-27 14:37:09.758500 voxio-1.0.1/voxio/utils/io.py
+-rw-r--r--   0        0        0     1603 2023-07-27 12:50:56.031102 voxio-1.0.1/voxio/utils/misc.py
+-rw-r--r--   0        0        0       29 2023-07-27 12:50:36.792204 voxio-1.0.1/voxio/utils/typings.py
+-rw-r--r--   0        0        0      336 2023-07-27 12:50:36.792204 voxio-1.0.1/voxio/volume_info/__init__.py
+-rw-r--r--   0        0        0     6101 2023-07-27 12:50:56.031102 voxio-1.0.1/voxio/volume_info/read.py
+-rw-r--r--   0        0        0     7788 2023-07-27 12:50:56.031102 voxio-1.0.1/voxio/volume_info/volume_info.py
+-rw-r--r--   0        0        0        0 2023-07-27 12:50:56.031102 voxio-1.0.1/voxio/workflows/__init__.py
+-rw-r--r--   0        0        0     9044 2023-07-27 12:50:56.031102 voxio-1.0.1/voxio/workflows/label_binary_image.py
+-rw-r--r--   0        0        0     2315 1970-01-01 00:00:00.000000 voxio-1.0.1/PKG-INFO
```

### Comparing `voxio-1.0.0/LICENSE.md` & `voxio-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/README.md` & `voxio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/pyproject.toml` & `voxio-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxio"
-version = "1.0.0"
+version = "1.0.1"
 description = "Library for ingesting and processing voxel (3D imaging) data"
 authors = ["caniko <canhtart@gmail.com>"]
 license = "BSD-4"
 repository = "https://github.com/caniko/voxio"
 readme = "README.md"
 
 keywords = ["voxel", "processing", "fix", "mesh"]
```

### Comparing `voxio-1.0.0/voxio/caching.py` & `voxio-1.0.1/voxio/caching.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/clean/single_big_obj_artifact_purge.py` & `voxio-1.0.1/voxio/clean/single_big_obj_artifact_purge.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/crop.py` & `voxio-1.0.1/voxio/crop.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/read.py` & `voxio-1.0.1/voxio/read.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/utils/distance.py` & `voxio-1.0.1/voxio/utils/distance.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/utils/interpolate.py` & `voxio-1.0.1/voxio/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/utils/misc.py` & `voxio-1.0.1/voxio/utils/misc.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/volume_info/read.py` & `voxio-1.0.1/voxio/volume_info/read.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/volume_info/volume_info.py` & `voxio-1.0.1/voxio/volume_info/volume_info.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/voxio/workflows/label_binary_image.py` & `voxio-1.0.1/voxio/workflows/label_binary_image.py`

 * *Files identical despite different names*

### Comparing `voxio-1.0.0/PKG-INFO` & `voxio-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library for ingesting and processing voxel (3D imaging) data
 Home-page: https://github.com/caniko/voxio
 License: BSD-4
 Keywords: voxel,processing,fix,mesh
 Author: caniko
 Author-email: canhtart@gmail.com
 Requires-Python: >=3.10,<3.11
```

