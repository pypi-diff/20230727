# Comparing `tmp/dimtown_spider-0.0.1.tar.gz` & `tmp/dimtown_spider-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimtown_spider-0.0.1.tar", max compression
+gzip compressed data, was "dimtown_spider-0.0.2.tar", max compression
```

## Comparing `dimtown_spider-0.0.1.tar` & `dimtown_spider-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/LICENSE
--rw-r--r--   0        0        0     1875 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/README.md
--rw-r--r--   0        0        0     1570 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/AnimeAvatar.py
--rw-r--r--   0        0        0     1124 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/ArtAlbum.py
--rw-r--r--   0        0        0      885 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/CoupleAvatar.py
--rw-r--r--   0        0        0     1049 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/FemaleAvatar.py
--rw-r--r--   0        0        0      978 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/Figure.py
--rw-r--r--   0        0        0     1058 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/MaleAvatar.py
--rw-r--r--   0        0        0     1346 2023-07-27 07:19:28.942220 dimtown_spider-0.0.1/dimtown/SelectedIllustrations.py
--rw-r--r--   0        0        0     1299 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/SelectedPixiv.py
--rw-r--r--   0        0        0      922 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/__init__.py
--rw-r--r--   0        0        0     1241 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/cosplay.py
--rw-r--r--   0        0        0     1073 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/hanfu.py
--rw-r--r--   0        0        0     1095 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/jk.py
--rw-r--r--   0        0        0     1292 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/lolita.py
--rw-r--r--   0        0        0     1502 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/pcpic.py
--rw-r--r--   0        0        0     1438 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/phonepic.py
--rw-r--r--   0        0        0     4208 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/dimtown/utils.py
--rw-r--r--   0        0        0      415 2023-07-27 07:19:28.946220 dimtown_spider-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 dimtown_spider-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1875 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/README.md
+-rw-r--r--   0        0        0     1570 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/AnimeAvatar.py
+-rw-r--r--   0        0        0     1124 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/ArtAlbum.py
+-rw-r--r--   0        0        0      885 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/CoupleAvatar.py
+-rw-r--r--   0        0        0     1049 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/FemaleAvatar.py
+-rw-r--r--   0        0        0      978 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/Figure.py
+-rw-r--r--   0        0        0     1058 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/MaleAvatar.py
+-rw-r--r--   0        0        0     1346 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/SelectedIllustrations.py
+-rw-r--r--   0        0        0     1299 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/SelectedPixiv.py
+-rw-r--r--   0        0        0      922 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/__init__.py
+-rw-r--r--   0        0        0     1241 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/cosplay.py
+-rw-r--r--   0        0        0     1073 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/hanfu.py
+-rw-r--r--   0        0        0     1095 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/jk.py
+-rw-r--r--   0        0        0     1292 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/lolita.py
+-rw-r--r--   0        0        0     1502 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/pcpic.py
+-rw-r--r--   0        0        0     1438 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/phonepic.py
+-rw-r--r--   0        0        0     4208 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/dimtown/utils.py
+-rw-r--r--   0        0        0      399 2023-07-27 07:26:40.648284 dimtown_spider-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 dimtown_spider-0.0.2/PKG-INFO
```

### Comparing `dimtown_spider-0.0.1/LICENSE` & `dimtown_spider-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/README.md` & `dimtown_spider-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/AnimeAvatar.py` & `dimtown_spider-0.0.2/dimtown/AnimeAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/ArtAlbum.py` & `dimtown_spider-0.0.2/dimtown/ArtAlbum.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/CoupleAvatar.py` & `dimtown_spider-0.0.2/dimtown/CoupleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/FemaleAvatar.py` & `dimtown_spider-0.0.2/dimtown/FemaleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/Figure.py` & `dimtown_spider-0.0.2/dimtown/Figure.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/MaleAvatar.py` & `dimtown_spider-0.0.2/dimtown/MaleAvatar.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/SelectedIllustrations.py` & `dimtown_spider-0.0.2/dimtown/SelectedIllustrations.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/SelectedPixiv.py` & `dimtown_spider-0.0.2/dimtown/SelectedPixiv.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/__init__.py` & `dimtown_spider-0.0.2/dimtown/__init__.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/cosplay.py` & `dimtown_spider-0.0.2/dimtown/cosplay.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/hanfu.py` & `dimtown_spider-0.0.2/dimtown/hanfu.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/jk.py` & `dimtown_spider-0.0.2/dimtown/jk.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/lolita.py` & `dimtown_spider-0.0.2/dimtown/lolita.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/pcpic.py` & `dimtown_spider-0.0.2/dimtown/pcpic.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/phonepic.py` & `dimtown_spider-0.0.2/dimtown/phonepic.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/dimtown/utils.py` & `dimtown_spider-0.0.2/dimtown/utils.py`

 * *Files identical despite different names*

### Comparing `dimtown_spider-0.0.1/PKG-INFO` & `dimtown_spider-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dimtown-spider
-Version: 0.0.1
+Version: 0.0.2
 Summary: A spider for https://dimtown.com
 Author: divandia
 Author-email: 106718176+Cvandia@users.noreply.github.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bs4 (>=3.2.2,<4.0.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: ujson (>=5.4.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <a href="https://dimtown.com"><img src="./ico/ico.png" width="180" alt="Logo"></a>
```

