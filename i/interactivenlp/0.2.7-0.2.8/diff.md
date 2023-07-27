# Comparing `tmp/interactivenlp-0.2.7.tar.gz` & `tmp/interactivenlp-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.2.7.tar", last modified: Thu Jul 27 21:10:55 2023, max compression
+gzip compressed data, was "interactivenlp-0.2.8.tar", last modified: Thu Jul 27 21:14:47 2023, max compression
```

## Comparing `interactivenlp-0.2.7.tar` & `interactivenlp-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.525257 interactivenlp-0.2.7/
--rw-r--r--   0 chunxuyang   (501) staff       (20)       75 2023-07-27 02:30:55.000000 interactivenlp-0.2.7/MANIFEST.in
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 21:10:55.525114 interactivenlp-0.2.7/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.7/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.516856 interactivenlp-0.2.7/interactivenlp/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      237 2023-07-27 02:48:17.000000 interactivenlp-0.2.7/interactivenlp/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.518888 interactivenlp-0.2.7/interactivenlp/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.7/interactivenlp/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6944 2023-07-27 02:49:58.000000 interactivenlp-0.2.7/interactivenlp/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 02:50:10.000000 interactivenlp-0.2.7/interactivenlp/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.520817 interactivenlp-0.2.7/interactivenlp/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.7/interactivenlp/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      331 2023-07-27 02:48:32.000000 interactivenlp-0.2.7/interactivenlp/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.7/interactivenlp/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.7/interactivenlp/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.7/interactivenlp/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5229 2023-07-27 02:49:58.000000 interactivenlp-0.2.7/interactivenlp/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-27 02:56:04.000000 interactivenlp-0.2.7/interactivenlp/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.515832 interactivenlp-0.2.7/interactivenlp/static/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.515875 interactivenlp-0.2.7/interactivenlp/static/dist/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.521659 interactivenlp-0.2.7/interactivenlp/static/dist/css/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      226 2023-07-24 20:39:17.000000 interactivenlp-0.2.7/interactivenlp/static/dist/css/custom.css
--rw-r--r--   0 chunxuyang   (501) staff       (20)    36102 2023-07-27 01:26:52.000000 interactivenlp-0.2.7/interactivenlp/static/dist/css/output.css
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.523630 interactivenlp-0.2.7/interactivenlp/templates/
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1113 2023-07-13 22:47:44.000000 interactivenlp-0.2.7/interactivenlp/templates/block.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)      891 2023-07-15 21:50:55.000000 interactivenlp-0.2.7/interactivenlp/templates/feed.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1276 2023-07-25 19:54:30.000000 interactivenlp-0.2.7/interactivenlp/templates/form.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1823 2023-07-25 20:02:34.000000 interactivenlp-0.2.7/interactivenlp/templates/reader.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)      652 2023-07-15 21:51:07.000000 interactivenlp-0.2.7/interactivenlp/templates/rss.html
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.524381 interactivenlp-0.2.7/interactivenlp/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.7/interactivenlp/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 02:48:59.000000 interactivenlp-0.2.7/interactivenlp/types/model.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.524795 interactivenlp-0.2.7/interactivenlp/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.7/interactivenlp/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 02:50:35.000000 interactivenlp-0.2.7/interactivenlp/utils/extraction.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:10:55.518164 interactivenlp-0.2.7/interactivenlp.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 21:10:55.000000 interactivenlp-0.2.7/interactivenlp.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      982 2023-07-27 21:10:55.000000 interactivenlp-0.2.7/interactivenlp.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 21:10:55.000000 interactivenlp-0.2.7/interactivenlp.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 21:10:55.000000 interactivenlp-0.2.7/interactivenlp.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 21:10:55.000000 interactivenlp-0.2.7/interactivenlp.egg-info/top_level.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 21:10:55.525298 interactivenlp-0.2.7/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1151 2023-07-27 21:10:52.000000 interactivenlp-0.2.7/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.816079 interactivenlp-0.2.8/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 21:14:47.815975 interactivenlp-0.2.8/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.8/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.809456 interactivenlp-0.2.8/interactivenlp/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      237 2023-07-27 02:48:17.000000 interactivenlp-0.2.8/interactivenlp/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.810760 interactivenlp-0.2.8/interactivenlp/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.8/interactivenlp/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6944 2023-07-27 02:49:58.000000 interactivenlp-0.2.8/interactivenlp/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 02:50:10.000000 interactivenlp-0.2.8/interactivenlp/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.812408 interactivenlp-0.2.8/interactivenlp/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.8/interactivenlp/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      331 2023-07-27 02:48:32.000000 interactivenlp-0.2.8/interactivenlp/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.8/interactivenlp/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.8/interactivenlp/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.8/interactivenlp/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5229 2023-07-27 02:49:58.000000 interactivenlp-0.2.8/interactivenlp/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-27 02:56:04.000000 interactivenlp-0.2.8/interactivenlp/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.808618 interactivenlp-0.2.8/interactivenlp/static/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.808666 interactivenlp-0.2.8/interactivenlp/static/dist/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.812995 interactivenlp-0.2.8/interactivenlp/static/dist/css/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      226 2023-07-24 20:39:17.000000 interactivenlp-0.2.8/interactivenlp/static/dist/css/custom.css
+-rw-r--r--   0 chunxuyang   (501) staff       (20)    36102 2023-07-27 01:26:52.000000 interactivenlp-0.2.8/interactivenlp/static/dist/css/output.css
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.814556 interactivenlp-0.2.8/interactivenlp/templates/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1113 2023-07-13 22:47:44.000000 interactivenlp-0.2.8/interactivenlp/templates/block.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      891 2023-07-15 21:50:55.000000 interactivenlp-0.2.8/interactivenlp/templates/feed.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1276 2023-07-25 19:54:30.000000 interactivenlp-0.2.8/interactivenlp/templates/form.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1823 2023-07-25 20:02:34.000000 interactivenlp-0.2.8/interactivenlp/templates/reader.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      652 2023-07-15 21:51:07.000000 interactivenlp-0.2.8/interactivenlp/templates/rss.html
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.815320 interactivenlp-0.2.8/interactivenlp/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.8/interactivenlp/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 02:48:59.000000 interactivenlp-0.2.8/interactivenlp/types/model.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.815725 interactivenlp-0.2.8/interactivenlp/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.8/interactivenlp/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 02:50:35.000000 interactivenlp-0.2.8/interactivenlp/utils/extraction.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 21:14:47.810204 interactivenlp-0.2.8/interactivenlp.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 21:14:47.000000 interactivenlp-0.2.8/interactivenlp.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      970 2023-07-27 21:14:47.000000 interactivenlp-0.2.8/interactivenlp.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 21:14:47.000000 interactivenlp-0.2.8/interactivenlp.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 21:14:47.000000 interactivenlp-0.2.8/interactivenlp.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 21:14:47.000000 interactivenlp-0.2.8/interactivenlp.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 21:14:47.816119 interactivenlp-0.2.8/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1277 2023-07-27 21:14:26.000000 interactivenlp-0.2.8/setup.py
```

### Comparing `interactivenlp-0.2.7/interactivenlp/controllers/reader_controller.py` & `interactivenlp-0.2.8/interactivenlp/controllers/reader_controller.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/controllers/rss_controller.py` & `interactivenlp-0.2.8/interactivenlp/controllers/rss_controller.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/models/block.py` & `interactivenlp-0.2.8/interactivenlp/models/block.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/models/form.py` & `interactivenlp-0.2.8/interactivenlp/models/form.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/models/task.py` & `interactivenlp-0.2.8/interactivenlp/models/task.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/server.py` & `interactivenlp-0.2.8/interactivenlp/server.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/static/dist/css/output.css` & `interactivenlp-0.2.8/interactivenlp/static/dist/css/output.css`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/templates/block.html` & `interactivenlp-0.2.8/interactivenlp/templates/block.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/templates/feed.html` & `interactivenlp-0.2.8/interactivenlp/templates/feed.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/templates/form.html` & `interactivenlp-0.2.8/interactivenlp/templates/form.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/templates/reader.html` & `interactivenlp-0.2.8/interactivenlp/templates/reader.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/templates/rss.html` & `interactivenlp-0.2.8/interactivenlp/templates/rss.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/types/model.py` & `interactivenlp-0.2.8/interactivenlp/types/model.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp/utils/extraction.py` & `interactivenlp-0.2.8/interactivenlp/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.7/interactivenlp.egg-info/SOURCES.txt` & `interactivenlp-0.2.8/interactivenlp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-MANIFEST.in
 README.md
 setup.py
 interactivenlp/__init__.py
 interactivenlp/server.py
 interactivenlp.egg-info/PKG-INFO
 interactivenlp.egg-info/SOURCES.txt
 interactivenlp.egg-info/dependency_links.txt
```

### Comparing `interactivenlp-0.2.7/setup.py` & `interactivenlp-0.2.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,23 +19,27 @@
 print(find_packages(
     exclude=["examples", "tests"],
 ))
 
 
 setup(
     name='interactivenlp',
-    version='0.2.7',
+    version='0.2.8',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     # include_package_data=True,
     packages=find_packages(
         exclude=["examples", "tests"],
     ),
+    package_data={
+        'templates': ["interactivenlp/templates/*"],
+        'static': ["interactivenlp/static/*"],
+    },
     zipSafe=False,
     install_requires=[
         'flask',
         'flask-cors',
         'newspaper3k',
         'nltk',
         'feedparser',
```

