# Comparing `tmp/wagtail-storages-1.0.0.tar.gz` & `tmp/wagtail-storages-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-storages-1.0.0.tar", last modified: Thu Jul 27 15:29:49 2023, max compression
+gzip compressed data, was "wagtail-storages-1.0.0rc1.tar", last modified: Tue Oct 11 15:48:17 2022, max compression
```

## Comparing `wagtail-storages-1.0.0.tar` & `wagtail-storages-1.0.0rc1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 15:29:49.188545 wagtail-storages-1.0.0/
--rw-r--r--   0 nick       (502) staff       (20)     1266 2023-07-27 15:29:30.000000 wagtail-storages-1.0.0/CHANGELOG.rst
--rw-r--r--   0 nick       (502) staff       (20)     1323 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/LICENSE
--rw-r--r--   0 nick       (502) staff       (20)      125 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/MANIFEST.in
--rw-r--r--   0 nick       (502) staff       (20)    11962 2023-07-27 15:29:49.188657 wagtail-storages-1.0.0/PKG-INFO
--rw-r--r--   0 nick       (502) staff       (20)    10953 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/README.rst
--rw-r--r--   0 nick       (502) staff       (20)     1580 2023-07-27 15:29:49.189229 wagtail-storages-1.0.0/setup.cfg
--rw-r--r--   0 nick       (502) staff       (20)       38 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/setup.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 15:29:49.186892 wagtail-storages-1.0.0/wagtail_storages/
--rw-r--r--   0 nick       (502) staff       (20)       90 2023-07-27 15:29:30.000000 wagtail-storages-1.0.0/wagtail_storages/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)      324 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/apps.py
--rw-r--r--   0 nick       (502) staff       (20)      360 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/backends.py
--rw-r--r--   0 nick       (502) staff       (20)     1372 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/factories.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 15:29:49.188085 wagtail-storages-1.0.0/wagtail_storages/management/
--rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/management/__init__.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 15:29:49.188386 wagtail-storages-1.0.0/wagtail_storages/management/commands/
--rw-r--r--   0 nick       (502) staff       (20)        0 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/management/commands/__init__.py
--rw-r--r--   0 nick       (502) staff       (20)      668 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/management/commands/fix_document_acls.py
--rw-r--r--   0 nick       (502) staff       (20)     2783 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/signal_handlers.py
--rw-r--r--   0 nick       (502) staff       (20)     3248 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/utils.py
--rw-r--r--   0 nick       (502) staff       (20)     1553 2023-07-27 15:15:44.000000 wagtail-storages-1.0.0/wagtail_storages/wagtail_hooks.py
-drwxr-xr-x   0 nick       (502) staff       (20)        0 2023-07-27 15:29:49.187817 wagtail-storages-1.0.0/wagtail_storages.egg-info/
--rw-r--r--   0 nick       (502) staff       (20)    11962 2023-07-27 15:29:49.000000 wagtail-storages-1.0.0/wagtail_storages.egg-info/PKG-INFO
--rw-r--r--   0 nick       (502) staff       (20)      618 2023-07-27 15:29:49.000000 wagtail-storages-1.0.0/wagtail_storages.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (502) staff       (20)        1 2023-07-27 15:29:49.000000 wagtail-storages-1.0.0/wagtail_storages.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (502) staff       (20)      124 2023-07-27 15:29:49.000000 wagtail-storages-1.0.0/wagtail_storages.egg-info/requires.txt
--rw-r--r--   0 nick       (502) staff       (20)       17 2023-07-27 15:29:49.000000 wagtail-storages-1.0.0/wagtail_storages.egg-info/top_level.txt
+drwxr-xr-x   0 tomaszk   (1000) tomaszk   (1000)        0 2022-10-11 15:48:17.470321 wagtail-storages-1.0.0rc1/
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     1003 2022-10-11 15:45:16.000000 wagtail-storages-1.0.0rc1/CHANGELOG.rst
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     1323 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/LICENSE
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      125 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)    11788 2022-10-11 15:48:17.470321 wagtail-storages-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)    10715 2022-05-11 13:23:50.000000 wagtail-storages-1.0.0rc1/README.rst
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     1616 2022-10-11 15:48:17.471321 wagtail-storages-1.0.0rc1/setup.cfg
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)       38 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/setup.py
+drwxr-xr-x   0 tomaszk   (1000) tomaszk   (1000)        0 2022-10-11 15:48:17.469321 wagtail-storages-1.0.0rc1/wagtail_storages/
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)       93 2022-10-11 15:45:35.000000 wagtail-storages-1.0.0rc1/wagtail_storages/__init__.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      324 2022-05-11 13:18:36.000000 wagtail-storages-1.0.0rc1/wagtail_storages/apps.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      360 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/wagtail_storages/backends.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     1495 2022-10-11 15:42:40.000000 wagtail-storages-1.0.0rc1/wagtail_storages/factories.py
+drwxr-xr-x   0 tomaszk   (1000) tomaszk   (1000)        0 2022-10-11 15:48:17.469321 wagtail-storages-1.0.0rc1/wagtail_storages/management/
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)        0 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/wagtail_storages/management/__init__.py
+drwxr-xr-x   0 tomaszk   (1000) tomaszk   (1000)        0 2022-10-11 15:48:17.470321 wagtail-storages-1.0.0rc1/wagtail_storages/management/commands/
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)        0 2020-02-12 19:38:43.000000 wagtail-storages-1.0.0rc1/wagtail_storages/management/commands/__init__.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      763 2022-05-30 09:35:49.000000 wagtail-storages-1.0.0rc1/wagtail_storages/management/commands/fix_document_acls.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     2879 2022-10-11 15:42:40.000000 wagtail-storages-1.0.0rc1/wagtail_storages/signal_handlers.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     3338 2022-10-11 15:42:40.000000 wagtail-storages-1.0.0rc1/wagtail_storages/utils.py
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)     1645 2022-10-11 15:42:40.000000 wagtail-storages-1.0.0rc1/wagtail_storages/wagtail_hooks.py
+drwxr-xr-x   0 tomaszk   (1000) tomaszk   (1000)        0 2022-10-11 15:48:17.469321 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)    11788 2022-10-11 15:48:17.000000 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      618 2022-10-11 15:48:17.000000 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)        1 2022-10-11 15:48:17.000000 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)      130 2022-10-11 15:48:17.000000 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/requires.txt
+-rw-r--r--   0 tomaszk   (1000) tomaszk   (1000)       17 2022-10-11 15:48:17.000000 wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/top_level.txt
```

### Comparing `wagtail-storages-1.0.0/CHANGELOG.rst` & `wagtail-storages-1.0.0rc1/CHANGELOG.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Unreleased
-----------
-
-1.0.0 - 27th July 2023
-----------------------
-* Support Wagtail 4.2 (@katdom13)
-* Drop support for Wagtail versions prior to 4.1 (@katdom13)
-* Updated test workflow to use tox-gh-actions (@katdom13)
-* Removed code conditionals (@katdom13)
-
 1.0.0rc1 - 11th October 2022
 ----------
 * Support Wagtail 4 (#33 - @nickmoreton)
 * Avoid unnecessary cache purges (#34 - @ababic)
 
 0.5.1rc1 - 30th May 2022
 ------------------------
```

### Comparing `wagtail-storages-1.0.0/LICENSE` & `wagtail-storages-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-storages-1.0.0/PKG-INFO` & `wagtail-storages-1.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: wagtail-storages
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Use AWS S3 with private documents in Wagtail.
 Home-page: https://github.com/torchbox/wagtail-storages
 Author: Tomasz Knapik
 Author-email: hi@tmkn.org
 License: BSD 2-Clause License
 Keywords: wagtail,s3,django,storages,storage
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Wagtail
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Provides-Extra: testing
 License-File: LICENSE
 
 .. image:: https://github.com/torchbox/wagtail-storages/raw/main/logo.png
 
 wagtail-storages
 ================
@@ -138,17 +140,14 @@
    - ``s3:ListBucket``
    - ``s3:GetBucketLocation``
    - ``s3:ListBucketMultipartUploads``
    - ``s3:ListBucketVersions``
 - Allow the user to perform all the actions (``s3:*``) on the objects within the
   bucket.
 - Allow the internet traffic to access Wagtail image renditions (``images/*``).
-- Allow use of public ACLs, by disabling:
-   - "Block public access to buckets and objects granted through new access control lists (ACLs)"
-   - "Block public access to buckets and objects granted through any access control lists (ACLs)"
 
 The user permissions can be set in the IAM or via a bucket policy. See example
 of all of those points being achieved in the bucket policy below.
 
 .. code:: json
 
    {
@@ -337,7 +336,9 @@
 ``WAGTAIL_STORAGES_DOCUMENTS_FRONTENDCACHE``.
 
 .. _WagtailFrontEndCache: https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html
 
 __ WagtailFrontEndCache_
 
 All done!
+
+
```

### Comparing `wagtail-storages-1.0.0/README.rst` & `wagtail-storages-1.0.0rc1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -110,17 +110,14 @@
    - ``s3:ListBucket``
    - ``s3:GetBucketLocation``
    - ``s3:ListBucketMultipartUploads``
    - ``s3:ListBucketVersions``
 - Allow the user to perform all the actions (``s3:*``) on the objects within the
   bucket.
 - Allow the internet traffic to access Wagtail image renditions (``images/*``).
-- Allow use of public ACLs, by disabling:
-   - "Block public access to buckets and objects granted through new access control lists (ACLs)"
-   - "Block public access to buckets and objects granted through any access control lists (ACLs)"
 
 The user permissions can be set in the IAM or via a bucket policy. See example
 of all of those points being achieved in the bucket policy below.
 
 .. code:: json
 
    {
```

### Comparing `wagtail-storages-1.0.0/setup.cfg` & `wagtail-storages-1.0.0rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 author_email = hi@tmkn.org
 url = https://github.com/torchbox/wagtail-storages
 license = BSD 2-Clause License
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved
 	License :: OSI Approved :: BSD License
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Framework :: Django
+	Framework :: Django :: 3.0
+	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.1
-	Framework :: Django :: 4.2
-	Framework :: Wagtail
+	Framework :: Django :: 4
+	Framework :: Wagtail :: 2
+	Framework :: Wagtail :: 3
 	Framework :: Wagtail :: 4
-	Framework :: Wagtail :: 5
 keywords = 
 	wagtail
 	s3
 	django
 	storages
 	storage
 
 [options]
 packages = find:
 install_requires = 
-	Wagtail >=4.1
+	Wagtail >=2.15,<5.0
 	django-storages[boto3] <2
-python_requires = >=3.8
+python_requires = >=3.6
 
 [options.packages.find]
 exclude = 
 	wagtail_storages.tests*
 
 [options.extras_require]
 testing =
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages/factories.py` & `wagtail-storages-1.0.0rc1/wagtail_storages/factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from wagtail.documents import get_document_model
-from wagtail.models import Collection, CollectionViewRestriction
 
 import factory
 import factory.django
 
+try:
+    from wagtail.models import Collection, CollectionViewRestriction
+except ImportError:
+    # Wagtail<3.0
+    from wagtail.core.models import Collection, CollectionViewRestriction
+
+
 Document = get_document_model()
 
 
 class DocumentFactory(factory.django.DjangoModelFactory):
     title = factory.Sequence(lambda n: "Document" + str(n))
     file = factory.django.FileField(
         filename="testfile.txt",
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages/management/commands/fix_document_acls.py` & `wagtail-storages-1.0.0rc1/wagtail_storages/management/commands/fix_document_acls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from django.core.management.base import BaseCommand, CommandError
 
-from wagtail.models import Collection
+try:
+    from wagtail.models import Collection
+except ImportError:
+    # Wagtail<3.0
+    from wagtail.core.models import Collection
+
 
 from wagtail_storages.utils import (
     is_s3_boto3_storage_used,
     update_collection_document_acls,
 )
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages/signal_handlers.py` & `wagtail-storages-1.0.0rc1/wagtail_storages/signal_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import functools
 import logging
 
 from django.db.models.signals import post_save, pre_delete
 
 from wagtail.documents import get_document_model
-from wagtail.models import Collection
+
+try:
+    from wagtail.models import Collection
+except ImportError:
+    # Wagtail<3.0
+    from wagtail.core.models import Collection
+
 
 from wagtail_storages.utils import (
     is_s3_boto3_storage_used,
     purge_collection_documents_from_cache,
     purge_document_from_cache,
     update_collection_document_acls,
     update_document_acl,
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages/utils.py` & `wagtail-storages-1.0.0rc1/wagtail_storages/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 import logging
 
 from django.conf import settings
 from django.core.files.storage import get_storage_class
 
 from wagtail.contrib.frontend_cache.utils import PurgeBatch
 from wagtail.documents import get_document_model
-from wagtail.models import Site
+
+try:
+    from wagtail.models import Site
+except ImportError:
+    # Wagtail<3.0
+    from wagtail.core.models import Site
+
 
 import storages.backends.s3boto3
 
 logger = logging.getLogger(__name__)
 
 
 def update_document_acl(document):
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages/wagtail_hooks.py` & `wagtail-storages-1.0.0rc1/wagtail_storages/wagtail_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import django
 
 import wagtail
 from wagtail.documents import get_document_model
-from wagtail.hooks import register
+
+try:
+    from wagtail.hooks import register
+except ImportError:
+    # Wagtail<3.0
+    from wagtail.core.hooks import register
 
 from wagtail_storages import backends, utils
 
 HOOK_ORDER = getattr(django.conf.settings, "WAGTAIL_STORAGES_DOCUMENT_HOOK_ORDER", 100)
 
 
 @register("before_serve_document", order=HOOK_ORDER)
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages.egg-info/PKG-INFO` & `wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: wagtail-storages
-Version: 1.0.0
+Version: 1.0.0rc1
 Summary: Use AWS S3 with private documents in Wagtail.
 Home-page: https://github.com/torchbox/wagtail-storages
 Author: Tomasz Knapik
 Author-email: hi@tmkn.org
 License: BSD 2-Clause License
 Keywords: wagtail,s3,django,storages,storage
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.1
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Wagtail
+Classifier: Framework :: Django :: 4
+Classifier: Framework :: Wagtail :: 2
+Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
-Classifier: Framework :: Wagtail :: 5
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Provides-Extra: testing
 License-File: LICENSE
 
 .. image:: https://github.com/torchbox/wagtail-storages/raw/main/logo.png
 
 wagtail-storages
 ================
@@ -138,17 +140,14 @@
    - ``s3:ListBucket``
    - ``s3:GetBucketLocation``
    - ``s3:ListBucketMultipartUploads``
    - ``s3:ListBucketVersions``
 - Allow the user to perform all the actions (``s3:*``) on the objects within the
   bucket.
 - Allow the internet traffic to access Wagtail image renditions (``images/*``).
-- Allow use of public ACLs, by disabling:
-   - "Block public access to buckets and objects granted through new access control lists (ACLs)"
-   - "Block public access to buckets and objects granted through any access control lists (ACLs)"
 
 The user permissions can be set in the IAM or via a bucket policy. See example
 of all of those points being achieved in the bucket policy below.
 
 .. code:: json
 
    {
@@ -337,7 +336,9 @@
 ``WAGTAIL_STORAGES_DOCUMENTS_FRONTENDCACHE``.
 
 .. _WagtailFrontEndCache: https://docs.wagtail.io/en/stable/reference/contrib/frontendcache.html
 
 __ WagtailFrontEndCache_
 
 All done!
+
+
```

### Comparing `wagtail-storages-1.0.0/wagtail_storages.egg-info/SOURCES.txt` & `wagtail-storages-1.0.0rc1/wagtail_storages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

