# Comparing `tmp/usolitaire-1.0.0.tar.gz` & `tmp/usolitaire-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usolitaire-1.0.0.tar", last modified: Thu Jul 27 12:37:07 2023, max compression
+gzip compressed data, was "usolitaire-1.0.1.tar", last modified: Thu Jul 27 12:53:39 2023, max compression
```

## Comparing `usolitaire-1.0.0.tar` & `usolitaire-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.405153 usolitaire-1.0.0/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.0/LICENSE
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:37:07.405153 usolitaire-1.0.0/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.0/README.rst
--rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.0/pyproject.toml
--rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-27 12:37:07.405153 usolitaire-1.0.0/setup.cfg
--rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-27 12:19:12.000000 usolitaire-1.0.0/setup.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.401153 usolitaire-1.0.0/usolitaire/
--rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-27 12:19:12.000000 usolitaire-1.0.0/usolitaire/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)    12253 2023-07-27 12:15:26.000000 usolitaire-1.0.0/usolitaire/app.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 12:14:41.000000 usolitaire-1.0.0/usolitaire/card_render.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.0/usolitaire/game.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 12:14:41.000000 usolitaire-1.0.0/usolitaire/textual_ui.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.405153 usolitaire-1.0.0/usolitaire.egg-info/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)      402 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/SOURCES.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/dependency_links.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/entry_points.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/not-zip-safe
--rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/requires.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/top_level.txt
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:53:39.638230 usolitaire-1.0.1/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.1/LICENSE
+-rw-rw-r--   0 elias     (1000) elias     (1000)      105 2023-07-27 12:52:48.000000 usolitaire-1.0.1/MANIFEST.in
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:53:39.638230 usolitaire-1.0.1/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.1/README.rst
+-rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.1/pyproject.toml
+-rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-27 12:53:39.638230 usolitaire-1.0.1/setup.cfg
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-27 12:53:21.000000 usolitaire-1.0.1/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:53:39.638230 usolitaire-1.0.1/usolitaire/
+-rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-27 12:53:21.000000 usolitaire-1.0.1/usolitaire/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    12253 2023-07-27 12:15:26.000000 usolitaire-1.0.1/usolitaire/app.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 12:14:41.000000 usolitaire-1.0.1/usolitaire/card_render.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.1/usolitaire/game.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      775 2023-07-27 12:15:26.000000 usolitaire-1.0.1/usolitaire/textual_app.css
+-rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 12:14:41.000000 usolitaire-1.0.1/usolitaire/textual_ui.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:53:39.638230 usolitaire-1.0.1/usolitaire.egg-info/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)      441 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/SOURCES.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/dependency_links.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/entry_points.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/not-zip-safe
+-rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/requires.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-27 12:53:39.000000 usolitaire-1.0.1/usolitaire.egg-info/top_level.txt
```

### Comparing `usolitaire-1.0.0/LICENSE` & `usolitaire-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/PKG-INFO` & `usolitaire-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.0
+Version: 1.0.1
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `usolitaire-1.0.0/README.rst` & `usolitaire-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/setup.py` & `usolitaire-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 requirements = [
     "textual",
 ]
 
 setup(
     name="usolitaire",
-    version="1.0.0",
+    version="1.0.1",
     description="Solitaire in your terminal",
     long_description=readme,
     author="Elias Dorneles",
     author_email="eliasdorneles@gmail.com",
     url="https://github.com/eliasdorneles/usolitaire",
     entry_points={
         "console_scripts": {
```

### Comparing `usolitaire-1.0.0/usolitaire/app.py` & `usolitaire-1.0.1/usolitaire/app.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/usolitaire/card_render.py` & `usolitaire-1.0.1/usolitaire/card_render.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/usolitaire/game.py` & `usolitaire-1.0.1/usolitaire/game.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/usolitaire/textual_ui.py` & `usolitaire-1.0.1/usolitaire/textual_ui.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.0/usolitaire.egg-info/PKG-INFO` & `usolitaire-1.0.1/usolitaire.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.0
+Version: 1.0.1
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

