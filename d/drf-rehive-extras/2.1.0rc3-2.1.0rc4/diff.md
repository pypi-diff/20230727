# Comparing `tmp/drf-rehive-extras-2.1.0rc3.tar.gz` & `tmp/drf-rehive-extras-2.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.1.0rc3.tar", last modified: Thu Jul 27 14:04:59 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.1.0rc4.tar", last modified: Thu Jul 27 16:18:32 2023, max compression
```

## Comparing `drf-rehive-extras-2.1.0rc3.tar` & `drf-rehive-extras-2.1.0rc4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.1.0rc3/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 13:52:28.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-07-27 13:20:38.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)    15119 2023-07-27 14:03:05.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/schema.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6873 2023-07-27 14:03:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1781 2023-07-27 14:04:04.000000 drf-rehive-extras-2.1.0rc3/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 16:18:32.000000 drf-rehive-extras-2.1.0rc4/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 16:18:32.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-27 16:18:31.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-07-27 16:18:31.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-07-27 16:18:31.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-27 16:18:31.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 16:18:31.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.1.0rc4/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-27 16:18:32.000000 drf-rehive-extras-2.1.0rc4/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 16:18:32.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 13:52:28.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-07-27 13:20:38.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)    15330 2023-07-27 16:17:12.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/schema.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6873 2023-07-27 14:03:59.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.1.0rc4/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1781 2023-07-27 16:17:16.000000 drf-rehive-extras-2.1.0rc4/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc4/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc4/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 16:18:32.000000 drf-rehive-extras-2.1.0rc4/PKG-INFO
```

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.1.0rc3
+Version: 2.1.0rc4
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.3.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.4.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.1.0rc3/README.md` & `drf-rehive-extras-2.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/schema.py` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import yaml
 from logging import getLogger
-from collections import OrderedDict
+from functools import lru_cache
 
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.openapi import AutoSchema
 from drf_spectacular.plumbing import (
     is_list_serializer, is_serializer, is_basic_type, force_instance,
     build_basic_type, is_list_serializer_customized, build_array_type,
@@ -101,14 +101,25 @@
                     if not all_docs:
                         all_docs = {}
                     all_docs.update(docs)
 
         return all_docs
 
 
+@lru_cache(maxsize=None)
+def get_additional_documentation():
+    """
+    Method to get additional documentation.
+
+    Cache the result so it does not have to call it repeatedly.
+    """
+
+    return Documentation()
+
+
 # Extensions
 
 class OneOfOpenApiSerializerExtensionMixin():
     """
     Mixin for SerializerExtensions that must offer a oneOf interface.
     """
 
@@ -151,15 +162,15 @@
         """
         Helper to get additional docs for a view.
 
         A `Documentation` instance must be found in settings.ADDITIONAL_DOCS.
         """
 
         try:
-            docs = getattr(settings, 'ADDITIONAL_DOCS')
+            docs = get_additional_documentation().docs
         except (NameError, AttributeError):
             return None
 
         # Create a key for the specific view and check if it exists.
         key = "{}.{}".format(self.view.__module__, self.view.__class__.__name__)
         try:
             return docs[key][self.method]
```

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras/generics.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.1.0rc4/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/setup.py` & `drf-rehive-extras-2.1.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.1.0-rc.3'
+VERSION = '2.1.0-rc.4'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.1.0rc3/LICENSE` & `drf-rehive-extras-2.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc3/PKG-INFO` & `drf-rehive-extras-2.1.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.1.0rc3
+Version: 2.1.0rc4
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.3.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.4.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

