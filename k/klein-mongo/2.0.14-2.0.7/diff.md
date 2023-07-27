# Comparing `tmp/klein_mongo-2.0.14.tar.gz` & `tmp/klein_mongo-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/klein_mongo-2.0.14.tar", last modified: Thu Jul 27 10:17:19 2023, max compression
+gzip compressed data, was "dist/klein_mongo-2.0.7.tar", last modified: Mon May 30 07:45:58 2022, max compression
```

## Comparing `klein_mongo-2.0.14.tar` & `klein_mongo-2.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/
--rw-rw-rw-   0 root         (0) root         (0)     9135 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1198 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1569 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/src/klein_mongo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3567 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/src/klein_mongo/connect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1198 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/src/klein_mongo.egg-info/zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/src/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 10:17:19.000000 klein_mongo-2.0.14/test/
--rw-rw-rw-   0 root         (0) root         (0)     2766 2023-07-27 10:16:59.000000 klein_mongo-2.0.14/test/test_connect.py
+drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     9135 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/LICENSE.txt
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       17 2022-05-23 09:20:55.000000 klein_mongo-2.0.7/MANIFEST.in
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1197 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/PKG-INFO
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)      867 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/README.md
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       38 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/setup.cfg
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1535 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/setup.py
+drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/
+drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo/
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       62 2022-05-23 09:20:55.000000 klein_mongo-2.0.7/src/klein_mongo/__init__.py
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     3216 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/src/klein_mongo/connect.py
+drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1197 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)      346 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        1 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       37 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/requires.txt
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       12 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/top_level.txt
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        1 2022-05-30 07:45:15.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/zip-safe
+drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/test/
+-rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     2766 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/test/test_connect.py
```

### Comparing `klein_mongo-2.0.14/LICENSE.txt` & `klein_mongo-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klein_mongo-2.0.14/PKG-INFO` & `klein_mongo-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klein_mongo
-Version: 2.0.14
+Version: 2.0.7
 Summary: MongoDB integration
 Home-page: https://github.com/mdcatapult/py-mongo
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `klein_mongo-2.0.14/README.md` & `klein_mongo-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `klein_mongo-2.0.14/setup.py` & `klein_mongo-2.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,12 +36,11 @@
       url='https://github.com/mdcatapult/py-mongo',
       author='Medicines Discovery Catapult',
       author_email='SoftwareEngineering@md.catapult.org.uk',
       license='Apache V2',
       packages=find_packages('src'),
       package_dir={'':'src'},
       install_requires=[
-          'klein_config>=3.0',
-          'pymongo[srv]>=4.4.1',
+          'klein_config~=3.0',
+          'pymongo[srv]~=3.11',
       ],
-      zip_safe=True,
-      include_package_data=True)
+      zip_safe=True)
```

### Comparing `klein_mongo-2.0.14/src/klein_mongo/connect.py` & `klein_mongo-2.0.7/src/klein_mongo/connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,19 +76,14 @@
         self.params["readPreference"] = config.get('mongo.readPreference', 'secondaryPreferred')
 
         # Use cross language compatible UUID encoding as default. Can be overridden with
         # 'pythonLegacy', 'javaLegacy' or 'csharpLegacy' if required.
         # ref: https://api.mongodb.com/python/current/api/pymongo/mongo_client.html?
         self.params['uuidRepresentation'] = config.get('mongo.uuidRepresentation', 'standard')
 
-        # There are some data with strings that cannot be handled by unicode
-        # This may cause an error during query
-        # Default this to ignore as there is no known good way to handle this other than ignoring corrupted data
-        self.params['unicode_decode_error_handler'] = config.get('mongo.unicode_decode_error_handler', 'ignore')
-
     @lazy_property
     def client(self):
         c = _MongoClient(*self.host, replicaset=self.replicaSet, **self.params)
         return c
 
 
 def get_client(config):
```

### Comparing `klein_mongo-2.0.14/src/klein_mongo.egg-info/PKG-INFO` & `klein_mongo-2.0.7/src/klein_mongo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klein-mongo
-Version: 2.0.14
+Version: 2.0.7
 Summary: MongoDB integration
 Home-page: https://github.com/mdcatapult/py-mongo
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `klein_mongo-2.0.14/test/test_connect.py` & `klein_mongo-2.0.7/test/test_connect.py`

 * *Files identical despite different names*

