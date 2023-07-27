# Comparing `tmp/interactivenlp-0.2.5.tar.gz` & `tmp/interactivenlp-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.2.5.tar", last modified: Thu Jul 27 02:45:41 2023, max compression
+gzip compressed data, was "interactivenlp-0.2.6.tar", last modified: Thu Jul 27 02:53:50 2023, max compression
```

## Comparing `interactivenlp-0.2.5.tar` & `interactivenlp-0.2.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.304805 interactivenlp-0.2.5/
--rw-r--r--   0 chunxuyang   (501) staff       (20)       75 2023-07-27 02:30:55.000000 interactivenlp-0.2.5/MANIFEST.in
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:45:41.304699 interactivenlp-0.2.5/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.5/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.300164 interactivenlp-0.2.5/interactivenlp/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      321 2023-07-27 02:41:52.000000 interactivenlp-0.2.5/interactivenlp/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.301324 interactivenlp-0.2.5/interactivenlp/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.5/interactivenlp/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6996 2023-07-27 02:42:06.000000 interactivenlp-0.2.5/interactivenlp/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      831 2023-07-27 02:42:09.000000 interactivenlp-0.2.5/interactivenlp/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.302473 interactivenlp-0.2.5/interactivenlp/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.5/interactivenlp/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      344 2023-07-27 02:42:20.000000 interactivenlp-0.2.5/interactivenlp/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.5/interactivenlp/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.5/interactivenlp/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.5/interactivenlp/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5263 2023-07-27 02:42:35.000000 interactivenlp-0.2.5/interactivenlp/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1047 2023-07-27 02:43:02.000000 interactivenlp-0.2.5/interactivenlp/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.299284 interactivenlp-0.2.5/interactivenlp/static/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.299329 interactivenlp-0.2.5/interactivenlp/static/dist/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.302961 interactivenlp-0.2.5/interactivenlp/static/dist/css/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      226 2023-07-24 20:39:17.000000 interactivenlp-0.2.5/interactivenlp/static/dist/css/custom.css
--rw-r--r--   0 chunxuyang   (501) staff       (20)    36102 2023-07-27 01:26:52.000000 interactivenlp-0.2.5/interactivenlp/static/dist/css/output.css
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.304072 interactivenlp-0.2.5/interactivenlp/templates/
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1113 2023-07-13 22:47:44.000000 interactivenlp-0.2.5/interactivenlp/templates/block.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)      891 2023-07-15 21:50:55.000000 interactivenlp-0.2.5/interactivenlp/templates/feed.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1276 2023-07-25 19:54:30.000000 interactivenlp-0.2.5/interactivenlp/templates/form.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1823 2023-07-25 20:02:34.000000 interactivenlp-0.2.5/interactivenlp/templates/reader.html
--rw-r--r--   0 chunxuyang   (501) staff       (20)      652 2023-07-15 21:51:07.000000 interactivenlp-0.2.5/interactivenlp/templates/rss.html
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.304296 interactivenlp-0.2.5/interactivenlp/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.5/interactivenlp/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2532 2023-07-27 02:42:49.000000 interactivenlp-0.2.5/interactivenlp/types/model.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.304519 interactivenlp-0.2.5/interactivenlp/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.5/interactivenlp/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      633 2023-07-27 02:41:39.000000 interactivenlp-0.2.5/interactivenlp/utils/extraction.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:45:41.300927 interactivenlp-0.2.5/interactivenlp.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:45:41.000000 interactivenlp-0.2.5/interactivenlp.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      982 2023-07-27 02:45:41.000000 interactivenlp-0.2.5/interactivenlp.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 02:45:41.000000 interactivenlp-0.2.5/interactivenlp.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 02:45:41.000000 interactivenlp-0.2.5/interactivenlp.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 02:45:41.000000 interactivenlp-0.2.5/interactivenlp.egg-info/top_level.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 02:45:41.304848 interactivenlp-0.2.5/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1323 2023-07-27 02:45:36.000000 interactivenlp-0.2.5/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.225130 interactivenlp-0.2.6/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       75 2023-07-27 02:30:55.000000 interactivenlp-0.2.6/MANIFEST.in
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:53:50.225018 interactivenlp-0.2.6/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.6/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.221933 interactivenlp-0.2.6/interactivenlp/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      237 2023-07-27 02:48:17.000000 interactivenlp-0.2.6/interactivenlp/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.222916 interactivenlp-0.2.6/interactivenlp/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.6/interactivenlp/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6944 2023-07-27 02:49:58.000000 interactivenlp-0.2.6/interactivenlp/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      818 2023-07-27 02:50:10.000000 interactivenlp-0.2.6/interactivenlp/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.223641 interactivenlp-0.2.6/interactivenlp/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.6/interactivenlp/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      331 2023-07-27 02:48:32.000000 interactivenlp-0.2.6/interactivenlp/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.6/interactivenlp/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.6/interactivenlp/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.6/interactivenlp/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5229 2023-07-27 02:49:58.000000 interactivenlp-0.2.6/interactivenlp/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1047 2023-07-27 02:43:02.000000 interactivenlp-0.2.6/interactivenlp/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.220880 interactivenlp-0.2.6/interactivenlp/static/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.220933 interactivenlp-0.2.6/interactivenlp/static/dist/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.223866 interactivenlp-0.2.6/interactivenlp/static/dist/css/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      226 2023-07-24 20:39:17.000000 interactivenlp-0.2.6/interactivenlp/static/dist/css/custom.css
+-rw-r--r--   0 chunxuyang   (501) staff       (20)    36102 2023-07-27 01:26:52.000000 interactivenlp-0.2.6/interactivenlp/static/dist/css/output.css
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.224459 interactivenlp-0.2.6/interactivenlp/templates/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1113 2023-07-13 22:47:44.000000 interactivenlp-0.2.6/interactivenlp/templates/block.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      891 2023-07-15 21:50:55.000000 interactivenlp-0.2.6/interactivenlp/templates/feed.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1276 2023-07-25 19:54:30.000000 interactivenlp-0.2.6/interactivenlp/templates/form.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1823 2023-07-25 20:02:34.000000 interactivenlp-0.2.6/interactivenlp/templates/reader.html
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      652 2023-07-15 21:51:07.000000 interactivenlp-0.2.6/interactivenlp/templates/rss.html
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.224659 interactivenlp-0.2.6/interactivenlp/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.6/interactivenlp/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 02:48:59.000000 interactivenlp-0.2.6/interactivenlp/types/model.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.224856 interactivenlp-0.2.6/interactivenlp/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.6/interactivenlp/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      607 2023-07-27 02:50:35.000000 interactivenlp-0.2.6/interactivenlp/utils/extraction.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 02:53:50.222540 interactivenlp-0.2.6/interactivenlp.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 02:53:50.000000 interactivenlp-0.2.6/interactivenlp.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      982 2023-07-27 02:53:50.000000 interactivenlp-0.2.6/interactivenlp.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 02:53:50.000000 interactivenlp-0.2.6/interactivenlp.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 02:53:50.000000 interactivenlp-0.2.6/interactivenlp.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 02:53:50.000000 interactivenlp-0.2.6/interactivenlp.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 02:53:50.225170 interactivenlp-0.2.6/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1323 2023-07-27 02:53:47.000000 interactivenlp-0.2.6/setup.py
```

### Comparing `interactivenlp-0.2.5/interactivenlp/controllers/reader_controller.py` & `interactivenlp-0.2.6/interactivenlp/controllers/reader_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import urllib.parse
 from collections import defaultdict
 from typing import List, DefaultDict
 
 from flask import Blueprint, render_template, request, current_app, redirect
 
-from interactivenlp.models.article import Article
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

### Comparing `interactivenlp-0.2.5/interactivenlp/controllers/rss_controller.py` & `interactivenlp-0.2.6/interactivenlp/controllers/rss_controller.py`

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

### Comparing `interactivenlp-0.2.5/interactivenlp/models/block.py` & `interactivenlp-0.2.6/interactivenlp/models/block.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/models/form.py` & `interactivenlp-0.2.6/interactivenlp/models/form.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/models/task.py` & `interactivenlp-0.2.6/interactivenlp/models/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional
 
 import nltk
 
-from interactivenlp.models.block import Block, BlockLevelEnum, BlockTypeEnum, BlockStatusEnum
-from interactivenlp.types.model import ModelConfiguration, InteractiveTaskType, InteractiveFunctionType, InteractiveRssType, \
+from .block import Block, BlockLevelEnum, BlockTypeEnum, BlockStatusEnum
+from ..types.model import ModelConfiguration, InteractiveTaskType, InteractiveFunctionType, InteractiveRssType, \
     InteractiveFunctionResultType, CompositionType
 
 try:
     nltk.data.find('tokenizers/punkt')
 except LookupError:
     nltk.download('punkt')
```

### Comparing `interactivenlp-0.2.5/interactivenlp/server.py` & `interactivenlp-0.2.6/interactivenlp/server.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/static/dist/css/output.css` & `interactivenlp-0.2.6/interactivenlp/static/dist/css/output.css`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/templates/block.html` & `interactivenlp-0.2.6/interactivenlp/templates/block.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/templates/feed.html` & `interactivenlp-0.2.6/interactivenlp/templates/feed.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/templates/form.html` & `interactivenlp-0.2.6/interactivenlp/templates/form.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/templates/reader.html` & `interactivenlp-0.2.6/interactivenlp/templates/reader.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/templates/rss.html` & `interactivenlp-0.2.6/interactivenlp/templates/rss.html`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/interactivenlp/types/model.py` & `interactivenlp-0.2.6/interactivenlp/types/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Callable, List, TypedDict, Optional
 from typing_extensions import NotRequired
 
-from interactivenlp.models.block import Block
+from ..models.block import Block
 import itertools
 
-from interactivenlp.models.form import Form
+from ..models.form import Form
 
 # composition type: parallel, exclusive
 CompositionType = Enum("parallel", "exclusive")
 
 
 class InteractiveRssType:
     def __init__(self, article: str, url: str, paragraphs: list[Block]):
```

### Comparing `interactivenlp-0.2.5/interactivenlp.egg-info/SOURCES.txt` & `interactivenlp-0.2.6/interactivenlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.5/setup.py` & `interactivenlp-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 print(find_packages(
     exclude=["examples", "tests"],
 ))
 
 
 setup(
     name='interactivenlp',
-    version='0.2.5',
+    version='0.2.6',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     # include_package_data=True,
     packages=["interactivenlp"],
     package_dir={
```

