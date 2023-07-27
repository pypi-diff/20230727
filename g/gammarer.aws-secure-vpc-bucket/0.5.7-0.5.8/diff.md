# Comparing `tmp/gammarer.aws-secure-vpc-bucket-0.5.7.tar.gz` & `tmp/gammarer.aws-secure-vpc-bucket-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-vpc-bucket-0.5.7.tar", last modified: Wed Jul 26 18:22:45 2023, max compression
+gzip compressed data, was "gammarer.aws-secure-vpc-bucket-0.5.8.tar", last modified: Thu Jul 27 18:23:57 2023, max compression
```

## Comparing `gammarer.aws-secure-vpc-bucket-0.5.7.tar` & `gammarer.aws-secure-vpc-bucket-0.5.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.474300 gammarer.aws-secure-vpc-bucket-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 18:22:45.474300 gammarer.aws-secure-vpc-bucket-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 18:22:45.474300 gammarer.aws-secure-vpc-bucket-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.470300 gammarer.aws-secure-vpc-bucket-0.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.470300 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.470300 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.474300 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29582 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:31.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:22:45.470300 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-26 18:22:45.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-26 18:22:45.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:22:45.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-26 18:22:45.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 18:22:45.000000 gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29581 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:23:44.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:23:57.150719 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-27 18:23:57.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-27 18:23:57.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:23:57.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-27 18:23:57.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 18:23:57.000000 gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/LICENSE` & `gammarer.aws-secure-vpc-bucket-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/PKG-INFO` & `gammarer.aws-secure-vpc-bucket-0.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-vpc-bucket
-Version: 0.5.7
+Version: 0.5.8
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/yicr/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/README.md` & `gammarer.aws-secure-vpc-bucket-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/setup.py` & `gammarer.aws-secure-vpc-bucket-0.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-vpc-bucket",
-    "version": "0.5.7",
+    "version": "0.5.8",
     "description": "Access from specific VPC Endpoint only Bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-vpc-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_secure_vpc_bucket",
         "gammarer.aws_secure_vpc_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_vpc_bucket._jsii": [
-            "aws-secure-vpc-bucket@0.5.7.jsii.tgz"
+            "aws-secure-vpc-bucket@0.5.8.jsii.tgz"
         ],
         "gammarer.aws_secure_vpc_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.65.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "gammarer.aws-secure-bucket>=0.9.9, <0.10.0",
+        "gammarer.aws-secure-bucket>=0.10.1, <0.11.0",
         "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer/aws_secure_vpc_bucket/__init__.py` & `gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer/aws_secure_vpc_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-vpc-bucket
-Version: 0.5.7
+Version: 0.5.8
 Summary: Access from specific VPC Endpoint only Bucket
 Home-page: https://github.com/yicr/aws-secure-vpc-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-vpc-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-vpc-bucket-0.5.7/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-vpc-bucket-0.5.8/src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_vpc_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_vpc_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_vpc_bucket/__init__.py
 src/gammarer/aws_secure_vpc_bucket/py.typed
 src/gammarer/aws_secure_vpc_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.7.jsii.tgz
+src/gammarer/aws_secure_vpc_bucket/_jsii/aws-secure-vpc-bucket@0.5.8.jsii.tgz
```

