# Comparing `tmp/drf-rehive-extras-2.1.0rc2.tar.gz` & `tmp/drf-rehive-extras-2.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.1.0rc2.tar", last modified: Thu Jul 27 13:43:41 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.1.0rc3.tar", last modified: Thu Jul 27 14:04:59 2023, max compression
```

## Comparing `drf-rehive-extras-2.1.0rc2.tar` & `drf-rehive-extras-2.1.0rc3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.1.0rc2/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 13:42:56.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-07-27 13:20:38.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)    15190 2023-07-27 13:26:30.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/schema.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6894 2023-07-27 10:28:32.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.1.0rc2/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1781 2023-07-27 13:42:59.000000 drf-rehive-extras-2.1.0rc2/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc2/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc2/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 13:43:41.000000 drf-rehive-extras-2.1.0rc2/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.1.0rc3/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 13:52:28.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-07-27 13:20:38.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)    15119 2023-07-27 14:03:05.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/schema.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6873 2023-07-27 14:03:59.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.1.0rc3/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1781 2023-07-27 14:04:04.000000 drf-rehive-extras-2.1.0rc3/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc3/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 14:04:59.000000 drf-rehive-extras-2.1.0rc3/PKG-INFO
```

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.2.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.3.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.1.0rc2/README.md` & `drf-rehive-extras-2.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras/schema.py` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,19 +101,14 @@
                     if not all_docs:
                         all_docs = {}
                     all_docs.update(docs)
 
         return all_docs
 
 
-# Initiate a global docs object that is used in swagger schema generation.
-# This value must be an instance of `Documentation`.
-ADDITIONAL_DOCS = Documentation()
-
-
 # Extensions
 
 class OneOfOpenApiSerializerExtensionMixin():
     """
     Mixin for SerializerExtensions that must offer a oneOf interface.
     """
 
@@ -129,15 +124,15 @@
             schema["oneOf"].append(sub_schema)
 
         return schema
 
 
 # Autoschema
 
-class RehiveAutoSchema(AutoSchema):
+class BaseAutoSchema(AutoSchema):
     """
     Custom extension of the drf-spectacular.AutoSchema to support automated
     documentation injection into the schema.
 
     Additionally updated the Swagger schema generation to:
         - Envelope the response in a `data` attribute.
     """
@@ -151,18 +146,20 @@
             return
 
         logger.warning(msg)
 
     def _get_view_docs(self):
         """
         Helper to get additional docs for a view.
+
+        A `Documentation` instance must be found in settings.ADDITIONAL_DOCS.
         """
 
         try:
-            docs = ADDITIONAL_DOCS.docs
+            docs = getattr(settings, 'ADDITIONAL_DOCS')
         except (NameError, AttributeError):
             return None
 
         # Create a key for the specific view and check if it exists.
         key = "{}.{}".format(self.view.__module__, self.view.__class__.__name__)
         try:
             return docs[key][self.method]
```

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from rest_framework.generics import GenericAPIView
 
 from . import mixins
 
 
 class BaseAPIView(GenericAPIView):
     """
-    Generic view with extended features for Rehive usage. All viewsets should
-    extend this class.
+    Generic view with extended features. All viewsets should extend this class.
     """
 
     # Modify the serializer classes used by the view based on the request
     # method.
     # This attribute can take two formats:
     #  - {"GET": ObjectSerializer}
     #  - {"GET": (RequestObjectSerializer, ResponseObjectSerializer,)}
```

### Comparing `drf-rehive-extras-2.1.0rc2/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.1.0rc3/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc2/setup.py` & `drf-rehive-extras-2.1.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.1.0-rc.2'
+VERSION = '2.1.0-rc.3'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.1.0rc2/LICENSE` & `drf-rehive-extras-2.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.1.0rc2/PKG-INFO` & `drf-rehive-extras-2.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.1.0rc2
+Version: 2.1.0rc3
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.2.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.3.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

