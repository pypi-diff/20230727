# Comparing `tmp/checklib-0.5.2.tar.gz` & `tmp/checklib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/checklib-0.5.2.tar", last modified: Wed Oct 14 10:11:12 2020, max compression
+gzip compressed data, was "checklib-0.6.0.tar", last modified: Thu Jul 27 15:47:04 2023, max compression
```

## Comparing `checklib-0.5.2.tar` & `checklib-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxr-xr-x   0 nikrom     (501) staff       (20)        0 2020-10-14 10:11:12.000000 checklib-0.5.2/
--rw-r--r--   0 nikrom     (501) staff       (20)      717 2020-10-14 10:11:12.000000 checklib-0.5.2/PKG-INFO
-drwxr-xr-x   0 nikrom     (501) staff       (20)        0 2020-10-14 10:11:12.000000 checklib-0.5.2/checklib/
--rw-r--r--   0 nikrom     (501) staff       (20)      645 2020-02-01 17:53:16.000000 checklib-0.5.2/checklib/__init__.py
--rw-r--r--   0 nikrom     (501) staff       (20)     3214 2020-10-13 06:24:53.000000 checklib-0.5.2/checklib/assertions.py
--rw-r--r--   0 nikrom     (501) staff       (20)     2319 2020-10-14 06:35:43.000000 checklib-0.5.2/checklib/checker.py
--rw-r--r--   0 nikrom     (501) staff       (20)      970 2020-10-13 06:32:01.000000 checklib-0.5.2/checklib/generators.py
--rw-r--r--   0 nikrom     (501) staff       (20)     2071 2020-10-13 06:32:47.000000 checklib-0.5.2/checklib/http.py
--rw-r--r--   0 nikrom     (501) staff       (20)      164 2020-10-13 06:32:01.000000 checklib-0.5.2/checklib/internal.py
-drwxr-xr-x   0 nikrom     (501) staff       (20)        0 2020-10-14 10:11:12.000000 checklib-0.5.2/checklib/resources/
--rw-r--r--   0 nikrom     (501) staff       (20)   693918 2019-09-11 06:57:03.000000 checklib-0.5.2/checklib/resources/useragents.txt
--rw-r--r--   0 nikrom     (501) staff       (20)    70338 2019-10-25 20:56:57.000000 checklib-0.5.2/checklib/resources/usernames.txt
--rw-r--r--   0 nikrom     (501) staff       (20)      182 2019-09-11 06:59:35.000000 checklib-0.5.2/checklib/status.py
--rw-r--r--   0 nikrom     (501) staff       (20)      674 2020-10-13 06:32:01.000000 checklib-0.5.2/checklib/utils.py
--rw-r--r--   0 nikrom     (501) staff       (20)       61 2019-09-11 07:16:14.000000 checklib-0.5.2/setup.cfg
--rw-r--r--   0 nikrom     (501) staff       (20)      916 2020-10-14 10:10:58.000000 checklib-0.5.2/setup.py
+drwxr-xr-x   0 rnikitin   (501) staff       (20)        0 2023-07-27 15:47:04.939912 checklib-0.6.0/
+-rw-r--r--   0 rnikitin   (501) staff       (20)     1068 2023-07-27 15:27:36.000000 checklib-0.6.0/LICENCE
+-rw-r--r--   0 rnikitin   (501) staff       (20)      702 2023-07-27 15:47:04.939961 checklib-0.6.0/PKG-INFO
+-rw-r--r--   0 rnikitin   (501) staff       (20)      998 2023-07-27 15:27:36.000000 checklib-0.6.0/README.md
+drwxr-xr-x   0 rnikitin   (501) staff       (20)        0 2023-07-27 15:47:04.938604 checklib-0.6.0/checklib/
+-rw-r--r--   0 rnikitin   (501) staff       (20)      822 2023-07-27 15:42:20.000000 checklib-0.6.0/checklib/__init__.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)     3214 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/assertions.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)     2319 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/checker.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)      970 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/generators.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)     2071 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/http.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)      164 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/internal.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)      916 2023-07-27 15:42:20.000000 checklib-0.6.0/checklib/requirements.py
+drwxr-xr-x   0 rnikitin   (501) staff       (20)        0 2023-07-27 15:47:04.939764 checklib-0.6.0/checklib/resources/
+-rw-r--r--   0 rnikitin   (501) staff       (20)   693918 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/resources/useragents.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)    70338 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/resources/usernames.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)      182 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/status.py
+-rw-r--r--   0 rnikitin   (501) staff       (20)      674 2023-07-27 15:27:36.000000 checklib-0.6.0/checklib/utils.py
+drwxr-xr-x   0 rnikitin   (501) staff       (20)        0 2023-07-27 15:47:04.939148 checklib-0.6.0/checklib.egg-info/
+-rw-r--r--   0 rnikitin   (501) staff       (20)      702 2023-07-27 15:47:04.000000 checklib-0.6.0/checklib.egg-info/PKG-INFO
+-rw-r--r--   0 rnikitin   (501) staff       (20)      449 2023-07-27 15:47:04.000000 checklib-0.6.0/checklib.egg-info/SOURCES.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)        1 2023-07-27 15:47:04.000000 checklib-0.6.0/checklib.egg-info/dependency_links.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)       21 2023-07-27 15:47:04.000000 checklib-0.6.0/checklib.egg-info/requires.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)        9 2023-07-27 15:47:04.000000 checklib-0.6.0/checklib.egg-info/top_level.txt
+-rw-r--r--   0 rnikitin   (501) staff       (20)       79 2023-07-27 15:47:04.940132 checklib-0.6.0/setup.cfg
+-rw-r--r--   0 rnikitin   (501) staff       (20)      941 2023-07-27 15:44:15.000000 checklib-0.6.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `checklib-0.5.2/PKG-INFO` & `checklib-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: checklib
-Version: 0.5.2
+Version: 0.6.0
 Summary: Library for convenient checker writing
 Home-page: https://github.com/pomo-mondreganto/
+Download-URL: https://github.com/pomo-mondreganto/checklib/archive/v_0.6.0.tar.gz
 Author: Roman Nikitin
 Author-email: nikrom.prog@gmail.com
 License: MIT
-Download-URL: https://github.com/pomo-mondreganto/checklib/archive/v_0.5.2.tar.gz
-Description: UNKNOWN
 Keywords: AD,CTF,checker
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENCE
```

### Comparing `checklib-0.5.2/checklib/__init__.py` & `checklib-0.6.0/checklib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,13 @@
 from checklib.status import (
     Status,
 )
 from checklib.utils import (
     cquit,
     handle_exception,
 )
+from checklib.requirements import (
+    assert_command_executed,
+    assert_pip_packages_installed,
+    assert_sage_pip_packages_installed,
+    assert_apt_packages_installed,
+)
```

### Comparing `checklib-0.5.2/checklib/assertions.py` & `checklib-0.6.0/checklib/assertions.py`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/checker.py` & `checklib-0.6.0/checklib/checker.py`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/generators.py` & `checklib-0.6.0/checklib/generators.py`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/http.py` & `checklib-0.6.0/checklib/http.py`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/resources/useragents.txt` & `checklib-0.6.0/checklib/resources/useragents.txt`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/resources/usernames.txt` & `checklib-0.6.0/checklib/resources/usernames.txt`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/checklib/utils.py` & `checklib-0.6.0/checklib/utils.py`

 * *Files identical despite different names*

### Comparing `checklib-0.5.2/setup.py` & `checklib-0.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 setup(
     name='checklib',
     packages=['checklib'],
     package_data={
         'checklib': ['resources/*']
     },
-    version='0.5.2',
+    version='0.6.0',
     license='MIT',
     description='Library for convenient checker writing',
     author='Roman Nikitin',
     author_email='nikrom.prog@gmail.com',
     url='https://github.com/pomo-mondreganto/',
-    download_url='https://github.com/pomo-mondreganto/checklib/archive/v_0.5.2.tar.gz',
+    download_url='https://github.com/pomo-mondreganto/checklib/archive/v_0.6.0.tar.gz',
     keywords=['AD', 'CTF', 'checker'],
     install_requires=[
         'requests',
+        'portalocker',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

