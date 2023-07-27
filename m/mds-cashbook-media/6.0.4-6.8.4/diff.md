# Comparing `tmp/mds_cashbook_media-6.0.4.tar.gz` & `tmp/mds_cashbook_media-6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_cashbook_media-6.0.4.tar", last modified: Thu Jul 27 10:58:21 2023, max compression
+gzip compressed data, was "mds_cashbook_media-6.8.4.tar", last modified: Thu Jul 27 10:54:31 2023, max compression
```

## Comparing `mds_cashbook_media-6.0.4.tar` & `mds_cashbook_media-6.8.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:58:21.526019 mds_cashbook_media-6.0.4/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1847 2023-07-27 10:58:21.526019 mds_cashbook_media-6.0.4/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      418 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      356 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     6538 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      491 2022-08-18 14:02:24.000000 mds_cashbook_media-6.0.4/line.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:58:21.506019 mds_cashbook_media-6.0.4/locale/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1337 2023-01-23 12:12:06.000000 mds_cashbook_media-6.0.4/locale/de.po
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     1125 2023-01-23 12:10:12.000000 mds_cashbook_media-6.0.4/locale/en.po
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:58:21.526019 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1847 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      518 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       79 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       77 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-07-27 10:58:21.000000 mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/top_level.txt
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      802 2022-11-29 09:33:29.000000 mds_cashbook_media-6.0.4/message.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-07-27 10:58:21.526019 mds_cashbook_media-6.0.4/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3914 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/setup.py
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:58:21.518019 mds_cashbook_media-6.0.4/tests/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      418 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/tests/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    74701 2022-10-14 13:21:44.000000 mds_cashbook_media-6.0.4/tests/img_data.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     8061 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/tests/test_line.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       80 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/tryton.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)       28 2023-06-12 07:19:34.000000 mds_cashbook_media-6.0.4/versiondep.txt
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-07-27 10:58:21.522019 mds_cashbook_media-6.0.4/view/
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      736 2023-01-23 12:12:06.000000 mds_cashbook_media-6.0.4/view/line_form.xml
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

### Comparing `mds_cashbook_media-6.0.4/PKG-INFO` & `mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds_cashbook_media
-Version: 6.0.4
+Name: mds-cashbook-media
+Version: 6.8.4
 Summary: Tryton module to add a file-field to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook_media
 Description: mds-cashbook-media
@@ -14,39 +14,22 @@
         Install
         =======
         
         pip install mds-cashbook-media
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.4 - 06.06.2023*
-        
-        - code optimized
-        
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
@@ -57,8 +40,9 @@
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

### Comparing `mds_cashbook_media-6.0.4/line.py` & `mds_cashbook_media-6.8.4/line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/locale/de.po` & `mds_cashbook_media-6.8.4/locale/de.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/locale/en.po` & `mds_cashbook_media-6.8.4/locale/en.po`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/PKG-INFO` & `mds_cashbook_media-6.8.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mds-cashbook-media
-Version: 6.0.4
+Name: mds_cashbook_media
+Version: 6.8.4
 Summary: Tryton module to add a file-field to cashbook.
 Home-page: https://www.m-ds.de/
 Author: martin-data services
 Author-email: service@m-ds.de
 License: GPL-3
 Download-URL: https://scmdev.m-ds.de/Tryton/Extra/cashbook_media
 Description: mds-cashbook-media
@@ -14,39 +14,22 @@
         Install
         =======
         
         pip install mds-cashbook-media
         
         Requires
         ========
-        - Tryton 6.0
+        - Tryton 6.8
         
         Changes
         =======
         
-        *6.0.4 - 06.06.2023*
-        
-        - code optimized
-        
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
@@ -57,8 +40,9 @@
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

### Comparing `mds_cashbook_media-6.0.4/mds_cashbook_media.egg-info/SOURCES.txt` & `mds_cashbook_media-6.8.4/mds_cashbook_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/message.xml` & `mds_cashbook_media-6.8.4/message.xml`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/setup.py` & `mds_cashbook_media-6.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
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
@@ -92,14 +92,15 @@
         'Topic :: Office/Business :: Financial :: Accounting',
         'Natural Language :: German',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
 
     keywords='tryton cashbook pdf png image file',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
```

### Comparing `mds_cashbook_media-6.0.4/tests/img_data.py` & `mds_cashbook_media-6.8.4/tests/img_data.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/tests/test_line.py` & `mds_cashbook_media-6.8.4/tests/test_line.py`

 * *Files identical despite different names*

### Comparing `mds_cashbook_media-6.0.4/view/line_form.xml` & `mds_cashbook_media-6.8.4/view/line_form.xml`

 * *Files identical despite different names*

