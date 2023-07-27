# Comparing `tmp/interactivenlp-0.2.3.tar.gz` & `tmp/interactivenlp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.2.3.tar", last modified: Thu Jul 27 00:20:37 2023, max compression
+gzip compressed data, was "interactivenlp-0.2.4.tar", last modified: Thu Jul 27 02:31:01 2023, max compression
```

## Comparing `interactivenlp-0.2.3.tar` & `interactivenlp-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.956711 interactivenlp-0.2.3/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.952870 interactivenlp-0.2.3/InteractiveNLP.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 00:20:37.000000 interactivenlp-0.2.3/InteractiveNLP.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      929 2023-07-27 00:20:37.000000 interactivenlp-0.2.3/InteractiveNLP.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 00:20:37.000000 interactivenlp-0.2.3/InteractiveNLP.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 00:20:37.000000 interactivenlp-0.2.3/InteractiveNLP.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 00:20:37.000000 interactivenlp-0.2.3/InteractiveNLP.egg-info/top_level.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 00:20:37.956603 interactivenlp-0.2.3/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.953232 interactivenlp-0.2.3/interactivenlp/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      243 2023-07-27 00:06:13.000000 interactivenlp-0.2.3/interactivenlp/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.954170 interactivenlp-0.2.3/interactivenlp/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6981 2023-07-25 19:46:01.000000 interactivenlp-0.2.3/interactivenlp/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      831 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.955467 interactivenlp-0.2.3/interactivenlp/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      323 2023-07-27 00:08:58.000000 interactivenlp-0.2.3/interactivenlp/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.3/interactivenlp/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.3/interactivenlp/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.3/interactivenlp/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5237 2023-07-27 00:09:23.000000 interactivenlp-0.2.3/interactivenlp/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-24 19:17:35.000000 interactivenlp-0.2.3/interactivenlp/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.956043 interactivenlp-0.2.3/interactivenlp/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 00:08:26.000000 interactivenlp-0.2.3/interactivenlp/types/model.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 interactivenlp-0.2.3/interactivenlp/types/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:20:37.956343 interactivenlp-0.2.3/interactivenlp/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      633 2023-07-11 20:32:46.000000 interactivenlp-0.2.3/interactivenlp/utils/extraction.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 00:20:37.956753 interactivenlp-0.2.3/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1068 2023-07-27 00:20:33.000000 interactivenlp-0.2.3/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.856759 interactivenlp-0.2.4/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       75 2023-07-27 02:30:55.000000 interactivenlp-0.2.4/MANIFEST.in
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:31:01.856570 interactivenlp-0.2.4/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.4/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.849092 interactivenlp-0.2.4/interactivenlp/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      237 2023-07-27 00:26:51.000000 interactivenlp-0.2.4/interactivenlp/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.850456 interactivenlp-0.2.4/interactivenlp/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.4/interactivenlp/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6944 2023-07-27 01:26:15.000000 interactivenlp-0.2.4/interactivenlp/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 01:26:20.000000 interactivenlp-0.2.4/interactivenlp/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.851961 interactivenlp-0.2.4/interactivenlp/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.4/interactivenlp/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      323 2023-07-27 00:08:58.000000 interactivenlp-0.2.4/interactivenlp/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.4/interactivenlp/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.4/interactivenlp/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.4/interactivenlp/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5237 2023-07-27 00:09:23.000000 interactivenlp-0.2.4/interactivenlp/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-24 19:17:35.000000 interactivenlp-0.2.4/interactivenlp/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.848239 interactivenlp-0.2.4/interactivenlp/static/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.848281 interactivenlp-0.2.4/interactivenlp/static/dist/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.852839 interactivenlp-0.2.4/interactivenlp/static/dist/css/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      226 2023-07-24 20:39:17.000000 interactivenlp-0.2.4/interactivenlp/static/dist/css/custom.css
+-rw-r--r--   0 chunxuyang   (501) staff       (20)    36102 2023-07-27 01:26:52.000000 interactivenlp-0.2.4/interactivenlp/static/dist/css/output.css
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.854824 interactivenlp-0.2.4/interactivenlp/templates/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1113 2023-07-13 22:47:44.000000 interactivenlp-0.2.4/interactivenlp/templates/block.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      891 2023-07-15 21:50:55.000000 interactivenlp-0.2.4/interactivenlp/templates/feed.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1276 2023-07-25 19:54:30.000000 interactivenlp-0.2.4/interactivenlp/templates/form.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1823 2023-07-25 20:02:34.000000 interactivenlp-0.2.4/interactivenlp/templates/reader.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      652 2023-07-15 21:51:07.000000 interactivenlp-0.2.4/interactivenlp/templates/rss.html
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.855862 interactivenlp-0.2.4/interactivenlp/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.4/interactivenlp/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 00:08:26.000000 interactivenlp-0.2.4/interactivenlp/types/model.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.856234 interactivenlp-0.2.4/interactivenlp/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.4/interactivenlp/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      621 2023-07-27 00:26:51.000000 interactivenlp-0.2.4/interactivenlp/utils/extraction.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:31:01.849817 interactivenlp-0.2.4/interactivenlp.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:31:01.000000 interactivenlp-0.2.4/interactivenlp.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      982 2023-07-27 02:31:01.000000 interactivenlp-0.2.4/interactivenlp.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 02:31:01.000000 interactivenlp-0.2.4/interactivenlp.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 02:31:01.000000 interactivenlp-0.2.4/interactivenlp.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 02:31:01.000000 interactivenlp-0.2.4/interactivenlp.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 02:31:01.856804 interactivenlp-0.2.4/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1323 2023-07-27 02:21:43.000000 interactivenlp-0.2.4/setup.py
```

### Comparing `interactivenlp-0.2.3/interactivenlp/controllers/reader_controller.py` & `interactivenlp-0.2.4/interactivenlp/controllers/reader_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import urllib.parse
 from collections import defaultdict
 from typing import List, DefaultDict
 
 from flask import Blueprint, render_template, request, current_app, redirect
 
-from interactivenlp import Article
-from interactivenlp.models.block import BlockTypeEnum, BlockLevelEnum, BlockStatusEnum, Block
-from interactivenlp.types.model import ModelConfiguration, InteractiveFunctionType, InteractiveRssType
-from interactivenlp.utils.extraction import extract_url_to_article
+from ..models.article import Article
+from ..models.block import BlockTypeEnum, BlockLevelEnum, BlockStatusEnum, Block
+from ..types.model import ModelConfiguration, InteractiveFunctionType, InteractiveRssType
+from ..utils.extraction import extract_url_to_article
 
 reader_page = Blueprint('reader_page', __name__)
 
 function_results = {}
 
 function_forms = defaultdict(lambda: {})  # type: DefaultDict[str, dict]
```

### Comparing `interactivenlp-0.2.3/interactivenlp/controllers/rss_controller.py` & `interactivenlp-0.2.4/interactivenlp/controllers/rss_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import urllib.parse
 
 from flask import Blueprint, render_template
 
-from interactivenlp.models.rss import RSS_SOURCES, RSS
+from ..models.rss import RSS_SOURCES, RSS
 
 rss_page = Blueprint('rss_page', __name__)
 
 
 @rss_page.route('/')
 def rss_page_index():
     context = {
```

### Comparing `interactivenlp-0.2.3/interactivenlp/models/block.py` & `interactivenlp-0.2.4/interactivenlp/models/block.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.3/interactivenlp/models/form.py` & `interactivenlp-0.2.4/interactivenlp/models/form.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.3/interactivenlp/models/task.py` & `interactivenlp-0.2.4/interactivenlp/models/task.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.3/interactivenlp/server.py` & `interactivenlp-0.2.4/interactivenlp/server.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.3/interactivenlp/types/model.py` & `interactivenlp-0.2.4/interactivenlp/types/model.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.3/interactivenlp/utils/extraction.py` & `interactivenlp-0.2.4/interactivenlp/utils/extraction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import newspaper
 
-from interactivenlp.models.article import Article
-from interactivenlp.models.block import Block, BlockLevelEnum, BlockTypeEnum
+from packages.models.article import Article
+from packages.models.block import Block, BlockLevelEnum, BlockTypeEnum
 
 
 def extract_url(url):
     article = newspaper.Article(url)
     article.download()
     article.parse()
     return article
```

### Comparing `interactivenlp-0.2.3/setup.py` & `interactivenlp-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,34 +12,45 @@
         nltk.download('punkt')
         install.run(self)
 
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
+print(find_packages(
+    exclude=["examples", "tests"],
+))
+
+
 setup(
     name='interactivenlp',
-    version='0.2.3',
+    version='0.2.4',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
-    include_package_data=True,
+    # include_package_data=True,
+    packages=["interactivenlp"],
+    package_dir={
+        "interactivenlp": "interactivenlp"
+    },
+    package_data={
+        "interactivenlp": ["interactivenlp/templates/*"
+                           "interactivenlp/static/*"
+                           ]
+    },
     install_requires=[
         'flask',
         'flask-cors',
         'newspaper3k',
         'nltk',
         'feedparser',
         'pydantic',
     ],
     license='MIT',
-    packages=find_packages(
-        exclude=["examples", "tests"]
-    ),
     platforms=["all"],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     cmdclass={
         'install': PostInstallCommand,
```

