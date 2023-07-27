# Comparing `tmp/dbcc-0.0.1.dev1.tar.gz` & `tmp/dbcc-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbcc-0.0.1.dev1.tar", last modified: Thu Jul 27 10:38:51 2023, max compression
+gzip compressed data, was "dbcc-0.0.1.dev2.tar", last modified: Thu Jul 27 10:43:26 2023, max compression
```

## Comparing `dbcc-0.0.1.dev1.tar` & `dbcc-0.0.1.dev2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:38:51.911918 dbcc-0.0.1.dev1/
--rw-r--r--   0 valid_var   (501) staff       (20)      326 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev1/AUTHORS
--rw-r--r--   0 valid_var   (501) staff       (20)      319 2023-07-27 09:21:39.000000 dbcc-0.0.1.dev1/CHANGES.rst
--rw-r--r--   0 valid_var   (501) staff       (20)     1585 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev1/LICENSE
--rw-r--r--   0 valid_var   (501) staff       (20)      385 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev1/MANIFEST.in
--rw-r--r--   0 valid_var   (501) staff       (20)     2063 2023-07-27 10:38:51.911984 dbcc-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 valid_var   (501) staff       (20)      980 2023-07-27 10:38:19.000000 dbcc-0.0.1.dev1/README.rst
-drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:38:51.910769 dbcc-0.0.1.dev1/dbcc/
--rw-r--r--   0 valid_var   (501) staff       (20)      328 2023-07-27 09:15:33.000000 dbcc-0.0.1.dev1/dbcc/__init__.py
--rw-r--r--   0 valid_var   (501) staff       (20)      891 2023-07-27 09:15:33.000000 dbcc-0.0.1.dev1/dbcc/base.py
--rw-r--r--   0 valid_var   (501) staff       (20)     2056 2023-07-27 09:15:33.000000 dbcc-0.0.1.dev1/dbcc/mongodb.py
-drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:38:51.911795 dbcc-0.0.1.dev1/dbcc.egg-info/
--rw-r--r--   0 valid_var   (501) staff       (20)     2063 2023-07-27 10:38:51.000000 dbcc-0.0.1.dev1/dbcc.egg-info/PKG-INFO
--rw-r--r--   0 valid_var   (501) staff       (20)      269 2023-07-27 10:38:51.000000 dbcc-0.0.1.dev1/dbcc.egg-info/SOURCES.txt
--rw-r--r--   0 valid_var   (501) staff       (20)        1 2023-07-27 10:38:51.000000 dbcc-0.0.1.dev1/dbcc.egg-info/dependency_links.txt
--rw-r--r--   0 valid_var   (501) staff       (20)      144 2023-07-27 10:38:51.000000 dbcc-0.0.1.dev1/dbcc.egg-info/requires.txt
--rw-r--r--   0 valid_var   (501) staff       (20)        5 2023-07-27 10:38:51.000000 dbcc-0.0.1.dev1/dbcc.egg-info/top_level.txt
--rw-r--r--   0 valid_var   (501) staff       (20)       38 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev1/pyproject.toml
--rw-r--r--   0 valid_var   (501) staff       (20)       67 2023-07-27 10:38:51.912343 dbcc-0.0.1.dev1/setup.cfg
--rwxr-xr-x   0 valid_var   (501) staff       (20)     1940 2023-07-27 09:31:00.000000 dbcc-0.0.1.dev1/setup.py
+drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:43:26.777604 dbcc-0.0.1.dev2/
+-rw-r--r--   0 valid_var   (501) staff       (20)      326 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev2/AUTHORS
+-rw-r--r--   0 valid_var   (501) staff       (20)      319 2023-07-27 09:21:39.000000 dbcc-0.0.1.dev2/CHANGES.rst
+-rw-r--r--   0 valid_var   (501) staff       (20)     1585 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev2/LICENSE
+-rw-r--r--   0 valid_var   (501) staff       (20)      385 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev2/MANIFEST.in
+-rw-r--r--   0 valid_var   (501) staff       (20)     2019 2023-07-27 10:43:26.777685 dbcc-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0 valid_var   (501) staff       (20)      980 2023-07-27 10:38:19.000000 dbcc-0.0.1.dev2/README.rst
+drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:43:26.776491 dbcc-0.0.1.dev2/dbcc/
+-rw-r--r--   0 valid_var   (501) staff       (20)      328 2023-07-27 10:43:11.000000 dbcc-0.0.1.dev2/dbcc/__init__.py
+-rw-r--r--   0 valid_var   (501) staff       (20)      891 2023-07-27 09:15:33.000000 dbcc-0.0.1.dev2/dbcc/base.py
+-rw-r--r--   0 valid_var   (501) staff       (20)     2056 2023-07-27 09:15:33.000000 dbcc-0.0.1.dev2/dbcc/mongodb.py
+drwxr-xr-x   0 valid_var   (501) staff       (20)        0 2023-07-27 10:43:26.777464 dbcc-0.0.1.dev2/dbcc.egg-info/
+-rw-r--r--   0 valid_var   (501) staff       (20)     2019 2023-07-27 10:43:26.000000 dbcc-0.0.1.dev2/dbcc.egg-info/PKG-INFO
+-rw-r--r--   0 valid_var   (501) staff       (20)      269 2023-07-27 10:43:26.000000 dbcc-0.0.1.dev2/dbcc.egg-info/SOURCES.txt
+-rw-r--r--   0 valid_var   (501) staff       (20)        1 2023-07-27 10:43:26.000000 dbcc-0.0.1.dev2/dbcc.egg-info/dependency_links.txt
+-rw-r--r--   0 valid_var   (501) staff       (20)      144 2023-07-27 10:43:26.000000 dbcc-0.0.1.dev2/dbcc.egg-info/requires.txt
+-rw-r--r--   0 valid_var   (501) staff       (20)        5 2023-07-27 10:43:26.000000 dbcc-0.0.1.dev2/dbcc.egg-info/top_level.txt
+-rw-r--r--   0 valid_var   (501) staff       (20)       38 2023-07-27 08:42:13.000000 dbcc-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0 valid_var   (501) staff       (20)       67 2023-07-27 10:43:26.777896 dbcc-0.0.1.dev2/setup.cfg
+-rwxr-xr-x   0 valid_var   (501) staff       (20)     1896 2023-07-27 10:42:28.000000 dbcc-0.0.1.dev2/setup.py
```

### Comparing `dbcc-0.0.1.dev1/LICENSE` & `dbcc-0.0.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbcc-0.0.1.dev1/PKG-INFO` & `dbcc-0.0.1.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbcc
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Database connector.
-Home-page: http://dbcc.startech.live
+Home-page: https://github.com/Profi-Devs/dbcc
 Author: Stepan Starovoitov
 Author-email: stepan.startech@gmail.com
 License: BSD
-Project-URL: Code, https://git.the-devs.com/opensource/py-modules/database-connector/database-connector
-Project-URL: Issue tracker, https://github.com/startech-live/teev/issues
+Project-URL: Code, https://github.com/Profi-Devs/dbcc
+Project-URL: Issue tracker, https://github.com/Profi-Devs/dbcc/issues
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dbcc-0.0.1.dev1/README.rst` & `dbcc-0.0.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `dbcc-0.0.1.dev1/dbcc/base.py` & `dbcc-0.0.1.dev2/dbcc/base.py`

 * *Files identical despite different names*

### Comparing `dbcc-0.0.1.dev1/dbcc/mongodb.py` & `dbcc-0.0.1.dev2/dbcc/mongodb.py`

 * *Files identical despite different names*

### Comparing `dbcc-0.0.1.dev1/dbcc.egg-info/PKG-INFO` & `dbcc-0.0.1.dev2/dbcc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbcc
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
 Summary: Database connector.
-Home-page: http://dbcc.startech.live
+Home-page: https://github.com/Profi-Devs/dbcc
 Author: Stepan Starovoitov
 Author-email: stepan.startech@gmail.com
 License: BSD
-Project-URL: Code, https://git.the-devs.com/opensource/py-modules/database-connector/database-connector
-Project-URL: Issue tracker, https://github.com/startech-live/teev/issues
+Project-URL: Code, https://github.com/Profi-Devs/dbcc
+Project-URL: Issue tracker, https://github.com/Profi-Devs/dbcc/issues
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dbcc-0.0.1.dev1/setup.py` & `dbcc-0.0.1.dev2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,20 +27,20 @@
     name="dbcc",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     author="Stepan Starovoitov",
     author_email="stepan.startech@gmail.com",
-    url="http://dbcc.startech.live",
+    url="https://github.com/Profi-Devs/dbcc",
     project_urls=OrderedDict(
         (
             # ("Documentation", "http://teev.startech.live"),
-            ("Code", "https://git.the-devs.com/opensource/py-modules/database-connector/database-connector"),
-            ("Issue tracker", "https://github.com/startech-live/teev/issues"),
+            ("Code", "https://github.com/Profi-Devs/dbcc"),
+            ("Issue tracker", "https://github.com/Profi-Devs/dbcc/issues"),
         )
     ),
     license="BSD",
     platforms=["any"],
     packages=find_packages(),
     # test_suite="dbcc.tests",
     install_requires=INSTALL_REQUIRES,
```

