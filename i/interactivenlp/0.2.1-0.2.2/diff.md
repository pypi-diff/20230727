# Comparing `tmp/interactivenlp-0.2.1.tar.gz` & `tmp/interactivenlp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interactivenlp-0.2.1.tar", last modified: Wed Jul 26 23:57:48 2023, max compression
+gzip compressed data, was "interactivenlp-0.2.2.tar", last modified: Thu Jul 27 00:15:19 2023, max compression
```

## Comparing `interactivenlp-0.2.1.tar` & `interactivenlp-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.920287 interactivenlp-0.2.1/
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918061 interactivenlp-0.2.1/InteractiveNLP.egg-info/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)      929 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/SOURCES.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/dependency_links.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/requires.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-26 23:57:48.000000 interactivenlp-0.2.1/InteractiveNLP.egg-info/top_level.txt
--rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-26 23:57:48.920187 interactivenlp-0.2.1/PKG-INFO
--rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/README.md
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918271 interactivenlp-0.2.1/interactivenlp/
--rw-r--r--   0 chunxuyang   (501) staff       (20)      327 2023-07-13 19:35:24.000000 interactivenlp-0.2.1/interactivenlp/__init__.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.918815 interactivenlp-0.2.1/interactivenlp/controllers/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/controllers/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     6981 2023-07-25 19:46:01.000000 interactivenlp-0.2.1/interactivenlp/controllers/reader_controller.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      831 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/controllers/rss_controller.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.919515 interactivenlp-0.2.1/interactivenlp/models/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/models/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      344 2023-07-13 20:16:56.000000 interactivenlp-0.2.1/interactivenlp/models/article.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.1/interactivenlp/models/block.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.1/interactivenlp/models/form.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.1/interactivenlp/models/rss.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     5531 2023-07-25 19:46:01.000000 interactivenlp-0.2.1/interactivenlp/models/task.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-24 19:17:35.000000 interactivenlp-0.2.1/interactivenlp/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.919812 interactivenlp-0.2.1/interactivenlp/types/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/types/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)     2532 2023-07-25 19:46:09.000000 interactivenlp-0.2.1/interactivenlp/types/model.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 interactivenlp-0.2.1/interactivenlp/types/server.py
-drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-26 23:57:48.920004 interactivenlp-0.2.1/interactivenlp/utils/
--rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/utils/__init__.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)      633 2023-07-11 20:32:46.000000 interactivenlp-0.2.1/interactivenlp/utils/extraction.py
--rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-26 23:57:48.920329 interactivenlp-0.2.1/setup.cfg
--rw-r--r--   0 chunxuyang   (501) staff       (20)     1037 2023-07-26 23:57:46.000000 interactivenlp-0.2.1/setup.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.637113 interactivenlp-0.2.2/
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.632659 interactivenlp-0.2.2/InteractiveNLP.egg-info/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 00:15:19.000000 interactivenlp-0.2.2/InteractiveNLP.egg-info/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      929 2023-07-27 00:15:19.000000 interactivenlp-0.2.2/InteractiveNLP.egg-info/SOURCES.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-27 00:15:19.000000 interactivenlp-0.2.2/InteractiveNLP.egg-info/dependency_links.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       54 2023-07-27 00:15:19.000000 interactivenlp-0.2.2/InteractiveNLP.egg-info/requires.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       15 2023-07-27 00:15:19.000000 interactivenlp-0.2.2/InteractiveNLP.egg-info/top_level.txt
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      322 2023-07-27 00:15:19.636981 interactivenlp-0.2.2/PKG-INFO
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       62 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/README.md
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.633073 interactivenlp-0.2.2/interactivenlp/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      243 2023-07-27 00:06:13.000000 interactivenlp-0.2.2/interactivenlp/__init__.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.634129 interactivenlp-0.2.2/interactivenlp/controllers/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/controllers/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     6981 2023-07-25 19:46:01.000000 interactivenlp-0.2.2/interactivenlp/controllers/reader_controller.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      831 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/controllers/rss_controller.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.635749 interactivenlp-0.2.2/interactivenlp/models/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/models/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      323 2023-07-27 00:08:58.000000 interactivenlp-0.2.2/interactivenlp/models/article.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2041 2023-07-24 20:16:58.000000 interactivenlp-0.2.2/interactivenlp/models/block.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      868 2023-07-24 23:42:14.000000 interactivenlp-0.2.2/interactivenlp/models/form.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      314 2023-07-24 19:14:33.000000 interactivenlp-0.2.2/interactivenlp/models/rss.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     5237 2023-07-27 00:09:23.000000 interactivenlp-0.2.2/interactivenlp/models/task.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1005 2023-07-24 19:17:35.000000 interactivenlp-0.2.2/interactivenlp/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.636340 interactivenlp-0.2.2/interactivenlp/types/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/types/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     2506 2023-07-27 00:08:26.000000 interactivenlp-0.2.2/interactivenlp/types/model.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        1 2023-07-17 20:45:05.000000 interactivenlp-0.2.2/interactivenlp/types/server.py
+drwxr-xr-x   0 chunxuyang   (501) staff       (20)        0 2023-07-27 00:15:19.636656 interactivenlp-0.2.2/interactivenlp/utils/
+-rw-r--r--   0 chunxuyang   (501) staff       (20)        0 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/utils/__init__.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)      633 2023-07-11 20:32:46.000000 interactivenlp-0.2.2/interactivenlp/utils/extraction.py
+-rw-r--r--   0 chunxuyang   (501) staff       (20)       38 2023-07-27 00:15:19.637159 interactivenlp-0.2.2/setup.cfg
+-rw-r--r--   0 chunxuyang   (501) staff       (20)     1037 2023-07-27 00:15:03.000000 interactivenlp-0.2.2/setup.py
```

### Comparing `interactivenlp-0.2.1/InteractiveNLP.egg-info/SOURCES.txt` & `interactivenlp-0.2.2/InteractiveNLP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/controllers/reader_controller.py` & `interactivenlp-0.2.2/interactivenlp/controllers/reader_controller.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/controllers/rss_controller.py` & `interactivenlp-0.2.2/interactivenlp/controllers/rss_controller.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/models/block.py` & `interactivenlp-0.2.2/interactivenlp/models/block.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/models/form.py` & `interactivenlp-0.2.2/interactivenlp/models/form.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/models/task.py` & `interactivenlp-0.2.2/interactivenlp/models/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 from typing import List, Optional
 
 import nltk
 
 from ..models.block import Block, BlockLevelEnum, BlockTypeEnum, BlockStatusEnum
 from ..types.model import ModelConfiguration, InteractiveTaskType, InteractiveFunctionType, InteractiveRssType, \
     InteractiveFunctionResultType, CompositionType
-from typing import List, Optional
-
-import nltk
-
-from ..models.block import Block, BlockLevelEnum, BlockTypeEnum, BlockStatusEnum
-from ..types.model import ModelConfiguration, InteractiveTaskType, InteractiveFunctionType, InteractiveRssType, \
-    InteractiveFunctionResultType, CompositionType
 
 try:
     nltk.data.find('tokenizers/punkt')
 except LookupError:
     nltk.download('punkt')
```

### Comparing `interactivenlp-0.2.1/interactivenlp/server.py` & `interactivenlp-0.2.2/interactivenlp/server.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/interactivenlp/types/model.py` & `interactivenlp-0.2.2/interactivenlp/types/model.py`

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

### Comparing `interactivenlp-0.2.1/interactivenlp/utils/extraction.py` & `interactivenlp-0.2.2/interactivenlp/utils/extraction.py`

 * *Files identical despite different names*

### Comparing `interactivenlp-0.2.1/setup.py` & `interactivenlp-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 with open('README.md', "r") as f:
     long_description = f.read()
 
 setup(
     name='interactivenlp',
-    version='0.2.1',
+    version='0.2.2',
     description='Interactive NLP',
     long_description=long_description,
     author="Chunxu Yang",
     author_email="chunxuyang@ucla.edu",
     install_requires=[
         'flask',
         'flask-cors',
```

