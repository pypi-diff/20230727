# Comparing `tmp/bkapi-plugins-py-0.7272.tar.gz` & `tmp/bkapi-plugins-py-0.7273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkapi-plugins-py-0.7272.tar", last modified: Thu Jul 27 12:00:34 2023, max compression
+gzip compressed data, was "bkapi-plugins-py-0.7273.tar", last modified: Thu Jul 27 12:26:15 2023, max compression
```

## Comparing `bkapi-plugins-py-0.7272.tar` & `bkapi-plugins-py-0.7273.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 12:00:34.403160 bkapi-plugins-py-0.7272/
--rw-rw-rw-   0        0        0       39 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.7272/MANIFEST.in
--rw-rw-rw-   0        0        0      188 2023-07-27 12:00:34.403160 bkapi-plugins-py-0.7272/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 12:00:34.390407 bkapi-plugins-py-0.7272/bkapi_plugins/
--rw-rw-rw-   0        0        0      172 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.7272/bkapi_plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-27 12:00:34.398339 bkapi-plugins-py-0.7272/bkapi_plugins/files/
--rw-rw-rw-   0        0        0      982 2023-07-27 11:50:28.000000 bkapi-plugins-py-0.7272/bkapi_plugins/files/docker-compose.yaml
--rw-rw-rw-   0        0        0  4193368 2023-07-27 11:55:52.000000 bkapi-plugins-py-0.7272/bkapi_plugins/files/redash-master.zip
--rw-rw-rw-   0        0        0    10384 2023-07-27 11:54:45.000000 bkapi-plugins-py-0.7272/bkapi_plugins/files/setup-master.zip
-drwxrwxrwx   0        0        0        0 2023-07-27 12:00:34.402393 bkapi-plugins-py-0.7272/bkapi_plugins_py.egg-info/
--rw-rw-rw-   0        0        0      188 2023-07-27 12:00:34.000000 bkapi-plugins-py-0.7272/bkapi_plugins_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-07-27 12:00:34.000000 bkapi-plugins-py-0.7272/bkapi_plugins_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 12:00:34.000000 bkapi-plugins-py-0.7272/bkapi_plugins_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-27 12:00:34.000000 bkapi-plugins-py-0.7272/bkapi_plugins_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 12:00:34.403160 bkapi-plugins-py-0.7272/setup.cfg
--rw-rw-rw-   0        0        0      891 2023-07-27 11:57:32.000000 bkapi-plugins-py-0.7272/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:26:15.009189 bkapi-plugins-py-0.7273/
+-rw-rw-rw-   0        0        0       39 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.7273/MANIFEST.in
+-rw-rw-rw-   0        0        0      188 2023-07-27 12:26:15.010267 bkapi-plugins-py-0.7273/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 12:26:15.003189 bkapi-plugins-py-0.7273/bkapi_plugins/
+-rw-rw-rw-   0        0        0      172 2023-07-27 00:30:58.000000 bkapi-plugins-py-0.7273/bkapi_plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 12:26:15.005196 bkapi-plugins-py-0.7273/bkapi_plugins/files/
+-rw-rw-rw-   0        0        0      534 2023-07-27 12:26:09.000000 bkapi-plugins-py-0.7273/bkapi_plugins/files/docker-compose.yaml
+drwxrwxrwx   0        0        0        0 2023-07-27 12:26:15.009189 bkapi-plugins-py-0.7273/bkapi_plugins_py.egg-info/
+-rw-rw-rw-   0        0        0      188 2023-07-27 12:26:14.000000 bkapi-plugins-py-0.7273/bkapi_plugins_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-07-27 12:26:14.000000 bkapi-plugins-py-0.7273/bkapi_plugins_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 12:26:14.000000 bkapi-plugins-py-0.7273/bkapi_plugins_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 12:26:14.000000 bkapi-plugins-py-0.7273/bkapi_plugins_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 12:26:15.010438 bkapi-plugins-py-0.7273/setup.cfg
+-rw-rw-rw-   0        0        0      891 2023-07-27 12:26:09.000000 bkapi-plugins-py-0.7273/setup.py
```

### Comparing `bkapi-plugins-py-0.7272/setup.py` & `bkapi-plugins-py-0.7273/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = ''
 
 setup(
     description='',
     long_description=readme,
     name='bkapi-plugins-py', # 包的名字
-    version='0.7272', # 版本号每次打包完要改一下
+    version='0.7273', # 版本号每次打包完要改一下
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*',
     author='fadewalk',
     license='Apach License 2.0',
     # packages=find_packages(),
     # namespace_packages=['bkapi_plugins'],
     package_dir={'': '.'},
     include_package_data=True,
```

