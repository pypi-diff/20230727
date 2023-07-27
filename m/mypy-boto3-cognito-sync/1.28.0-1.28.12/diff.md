# Comparing `tmp/mypy-boto3-cognito-sync-1.28.0.tar.gz` & `tmp/mypy-boto3-cognito-sync-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-sync-1.28.0.tar", last modified: Thu Jul  6 20:59:16 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-sync-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
```

## Comparing `mypy-boto3-cognito-sync-1.28.0.tar` & `mypy-boto3-cognito-sync-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.406260 mypy-boto3-cognito-sync-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-06 20:59:16.402260 mypy-boto3-cognito-sync-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.402260 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12760 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:29.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.402260 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:16.000000 mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:16.406260 mypy-boto3-cognito-sync-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:36:28.000000 mypy-boto3-cognito-sync-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.624548 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:29.000000 mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.632548 mypy-boto3-cognito-sync-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:19:22.000000 mypy-boto3-cognito-sync-1.28.12/setup.py
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/LICENSE` & `mypy-boto3-cognito-sync-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.0/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoSync 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,51 +302,53 @@
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
+    CognitoStreamsOutputTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncTypeDef,
+    PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
+    PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     RegisterDeviceResponseTypeDef,
     ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    SetIdentityPoolConfigurationRequestRequestTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/README.md` & `mypy-boto3-cognito-sync-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,51 +270,53 @@
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
+    CognitoStreamsOutputTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncTypeDef,
+    PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
+    PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     RegisterDeviceResponseTypeDef,
     ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    SetIdentityPoolConfigurationRequestRequestTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/__main__.py` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoSync 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CognitoSync 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/client.py` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/client.pyi` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/literals.py` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -237,26 +238,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/literals.pyi` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -235,26 +236,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/type_defs.py` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,51 +22,53 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
+    "CognitoStreamsOutputTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
     "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
     "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
-    "PushSyncTypeDef",
+    "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
+    "PushSyncTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "RegisterDeviceResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
-    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
+    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -77,14 +79,24 @@
     "BulkPublishResponseTypeDef",
     {
         "IdentityPoolId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CognitoStreamsOutputTypeDef = TypedDict(
+    "CognitoStreamsOutputTypeDef",
+    {
+        "StreamName": str,
+        "RoleArn": str,
+        "StreamingStatus": StreamingStatusType,
+    },
+    total=False,
+)
+
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
         "RoleArn": str,
         "StreamingStatus": StreamingStatusType,
     },
@@ -205,16 +217,16 @@
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-PushSyncTypeDef = TypedDict(
-    "PushSyncTypeDef",
+PushSyncOutputTypeDef = TypedDict(
+    "PushSyncOutputTypeDef",
     {
         "ApplicationArns": List[str],
         "RoleArn": str,
     },
     total=False,
 )
 
@@ -285,14 +297,23 @@
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "DeviceLastModifiedDate": datetime,
     },
     total=False,
 )
 
+PushSyncTypeDef = TypedDict(
+    "PushSyncTypeDef",
+    {
+        "ApplicationArns": Sequence[str],
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 _RequiredRecordPatchTypeDef = TypedDict(
     "_RequiredRecordPatchTypeDef",
     {
         "Op": OperationType,
         "Key": str,
         "SyncCount": int,
     },
@@ -421,49 +442,26 @@
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
+        "PushSync": PushSyncOutputTypeDef,
+        "CognitoStreams": CognitoStreamsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "IdentityPoolId": str,
-    },
-)
-_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
-    },
-    total=False,
-)
-
-
-class SetIdentityPoolConfigurationRequestRequestTypeDef(
-    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
-    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
+        "PushSync": PushSyncOutputTypeDef,
+        "CognitoStreams": CognitoStreamsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
@@ -484,14 +482,37 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "IdentityPoolId": str,
+    },
+)
+_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "PushSync": PushSyncTypeDef,
+        "CognitoStreams": CognitoStreamsTypeDef,
+    },
+    total=False,
+)
+
+
+class SetIdentityPoolConfigurationRequestRequestTypeDef(
+    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
+    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync/type_defs.pyi` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,51 +21,53 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BulkPublishRequestRequestTypeDef",
     "BulkPublishResponseTypeDef",
+    "CognitoStreamsOutputTypeDef",
     "CognitoStreamsTypeDef",
     "DatasetTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeIdentityPoolUsageRequestRequestTypeDef",
     "IdentityPoolUsageTypeDef",
     "DescribeIdentityUsageRequestRequestTypeDef",
     "IdentityUsageTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetBulkPublishDetailsRequestRequestTypeDef",
     "GetBulkPublishDetailsResponseTypeDef",
     "GetCognitoEventsRequestRequestTypeDef",
     "GetCognitoEventsResponseTypeDef",
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
-    "PushSyncTypeDef",
+    "PushSyncOutputTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListIdentityPoolUsageRequestRequestTypeDef",
     "ListRecordsRequestRequestTypeDef",
     "RecordTypeDef",
+    "PushSyncTypeDef",
     "RecordPatchTypeDef",
     "RegisterDeviceRequestRequestTypeDef",
     "RegisterDeviceResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SetCognitoEventsRequestRequestTypeDef",
     "SubscribeToDatasetRequestRequestTypeDef",
     "UnsubscribeFromDatasetRequestRequestTypeDef",
     "DeleteDatasetResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeIdentityPoolUsageResponseTypeDef",
     "ListIdentityPoolUsageResponseTypeDef",
     "DescribeIdentityUsageResponseTypeDef",
     "GetIdentityPoolConfigurationResponseTypeDef",
-    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "SetIdentityPoolConfigurationResponseTypeDef",
     "ListRecordsResponseTypeDef",
     "UpdateRecordsResponseTypeDef",
+    "SetIdentityPoolConfigurationRequestRequestTypeDef",
     "UpdateRecordsRequestRequestTypeDef",
 )
 
 BulkPublishRequestRequestTypeDef = TypedDict(
     "BulkPublishRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
@@ -76,14 +78,24 @@
     "BulkPublishResponseTypeDef",
     {
         "IdentityPoolId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CognitoStreamsOutputTypeDef = TypedDict(
+    "CognitoStreamsOutputTypeDef",
+    {
+        "StreamName": str,
+        "RoleArn": str,
+        "StreamingStatus": StreamingStatusType,
+    },
+    total=False,
+)
+
 CognitoStreamsTypeDef = TypedDict(
     "CognitoStreamsTypeDef",
     {
         "StreamName": str,
         "RoleArn": str,
         "StreamingStatus": StreamingStatusType,
     },
@@ -204,16 +216,16 @@
 GetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
     "GetIdentityPoolConfigurationRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
     },
 )
 
-PushSyncTypeDef = TypedDict(
-    "PushSyncTypeDef",
+PushSyncOutputTypeDef = TypedDict(
+    "PushSyncOutputTypeDef",
     {
         "ApplicationArns": List[str],
         "RoleArn": str,
     },
     total=False,
 )
 
@@ -280,14 +292,23 @@
         "LastModifiedDate": datetime,
         "LastModifiedBy": str,
         "DeviceLastModifiedDate": datetime,
     },
     total=False,
 )
 
+PushSyncTypeDef = TypedDict(
+    "PushSyncTypeDef",
+    {
+        "ApplicationArns": Sequence[str],
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 _RequiredRecordPatchTypeDef = TypedDict(
     "_RequiredRecordPatchTypeDef",
     {
         "Op": OperationType,
         "Key": str,
         "SyncCount": int,
     },
@@ -414,47 +435,26 @@
     },
 )
 
 GetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "GetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
+        "PushSync": PushSyncOutputTypeDef,
+        "CognitoStreams": CognitoStreamsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "IdentityPoolId": str,
-    },
-)
-_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
-    {
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
-    },
-    total=False,
-)
-
-class SetIdentityPoolConfigurationRequestRequestTypeDef(
-    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
-    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
-):
-    pass
-
 SetIdentityPoolConfigurationResponseTypeDef = TypedDict(
     "SetIdentityPoolConfigurationResponseTypeDef",
     {
         "IdentityPoolId": str,
-        "PushSync": PushSyncTypeDef,
-        "CognitoStreams": CognitoStreamsTypeDef,
+        "PushSync": PushSyncOutputTypeDef,
+        "CognitoStreams": CognitoStreamsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListRecordsResponseTypeDef = TypedDict(
     "ListRecordsResponseTypeDef",
     {
@@ -475,14 +475,35 @@
     "UpdateRecordsResponseTypeDef",
     {
         "Records": List[RecordTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "IdentityPoolId": str,
+    },
+)
+_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalSetIdentityPoolConfigurationRequestRequestTypeDef",
+    {
+        "PushSync": PushSyncTypeDef,
+        "CognitoStreams": CognitoStreamsTypeDef,
+    },
+    total=False,
+)
+
+class SetIdentityPoolConfigurationRequestRequestTypeDef(
+    _RequiredSetIdentityPoolConfigurationRequestRequestTypeDef,
+    _OptionalSetIdentityPoolConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRecordsRequestRequestTypeDef",
     {
         "IdentityPoolId": str,
         "IdentityId": str,
         "DatasetName": str,
         "SyncSessionToken": str,
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/PKG-INFO` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-sync
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoSync 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cognito-sync"></a>
 
 # mypy-boto3-cognito-sync
 
 [![PyPI - mypy-boto3-cognito-sync](https://img.shields.io/pypi/v/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-sync.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-sync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-sync?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-sync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cognito-sync)](https://pepy.tech/project/mypy-boto3-cognito-sync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoSync 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
+[boto3.CognitoSync 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-cognito-sync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_sync/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,51 +302,53 @@
 `mypy_boto3_cognito_sync.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cognito_sync.type_defs import (
     BulkPublishRequestRequestTypeDef,
     BulkPublishResponseTypeDef,
+    CognitoStreamsOutputTypeDef,
     CognitoStreamsTypeDef,
     DatasetTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeIdentityPoolUsageRequestRequestTypeDef,
     IdentityPoolUsageTypeDef,
     DescribeIdentityUsageRequestRequestTypeDef,
     IdentityUsageTypeDef,
     EmptyResponseMetadataTypeDef,
     GetBulkPublishDetailsRequestRequestTypeDef,
     GetBulkPublishDetailsResponseTypeDef,
     GetCognitoEventsRequestRequestTypeDef,
     GetCognitoEventsResponseTypeDef,
     GetIdentityPoolConfigurationRequestRequestTypeDef,
-    PushSyncTypeDef,
+    PushSyncOutputTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListIdentityPoolUsageRequestRequestTypeDef,
     ListRecordsRequestRequestTypeDef,
     RecordTypeDef,
+    PushSyncTypeDef,
     RecordPatchTypeDef,
     RegisterDeviceRequestRequestTypeDef,
     RegisterDeviceResponseTypeDef,
     ResponseMetadataTypeDef,
     SetCognitoEventsRequestRequestTypeDef,
     SubscribeToDatasetRequestRequestTypeDef,
     UnsubscribeFromDatasetRequestRequestTypeDef,
     DeleteDatasetResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     ListDatasetsResponseTypeDef,
     DescribeIdentityPoolUsageResponseTypeDef,
     ListIdentityPoolUsageResponseTypeDef,
     DescribeIdentityUsageResponseTypeDef,
     GetIdentityPoolConfigurationResponseTypeDef,
-    SetIdentityPoolConfigurationRequestRequestTypeDef,
     SetIdentityPoolConfigurationResponseTypeDef,
     ListRecordsResponseTypeDef,
     UpdateRecordsResponseTypeDef,
+    SetIdentityPoolConfigurationRequestRequestTypeDef,
     UpdateRecordsRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BulkPublishRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-sync-1.28.0/mypy_boto3_cognito_sync.egg-info/SOURCES.txt` & `mypy-boto3-cognito-sync-1.28.12/mypy_boto3_cognito_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-sync-1.28.0/setup.py` & `mypy-boto3-cognito-sync-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-sync",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cognito_sync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoSync 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CognitoSync 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

