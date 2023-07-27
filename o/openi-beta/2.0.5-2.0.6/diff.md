# Comparing `tmp/openi-beta-2.0.5.tar.gz` & `tmp/openi-beta-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-beta-2.0.5.tar", last modified: Thu Jul 27 10:02:58 2023, max compression
+gzip compressed data, was "openi-beta-2.0.6.tar", last modified: Thu Jul 27 10:09:10 2023, max compression
```

## Comparing `openi-beta-2.0.5.tar` & `openi-beta-2.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.801853 openi-beta-2.0.5/
--rw-rw-rw-   0        0        0     5381 2023-07-27 10:02:58.800850 openi-beta-2.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 10:02:58.801853 openi-beta-2.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-07-27 10:02:56.000000 openi-beta-2.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.773010 openi-beta-2.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.777640 openi-beta-2.0.5/src/openi/
--rw-rw-rw-   0        0        0      194 2023-07-26 01:33:14.000000 openi-beta-2.0.5/src/openi/__init__.py
--rw-rw-rw-   0        0        0     6456 2023-07-26 01:30:58.000000 openi-beta-2.0.5/src/openi/apis.py
--rw-rw-rw-   0        0        0     5238 2023-07-26 01:33:22.000000 openi-beta-2.0.5/src/openi/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.781716 openi-beta-2.0.5/src/openi/cloudbrain/
--rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.5/src/openi/cloudbrain/__init__.py
--rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.5/src/openi/cloudbrain/env_check.py
--rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.5/src/openi/cloudbrain/helper.py
--rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.5/src/openi/cloudbrain/minio_operate.py
--rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.5/src/openi/cloudbrain/obs_operate.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.784886 openi-beta-2.0.5/src/openi/dataset/
--rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.5/src/openi/dataset/__init__.py
--rw-rw-rw-   0        0        0     2752 2023-07-26 01:32:22.000000 openi-beta-2.0.5/src/openi/dataset/dataset_file.py
--rw-rw-rw-   0        0        0     2685 2023-07-26 01:32:31.000000 openi-beta-2.0.5/src/openi/dataset/download.py
--rw-rw-rw-   0        0        0     4392 2023-07-27 10:02:33.000000 openi-beta-2.0.5/src/openi/dataset/upload.py
--rw-rw-rw-   0        0        0     3029 2023-07-26 01:31:33.000000 openi-beta-2.0.5/src/openi/login.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.785890 openi-beta-2.0.5/src/openi/path/
--rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.5/src/openi/path/__init__.py
--rw-rw-rw-   0        0        0     2405 2023-07-26 01:32:02.000000 openi-beta-2.0.5/src/openi/path/path.py
--rw-rw-rw-   0        0        0     4081 2023-07-26 01:33:29.000000 openi-beta-2.0.5/src/openi/settings.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.788219 openi-beta-2.0.5/src/openi/utils/
--rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.5/src/openi/utils/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-07-26 01:31:45.000000 openi-beta-2.0.5/src/openi/utils/file_utils.py
--rw-rw-rw-   0        0        0      723 2023-07-26 01:33:04.000000 openi-beta-2.0.5/src/openi/utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.799384 openi-beta-2.0.5/src/openi_beta.egg-info/
--rw-rw-rw-   0        0        0     5381 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      787 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 10:02:58.000000 openi-beta-2.0.5/src/openi_beta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 10:02:58.800850 openi-beta-2.0.5/test/
--rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.5/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.321934 openi-beta-2.0.6/
+-rw-rw-rw-   0        0        0     5381 2023-07-27 10:09:10.320836 openi-beta-2.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4735 2023-07-24 07:49:31.000000 openi-beta-2.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-27 10:09:10.321934 openi-beta-2.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-27 10:08:35.000000 openi-beta-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.282755 openi-beta-2.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.287652 openi-beta-2.0.6/src/openi/
+-rw-rw-rw-   0        0        0      194 2023-07-26 01:33:14.000000 openi-beta-2.0.6/src/openi/__init__.py
+-rw-rw-rw-   0        0        0     6456 2023-07-26 01:30:58.000000 openi-beta-2.0.6/src/openi/apis.py
+-rw-rw-rw-   0        0        0     5238 2023-07-26 01:33:22.000000 openi-beta-2.0.6/src/openi/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.289389 openi-beta-2.0.6/src/openi/cloudbrain/
+-rw-rw-rw-   0        0        0       84 2023-07-24 07:06:23.000000 openi-beta-2.0.6/src/openi/cloudbrain/__init__.py
+-rw-rw-rw-   0        0        0     1609 2023-07-24 07:06:26.000000 openi-beta-2.0.6/src/openi/cloudbrain/env_check.py
+-rw-rw-rw-   0        0        0     5313 2023-07-24 07:06:29.000000 openi-beta-2.0.6/src/openi/cloudbrain/helper.py
+-rw-rw-rw-   0        0        0     1559 2023-07-24 07:06:31.000000 openi-beta-2.0.6/src/openi/cloudbrain/minio_operate.py
+-rw-rw-rw-   0        0        0     2886 2023-07-24 07:06:32.000000 openi-beta-2.0.6/src/openi/cloudbrain/obs_operate.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.297347 openi-beta-2.0.6/src/openi/dataset/
+-rw-rw-rw-   0        0        0      109 2023-07-24 07:06:34.000000 openi-beta-2.0.6/src/openi/dataset/__init__.py
+-rw-rw-rw-   0        0        0     2752 2023-07-26 01:32:22.000000 openi-beta-2.0.6/src/openi/dataset/dataset_file.py
+-rw-rw-rw-   0        0        0     2685 2023-07-26 01:32:31.000000 openi-beta-2.0.6/src/openi/dataset/download.py
+-rw-rw-rw-   0        0        0     4392 2023-07-27 10:08:25.000000 openi-beta-2.0.6/src/openi/dataset/upload.py
+-rw-rw-rw-   0        0        0     3029 2023-07-26 01:31:33.000000 openi-beta-2.0.6/src/openi/login.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.299352 openi-beta-2.0.6/src/openi/path/
+-rw-rw-rw-   0        0        0       21 2023-07-24 07:06:52.000000 openi-beta-2.0.6/src/openi/path/__init__.py
+-rw-rw-rw-   0        0        0     2405 2023-07-26 01:32:02.000000 openi-beta-2.0.6/src/openi/path/path.py
+-rw-rw-rw-   0        0        0     4081 2023-07-26 01:33:29.000000 openi-beta-2.0.6/src/openi/settings.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.307580 openi-beta-2.0.6/src/openi/utils/
+-rw-rw-rw-   0        0        0       50 2023-07-24 07:07:03.000000 openi-beta-2.0.6/src/openi/utils/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-07-26 01:31:45.000000 openi-beta-2.0.6/src/openi/utils/file_utils.py
+-rw-rw-rw-   0        0        0      723 2023-07-26 01:33:04.000000 openi-beta-2.0.6/src/openi/utils/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.319648 openi-beta-2.0.6/src/openi_beta.egg-info/
+-rw-rw-rw-   0        0        0     5381 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      787 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 10:09:10.000000 openi-beta-2.0.6/src/openi_beta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 10:09:10.320836 openi-beta-2.0.6/test/
+-rw-rw-rw-   0        0        0       87 2023-07-24 07:35:25.000000 openi-beta-2.0.6/test/test.py
```

### Comparing `openi-beta-2.0.5/PKG-INFO` & `openi-beta-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.5
+Version: 2.0.6
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.5/README.md` & `openi-beta-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/setup.py` & `openi-beta-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi-beta",
-    version="2.0.5",
+    version="2.0.6",
     description="Beta package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages("src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-beta-2.0.5/src/openi/apis.py` & `openi-beta-2.0.6/src/openi/apis.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/cli.py` & `openi-beta-2.0.6/src/openi/cli.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/cloudbrain/env_check.py` & `openi-beta-2.0.6/src/openi/cloudbrain/env_check.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/cloudbrain/helper.py` & `openi-beta-2.0.6/src/openi/cloudbrain/helper.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/cloudbrain/minio_operate.py` & `openi-beta-2.0.6/src/openi/cloudbrain/minio_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/cloudbrain/obs_operate.py` & `openi-beta-2.0.6/src/openi/cloudbrain/obs_operate.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/dataset/dataset_file.py` & `openi-beta-2.0.6/src/openi/dataset/dataset_file.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/dataset/download.py` & `openi-beta-2.0.6/src/openi/dataset/download.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/dataset/upload.py` & `openi-beta-2.0.6/src/openi/dataset/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     # upload completed
     if _get_chunks["uploaded"] == "1":
         if _get_chunks["datasetID"] != "" and _get_chunks["datasetName"] != "":
             msg = (
                 f"❌ Upload failed: `{_file.filename}` ({cluster})"
                 " already exists in "
-                f"{api.endpoint.split('/api')[0]}/{_get_chunks['repoOnwer']}/{_get_chunks['repoName']}/datasets"
+                f"{api.endpoint.split('/api')[0]}/{_get_chunks['repoOwner']}/{_get_chunks['repoName']}/datasets"
             )
             logging.error(msg)
             raise ValueError(msg)
 
     # upload continue
     if _get_chunks["uuid"] != "" or _get_chunks["uploadID"] != "":
         _file.uuid, _file.upload_id = _get_chunks["uuid"], _get_chunks["uploadID"]
```

### Comparing `openi-beta-2.0.5/src/openi/login.py` & `openi-beta-2.0.6/src/openi/login.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/path/path.py` & `openi-beta-2.0.6/src/openi/path/path.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/settings.py` & `openi-beta-2.0.6/src/openi/settings.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/utils/file_utils.py` & `openi-beta-2.0.6/src/openi/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi/utils/logger.py` & `openi-beta-2.0.6/src/openi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openi-beta-2.0.5/src/openi_beta.egg-info/PKG-INFO` & `openi-beta-2.0.6/src/openi_beta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi-beta
-Version: 2.0.5
+Version: 2.0.6
 Summary: Beta package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-beta-2.0.5/src/openi_beta.egg-info/SOURCES.txt` & `openi-beta-2.0.6/src/openi_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

