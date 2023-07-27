# Comparing `tmp/wafermap-clustering-0.3.5.tar.gz` & `tmp/wafermap-clustering-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.5.tar", last modified: Wed Jul 26 15:01:34 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.6.tar", last modified: Thu Jul 27 09:16:19 2023, max compression
```

## Comparing `wafermap-clustering-0.3.5.tar` & `wafermap-clustering-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.082036 wafermap-clustering-0.3.5/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-26 15:01:34.075908 wafermap-clustering-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-26 15:01:34.082724 wafermap-clustering-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-07-26 14:49:57.000000 wafermap-clustering-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:33.989505 wafermap-clustering-0.3.5/tests/
--rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.5/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:33.996645 wafermap-clustering-0.3.5/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.040639 wafermap-clustering-0.3.5/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.5/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.049032 wafermap-clustering-0.3.5/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.5/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.071885 wafermap-clustering-0.3.5/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     6949 2023-07-26 14:32:07.000000 wafermap-clustering-0.3.5/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.033777 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.234962 wafermap-clustering-0.3.6/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-27 09:16:19.232898 wafermap-clustering-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 09:16:19.235696 wafermap-clustering-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-07-27 09:15:51.000000 wafermap-clustering-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.188587 wafermap-clustering-0.3.6/tests/
+-rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.6/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.194041 wafermap-clustering-0.3.6/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.217190 wafermap-clustering-0.3.6/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.6/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.219694 wafermap-clustering-0.3.6/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.6/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.229390 wafermap-clustering-0.3.6/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     7008 2023-07-27 09:15:39.000000 wafermap-clustering-0.3.6/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-27 09:16:19.213862 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 09:16:19.000000 wafermap-clustering-0.3.6/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.5/LICENSE.txt` & `wafermap-clustering-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.5/PKG-INFO` & `wafermap-clustering-0.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.5/setup.py` & `wafermap-clustering-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.5"
+version = "0.3.6"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.5/tests/test_clustering.py` & `wafermap-clustering-0.3.6/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.6/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.6/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.6/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.6/wafermap_clustering/wafermap_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,18 @@
         self,
         klarf_path: Path,
         output_directory: str = None,
         klarf_format=KlarfFormat.BABY.value,
         clustering_mode=ClusteringMode.DBSCAN.value,
     ) -> List[ClusteringResult]:
 
-        content = Klarf.load_from_file_with_raw_content(filepath=klarf_path)
+        content = Klarf.load_from_file_with_raw_content(
+            filepath=klarf_path,
+            parse_summary=False,
+        )
 
         return self.apply_from_content(
             content=content,
             output_directory=output_directory,
             original_klarf_name=klarf_path.stem,
             original_klarf_extension=klarf_path.suffix,
             klarf_format=klarf_format,
```

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.6/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.5/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.6/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

