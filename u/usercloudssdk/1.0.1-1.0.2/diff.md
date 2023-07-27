# Comparing `tmp/usercloudssdk-1.0.1.tar.gz` & `tmp/usercloudssdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usercloudssdk-1.0.1.tar", last modified: Thu Jul 27 13:35:34 2023, max compression
+gzip compressed data, was "usercloudssdk-1.0.2.tar", last modified: Thu Jul 27 13:40:15 2023, max compression
```

## Comparing `usercloudssdk-1.0.1.tar` & `usercloudssdk-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:35:34.185524 usercloudssdk-1.0.1/
--rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-07-27 00:46:25.000000 usercloudssdk-1.0.1/LICENSE
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:35:34.185376 usercloudssdk-1.0.1/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.1/README.md
--rw-r--r--   0 jwang      (501) staff       (20)      380 2023-07-27 13:34:45.000000 usercloudssdk-1.0.1/pyproject.toml
--rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-27 13:35:34.185567 usercloudssdk-1.0.1/setup.cfg
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:35:34.181919 usercloudssdk-1.0.1/src/
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:35:34.184589 usercloudssdk-1.0.1/src/usercloudssdk/
--rw-r--r--   0 jwang      (501) staff       (20)        0 2023-06-13 16:36:00.000000 usercloudssdk-1.0.1/src/usercloudssdk/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)    17689 2023-07-27 13:23:56.000000 usercloudssdk-1.0.1/src/usercloudssdk/client.py
--rw-r--r--   0 jwang      (501) staff       (20)      636 2023-06-30 17:46:25.000000 usercloudssdk-1.0.1/src/usercloudssdk/constants.py
--rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-07-27 13:23:37.000000 usercloudssdk-1.0.1/src/usercloudssdk/models.py
--rw-r--r--   0 jwang      (501) staff       (20)      790 2023-07-27 13:34:23.000000 usercloudssdk-1.0.1/src/usercloudssdk/policies.py
--rw-r--r--   0 jwang      (501) staff       (20)     6377 2023-07-27 13:28:09.000000 usercloudssdk-1.0.1/src/usercloudssdk/tokenizer_sample.py
--rw-r--r--   0 jwang      (501) staff       (20)      405 2023-06-13 16:36:00.000000 usercloudssdk-1.0.1/src/usercloudssdk/ucjson.py
--rw-r--r--   0 jwang      (501) staff       (20)    11160 2023-07-27 13:28:36.000000 usercloudssdk-1.0.1/src/usercloudssdk/userstore_sample.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:35:34.185202 usercloudssdk-1.0.1/src/usercloudssdk.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:35:34.000000 usercloudssdk-1.0.1/src/usercloudssdk.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      447 2023-07-27 13:35:34.000000 usercloudssdk-1.0.1/src/usercloudssdk.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-27 13:35:34.000000 usercloudssdk-1.0.1/src/usercloudssdk.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)       14 2023-07-27 13:35:34.000000 usercloudssdk-1.0.1/src/usercloudssdk.egg-info/top_level.txt
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.431465 usercloudssdk-1.0.2/
+-rw-r--r--   0 jwang      (501) staff       (20)     1103 2023-07-27 00:46:25.000000 usercloudssdk-1.0.2/LICENSE
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:40:15.431352 usercloudssdk-1.0.2/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)       12 2023-07-27 00:40:23.000000 usercloudssdk-1.0.2/README.md
+-rw-r--r--   0 jwang      (501) staff       (20)      380 2023-07-27 13:39:01.000000 usercloudssdk-1.0.2/pyproject.toml
+-rw-r--r--   0 jwang      (501) staff       (20)       38 2023-07-27 13:40:15.431499 usercloudssdk-1.0.2/setup.cfg
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.428290 usercloudssdk-1.0.2/src/
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.430628 usercloudssdk-1.0.2/src/usercloudssdk/
+-rw-r--r--   0 jwang      (501) staff       (20)        0 2023-06-13 16:36:00.000000 usercloudssdk-1.0.2/src/usercloudssdk/__init__.py
+-rw-r--r--   0 jwang      (501) staff       (20)    17689 2023-07-27 13:23:56.000000 usercloudssdk-1.0.2/src/usercloudssdk/client.py
+-rw-r--r--   0 jwang      (501) staff       (20)      636 2023-06-30 17:46:25.000000 usercloudssdk-1.0.2/src/usercloudssdk/constants.py
+-rw-r--r--   0 jwang      (501) staff       (20)    14342 2023-07-27 13:23:37.000000 usercloudssdk-1.0.2/src/usercloudssdk/models.py
+-rw-r--r--   0 jwang      (501) staff       (20)      790 2023-07-27 13:34:23.000000 usercloudssdk-1.0.2/src/usercloudssdk/policies.py
+-rw-r--r--   0 jwang      (501) staff       (20)     6377 2023-07-27 13:28:09.000000 usercloudssdk-1.0.2/src/usercloudssdk/tokenizer_sample.py
+-rw-r--r--   0 jwang      (501) staff       (20)      405 2023-06-13 16:36:00.000000 usercloudssdk-1.0.2/src/usercloudssdk/ucjson.py
+-rw-r--r--   0 jwang      (501) staff       (20)    11159 2023-07-27 13:36:23.000000 usercloudssdk-1.0.2/src/usercloudssdk/userstore_sample.py
+drwxr-xr-x   0 jwang      (501) staff       (20)        0 2023-07-27 13:40:15.431204 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/
+-rw-r--r--   0 jwang      (501) staff       (20)     1507 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/PKG-INFO
+-rw-r--r--   0 jwang      (501) staff       (20)      447 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jwang      (501) staff       (20)        1 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jwang      (501) staff       (20)       14 2023-07-27 13:40:15.000000 usercloudssdk-1.0.2/src/usercloudssdk.egg-info/top_level.txt
```

### Comparing `usercloudssdk-1.0.1/LICENSE` & `usercloudssdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/PKG-INFO` & `usercloudssdk-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/client.py` & `usercloudssdk-1.0.2/src/usercloudssdk/client.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/constants.py` & `usercloudssdk-1.0.2/src/usercloudssdk/constants.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/models.py` & `usercloudssdk-1.0.2/src/usercloudssdk/models.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/policies.py` & `usercloudssdk-1.0.2/src/usercloudssdk/policies.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/tokenizer_sample.py` & `usercloudssdk-1.0.2/src/usercloudssdk/tokenizer_sample.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk/userstore_sample.py` & `usercloudssdk-1.0.2/src/usercloudssdk/userstore_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 
 from usercloudssdk.client import Client, Error
-from userclooudssdk.models import (
+from usercloudssdk.models import (
     AccessPolicy,
     AccessPolicyTemplate,
     AccessPolicyComponent,
     Column,
     ColumnInputConfig,
     ColumnOutputConfig,
     Accessor,
```

### Comparing `usercloudssdk-1.0.1/src/usercloudssdk.egg-info/PKG-INFO` & `usercloudssdk-1.0.2/src/usercloudssdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usercloudssdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python SDK for UserClouds
 Author-email: Real Python <info@realpython.com>
 License: The MIT License
         
         Copyright (c) 2021- UserClouds, Inc. (https://userclouds.com)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

