# Comparing `tmp/latch-sdk-gql-0.0.4.tar.gz` & `tmp/latch-sdk-gql-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-sdk-gql-0.0.4.tar", last modified: Thu Jul 27 21:28:28 2023, max compression
+gzip compressed data, was "latch-sdk-gql-0.0.5.tar", last modified: Thu Jul 27 21:29:53 2023, max compression
```

## Comparing `latch-sdk-gql-0.0.4.tar` & `latch-sdk-gql-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:28:28.627274 latch-sdk-gql-0.0.4/
--rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.4/LICENSE
--rw-r--r--   0 aidan      (501) staff       (20)      440 2023-07-27 21:28:28.627025 latch-sdk-gql-0.0.4/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)       15 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.4/README.md
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:28:28.625415 latch-sdk-gql-0.0.4/latch_sdk_gql/
--rw-r--r--   0 aidan      (501) staff       (20)      442 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.4/latch_sdk_gql/__init__.py
--rw-r--r--   0 aidan      (501) staff       (20)     1319 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.4/latch_sdk_gql/execute.py
--rw-r--r--   0 aidan      (501) staff       (20)     2233 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.4/latch_sdk_gql/utils.py
-drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:28:28.626709 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/
--rw-r--r--   0 aidan      (501) staff       (20)      440 2023-07-27 21:28:28.000000 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/PKG-INFO
--rw-r--r--   0 aidan      (501) staff       (20)      284 2023-07-27 21:28:28.000000 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/SOURCES.txt
--rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 21:28:28.000000 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/dependency_links.txt
--rw-r--r--   0 aidan      (501) staff       (20)       81 2023-07-27 21:28:28.000000 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/requires.txt
--rw-r--r--   0 aidan      (501) staff       (20)       14 2023-07-27 21:28:28.000000 latch-sdk-gql-0.0.4/latch_sdk_gql.egg-info/top_level.txt
--rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 21:28:28.627355 latch-sdk-gql-0.0.4/setup.cfg
--rw-r--r--   0 aidan      (501) staff       (20)      658 2023-07-27 21:27:52.000000 latch-sdk-gql-0.0.4/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:29:53.074429 latch-sdk-gql-0.0.5/
+-rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.5/LICENSE
+-rw-r--r--   0 aidan      (501) staff       (20)      440 2023-07-27 21:29:53.074164 latch-sdk-gql-0.0.5/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)       15 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.5/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:29:53.071948 latch-sdk-gql-0.0.5/latch_sdk_gql/
+-rw-r--r--   0 aidan      (501) staff       (20)      442 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.5/latch_sdk_gql/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     1319 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.5/latch_sdk_gql/execute.py
+-rw-r--r--   0 aidan      (501) staff       (20)     2233 2023-07-27 21:27:25.000000 latch-sdk-gql-0.0.5/latch_sdk_gql/utils.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 21:29:53.073775 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      440 2023-07-27 21:29:53.000000 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      284 2023-07-27 21:29:53.000000 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 21:29:53.000000 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       81 2023-07-27 21:29:53.000000 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/requires.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       14 2023-07-27 21:29:53.000000 latch-sdk-gql-0.0.5/latch_sdk_gql.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 21:29:53.074507 latch-sdk-gql-0.0.5/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)      658 2023-07-27 21:29:49.000000 latch-sdk-gql-0.0.5/setup.py
```

### Comparing `latch-sdk-gql-0.0.4/LICENSE` & `latch-sdk-gql-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.4/latch_sdk_gql/execute.py` & `latch-sdk-gql-0.0.5/latch_sdk_gql/execute.py`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.4/latch_sdk_gql/utils.py` & `latch-sdk-gql-0.0.5/latch_sdk_gql/utils.py`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.4/setup.py` & `latch-sdk-gql-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="latch-sdk-gql",
-    version="v0.0.4",
+    version="v0.0.5",
     author_email="ayush@latch.bio",
     description="Internal Latch GQL package",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8,<3.12",
     install_requires=[
-        "latch-sdk-config==0.0.1",
+        "latch-sdk-config==0.0.2",
         "gql==3.4.0",
         "graphql-core==3.2.3",
         "requests-toolbelt==0.10.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

