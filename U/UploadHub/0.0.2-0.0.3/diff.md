# Comparing `tmp/UploadHub-0.0.2.tar.gz` & `tmp/UploadHub-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UploadHub-0.0.2.tar", last modified: Sun Jul 23 05:11:06 2023, max compression
+gzip compressed data, was "UploadHub-0.0.3.tar", last modified: Thu Jul 27 01:40:26 2023, max compression
```

## Comparing `UploadHub-0.0.2.tar` & `UploadHub-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 05:11:06.469848 UploadHub-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      516 2023-07-23 05:11:06.467849 UploadHub-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 05:11:06.428014 UploadHub-0.0.2/UploadHub/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.2/UploadHub/__init__.py
--rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.2/UploadHub/__main__.py
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.2/UploadHub/license.py
--rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.2/UploadHub/new.py
--rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.2/UploadHub/setup.py
--rw-rw-rw-   0        0        0     8234 2023-07-23 05:09:49.000000 UploadHub-0.0.2/UploadHub/upload.py
--rw-rw-rw-   0        0        0     2335 2023-07-23 04:57:52.000000 UploadHub-0.0.2/UploadHub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-23 05:11:06.464863 UploadHub-0.0.2/UploadHub.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-23 05:11:06.000000 UploadHub-0.0.2/UploadHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-23 05:11:06.000000 UploadHub-0.0.2/UploadHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 05:11:06.000000 UploadHub-0.0.2/UploadHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-23 05:11:06.000000 UploadHub-0.0.2/UploadHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-23 05:11:06.000000 UploadHub-0.0.2/UploadHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 05:11:06.470849 UploadHub-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      811 2023-07-23 05:10:44.000000 UploadHub-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.999223 UploadHub-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      516 2023-07-27 01:40:25.996220 UploadHub-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.954217 UploadHub-0.0.3/UploadHub/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.3/UploadHub/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.3/UploadHub/__main__.py
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.3/UploadHub/license.py
+-rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.3/UploadHub/new.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.3/UploadHub/setup.py
+-rw-rw-rw-   0        0        0     8234 2023-07-23 05:09:49.000000 UploadHub-0.0.3/UploadHub/upload.py
+-rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.3/UploadHub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 01:40:25.992220 UploadHub-0.0.3/UploadHub.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 01:40:25.000000 UploadHub-0.0.3/UploadHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 01:40:25.999223 UploadHub-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      883 2023-07-27 01:40:13.000000 UploadHub-0.0.3/setup.py
```

### Comparing `UploadHub-0.0.2/LICENSE` & `UploadHub-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/PKG-INFO` & `UploadHub-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.2
+Version: 0.0.3
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.2/UploadHub/__main__.py` & `UploadHub-0.0.3/UploadHub/__main__.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/UploadHub/license.py` & `UploadHub-0.0.3/UploadHub/license.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/UploadHub/new.py` & `UploadHub-0.0.3/UploadHub/new.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/UploadHub/setup.py` & `UploadHub-0.0.3/UploadHub/setup.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/UploadHub/upload.py` & `UploadHub-0.0.3/UploadHub/upload.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.2/UploadHub/utils.py` & `UploadHub-0.0.3/UploadHub/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import ttkbootstrap as ttk
 from ttkbootstrap.dialogs import Messagebox
 
 
 def load_config() -> dict:
     """Loads the json file for configuration"""
     config_path = os.path.dirname(__file__)
-    config_path = os.path.join(config_path, 'config.json')
+    config_path = os.path.join(config_path, 'data/config.json')
     with open(config_path, 'r') as f:
         config = json.load(f)
     return config
 
 
 def save_config(config: dict) -> None:
     """Saves the json file for configuration"""
     config_path = os.path.dirname(__file__)
-    config_path = os.path.join(config_path, 'config.json')
+    config_path = os.path.join(config_path, 'data/config.json')
     with open(config_path, 'r') as f:
         json.dump(config, f, indent=4)
 
 
 class StatusBar(ttk.Frame):
     def __init__(self, master: ttk.Frame, **kwargs):
         super().__init__(master, **kwargs)
```

### Comparing `UploadHub-0.0.2/UploadHub.egg-info/PKG-INFO` & `UploadHub-0.0.3/UploadHub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.2
+Version: 0.0.3
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.2/setup.py` & `UploadHub-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'PYPI and GitHub package uploader.'
 LONG_DESCRIPTION = 'Manages all the commands to upload a package to PYPI and GitHub repo.'
 
 setup(
     name='UploadHub',
     version=VERSION,
     author="Armando Chaparro",
@@ -18,9 +18,11 @@
     ],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
-    ]
+    ],
+    include_package_data=True,
+    package_data={'': ['data/*.csv']}
 )
```

