# Comparing `tmp/mypy-boto3-route53resolver-1.28.12.tar.gz` & `tmp/mypy-boto3-route53resolver-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53resolver-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
+gzip compressed data, was "mypy-boto3-route53resolver-1.28.8.tar", last modified: Thu Jul 20 19:47:56 2023, max compression
```

## Comparing `mypy-boto3-route53resolver-1.28.12.tar` & `mypy-boto3-route53resolver-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.057239 mypy-boto3-route53resolver-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-07-27 11:49:33.053239 mypy-boto3-route53resolver-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.053239 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59202 2023-07-27 11:44:57.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59111 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14376 2023-07-27 11:44:57.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14374 2023-07-27 11:44:57.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-07-27 11:44:57.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-07-27 11:44:57.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61501 2023-07-27 11:45:00.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61456 2023-07-27 11:44:58.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.053239 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25421 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:32.000000 mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.057239 mypy-boto3-route53resolver-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-27 11:44:56.000000 mypy-boto3-route53resolver-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.004775 mypy-boto3-route53resolver-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59202 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59111 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20774 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20756 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:03.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    61212 2023-07-20 19:47:05.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61167 2023-07-20 19:47:04.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:56.000775 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25434 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-20 19:47:55.000000 mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:56.004775 mypy-boto3-route53resolver-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-20 19:47:02.000000 mypy-boto3-route53resolver-1.28.8/setup.py
```

### Comparing `mypy-boto3-route53resolver-1.28.12/LICENSE` & `mypy-boto3-route53resolver-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/PKG-INFO` & `mypy-boto3-route53resolver-1.28.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53Resolver 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.Route53Resolver 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.28.12/README.md` & `mypy-boto3-route53resolver-1.28.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__init__.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__init__.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/__main__.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53Resolver 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.Route53Resolver 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/client.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/client.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/literals.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,15 +277,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -364,15 +363,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/literals.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -362,15 +361,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/paginator.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/paginator.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/type_defs.py` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,14 @@
         "ManagedOwnerName": str,
         "Status": FirewallRuleGroupAssociationStatusType,
         "StatusMessage": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -297,15 +296,14 @@
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
         "OutpostArn": str,
         "PreferredInstanceType": str,
     },
-    total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
@@ -319,15 +317,14 @@
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
         "Status": ResolverQueryLogConfigAssociationStatusType,
         "Error": ResolverQueryLogConfigAssociationErrorType,
         "ErrorMessage": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 _RequiredAssociateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "VPCId": str,
@@ -355,15 +352,14 @@
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
         "Status": ResolverRuleAssociationStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 FirewallDomainListTypeDef = TypedDict(
     "FirewallDomainListTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -372,15 +368,14 @@
         "Status": FirewallDomainListStatusType,
         "StatusMessage": str,
         "ManagedOwnerName": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupTypeDef = TypedDict(
     "FirewallRuleGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -390,15 +385,14 @@
         "StatusMessage": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredCreateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "FirewallRuleGroupId": str,
@@ -439,15 +433,14 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 OutpostResolverTypeDef = TypedDict(
     "OutpostResolverTypeDef",
     {
         "Arn": str,
         "CreationTime": str,
@@ -457,15 +450,14 @@
         "InstanceCount": int,
         "PreferredInstanceType": str,
         "Name": str,
         "Status": OutpostResolverStatusType,
         "StatusMessage": str,
         "OutpostArn": str,
     },
-    total=False,
 )
 
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
@@ -494,15 +486,14 @@
         "AssociationCount": int,
         "Arn": str,
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 TargetAddressTypeDef = TypedDict(
     "TargetAddressTypeDef",
     {
         "Ip": str,
         "Port": int,
@@ -597,40 +588,37 @@
     "FirewallConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "FirewallFailOpen": FirewallFailOpenStatusType,
     },
-    total=False,
 )
 
 FirewallDomainListMetadataTypeDef = TypedDict(
     "FirewallDomainListMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "CreatorRequestId": str,
         "ManagedOwnerName": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupMetadataTypeDef = TypedDict(
     "FirewallRuleGroupMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
     },
-    total=False,
 )
 
 GetFirewallConfigRequestRequestTypeDef = TypedDict(
     "GetFirewallConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -682,15 +670,14 @@
     "ResolverConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "AutodefinedReverse": ResolverAutodefinedReverseStatusType,
     },
-    total=False,
 )
 
 GetResolverDnssecConfigRequestRequestTypeDef = TypedDict(
     "GetResolverDnssecConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -700,15 +687,14 @@
     "ResolverDnssecConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "ResourceId": str,
         "ValidationStatus": ResolverDNSSECValidationStatusType,
     },
-    total=False,
 )
 
 GetResolverEndpointRequestRequestTypeDef = TypedDict(
     "GetResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
@@ -773,15 +759,14 @@
         "Ip": str,
         "Ipv6": str,
         "Status": IpAddressStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -977,15 +962,14 @@
 TargetAddressOutputTypeDef = TypedDict(
     "TargetAddressOutputTypeDef",
     {
         "Ip": str,
         "Port": int,
         "Ipv6": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -2120,15 +2104,14 @@
         "TargetIps": List[TargetAddressOutputTypeDef],
         "ResolverEndpointId": str,
         "OwnerId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver/type_defs.pyi` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,14 @@
         "ManagedOwnerName": str,
         "Status": FirewallRuleGroupAssociationStatusType,
         "StatusMessage": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
@@ -296,15 +295,14 @@
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
         "ResolverEndpointType": ResolverEndpointTypeType,
         "OutpostArn": str,
         "PreferredInstanceType": str,
     },
-    total=False,
 )
 
 AssociateResolverQueryLogConfigRequestRequestTypeDef = TypedDict(
     "AssociateResolverQueryLogConfigRequestRequestTypeDef",
     {
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
@@ -318,15 +316,14 @@
         "ResolverQueryLogConfigId": str,
         "ResourceId": str,
         "Status": ResolverQueryLogConfigAssociationStatusType,
         "Error": ResolverQueryLogConfigAssociationErrorType,
         "ErrorMessage": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 _RequiredAssociateResolverRuleRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateResolverRuleRequestRequestTypeDef",
     {
         "ResolverRuleId": str,
         "VPCId": str,
@@ -352,15 +349,14 @@
         "Id": str,
         "ResolverRuleId": str,
         "Name": str,
         "VPCId": str,
         "Status": ResolverRuleAssociationStatusType,
         "StatusMessage": str,
     },
-    total=False,
 )
 
 FirewallDomainListTypeDef = TypedDict(
     "FirewallDomainListTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -369,15 +365,14 @@
         "Status": FirewallDomainListStatusType,
         "StatusMessage": str,
         "ManagedOwnerName": str,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupTypeDef = TypedDict(
     "FirewallRuleGroupTypeDef",
     {
         "Id": str,
         "Arn": str,
@@ -387,15 +382,14 @@
         "StatusMessage": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredCreateFirewallRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFirewallRuleRequestRequestTypeDef",
     {
         "CreatorRequestId": str,
         "FirewallRuleGroupId": str,
@@ -434,15 +428,14 @@
         "BlockOverrideDomain": str,
         "BlockOverrideDnsType": Literal["CNAME"],
         "BlockOverrideTtl": int,
         "CreatorRequestId": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 OutpostResolverTypeDef = TypedDict(
     "OutpostResolverTypeDef",
     {
         "Arn": str,
         "CreationTime": str,
@@ -452,15 +445,14 @@
         "InstanceCount": int,
         "PreferredInstanceType": str,
         "Name": str,
         "Status": OutpostResolverStatusType,
         "StatusMessage": str,
         "OutpostArn": str,
     },
-    total=False,
 )
 
 _RequiredIpAddressRequestTypeDef = TypedDict(
     "_RequiredIpAddressRequestTypeDef",
     {
         "SubnetId": str,
     },
@@ -487,15 +479,14 @@
         "AssociationCount": int,
         "Arn": str,
         "Name": str,
         "DestinationArn": str,
         "CreatorRequestId": str,
         "CreationTime": str,
     },
-    total=False,
 )
 
 TargetAddressTypeDef = TypedDict(
     "TargetAddressTypeDef",
     {
         "Ip": str,
         "Port": int,
@@ -590,40 +581,37 @@
     "FirewallConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "FirewallFailOpen": FirewallFailOpenStatusType,
     },
-    total=False,
 )
 
 FirewallDomainListMetadataTypeDef = TypedDict(
     "FirewallDomainListMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "CreatorRequestId": str,
         "ManagedOwnerName": str,
     },
-    total=False,
 )
 
 FirewallRuleGroupMetadataTypeDef = TypedDict(
     "FirewallRuleGroupMetadataTypeDef",
     {
         "Id": str,
         "Arn": str,
         "Name": str,
         "OwnerId": str,
         "CreatorRequestId": str,
         "ShareStatus": ShareStatusType,
     },
-    total=False,
 )
 
 GetFirewallConfigRequestRequestTypeDef = TypedDict(
     "GetFirewallConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -675,15 +663,14 @@
     "ResolverConfigTypeDef",
     {
         "Id": str,
         "ResourceId": str,
         "OwnerId": str,
         "AutodefinedReverse": ResolverAutodefinedReverseStatusType,
     },
-    total=False,
 )
 
 GetResolverDnssecConfigRequestRequestTypeDef = TypedDict(
     "GetResolverDnssecConfigRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
@@ -693,15 +680,14 @@
     "ResolverDnssecConfigTypeDef",
     {
         "Id": str,
         "OwnerId": str,
         "ResourceId": str,
         "ValidationStatus": ResolverDNSSECValidationStatusType,
     },
-    total=False,
 )
 
 GetResolverEndpointRequestRequestTypeDef = TypedDict(
     "GetResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
@@ -766,15 +752,14 @@
         "Ip": str,
         "Ipv6": str,
         "Status": IpAddressStatusType,
         "StatusMessage": str,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -962,15 +947,14 @@
 TargetAddressOutputTypeDef = TypedDict(
     "TargetAddressOutputTypeDef",
     {
         "Ip": str,
         "Port": int,
         "Ipv6": str,
     },
-    total=False,
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
@@ -2077,15 +2061,14 @@
         "TargetIps": List[TargetAddressOutputTypeDef],
         "ResolverEndpointId": str,
         "OwnerId": str,
         "ShareStatus": ShareStatusType,
         "CreationTime": str,
         "ModificationTime": str,
     },
-    total=False,
 )
 
 _RequiredUpdateResolverEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResolverEndpointRequestRequestTypeDef",
     {
         "ResolverEndpointId": str,
     },
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/PKG-INFO` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53resolver
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53Resolver 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.8
+Summary: Type annotations for boto3.Route53Resolver 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-route53resolver"></a>
 
 # mypy-boto3-route53resolver
 
 [![PyPI - mypy-boto3-route53resolver](https://img.shields.io/pypi/v/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53resolver.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53resolver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53resolver)](https://pepy.tech/project/mypy-boto3-route53resolver)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-route53resolver?color=blue)](https://pypistats.org/packages/mypy-boto3-route53resolver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53Resolver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
+[boto3.Route53Resolver 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-route53resolver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53resolver/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-route53resolver-1.28.12/mypy_boto3_route53resolver.egg-info/SOURCES.txt` & `mypy-boto3-route53resolver-1.28.8/mypy_boto3_route53resolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53resolver-1.28.12/setup.py` & `mypy-boto3-route53resolver-1.28.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53resolver",
-    version="1.28.12",
+    version="1.28.8",
     packages=["mypy_boto3_route53resolver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53Resolver 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Route53Resolver 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

