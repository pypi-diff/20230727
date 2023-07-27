# Comparing `tmp/UploadHub-0.0.4.tar.gz` & `tmp/UploadHub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UploadHub-0.0.4.tar", last modified: Thu Jul 27 01:45:15 2023, max compression
+gzip compressed data, was "UploadHub-0.0.5.tar", last modified: Thu Jul 27 19:30:01 2023, max compression
```

## Comparing `UploadHub-0.0.4.tar` & `UploadHub-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.405163 UploadHub-0.0.4/
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      516 2023-07-27 01:45:15.404183 UploadHub-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.354145 UploadHub-0.0.4/UploadHub/
--rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.4/UploadHub/__init__.py
--rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.4/UploadHub/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.401168 UploadHub-0.0.4/UploadHub/data/
--rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.4/UploadHub/data/config.json
--rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.4/UploadHub/license.py
--rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.4/UploadHub/new.py
--rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.4/UploadHub/setup.py
--rw-rw-rw-   0        0        0     8234 2023-07-23 05:09:49.000000 UploadHub-0.0.4/UploadHub/upload.py
--rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.4/UploadHub/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:45:15.391151 UploadHub-0.0.4/UploadHub.egg-info/
--rw-rw-rw-   0        0        0      516 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-27 01:45:15.000000 UploadHub-0.0.4/UploadHub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 01:45:15.406163 UploadHub-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      884 2023-07-27 01:45:13.000000 UploadHub-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.890541 UploadHub-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:02.000000 UploadHub-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      516 2023-07-27 19:30:01.888539 UploadHub-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 18:43:42.000000 UploadHub-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.843536 UploadHub-0.0.5/UploadHub/
+-rw-rw-rw-   0        0        0        0 2023-07-23 05:01:02.000000 UploadHub-0.0.5/UploadHub/__init__.py
+-rw-rw-rw-   0        0        0      704 2023-07-23 05:09:33.000000 UploadHub-0.0.5/UploadHub/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.885537 UploadHub-0.0.5/UploadHub/data/
+-rw-rw-rw-   0        0        0      112 2023-07-23 04:18:02.000000 UploadHub-0.0.5/UploadHub/data/config.json
+-rw-rw-rw-   0        0        0     1088 2023-07-19 04:27:06.000000 UploadHub-0.0.5/UploadHub/license.py
+-rw-rw-rw-   0        0        0     9815 2023-07-23 05:09:52.000000 UploadHub-0.0.5/UploadHub/new.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 04:20:31.000000 UploadHub-0.0.5/UploadHub/setup.py
+-rw-rw-rw-   0        0        0     8234 2023-07-27 19:28:22.000000 UploadHub-0.0.5/UploadHub/upload.py
+-rw-rw-rw-   0        0        0     2345 2023-07-27 01:39:15.000000 UploadHub-0.0.5/UploadHub/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:30:01.881540 UploadHub-0.0.5/UploadHub.egg-info/
+-rw-rw-rw-   0        0        0      516 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-27 19:30:01.000000 UploadHub-0.0.5/UploadHub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 19:30:01.891540 UploadHub-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-07-27 19:29:53.000000 UploadHub-0.0.5/setup.py
```

### Comparing `UploadHub-0.0.4/LICENSE` & `UploadHub-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/PKG-INFO` & `UploadHub-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.4
+Version: 0.0.5
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.4/UploadHub/__main__.py` & `UploadHub-0.0.5/UploadHub/__main__.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/UploadHub/license.py` & `UploadHub-0.0.5/UploadHub/license.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/UploadHub/new.py` & `UploadHub-0.0.5/UploadHub/new.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/UploadHub/setup.py` & `UploadHub-0.0.5/UploadHub/setup.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/UploadHub/upload.py` & `UploadHub-0.0.5/UploadHub/upload.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -146,21 +146,14 @@
         # GIT INFO
         push_git = self.push_git.get()
         delete_past = self.delete_past.get()
         update_version = self.update_version.get()
         upload_pypi = self.upload_pypi.get()
         dist_folder = os.path.join(package_dir, 'dist')
 
-        # UPDATE GIT REPOSITORY IF NEEDED
-        if push_git == 'Yes':
-            if not (commit_git := self.check_entry(self.commit_git)): return
-            self.run('git add .', package_dir)
-            subprocess.run(['git', 'commit', '-m', f'"{commit_git}"'], cwd=package_dir)
-            self.run('git push', package_dir)
-
         # DELETE PREVIOUS VERSIONS IF NEEDED
         if delete_past == 'Yes' and os.path.isdir(dist_folder):
             for file in os.listdir(dist_folder):
                 os.remove(os.path.join(dist_folder, file))
 
         # UPDATE VERSION IF NEEDED
         if update_version == 'Yes':
@@ -170,8 +163,15 @@
             self.update_new_version(package_dir, version)
 
         # UPLOAD TO PYPI
         if upload_pypi == 'Yes':
             self.run('python setup.py sdist bdist_wheel', package_dir)
             self.run('twine upload dist/*', package_dir)
         
+        # UPDATE GIT REPOSITORY IF NEEDED
+        if push_git == 'Yes':
+            if not (commit_git := self.check_entry(self.commit_git)): return
+            self.run('git add .', package_dir)
+            subprocess.run(['git', 'commit', '-m', f'"{commit_git}"'], cwd=package_dir)
+            self.run('git push', package_dir)
+
         self.status_bar.info('Package successfully uploaded...')
```

### Comparing `UploadHub-0.0.4/UploadHub/utils.py` & `UploadHub-0.0.5/UploadHub/utils.py`

 * *Files identical despite different names*

### Comparing `UploadHub-0.0.4/UploadHub.egg-info/PKG-INFO` & `UploadHub-0.0.5/UploadHub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UploadHub
-Version: 0.0.4
+Version: 0.0.5
 Summary: PYPI and GitHub package uploader.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `UploadHub-0.0.4/setup.py` & `UploadHub-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'PYPI and GitHub package uploader.'
 LONG_DESCRIPTION = 'Manages all the commands to upload a package to PYPI and GitHub repo.'
 
 setup(
     name='UploadHub',
     version=VERSION,
     author="Armando Chaparro",
```

