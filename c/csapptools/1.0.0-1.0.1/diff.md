# Comparing `tmp/csapptools-1.0.0.tar.gz` & `tmp/csapptools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csapptools-1.0.0.tar", last modified: Wed Jul 26 04:39:35 2023, max compression
+gzip compressed data, was "csapptools-1.0.1.tar", last modified: Thu Jul 27 03:07:25 2023, max compression
```

## Comparing `csapptools-1.0.0.tar` & `csapptools-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 04:39:35.795096 csapptools-1.0.0/
--rw-rw-rw-   0        0        0     1074 2023-07-26 04:38:28.000000 csapptools-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1272 2023-07-26 04:39:35.795096 csapptools-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-07-26 03:57:07.000000 csapptools-1.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-26 04:36:20.000000 csapptools-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-07-26 04:39:35.797095 csapptools-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 04:39:35.746095 csapptools-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 04:39:35.775095 csapptools-1.0.0/src/csapptools/
--rw-rw-rw-   0        0        0       70 2023-07-26 03:35:25.000000 csapptools-1.0.0/src/csapptools/__init__.py
--rw-rw-rw-   0        0        0     4265 2023-07-26 03:35:11.000000 csapptools-1.0.0/src/csapptools/librariesiolib.py
--rw-rw-rw-   0        0        0     1287 2023-07-26 03:02:13.000000 csapptools-1.0.0/src/csapptools/pypilib.py
-drwxrwxrwx   0        0        0        0 2023-07-26 04:39:35.793096 csapptools-1.0.0/src/csapptools.egg-info/
--rw-rw-rw-   0        0        0     1272 2023-07-26 04:39:35.000000 csapptools-1.0.0/src/csapptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-26 04:39:35.000000 csapptools-1.0.0/src/csapptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 04:39:35.000000 csapptools-1.0.0/src/csapptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 04:39:35.000000 csapptools-1.0.0/src/csapptools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 03:07:25.050093 csapptools-1.0.1/
+-rw-rw-rw-   0        0        0     1074 2023-07-26 04:38:28.000000 csapptools-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1272 2023-07-27 03:07:25.050093 csapptools-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-07-26 03:57:07.000000 csapptools-1.0.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-26 04:36:20.000000 csapptools-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      707 2023-07-27 03:07:25.052094 csapptools-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-27 03:07:25.016094 csapptools-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-27 03:07:25.032094 csapptools-1.0.1/src/csapptools/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:53:57.000000 csapptools-1.0.1/src/csapptools/__init__.py
+-rw-rw-rw-   0        0        0     4265 2023-07-26 03:35:11.000000 csapptools-1.0.1/src/csapptools/librariesiolib.py
+-rw-rw-rw-   0        0        0     1287 2023-07-26 03:02:13.000000 csapptools-1.0.1/src/csapptools/pypilib.py
+drwxrwxrwx   0        0        0        0 2023-07-27 03:07:25.047093 csapptools-1.0.1/src/csapptools.egg-info/
+-rw-rw-rw-   0        0        0     1272 2023-07-27 03:07:24.000000 csapptools-1.0.1/src/csapptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-27 03:07:25.000000 csapptools-1.0.1/src/csapptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 03:07:24.000000 csapptools-1.0.1/src/csapptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-27 03:07:24.000000 csapptools-1.0.1/src/csapptools.egg-info/top_level.txt
```

### Comparing `csapptools-1.0.0/LICENSE.txt` & `csapptools-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csapptools-1.0.0/PKG-INFO` & `csapptools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csapptools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scraping tools for https://github.com/adamcysec/CSAPP
 Home-page: https://github.com/adamcysec/csapptools
 Author: adamcysec
 Project-URL: repository, https://github.com/adamcysec/csapptools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `csapptools-1.0.0/README.md` & `csapptools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `csapptools-1.0.0/setup.cfg` & `csapptools-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 7361 7070 746f 6f6c 730d 0a76   = csapptools..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e30 0d0a  ersion = 1.0.0..
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
 00000030: 6175 7468 6f72 203d 2061 6461 6d63 7973  author = adamcys
 00000040: 6563 0d0a 6465 7363 7269 7074 696f 6e20  ec..description 
 00000050: 3d20 5363 7261 7069 6e67 2074 6f6f 6c73  = Scraping tools
 00000060: 2066 6f72 2068 7474 7073 3a2f 2f67 6974   for https://git
 00000070: 6875 622e 636f 6d2f 6164 616d 6379 7365  hub.com/adamcyse
 00000080: 632f 4353 4150 500d 0a6c 6f6e 675f 6465  c/CSAPP..long_de
 00000090: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
```

### Comparing `csapptools-1.0.0/src/csapptools/librariesiolib.py` & `csapptools-1.0.1/src/csapptools/librariesiolib.py`

 * *Files identical despite different names*

### Comparing `csapptools-1.0.0/src/csapptools/pypilib.py` & `csapptools-1.0.1/src/csapptools/pypilib.py`

 * *Files identical despite different names*

### Comparing `csapptools-1.0.0/src/csapptools.egg-info/PKG-INFO` & `csapptools-1.0.1/src/csapptools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csapptools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Scraping tools for https://github.com/adamcysec/CSAPP
 Home-page: https://github.com/adamcysec/csapptools
 Author: adamcysec
 Project-URL: repository, https://github.com/adamcysec/csapptools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

