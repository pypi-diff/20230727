# Comparing `tmp/latch-sdk-gql-0.0.2.tar.gz` & `tmp/latch-sdk-gql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-sdk-gql-0.0.2.tar", last modified: Thu Jun 22 20:30:56 2023, max compression
+gzip compressed data, was "latch-sdk-gql-0.0.3.tar", last modified: Thu Jul 27 20:45:24 2023, max compression
```

## Comparing `latch-sdk-gql-0.0.2.tar` & `latch-sdk-gql-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.354830 latch-sdk-gql-0.0.2/
--rw-r--r--   0 ayush      (504) staff       (20)     1065 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.2/LICENSE
--rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:30:56.354445 latch-sdk-gql-0.0.2/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)       15 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.2/README.md
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.351374 latch-sdk-gql-0.0.2/latch_sdk_gql/
--rw-r--r--   0 ayush      (504) staff       (20)      442 2023-06-22 20:29:14.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     1319 2023-06-22 20:29:26.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/execute.py
--rw-r--r--   0 ayush      (504) staff       (20)     2233 2023-06-22 20:02:17.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.353911 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/
--rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)      284 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/SOURCES.txt
--rw-r--r--   0 ayush      (504) staff       (20)        1 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/dependency_links.txt
--rw-r--r--   0 ayush      (504) staff       (20)       81 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/requires.txt
--rw-r--r--   0 ayush      (504) staff       (20)       14 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/top_level.txt
--rw-r--r--   0 ayush      (504) staff       (20)       38 2023-06-22 20:30:56.354948 latch-sdk-gql-0.0.2/setup.cfg
--rw-r--r--   0 ayush      (504) staff       (20)      608 2023-06-22 20:29:50.000000 latch-sdk-gql-0.0.2/setup.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:45:24.025397 latch-sdk-gql-0.0.3/
+-rw-r--r--   0 aidan      (501) staff       (20)     1065 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.3/LICENSE
+-rw-r--r--   0 aidan      (501) staff       (20)      376 2023-07-27 20:45:24.025126 latch-sdk-gql-0.0.3/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)       15 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.3/README.md
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:45:24.023548 latch-sdk-gql-0.0.3/latch_sdk_gql/
+-rw-r--r--   0 aidan      (501) staff       (20)       49 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.3/latch_sdk_gql/__init__.py
+-rw-r--r--   0 aidan      (501) staff       (20)     1343 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.3/latch_sdk_gql/_execute.py
+-rw-r--r--   0 aidan      (501) staff       (20)     2233 2023-07-27 20:34:48.000000 latch-sdk-gql-0.0.3/latch_sdk_gql/_utils.py
+drwxr-xr-x   0 aidan      (501) staff       (20)        0 2023-07-27 20:45:24.024820 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/
+-rw-r--r--   0 aidan      (501) staff       (20)      376 2023-07-27 20:45:24.000000 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/PKG-INFO
+-rw-r--r--   0 aidan      (501) staff       (20)      286 2023-07-27 20:45:24.000000 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/SOURCES.txt
+-rw-r--r--   0 aidan      (501) staff       (20)        1 2023-07-27 20:45:24.000000 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/dependency_links.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       57 2023-07-27 20:45:24.000000 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/requires.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       14 2023-07-27 20:45:24.000000 latch-sdk-gql-0.0.3/latch_sdk_gql.egg-info/top_level.txt
+-rw-r--r--   0 aidan      (501) staff       (20)       38 2023-07-27 20:45:24.025480 latch-sdk-gql-0.0.3/setup.cfg
+-rw-r--r--   0 aidan      (501) staff       (20)      623 2023-07-27 20:43:08.000000 latch-sdk-gql-0.0.3/setup.py
```

### Comparing `latch-sdk-gql-0.0.2/LICENSE` & `latch-sdk-gql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.2/latch_sdk_gql/execute.py` & `latch-sdk-gql-0.0.3/latch_sdk_gql/_execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,19 @@
     from functools import lru_cache as cache
 
 from typing import Dict, Optional
 
 import gql
 from gql.transport.requests import RequestsHTTPTransport
 from graphql import DocumentNode
-from latch_sdk_config.latch import config
-from latch_sdk_config.user import user_config
 
-from latch_sdk_gql import AuthenticationError, JsonValue
+from latch.gql import AuthenticationError
+from latch.types.json import JsonValue
+from latch_cli.config.latch import config
+from latch_cli.config.user import user_config
 
 
 @cache
 def _get_client():
     auth_header: Optional[str] = None
 
     if auth_header is None:
```

### Comparing `latch-sdk-gql-0.0.2/latch_sdk_gql/utils.py` & `latch-sdk-gql-0.0.3/latch_sdk_gql/_utils.py`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.2/setup.py` & `latch-sdk-gql-0.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(
     name="latch-sdk-gql",
-    version="v0.0.2",
+    version="v0.0.3",
     author_email="ayush@latch.bio",
     description="Internal Latch GQL package",
     packages=find_packages(),
     include_package_data=True,
-    python_requires=">=3.8,<3.11",
+    python_requires=">=3.8,<3.12",
     install_requires=[
-        "latch-sdk-config==0.0.1",
         "gql==3.4.0",
         "graphql-core==3.2.3",
         "requests-toolbelt==0.10.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

