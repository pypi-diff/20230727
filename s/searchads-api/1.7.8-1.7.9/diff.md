# Comparing `tmp/searchads_api-1.7.8.tar.gz` & `tmp/searchads_api-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchads_api-1.7.8.tar", last modified: Wed Jul 26 08:11:45 2023, max compression
+gzip compressed data, was "searchads_api-1.7.9.tar", last modified: Thu Jul 27 08:24:53 2023, max compression
```

## Comparing `searchads_api-1.7.8.tar` & `searchads_api-1.7.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.422456 searchads_api-1.7.8/
--rw-r--r--   0 alkattan   (501) staff       (20)     1055 2021-04-15 17:45:24.000000 searchads_api-1.7.8/LICENSE
--rw-r--r--   0 alkattan   (501) staff       (20)     2485 2023-07-26 08:11:45.422761 searchads_api-1.7.8/PKG-INFO
--rw-r--r--   0 alkattan   (501) staff       (20)    14059 2023-03-30 00:14:00.000000 searchads_api-1.7.8/README.md
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.414553 searchads_api-1.7.8/searchads_api/
--rw-r--r--   0 alkattan   (501) staff       (20)       30 2022-09-04 20:49:59.000000 searchads_api-1.7.8/searchads_api/__init__.py
--rw-r--r--   0 alkattan   (501) staff       (20)    68689 2023-03-29 21:15:26.000000 searchads_api-1.7.8/searchads_api/api.py
-drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-26 08:11:45.421596 searchads_api-1.7.8/searchads_api.egg-info/
--rw-r--r--   0 alkattan   (501) staff       (20)     2485 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/PKG-INFO
--rw-r--r--   0 alkattan   (501) staff       (20)      267 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/SOURCES.txt
--rw-r--r--   0 alkattan   (501) staff       (20)        1 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/dependency_links.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       51 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/requires.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       14 2023-07-26 08:11:45.000000 searchads_api-1.7.8/searchads_api.egg-info/top_level.txt
--rw-r--r--   0 alkattan   (501) staff       (20)       79 2023-07-26 08:11:45.424143 searchads_api-1.7.8/setup.cfg
--rw-r--r--   0 alkattan   (501) staff       (20)     2687 2023-07-26 08:11:21.000000 searchads_api-1.7.8/setup.py
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-27 08:24:53.119143 searchads_api-1.7.9/
+-rw-r--r--   0 alkattan   (501) staff       (20)     1055 2021-04-15 17:45:24.000000 searchads_api-1.7.9/LICENSE
+-rw-r--r--   0 alkattan   (501) staff       (20)     2544 2023-07-27 08:24:53.119339 searchads_api-1.7.9/PKG-INFO
+-rw-r--r--   0 alkattan   (501) staff       (20)    14059 2023-03-30 00:14:00.000000 searchads_api-1.7.9/README.md
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-27 08:24:53.113144 searchads_api-1.7.9/searchads_api/
+-rw-r--r--   0 alkattan   (501) staff       (20)       30 2022-09-04 20:49:59.000000 searchads_api-1.7.9/searchads_api/__init__.py
+-rw-r--r--   0 alkattan   (501) staff       (20)    68689 2023-03-29 21:15:26.000000 searchads_api-1.7.9/searchads_api/api.py
+drwxr-xr-x   0 alkattan   (501) staff       (20)        0 2023-07-27 08:24:53.118548 searchads_api-1.7.9/searchads_api.egg-info/
+-rw-r--r--   0 alkattan   (501) staff       (20)     2544 2023-07-27 08:24:53.000000 searchads_api-1.7.9/searchads_api.egg-info/PKG-INFO
+-rw-r--r--   0 alkattan   (501) staff       (20)      267 2023-07-27 08:24:53.000000 searchads_api-1.7.9/searchads_api.egg-info/SOURCES.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)        1 2023-07-27 08:24:53.000000 searchads_api-1.7.9/searchads_api.egg-info/dependency_links.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       43 2023-07-27 08:24:53.000000 searchads_api-1.7.9/searchads_api.egg-info/requires.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       14 2023-07-27 08:24:53.000000 searchads_api-1.7.9/searchads_api.egg-info/top_level.txt
+-rw-r--r--   0 alkattan   (501) staff       (20)       79 2023-07-27 08:24:53.120125 searchads_api-1.7.9/setup.cfg
+-rw-r--r--   0 alkattan   (501) staff       (20)     2738 2023-07-27 08:24:41.000000 searchads_api-1.7.9/setup.py
```

### Comparing `searchads_api-1.7.8/LICENSE` & `searchads_api-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `searchads_api-1.7.8/PKG-INFO` & `searchads_api-1.7.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchads_api
-Version: 1.7.8
+Version: 1.7.9
 Summary: Apple Searchads API non-official python library
 Home-page: https://github.com/phiture/searchads_api
 Author: Abdul Majeed Alkattan
 Author-email: alkattan@phiture.com
 Keywords: python,searchads,library
 License-File: LICENSE
 
@@ -39,15 +39,15 @@
 
 ### Campaign Methods
 
 - Create a new campaign
 
          res = api.create_campaign(1433439534, ['AU'], "test", 1, 1, "EUR")
 
-Backlog
+## Changelog
 
 version 0.1.1 Added granularity level reports
 
 version 0.7.1 fixed some issues with granularity
 
 version 1.1.1 added support for the v4 of the Apple Search Ads API
 
@@ -64,8 +64,10 @@
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
 
 version 1.7.8 updated the dependencies
+
+version 1.7.9 always use the latest requests package
```

### Comparing `searchads_api-1.7.8/README.md` & `searchads_api-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `searchads_api-1.7.8/searchads_api/api.py` & `searchads_api-1.7.9/searchads_api/api.py`

 * *Files identical despite different names*

### Comparing `searchads_api-1.7.8/searchads_api.egg-info/PKG-INFO` & `searchads_api-1.7.9/searchads_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchads-api
-Version: 1.7.8
+Version: 1.7.9
 Summary: Apple Searchads API non-official python library
 Home-page: https://github.com/phiture/searchads_api
 Author: Abdul Majeed Alkattan
 Author-email: alkattan@phiture.com
 Keywords: python,searchads,library
 License-File: LICENSE
 
@@ -39,15 +39,15 @@
 
 ### Campaign Methods
 
 - Create a new campaign
 
          res = api.create_campaign(1433439534, ['AU'], "test", 1, 1, "EUR")
 
-Backlog
+## Changelog
 
 version 0.1.1 Added granularity level reports
 
 version 0.7.1 fixed some issues with granularity
 
 version 1.1.1 added support for the v4 of the Apple Search Ads API
 
@@ -64,8 +64,10 @@
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
 
 version 1.7.8 updated the dependencies
+
+version 1.7.9 always use the latest requests package
```

### Comparing `searchads_api-1.7.8/setup.py` & `searchads_api-1.7.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 from setuptools import setup
 
 setup(
     name='searchads_api',
     description='Apple Searchads API non-official python library',
-    version='1.7.8',
+    version='1.7.9',
     url='https://github.com/phiture/searchads_api',
     author='Abdul Majeed Alkattan',
     author_email='alkattan@phiture.com',
     packages=["searchads_api"], 
     keywords=['python','searchads','library'],
-    install_requires=['requests>=2.31.0', 'PyJWT==2.8.0', 'cryptography==41.0.2'],
+    install_requires=['requests', 'PyJWT==2.8.0', 'cryptography==41.0.2'],
     long_description="""
 
 # About Phiture
 
 http://phiture.com is a Berlin-based mobile growth consultancy working with the teams behind leading apps. Using the company’s industry-acclaimed Mobile Growth Stack as a strategic framework, Phiture team offers 4 key services: App Store Optimization, Apple Search Ads, User Retention services and Growth Consulting.
 
 
@@ -42,15 +42,15 @@
 
 ### Campaign Methods
 
 - Create a new campaign
 
          res = api.create_campaign(1433439534, ['AU'], "test", 1, 1, "EUR")
 
-Backlog
+## Changelog
 
 version 0.1.1 Added granularity level reports
 
 version 0.7.1 fixed some issues with granularity
 
 version 1.1.1 added support for the v4 of the Apple Search Ads API
 
@@ -67,9 +67,11 @@
 version 1.7.1 added impression share reports and new find methods along product pages to match Searchads API version 4.7
 
 version 1.7.6 fixed an issue with token update
 
 version 1.7.7 fixed an issue update_campaign
 
 version 1.7.8 updated the dependencies
+
+version 1.7.9 always use the latest requests package
     """,
 )
```

