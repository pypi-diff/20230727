# Comparing `tmp/drf-rehive-extras-2.0.6.tar.gz` & `tmp/drf-rehive-extras-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.0.6.tar", last modified: Thu Jul  6 18:20:11 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.1.0rc1.tar", last modified: Thu Jul 27 13:28:45 2023, max compression
```

## Comparing `drf-rehive-extras-2.0.6.tar` & `drf-rehive-extras-2.1.0rc1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.6/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      120 2023-07-06 18:18:56.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6490 2023-07-06 18:19:22.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6579 2023-07-06 15:32:54.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-06 15:33:03.000000 drf-rehive-extras-2.0.6/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-07-06 18:19:02.000000 drf-rehive-extras-2.0.6/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.6/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.6/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-07-06 18:20:11.000000 drf-rehive-extras-2.0.6/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.1.0rc1/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      328 2023-07-27 10:33:55.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-07-27 13:20:38.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)    15190 2023-07-27 13:26:30.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/schema.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2023-07-06 15:33:27.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6894 2023-07-27 10:28:32.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.1.0rc1/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1781 2023-07-27 13:27:52.000000 drf-rehive-extras-2.1.0rc1/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc1/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.1.0rc1/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1868 2023-07-27 13:28:45.000000 drf-rehive-extras-2.1.0rc1/PKG-INFO
```

### Comparing `drf-rehive-extras-2.0.6/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.1.0rc1/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.6
+Version: 2.1.0rc1
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.6.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.1.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.0.6/README.md` & `drf-rehive-extras-2.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.6/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.1.0rc1/drf_rehive_extras/mixins.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,14 +39,39 @@
         resource_id = getattr(instance, field)
     except AttributeError:
         return
     else:
         request._resource_id = str(resource_id)
 
 
+class ActionMixin(DRFCreateModelMixin):
+    """
+    Perform a generic action.
+    """
+
+    def create(self, request, *args, **kwargs):
+        """
+        Handle object creation on the view.
+        """
+
+        # Handle the request serialization and creation.
+        serializer = self.get_serializer(data=request.data)
+        serializer.is_valid(raise_exception=True)
+        self.perform_create(serializer)
+
+        # Attach creation success headers.
+        headers = self.get_success_headers(serializer.data)
+
+        return Response(
+            data={'status': 'success'},
+            status=self.get_response_status_code(),
+            headers=headers
+        )
+
+
 class CreateModelMixin(DRFCreateModelMixin):
     """
     Create a model instance.
     """
 
     def create(self, request, *args, **kwargs):
         """
```

### Comparing `drf-rehive-extras-2.0.6/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.1.0rc1/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.6/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.1.0rc1/drf_rehive_extras/generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,28 @@
 
         try:
             return self.response_status_codes[self.request.method]
         except KeyError:
             return self.default_response_status_codes[self.request.method]
 
 
+class ActionAPIView(mixins.ActionMixin,
+                    BaseAPIView):
+    """
+    Concrete view for performing a generic action.
+    """
+
+    response_status_codes = {
+        "POST": status.HTTP_200_OK
+    }
+
+    def post(self, request, *args, **kwargs):
+        return self.create(request, *args, **kwargs)
+
+
 class CreateAPIView(mixins.CreateModelMixin,
                     BaseAPIView):
     """
     Concrete view for creating a model instance.
     """
 
     def post(self, request, *args, **kwargs):
```

### Comparing `drf-rehive-extras-2.0.6/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.1.0rc1/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.6/setup.py` & `drf-rehive-extras-2.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.0.6'
+VERSION = '2.1.0-rc.1'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
@@ -25,15 +25,16 @@
     author_email='info@rehive.com',
     license='MIT',
     install_requires=[
         "Django>=3.0",
         "djangorestframework>=3.13.1",
         "drf-flex-fields>=0.9.7",
         "django-filter>=21.0",
-        "django-enumfields>=2.1.1"
+        "django-enumfields>=2.1.1",
+        "drf-spectacular>=0.26.3"
     ],
     python_requires='>=3.6',
     classifiers=[
         'Framework :: Django',
         'Framework :: Django :: 3.0',
         'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
```

### Comparing `drf-rehive-extras-2.0.6/LICENSE` & `drf-rehive-extras-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.0.6/PKG-INFO` & `drf-rehive-extras-2.1.0rc1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.0.6
+Version: 2.1.0rc1
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.6.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.1.0-rc.1.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

