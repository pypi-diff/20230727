# Comparing `tmp/usolitaire-0.2.1.tar.gz` & `tmp/usolitaire-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/usolitaire-0.2.1.tar", last modified: Sat Apr 22 01:09:26 2017, max compression
+gzip compressed data, was "usolitaire-1.0.0.tar", last modified: Thu Jul 27 12:37:07 2023, max compression
```

## Comparing `usolitaire-0.2.1.tar` & `usolitaire-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-22 01:09:26.000000 usolitaire-0.2.1/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire/
--rw-r--r--   0 travis    (1000) travis    (1000)      119 2017-04-22 01:08:51.000000 usolitaire-0.2.1/usolitaire/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     6697 2017-04-22 01:08:51.000000 usolitaire-0.2.1/usolitaire/app.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4988 2017-04-22 01:08:51.000000 usolitaire-0.2.1/usolitaire/game.py
--rw-r--r--   0 travis    (1000) travis    (1000)     5737 2017-04-22 01:08:51.000000 usolitaire-0.2.1/usolitaire/ui.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     1521 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      345 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       52 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-04-22 01:08:58.000000 usolitaire-0.2.1/usolitaire.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)        6 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       11 2017-04-22 01:09:26.000000 usolitaire-0.2.1/usolitaire.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      570 2017-04-22 01:08:51.000000 usolitaire-0.2.1/README.rst
--rw-r--r--   0 travis    (1000) travis    (1000)      404 2017-04-22 01:09:26.000000 usolitaire-0.2.1/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     1293 2017-04-22 01:08:51.000000 usolitaire-0.2.1/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1521 2017-04-22 01:09:26.000000 usolitaire-0.2.1/PKG-INFO
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.405153 usolitaire-1.0.0/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.0/LICENSE
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:37:07.405153 usolitaire-1.0.0/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.0/README.rst
+-rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.0/pyproject.toml
+-rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-27 12:37:07.405153 usolitaire-1.0.0/setup.cfg
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-27 12:19:12.000000 usolitaire-1.0.0/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.401153 usolitaire-1.0.0/usolitaire/
+-rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-27 12:19:12.000000 usolitaire-1.0.0/usolitaire/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    12253 2023-07-27 12:15:26.000000 usolitaire-1.0.0/usolitaire/app.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 12:14:41.000000 usolitaire-1.0.0/usolitaire/card_render.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.0/usolitaire/game.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 12:14:41.000000 usolitaire-1.0.0/usolitaire/textual_ui.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-27 12:37:07.405153 usolitaire-1.0.0/usolitaire.egg-info/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)      402 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/SOURCES.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/dependency_links.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/entry_points.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/not-zip-safe
+-rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/requires.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-27 12:37:07.000000 usolitaire-1.0.0/usolitaire.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `usolitaire-0.2.1/usolitaire.egg-info/PKG-INFO` & `usolitaire-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: usolitaire
-Version: 0.2.1
+Version: 1.0.0
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
-Description: ===============================
-        usolitaire
-        ===============================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/usolitaire.svg
-                :target: https://pypi.python.org/pypi/usolitaire
-        
-        .. image:: https://img.shields.io/travis/eliasdorneles/usolitaire.svg
-                :target: https://travis-ci.org/eliasdorneles/usolitaire
-        
-        
-        Play solitaire in your terminal.
-        
-        Point and click to move cards.
-        
-        Install with:
-        
-            pip install usolitaire
-        
-        .. image:: https://raw.githubusercontent.com/eliasdorneles/usolitaire/master/screenshot-usolitaire.png
-        
-        
-        * Free software: MIT license
-        
 Keywords: usolitaire
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+===============================
+usolitaire
+===============================
+
+
+.. image:: https://img.shields.io/pypi/v/usolitaire.svg
+        :target: https://pypi.python.org/pypi/usolitaire
+
+.. image:: https://img.shields.io/travis/eliasdorneles/usolitaire.svg
+        :target: https://travis-ci.org/eliasdorneles/usolitaire
+
+
+Play solitaire in your terminal.
+
+Point and click to move cards, or use the keyboard shortcuts.
+
+Install with:
+
+    pip install usolitaire
+
+Run with:
+
+    usolitaire
+
+To run from sources, you can run with:
+
+    python -m usolitaire.app
+
+.. image:: https://raw.githubusercontent.com/eliasdorneles/usolitaire/master/screenshot-usolitaire.png
+
+* Free software: MIT license
+
+
+History
+-------
+
+I built the first version of this app in 2017 using the `urwid`_ library, while
+I was attending `Recurse Center`_.
+
+In 2023, after attending Europython and learning the `Textual`_ framework,
+which solved all the gripes I had with ``urwid`` before, I decided to rewrite
+it in Textual and added the features that were missing.
+
+.. _urwid: https://urwid.org
+.. _Recurse Center: https://www.recurse.com/
+.. _Textual: https://textual.textualize.io
```

### Comparing `usolitaire-0.2.1/setup.py` & `usolitaire-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
-with open('README.rst') as readme_file:
+with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 requirements = [
-    'urwid',
+    "textual",
 ]
 
 setup(
-    name='usolitaire',
-    version='0.2.1',
+    name="usolitaire",
+    version="1.0.0",
     description="Solitaire in your terminal",
     long_description=readme,
     author="Elias Dorneles",
-    author_email='eliasdorneles@gmail.com',
-    url='https://github.com/eliasdorneles/usolitaire',
+    author_email="eliasdorneles@gmail.com",
+    url="https://github.com/eliasdorneles/usolitaire",
     entry_points={
-        'console_scripts': {
-            'usolitaire = usolitaire.app:main',
+        "console_scripts": {
+            "usolitaire = usolitaire.app:main",
         }
     },
     packages=[
-        'usolitaire',
+        "usolitaire",
     ],
-    package_dir={'usolitaire':
-                 'usolitaire'},
+    package_dir={"usolitaire": "usolitaire"},
     include_package_data=True,
     install_requires=requirements,
     license="MIT license",
     zip_safe=False,
-    keywords='usolitaire',
+    keywords="usolitaire",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `usolitaire-0.2.1/PKG-INFO` & `usolitaire-1.0.0/usolitaire.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: usolitaire
-Version: 0.2.1
+Version: 1.0.0
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
-Description: ===============================
-        usolitaire
-        ===============================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/usolitaire.svg
-                :target: https://pypi.python.org/pypi/usolitaire
-        
-        .. image:: https://img.shields.io/travis/eliasdorneles/usolitaire.svg
-                :target: https://travis-ci.org/eliasdorneles/usolitaire
-        
-        
-        Play solitaire in your terminal.
-        
-        Point and click to move cards.
-        
-        Install with:
-        
-            pip install usolitaire
-        
-        .. image:: https://raw.githubusercontent.com/eliasdorneles/usolitaire/master/screenshot-usolitaire.png
-        
-        
-        * Free software: MIT license
-        
 Keywords: usolitaire
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+===============================
+usolitaire
+===============================
+
+
+.. image:: https://img.shields.io/pypi/v/usolitaire.svg
+        :target: https://pypi.python.org/pypi/usolitaire
+
+.. image:: https://img.shields.io/travis/eliasdorneles/usolitaire.svg
+        :target: https://travis-ci.org/eliasdorneles/usolitaire
+
+
+Play solitaire in your terminal.
+
+Point and click to move cards, or use the keyboard shortcuts.
+
+Install with:
+
+    pip install usolitaire
+
+Run with:
+
+    usolitaire
+
+To run from sources, you can run with:
+
+    python -m usolitaire.app
+
+.. image:: https://raw.githubusercontent.com/eliasdorneles/usolitaire/master/screenshot-usolitaire.png
+
+* Free software: MIT license
+
+
+History
+-------
+
+I built the first version of this app in 2017 using the `urwid`_ library, while
+I was attending `Recurse Center`_.
+
+In 2023, after attending Europython and learning the `Textual`_ framework,
+which solved all the gripes I had with ``urwid`` before, I decided to rewrite
+it in Textual and added the features that were missing.
+
+.. _urwid: https://urwid.org
+.. _Recurse Center: https://www.recurse.com/
+.. _Textual: https://textual.textualize.io
```

