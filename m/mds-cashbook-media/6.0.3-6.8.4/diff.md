# Comparing `tmp/mds_cashbook_media-6.0.3.tar.gz` & `tmp/mds_cashbook_media-6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook_media-6.0.3.tar", last modified: Tue Feb 14 09:54:15 2023, max compression
+gzip compressed data, was "mds_cashbook_media-6.8.4.tar", last modified: Thu Jul 27 10:54:31 2023, max compression
```

## Comparing `mds_cashbook_media-6.0.3.tar` & `mds_cashbook_media-6.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:54:15.089504 mds_cashbook_media-6.0.3/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1775 2023-02-14 09:54:15.089504 mds_cashbook_media-6.0.3/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      378 2023-02-14 09:53:07.000000 mds_cashbook_media-6.0.3/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      355 2022-10-14 09:01:54.000000 mds_cashbook_media-6.0.3/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6539 2023-01-23 12:12:06.000000 mds_cashbook_media-6.0.3/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      491 2022-08-18 14:02:24.000000 mds_cashbook_media-6.0.3/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:54:14.981504 mds_cashbook_media-6.0.3/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1337 2023-01-23 12:12:06.000000 mds_cashbook_media-6.0.3/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1125 2023-01-23 12:10:12.000000 mds_cashbook_media-6.0.3/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:54:15.089504 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1775 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      518 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       79 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       77 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-02-14 09:54:14.000000 mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      802 2022-11-29 09:33:29.000000 mds_cashbook_media-6.0.3/message.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-02-14 09:54:15.089504 mds_cashbook_media-6.0.3/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3726 2023-02-14 09:52:42.000000 mds_cashbook_media-6.0.3/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:54:15.081504 mds_cashbook_media-6.0.3/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      581 2022-10-14 09:02:22.000000 mds_cashbook_media-6.0.3/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    74701 2022-10-14 13:21:44.000000 mds_cashbook_media-6.0.3/tests/img_data.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8034 2022-10-14 13:27:23.000000 mds_cashbook_media-6.0.3/tests/test_line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       80 2023-02-14 09:53:17.000000 mds_cashbook_media-6.0.3/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       28 2023-02-14 09:53:14.000000 mds_cashbook_media-6.0.3/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-02-14 09:54:15.085504 mds_cashbook_media-6.0.3/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      736 2023-01-23 12:12:06.000000 mds_cashbook_media-6.0.3/view/line_form.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1572 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      229 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      356 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     6538 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      491 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/line.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:54:31.902653 mds_cashbook_media-6.8.4/locale/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1337 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/locale/de.po
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1125 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/locale/en.po
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1572 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      518 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       79 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       77 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-27 10:54:31.000000 mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      802 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/message.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/setup.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     3963 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/setup.py
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/tests/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      144 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/tests/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    74701 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/tests/img_data.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     8061 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/tests/test_line.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       79 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/tryton.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)       29 2023-07-27 10:52:58.000000 mds_cashbook_media-6.8.4/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:54:31.910653 mds_cashbook_media-6.8.4/view/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      736 2023-06-12 07:42:26.000000 mds_cashbook_media-6.8.4/view/line_form.xml
```

### Comparing `mds_cashbook_media-6.0.3/PKG-INFO` & `mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds_cashbook_media
-Version: 6.0.3
+Name: mds-cashbook-media
+Version: 6.8.4
 Summary: Tryton module to add a file-field to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook_media
 Description: mds-cashbook-media
@@ -14,35 +14,22 @@
         Install
         =======
         
         pip install mds-cashbook-media
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.3 - 14.02.2023*
-        
-        - updt: setup.py
-        
-        *6.0.2 - 23.01.2023*
-        
-        - add: show image in tab 'image/pdf'
-        
-        *6.0.1 - 29.11.2022*
-        
-        - fix: exception when image type unknown
-        
-        *6.0.0 - 14.10.2022*
-        
-        - init
+        *6.8.4 - 06.06.2023*
         
+        - ported to Tryton 6.8
         
 Keywords: tryton cashbook pdf png image file
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -53,8 +40,9 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
```

### Comparing `mds_cashbook_media-6.0.3/line.py` & `mds_cashbook_media-6.8.4/line.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
-import mimetypes, magic
+import mimetypes
+import magic
 from io import BytesIO
 from PIL import Image, UnidentifiedImageError
 from trytond.model import fields
-from trytond.pool import Pool, PoolMeta
+from trytond.pool import PoolMeta
 from trytond.config import config
-from trytond.transaction import Transaction
 from trytond.exceptions import UserError
 from trytond.i18n import gettext
 from trytond.pyson import Eval, Bool
 from trytond.modules.cashbook.line import STATES, DEPENDS
 
 
 store_prefix = config.get('cashbook', 'store_prefix', default='cashbook')
 image_limit = config.get('cashbook', 'image_max_pixel', default='2000')
-try :
+try:
     image_limit = int(image_limit)
     if image_limit < 100:
         image_limit = 100
     if image_limit > 10000:
         image_limit = 10000
-except :
+except Exception:
     image_limit = 2000
 
 
 STATES2 = {}
 STATES2.update(STATES)
 DEPENDS2 = []
 DEPENDS2.extend(DEPENDS)
 
 
 class Line(metaclass=PoolMeta):
     __name__ = 'cashbook.line'
 
-    media = fields.Binary(string='Image of PDF', filename='media_name',
-        file_id='media_id', store_prefix=store_prefix,
-        states=STATES2, depends=DEPENDS2)
-    media_name = fields.Char(string='File name',
+    media = fields.Binary(
+        string='Image of PDF', filename='media_name', file_id='media_id',
+        store_prefix=store_prefix, states=STATES2, depends=DEPENDS2)
+    media_name = fields.Char(
+        string='File name',
         states={
             'required': Bool(Eval('media')),
             'readonly': STATES2['readonly'],
         }, depends=DEPENDS2)
     media_id = fields.Char(string='File ID', readonly=True)
     media_mime = fields.Char(string='MIME', readonly=True)
     media_size = fields.Integer(string='File size', readonly=True)
-    media_image = fields.Function(fields.Binary(string='Image', readonly=True,
+    media_image = fields.Function(fields.Binary(
+        string='Image', readonly=True,
         states={
-            'invisible': ~Eval('media_mime', '').in_(['image/png', 'image/jpg', 'image/jpeg']),
-        }, depends=['media_mime']),
-        'on_change_with_media_image')
+            'invisible': ~Eval('media_mime', '').in_([
+                'image/png', 'image/jpg', 'image/jpeg']),
+        }, depends=['media_mime']), 'on_change_with_media_image')
 
     @fields.depends('media', 'media_mime')
     def on_change_with_media_image(self, name=True):
         """ return binary if its a image
         """
         if (self.media_mime or '-').startswith('image/'):
             return self.media
@@ -79,25 +81,25 @@
 
     @classmethod
     def resize_image_file(cls, image_data):
         """ shrink image 'image_limit' pixel if its bigger
         """
         image_data2 = None
         with BytesIO(image_data) as fhdl:
-            try :
+            try:
                 image = Image.open(fhdl, 'r')
             except UnidentifiedImageError:
                 raise UserError(gettext('cashbook_media.msg_file_unknown_type'))
 
             (width, height) = image.size
             if (width > image_limit) or (height > image_limit):
 
                 if width > height:
                     new_size = (image_limit, int(height * image_limit / width))
-                else :
+                else:
                     new_size = (int(width * image_limit / height), image_limit)
 
                 # resize - fit in (image_limit x image_limit)
                 img2 = image.resize(new_size, Image.LANCZOS)
                 with BytesIO() as fhdl2:
                     img2.save(fhdl2, 'JPEG', optimize=True, quality=80)
                     fhdl2.seek(0)
@@ -112,23 +114,25 @@
         """ get mime-type, update file-name
         """
         if len(values['media'] or '') < 100:
             values['media'] = None
             values['media_mime'] = None
             values['media_size'] = None
             values['media_name'] = None
-        else :
+        else:
             values['media_mime'] = cls._identify_file(values['media'][:1024])
 
-            # if its a image, resize it to fit in (image_limit x image_limit) pixel
+            # if its a image, resize it to fit
+            # in (image_limit x image_limit) pixel
             if values['media_mime'].startswith('image'):
                 new_image = cls.resize_image_file(values['media'])
                 if new_image is not None:
                     values['media'] = new_image
-                    values['media_mime'] = cls._identify_file(values['media'][:1024])
+                    values['media_mime'] = cls._identify_file(
+                        values['media'][:1024])
 
             values['media_size'] = len(values['media'])
             file_ext = mimetypes.guess_extension(values['media_mime'])
             if 'media_name' in values.keys():
                 if not values['media_name'].endswith(file_ext):
                     # cut extension
                     if values['media_name'][-4] == '.':
@@ -143,23 +147,22 @@
         super(Line, cls).validate(lines)
 
         for line in lines:
             if line.media is not None:
                 if line.media_size > 1024*1024*5:
                     raise UserError(gettext(
                         'cashbook_media.msg_file_too_big',
-                        recname = line.rec_name,
-                        ))
-                if not line.media_mime in ['application/pdf',
-                    'image/png', 'image/jpg', 'image/jpeg']:
+                        recname=line.rec_name))
+                if line.media_mime not in [
+                        'application/pdf',
+                        'image/png', 'image/jpg', 'image/jpeg']:
                     raise UserError(gettext(
                         'cashbook_media.msg_file_invalid_mime',
-                        recname = line.rec_name,
-                        fmime = line.media_mime,
-                        ))
+                        recname=line.rec_name,
+                        fmime=line.media_mime))
 
     @classmethod
     def create(cls, vlist):
         """ add media-info
         """
         vlist = [x.copy() for x in vlist]
         for values in vlist:
```

### Comparing `mds_cashbook_media-6.0.3/locale/de.po` & `mds_cashbook_media-6.8.4/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.3/locale/en.po` & `mds_cashbook_media-6.8.4/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/PKG-INFO` & `mds_cashbook_media-6.8.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds-cashbook-media
-Version: 6.0.3
+Name: mds_cashbook_media
+Version: 6.8.4
 Summary: Tryton module to add a file-field to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook_media
 Description: mds-cashbook-media
@@ -14,35 +14,22 @@
         Install
         =======
         
         pip install mds-cashbook-media
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.3 - 14.02.2023*
-        
-        - updt: setup.py
-        
-        *6.0.2 - 23.01.2023*
-        
-        - add: show image in tab 'image/pdf'
-        
-        *6.0.1 - 29.11.2022*
-        
-        - fix: exception when image type unknown
-        
-        *6.0.0 - 14.10.2022*
-        
-        - init
+        *6.8.4 - 06.06.2023*
         
+        - ported to Tryton 6.8
         
 Keywords: tryton cashbook pdf png image file
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
@@ -53,8 +40,9 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Natural Language :: German
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
```

### Comparing `mds_cashbook_media-6.0.3/mds_cashbook_media.egg-info/SOURCES.txt` & `mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.3/message.xml` & `mds_cashbook_media-6.8.4/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.3/setup.py` & `mds_cashbook_media-6.8.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Tryton module to add a file-field to cashbook
 """
 
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+from setuptools import setup
 # To use a consistent encoding
 from codecs import open
 from os import path
 import re
 try:
     from configparser import ConfigParser
 except ImportError:
@@ -32,76 +32,85 @@
 modversion = {}
 with open(path.join(here, 'versiondep.txt'), encoding='utf-8') as f:
     l1 = f.readlines()
     for i in l1:
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
-        modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
+        modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 0
+minor_version = 8
 
 requires = ['python-magic>=0.4.24', 'Pillow']
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
                 prefix = modversion[dep]['prefix']
 
             if len(modversion[dep]['max']) > 0:
-                requires.append('%s_%s >= %s, <= %s' %
-                    (prefix, dep, modversion[dep]['min'], modversion[dep]['max']))
-            else :
-                requires.append('%s_%s >= %s' %
+                requires.append(
+                    '%s_%s >= %s, <= %s' %
+                    (prefix, dep,
+                        modversion[dep]['min'],
+                        modversion[dep]['max']))
+            else:
+                requires.append(
+                    '%s_%s >= %s' %
                     (prefix, dep, modversion[dep]['min']))
-        else :
-          requires.append('%s_%s >= %s.%s, < %s.%s' %
-                ('trytond', dep, major_version, minor_version,
-                major_version, minor_version + 1))
-requires.append('trytond >= %s.%s, < %s.%s' %
-        (major_version, minor_version, major_version, minor_version + 1))
+        else:
+            requires.append(
+                '%s_%s >= %s.%s, < %s.%s' % (
+                    'trytond', dep, major_version, minor_version,
+                    major_version, minor_version + 1))
+requires.append(
+    'trytond >= %s.%s, < %s.%s' % (
+        major_version, minor_version, major_version, minor_version + 1))
 
-setup(name='%s_%s' % (PREFIX, MODULE),
+setup(
+    name='%s_%s' % (PREFIX, MODULE),
     version=info.get('version', '0.0.1'),
     description='Tryton module to add a file-field to cashbook.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://www.m-ds.de/',
     download_url='https://scmdev.m-ds.de/Tryton/Extra/cashbook_media',
     author='martin-data services',
     author_email='service@m-ds.de',
     license='GPL-3',
     classifiers=[
-    'Development Status :: 5 - Production/Stable',
-    'Environment :: Plugins',
-    'Framework :: Tryton',
-    'Intended Audience :: Developers',
-    'Intended Audience :: Customer Service',
-    'Intended Audience :: Information Technology',
-    'Intended Audience :: Financial and Insurance Industry',
-    'Topic :: Office/Business',
-    'Topic :: Office/Business :: Financial :: Accounting',
-    'Natural Language :: German',
-    'Natural Language :: English',
-    'Operating System :: OS Independent',
-    'License :: OSI Approved :: GNU General Public License (GPL)',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
+        'Development Status :: 5 - Production/Stable',
+        'Environment :: Plugins',
+        'Framework :: Tryton',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Customer Service',
+        'Intended Audience :: Information Technology',
+        'Intended Audience :: Financial and Insurance Industry',
+        'Topic :: Office/Business',
+        'Topic :: Office/Business :: Financial :: Accounting',
+        'Natural Language :: German',
+        'Natural Language :: English',
+        'Operating System :: OS Independent',
+        'License :: OSI Approved :: GNU General Public License (GPL)',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton cashbook pdf png image file',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
     package_data={
-        'trytond.modules.%s' % MODULE: (info.get('xml', [])
+        'trytond.modules.%s' % MODULE: (
+            info.get('xml', [])
             + ['tryton.cfg', 'locale/*.po', 'tests/*.py',
                 'view/*.xml', 'versiondep.txt', 'README.rst']),
         },
 
     install_requires=requires,
     zip_safe=False,
     entry_points="""
```

### Comparing `mds_cashbook_media-6.0.3/tests/img_data.py` & `mds_cashbook_media-6.8.4/tests/img_data.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.3/tests/test_line.py` & `mds_cashbook_media-6.8.4/tests/test_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 # This file is part of the cashbook-module from m-ds for Tryton.
 # The COPYRIGHT file at the top level of this repository contains the
 # full copyright notices and license terms.
 
 from io import BytesIO
 from PIL import Image
-from trytond.tests.test_tryton import ModuleTestCase, with_transaction
+from trytond.tests.test_tryton import with_transaction
 from trytond.pool import Pool
-from trytond.transaction import Transaction
 from trytond.exceptions import UserError
-from trytond.modules.cashbook.tests import CashbookTestCase
+from trytond.modules.cashbook.tests.test_module import CashbookTestCase
 from datetime import date
 from decimal import Decimal
 from .img_data import img_data_png, dok_data_pdf, text_data
 
 
 class LineTestCase(CashbookTestCase):
     'Test cashbook line module'
@@ -122,16 +121,19 @@
                 },])],
             }])
         self.assertEqual(book.name, 'Book 1')
         self.assertEqual(len(book.lines), 1)
         self.assertEqual(book.state, 'open')
 
         # add invalid file
-        self.assertRaisesRegex(UserError,
-            "The file type 'text/plain' of the record '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]' is not allowed. (allowed: PNG, JPG, PDF)",
+        self.assertRaisesRegex(
+            UserError,
+            "The file type 'text/plain' of the record " +
+            "'05/02/2022|Rev|1.00 usd|Text 2 [Cat1]' is not allowed. " +
+            "(allowed: PNG, JPG, PDF)",
             Book.write,
             *[
                 [book],
                 {
                     'lines': [('create', [{
                         'date': date(2022, 5, 2),
                         'description': 'Text 2',
@@ -142,16 +144,19 @@
                         'media': text_data,
                         'media_name': 'text.txt',
                         }])],
                 }
             ])
 
         # replace image at line-1 by invalid file
-        self.assertRaisesRegex(UserError,
-            "The file type 'text/plain' of the record '05/02/2022|Rev|1.00 usd|Text 2 [Cat1]' is not allowed. (allowed: PNG, JPG, PDF)",
+        self.assertRaisesRegex(
+            UserError,
+            "The file type 'text/plain' of the record " +
+            "'05/02/2022|Rev|1.00 usd|Text 2 [Cat1]' is not allowed. " +
+            "(allowed: PNG, JPG, PDF)",
             Lines.write,
             *[
                 [book.lines[0]],
                 {
                     'media': text_data,
                     'media_name': 'text.txt',
                 },
@@ -159,15 +164,14 @@
 
     @with_transaction()
     def test_media_add_big_file(self):
         """ create cook/line, add big png-file
         """
         pool = Pool()
         Book = pool.get('cashbook.book')
-        Lines = pool.get('cashbook.line')
 
         types = self.prep_type()
         category = self.prep_category(cattype='in')
         company = self.prep_company()
         party = self.prep_party()
 
         book, = Book.create([{
@@ -222,7 +226,10 @@
 
         # check image size
         with BytesIO(book.lines[1].media) as fhdl:
             img2 = Image.open(fhdl, 'r')
             self.assertEqual(img2.size, (2000, 837))
 
 # end LineTestCase
+
+
+del CashbookTestCase
```

### Comparing `mds_cashbook_media-6.0.3/view/line_form.xml` & `mds_cashbook_media-6.8.4/view/line_form.xml`

 * *Files identical despite different names*

