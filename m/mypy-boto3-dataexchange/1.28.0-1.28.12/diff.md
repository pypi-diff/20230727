# Comparing `tmp/mypy-boto3-dataexchange-1.28.0.tar.gz` & `tmp/mypy-boto3-dataexchange-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dataexchange-1.28.0.tar", last modified: Thu Jul  6 20:59:22 2023, max compression
+gzip compressed data, was "mypy-boto3-dataexchange-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
```

## Comparing `mypy-boto3-dataexchange-1.28.0.tar` & `mypy-boto3-dataexchange-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.698274 mypy-boto3-dataexchange-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-06 20:59:22.686274 mypy-boto3-dataexchange-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.686274 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-06 20:37:26.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45212 2023-07-06 20:37:27.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45145 2023-07-06 20:37:27.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:22.686274 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18157 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:22.000000 mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:22.698274 mypy-boto3-dataexchange-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:37:25.000000 mypy-boto3-dataexchange-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17249 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.392537 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-27 05:19:59.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50714 2023-07-27 05:19:59.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:33.000000 mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.396537 mypy-boto3-dataexchange-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:58.000000 mypy-boto3-dataexchange-1.28.12/setup.py
```

### Comparing `mypy-boto3-dataexchange-1.28.0/LICENSE` & `mypy-boto3-dataexchange-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/PKG-INFO` & `mypy-boto3-dataexchange-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.28.0
-Summary: Type annotations for boto3.DataExchange 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,47 +352,56 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
+    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
+    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
+    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
+    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
     CreateRevisionRequestRequestTypeDef,
     CreateRevisionResponseTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
+    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
+    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
+    RedshiftDataShareAssetSourceEntryOutputTypeDef,
+    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
     ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
     ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
     ListEventActionsRequestListEventActionsPaginateTypeDef,
@@ -412,59 +421,65 @@
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
     UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3RequestDetailsTypeDef,
+    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
     CreateDataSetResponseTypeDef,
     DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
-    TableLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
+    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
-    S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetSourceEntryOutputTypeDef,
     S3DataAccessAssetTypeDef,
+    S3DataAccessAssetSourceEntryTypeDef,
     ListDataSetRevisionsResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
-    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
+    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
-    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
-    CreateEventActionRequestRequestTypeDef,
+    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionRequestRequestTypeDef,
     UpdateEventActionResponseTypeDef,
+    CreateEventActionRequestRequestTypeDef,
+    UpdateEventActionRequestRequestTypeDef,
     LFTagPolicyDetailsTypeDef,
-    RequestDetailsTypeDef,
     ResponseDetailsTypeDef,
+    RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
-    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     JobEntryTypeDef,
+    CreateJobRequestRequestTypeDef,
     LakeFormationDataPermissionAssetTypeDef,
     ListJobsResponseTypeDef,
     AssetDetailsTypeDef,
     AssetEntryTypeDef,
     GetAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListRevisionAssetsResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.0/README.md` & `mypy-boto3-dataexchange-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -320,47 +320,56 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
+    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
+    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
+    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
+    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
     CreateRevisionRequestRequestTypeDef,
     CreateRevisionResponseTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
+    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
+    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
+    RedshiftDataShareAssetSourceEntryOutputTypeDef,
+    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
     ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
     ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
     ListEventActionsRequestListEventActionsPaginateTypeDef,
@@ -380,59 +389,65 @@
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
     UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3RequestDetailsTypeDef,
+    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
     CreateDataSetResponseTypeDef,
     DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
-    TableLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
+    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
-    S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetSourceEntryOutputTypeDef,
     S3DataAccessAssetTypeDef,
+    S3DataAccessAssetSourceEntryTypeDef,
     ListDataSetRevisionsResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
-    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
+    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
-    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
-    CreateEventActionRequestRequestTypeDef,
+    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionRequestRequestTypeDef,
     UpdateEventActionResponseTypeDef,
+    CreateEventActionRequestRequestTypeDef,
+    UpdateEventActionRequestRequestTypeDef,
     LFTagPolicyDetailsTypeDef,
-    RequestDetailsTypeDef,
     ResponseDetailsTypeDef,
+    RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
-    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     JobEntryTypeDef,
+    CreateJobRequestRequestTypeDef,
     LakeFormationDataPermissionAssetTypeDef,
     ListJobsResponseTypeDef,
     AssetDetailsTypeDef,
     AssetEntryTypeDef,
     GetAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListRevisionAssetsResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__init__.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__init__.pyi` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/__main__.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataExchange 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.DataExchange 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
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

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/client.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/client.pyi` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/literals.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/literals.pyi` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -296,26 +297,28 @@
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

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/paginator.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/paginator.pyi` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/type_defs.py` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,47 +37,56 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiGatewayApiAssetTypeDef",
+    "AssetDestinationEntryOutputTypeDef",
     "AssetDestinationEntryTypeDef",
     "RedshiftDataShareAssetTypeDef",
     "S3SnapshotAssetTypeDef",
+    "AssetSourceEntryOutputTypeDef",
     "AssetSourceEntryTypeDef",
+    "AutoExportRevisionDestinationEntryOutputTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
+    "ExportServerSideEncryptionOutputTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
     "CreateRevisionRequestRequestTypeDef",
     "CreateRevisionResponseTypeDef",
+    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "RevisionPublishedOutputTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
+    "RevisionDestinationEntryOutputTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
+    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
+    "KmsKeyToGrantOutputTypeDef",
     "KmsKeyToGrantTypeDef",
     "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListEventActionsRequestListEventActionsPaginateTypeDef",
@@ -97,59 +106,65 @@
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
     "UpdateRevisionResponseTypeDef",
-    "ImportAssetsFromS3RequestDetailsTypeDef",
     "ImportAssetsFromS3ResponseDetailsTypeDef",
+    "ImportAssetsFromS3RequestDetailsTypeDef",
+    "AutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    "ExportAssetsToS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
-    "ExportAssetsToS3ResponseDetailsTypeDef",
     "CreateDataSetResponseTypeDef",
     "DataSetEntryTypeDef",
     "GetDataSetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     "DatabaseLFTagPolicyTypeDef",
-    "TableLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyAndPermissionsOutputTypeDef",
     "TableLFTagPolicyTypeDef",
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyAndPermissionsTypeDef",
     "DetailsTypeDef",
+    "EventOutputTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
-    "S3DataAccessAssetSourceEntryTypeDef",
+    "S3DataAccessAssetSourceEntryOutputTypeDef",
     "S3DataAccessAssetTypeDef",
+    "S3DataAccessAssetSourceEntryTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
-    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
+    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
-    "CreateEventActionRequestRequestTypeDef",
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
-    "UpdateEventActionRequestRequestTypeDef",
     "UpdateEventActionResponseTypeDef",
+    "CreateEventActionRequestRequestTypeDef",
+    "UpdateEventActionRequestRequestTypeDef",
     "LFTagPolicyDetailsTypeDef",
-    "RequestDetailsTypeDef",
     "ResponseDetailsTypeDef",
+    "RequestDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "JobEntryTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "LakeFormationDataPermissionAssetTypeDef",
     "ListJobsResponseTypeDef",
     "AssetDetailsTypeDef",
     "AssetEntryTypeDef",
     "GetAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListRevisionAssetsResponseTypeDef",
@@ -167,14 +182,36 @@
         "ApiSpecificationDownloadUrlExpiresAt": datetime,
         "ProtocolType": Literal["REST"],
         "Stage": str,
     },
     total=False,
 )
 
+_RequiredAssetDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredAssetDestinationEntryOutputTypeDef",
+    {
+        "AssetId": str,
+        "Bucket": str,
+    },
+)
+_OptionalAssetDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalAssetDestinationEntryOutputTypeDef",
+    {
+        "Key": str,
+    },
+    total=False,
+)
+
+
+class AssetDestinationEntryOutputTypeDef(
+    _RequiredAssetDestinationEntryOutputTypeDef, _OptionalAssetDestinationEntryOutputTypeDef
+):
+    pass
+
+
 _RequiredAssetDestinationEntryTypeDef = TypedDict(
     "_RequiredAssetDestinationEntryTypeDef",
     {
         "AssetId": str,
         "Bucket": str,
     },
 )
@@ -203,22 +240,52 @@
 S3SnapshotAssetTypeDef = TypedDict(
     "S3SnapshotAssetTypeDef",
     {
         "Size": float,
     },
 )
 
+AssetSourceEntryOutputTypeDef = TypedDict(
+    "AssetSourceEntryOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+
 AssetSourceEntryTypeDef = TypedDict(
     "AssetSourceEntryTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
+_RequiredAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredAutoExportRevisionDestinationEntryOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalAutoExportRevisionDestinationEntryOutputTypeDef",
+    {
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+
+class AutoExportRevisionDestinationEntryOutputTypeDef(
+    _RequiredAutoExportRevisionDestinationEntryOutputTypeDef,
+    _OptionalAutoExportRevisionDestinationEntryOutputTypeDef,
+):
+    pass
+
+
 _RequiredAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredAutoExportRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalAutoExportRevisionDestinationEntryTypeDef = TypedDict(
@@ -233,14 +300,36 @@
 class AutoExportRevisionDestinationEntryTypeDef(
     _RequiredAutoExportRevisionDestinationEntryTypeDef,
     _OptionalAutoExportRevisionDestinationEntryTypeDef,
 ):
     pass
 
 
+_RequiredExportServerSideEncryptionOutputTypeDef = TypedDict(
+    "_RequiredExportServerSideEncryptionOutputTypeDef",
+    {
+        "Type": ServerSideEncryptionTypesType,
+    },
+)
+_OptionalExportServerSideEncryptionOutputTypeDef = TypedDict(
+    "_OptionalExportServerSideEncryptionOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
+
+class ExportServerSideEncryptionOutputTypeDef(
+    _RequiredExportServerSideEncryptionOutputTypeDef,
+    _OptionalExportServerSideEncryptionOutputTypeDef,
+):
+    pass
+
+
 _RequiredExportServerSideEncryptionTypeDef = TypedDict(
     "_RequiredExportServerSideEncryptionTypeDef",
     {
         "Type": ServerSideEncryptionTypesType,
     },
 )
 _OptionalExportServerSideEncryptionTypeDef = TypedDict(
@@ -332,14 +421,22 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -385,14 +482,21 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RevisionPublishedOutputTypeDef = TypedDict(
+    "RevisionPublishedOutputTypeDef",
+    {
+        "DataSetId": str,
+    },
+)
+
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -448,14 +552,36 @@
 
 class RevisionDestinationEntryTypeDef(
     _RequiredRevisionDestinationEntryTypeDef, _OptionalRevisionDestinationEntryTypeDef
 ):
     pass
 
 
+_RequiredRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredRevisionDestinationEntryOutputTypeDef",
+    {
+        "Bucket": str,
+        "RevisionId": str,
+    },
+)
+_OptionalRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalRevisionDestinationEntryOutputTypeDef",
+    {
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+
+class RevisionDestinationEntryOutputTypeDef(
+    _RequiredRevisionDestinationEntryOutputTypeDef, _OptionalRevisionDestinationEntryOutputTypeDef
+):
+    pass
+
+
 GetAssetRequestRequestTypeDef = TypedDict(
     "GetAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -608,14 +734,28 @@
 RedshiftDataShareAssetSourceEntryTypeDef = TypedDict(
     "RedshiftDataShareAssetSourceEntryTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
+RedshiftDataShareAssetSourceEntryOutputTypeDef = TypedDict(
+    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
+    {
+        "DataShareArn": str,
+    },
+)
+
+KmsKeyToGrantOutputTypeDef = TypedDict(
+    "KmsKeyToGrantOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
@@ -989,31 +1129,76 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
+    {
+        "AssetSources": List[AssetSourceEntryOutputTypeDef],
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
+_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
+    "_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    {
+        "RevisionDestination": AutoExportRevisionDestinationEntryOutputTypeDef,
+    },
+)
+_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
+    "_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AutoExportRevisionToS3RequestDetailsOutputTypeDef(
+    _RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    _OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef,
+):
+    pass
+
+
+_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
     {
-        "AssetSources": List[AssetSourceEntryTypeDef],
+        "AssetDestinations": List[AssetDestinationEntryOutputTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
+_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ExportAssetsToS3ResponseDetailsTypeDef(
+    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
+):
+    pass
+
 
 _RequiredAutoExportRevisionToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "RevisionDestination": AutoExportRevisionDestinationEntryTypeDef,
     },
 )
@@ -1052,37 +1237,14 @@
 
 class ExportAssetsToS3RequestDetailsTypeDef(
     _RequiredExportAssetsToS3RequestDetailsTypeDef, _OptionalExportAssetsToS3RequestDetailsTypeDef
 ):
     pass
 
 
-_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "AssetDestinations": List[AssetDestinationEntryTypeDef],
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionTypeDef,
-    },
-    total=False,
-)
-
-
-class ExportAssetsToS3ResponseDetailsTypeDef(
-    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
-):
-    pass
-
-
 CreateDataSetResponseTypeDef = TypedDict(
     "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
@@ -1155,49 +1317,73 @@
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[Literal["DESCRIBE"]],
+        "Expression": List[LFTagOutputTypeDef],
+        "Permissions": List[Literal["DESCRIBE"]],
     },
 )
 
 DatabaseLFTagPolicyTypeDef = TypedDict(
     "DatabaseLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagTypeDef],
+        "Expression": List[LFTagOutputTypeDef],
     },
 )
 
-TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsTypeDef",
+TableLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsOutputTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[TableTagPolicyLFPermissionType],
+        "Expression": List[LFTagOutputTypeDef],
+        "Permissions": List[TableTagPolicyLFPermissionType],
     },
 )
 
 TableLFTagPolicyTypeDef = TypedDict(
     "TableLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagTypeDef],
+        "Expression": List[LFTagOutputTypeDef],
+    },
+)
+
+DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[Literal["DESCRIBE"]],
+    },
+)
+
+TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[TableTagPolicyLFPermissionType],
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryTypeDef],
+        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryOutputTypeDef],
+    },
+    total=False,
+)
+
+EventOutputTypeDef = TypedDict(
+    "EventOutputTypeDef",
+    {
+        "RevisionPublished": RevisionPublishedOutputTypeDef,
     },
     total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
@@ -1229,21 +1415,21 @@
     pass
 
 
 _RequiredExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_RequiredExportRevisionsToS3ResponseDetailsTypeDef",
     {
         "DataSetId": str,
-        "RevisionDestinations": List[RevisionDestinationEntryTypeDef],
+        "RevisionDestinations": List[RevisionDestinationEntryOutputTypeDef],
     },
 )
 _OptionalExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_OptionalExportRevisionsToS3ResponseDetailsTypeDef",
     {
-        "Encryption": ExportServerSideEncryptionTypeDef,
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
         "EventActionArn": str,
     },
     total=False,
 )
 
 
 class ExportRevisionsToS3ResponseDetailsTypeDef(
@@ -1261,39 +1447,40 @@
         "RevisionId": str,
     },
 )
 
 ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     {
-        "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
+        "AssetSources": List[RedshiftDataShareAssetSourceEntryOutputTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+_RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
     {
         "Bucket": str,
     },
 )
-_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+_OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
     {
-        "KeyPrefixes": Sequence[str],
-        "Keys": Sequence[str],
-        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+        "KeyPrefixes": List[str],
+        "Keys": List[str],
+        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
     },
     total=False,
 )
 
 
-class S3DataAccessAssetSourceEntryTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+class S3DataAccessAssetSourceEntryOutputTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
+    _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
 ):
     pass
 
 
 _RequiredS3DataAccessAssetTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetTypeDef",
     {
@@ -1303,35 +1490,66 @@
 _OptionalS3DataAccessAssetTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
         "S3AccessPointAlias": str,
         "S3AccessPointArn": str,
-        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
     },
     total=False,
 )
 
 
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
 
+_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "KeyPrefixes": Sequence[str],
+        "Keys": Sequence[str],
+        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+    },
+    total=False,
+)
+
+
+class S3DataAccessAssetSourceEntryTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+):
+    pass
+
+
 ListDataSetRevisionsResponseTypeDef = TypedDict(
     "ListDataSetRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[RevisionEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
     },
     total=False,
 )
@@ -1341,75 +1559,75 @@
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
-        "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
-        "Table": TableLFTagPolicyAndPermissionsTypeDef,
+        "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
+        "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
     },
     total=False,
 )
 
 
-class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
 
-_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+LFResourceDetailsTypeDef = TypedDict(
+    "LFResourceDetailsTypeDef",
+    {
+        "Database": DatabaseLFTagPolicyTypeDef,
+        "Table": TableLFTagPolicyTypeDef,
+    },
+    total=False,
+)
+
+_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
 
-class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
 
-LFResourceDetailsTypeDef = TypedDict(
-    "LFResourceDetailsTypeDef",
-    {
-        "Database": DatabaseLFTagPolicyTypeDef,
-        "Table": TableLFTagPolicyTypeDef,
-    },
-    total=False,
-)
-
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1426,78 +1644,91 @@
 )
 
 
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
 
-CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
-        "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
+        "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
+CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateEventActionRequestRequestTypeDef = TypedDict(
-    "CreateEventActionRequestRequestTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Event": EventTypeDef,
-    },
-)
-
 CreateEventActionResponseTypeDef = TypedDict(
     "CreateEventActionResponseTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
     },
 )
 
 GetEventActionResponseTypeDef = TypedDict(
     "GetEventActionResponseTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateEventActionResponseTypeDef = TypedDict(
+    "UpdateEventActionResponseTypeDef",
+    {
+        "Action": ActionOutputTypeDef,
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Event": EventOutputTypeDef,
+        "Id": str,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateEventActionRequestRequestTypeDef = TypedDict(
+    "CreateEventActionRequestRequestTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Event": EventTypeDef,
+    },
+)
+
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
     },
 )
 _OptionalUpdateEventActionRequestRequestTypeDef = TypedDict(
@@ -1511,56 +1742,23 @@
 
 class UpdateEventActionRequestRequestTypeDef(
     _RequiredUpdateEventActionRequestRequestTypeDef, _OptionalUpdateEventActionRequestRequestTypeDef
 ):
     pass
 
 
-UpdateEventActionResponseTypeDef = TypedDict(
-    "UpdateEventActionResponseTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Arn": str,
-        "CreatedAt": datetime,
-        "Event": EventTypeDef,
-        "Id": str,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
     },
 )
 
-RequestDetailsTypeDef = TypedDict(
-    "RequestDetailsTypeDef",
-    {
-        "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
-        "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
-        "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
-        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
-        "ImportAssetsFromS3": ImportAssetsFromS3RequestDetailsTypeDef,
-        "ImportAssetsFromRedshiftDataShares": (
-            ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef
-        ),
-        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
-        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
-        "ImportAssetsFromLakeFormationTagPolicy": (
-            ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
-        ),
-    },
-    total=False,
-)
-
 ResponseDetailsTypeDef = TypedDict(
     "ResponseDetailsTypeDef",
     {
         "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
         "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
         "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
         "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
@@ -1573,14 +1771,34 @@
         "ImportAssetsFromLakeFormationTagPolicy": (
             ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
         ),
     },
     total=False,
 )
 
+RequestDetailsTypeDef = TypedDict(
+    "RequestDetailsTypeDef",
+    {
+        "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
+        "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
+        "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
+        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
+        "ImportAssetsFromS3": ImportAssetsFromS3RequestDetailsTypeDef,
+        "ImportAssetsFromRedshiftDataShares": (
+            ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef
+        ),
+        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
+        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
+        "ImportAssetsFromLakeFormationTagPolicy": (
+            ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
+        ),
+    },
+    total=False,
+)
+
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1590,22 +1808,14 @@
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
     },
     total=False,
 )
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
-    {
-        "Details": RequestDetailsTypeDef,
-        "Type": TypeType,
-    },
-)
-
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
@@ -1653,14 +1863,22 @@
 )
 
 
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
 
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
+    {
+        "Details": RequestDetailsTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredLakeFormationDataPermissionAssetTypeDef = TypedDict(
     "_RequiredLakeFormationDataPermissionAssetTypeDef",
     {
         "LakeFormationDataPermissionDetails": LakeFormationDataPermissionDetailsTypeDef,
         "LakeFormationDataPermissionType": Literal["LFTagPolicy"],
         "Permissions": List[LFPermissionType],
     },
```

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange/type_defs.pyi` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -36,47 +36,56 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiGatewayApiAssetTypeDef",
+    "AssetDestinationEntryOutputTypeDef",
     "AssetDestinationEntryTypeDef",
     "RedshiftDataShareAssetTypeDef",
     "S3SnapshotAssetTypeDef",
+    "AssetSourceEntryOutputTypeDef",
     "AssetSourceEntryTypeDef",
+    "AutoExportRevisionDestinationEntryOutputTypeDef",
     "AutoExportRevisionDestinationEntryTypeDef",
+    "ExportServerSideEncryptionOutputTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
     "CreateRevisionRequestRequestTypeDef",
     "CreateRevisionResponseTypeDef",
+    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "RevisionPublishedOutputTypeDef",
     "RevisionPublishedTypeDef",
     "ExportAssetToSignedUrlRequestDetailsTypeDef",
     "ExportAssetToSignedUrlResponseDetailsTypeDef",
     "RevisionDestinationEntryTypeDef",
+    "RevisionDestinationEntryOutputTypeDef",
     "GetAssetRequestRequestTypeDef",
     "GetDataSetRequestRequestTypeDef",
     "GetEventActionRequestRequestTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "ImportAssetFromApiGatewayApiRequestDetailsTypeDef",
     "ImportAssetFromApiGatewayApiResponseDetailsTypeDef",
     "ImportAssetFromSignedUrlRequestDetailsTypeDef",
     "ImportAssetFromSignedUrlResponseDetailsTypeDef",
     "RedshiftDataShareAssetSourceEntryTypeDef",
+    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
+    "KmsKeyToGrantOutputTypeDef",
     "KmsKeyToGrantTypeDef",
     "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetRevisionsRequestRequestTypeDef",
     "RevisionEntryTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
     "ListEventActionsRequestListEventActionsPaginateTypeDef",
@@ -96,59 +105,65 @@
     "StartJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssetRequestRequestTypeDef",
     "UpdateDataSetRequestRequestTypeDef",
     "UpdateRevisionRequestRequestTypeDef",
     "UpdateRevisionResponseTypeDef",
-    "ImportAssetsFromS3RequestDetailsTypeDef",
     "ImportAssetsFromS3ResponseDetailsTypeDef",
+    "ImportAssetsFromS3RequestDetailsTypeDef",
+    "AutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    "ExportAssetsToS3ResponseDetailsTypeDef",
     "AutoExportRevisionToS3RequestDetailsTypeDef",
     "ExportAssetsToS3RequestDetailsTypeDef",
-    "ExportAssetsToS3ResponseDetailsTypeDef",
     "CreateDataSetResponseTypeDef",
     "DataSetEntryTypeDef",
     "GetDataSetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     "DatabaseLFTagPolicyTypeDef",
-    "TableLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyAndPermissionsOutputTypeDef",
     "TableLFTagPolicyTypeDef",
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyAndPermissionsTypeDef",
     "DetailsTypeDef",
+    "EventOutputTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
-    "S3DataAccessAssetSourceEntryTypeDef",
+    "S3DataAccessAssetSourceEntryOutputTypeDef",
     "S3DataAccessAssetTypeDef",
+    "S3DataAccessAssetSourceEntryTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
-    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
+    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
-    "CreateEventActionRequestRequestTypeDef",
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
-    "UpdateEventActionRequestRequestTypeDef",
     "UpdateEventActionResponseTypeDef",
+    "CreateEventActionRequestRequestTypeDef",
+    "UpdateEventActionRequestRequestTypeDef",
     "LFTagPolicyDetailsTypeDef",
-    "RequestDetailsTypeDef",
     "ResponseDetailsTypeDef",
+    "RequestDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "JobEntryTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "LakeFormationDataPermissionAssetTypeDef",
     "ListJobsResponseTypeDef",
     "AssetDetailsTypeDef",
     "AssetEntryTypeDef",
     "GetAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListRevisionAssetsResponseTypeDef",
@@ -166,14 +181,34 @@
         "ApiSpecificationDownloadUrlExpiresAt": datetime,
         "ProtocolType": Literal["REST"],
         "Stage": str,
     },
     total=False,
 )
 
+_RequiredAssetDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredAssetDestinationEntryOutputTypeDef",
+    {
+        "AssetId": str,
+        "Bucket": str,
+    },
+)
+_OptionalAssetDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalAssetDestinationEntryOutputTypeDef",
+    {
+        "Key": str,
+    },
+    total=False,
+)
+
+class AssetDestinationEntryOutputTypeDef(
+    _RequiredAssetDestinationEntryOutputTypeDef, _OptionalAssetDestinationEntryOutputTypeDef
+):
+    pass
+
 _RequiredAssetDestinationEntryTypeDef = TypedDict(
     "_RequiredAssetDestinationEntryTypeDef",
     {
         "AssetId": str,
         "Bucket": str,
     },
 )
@@ -200,22 +235,50 @@
 S3SnapshotAssetTypeDef = TypedDict(
     "S3SnapshotAssetTypeDef",
     {
         "Size": float,
     },
 )
 
+AssetSourceEntryOutputTypeDef = TypedDict(
+    "AssetSourceEntryOutputTypeDef",
+    {
+        "Bucket": str,
+        "Key": str,
+    },
+)
+
 AssetSourceEntryTypeDef = TypedDict(
     "AssetSourceEntryTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
 )
 
+_RequiredAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredAutoExportRevisionDestinationEntryOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalAutoExportRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalAutoExportRevisionDestinationEntryOutputTypeDef",
+    {
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+class AutoExportRevisionDestinationEntryOutputTypeDef(
+    _RequiredAutoExportRevisionDestinationEntryOutputTypeDef,
+    _OptionalAutoExportRevisionDestinationEntryOutputTypeDef,
+):
+    pass
+
 _RequiredAutoExportRevisionDestinationEntryTypeDef = TypedDict(
     "_RequiredAutoExportRevisionDestinationEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalAutoExportRevisionDestinationEntryTypeDef = TypedDict(
@@ -228,14 +291,34 @@
 
 class AutoExportRevisionDestinationEntryTypeDef(
     _RequiredAutoExportRevisionDestinationEntryTypeDef,
     _OptionalAutoExportRevisionDestinationEntryTypeDef,
 ):
     pass
 
+_RequiredExportServerSideEncryptionOutputTypeDef = TypedDict(
+    "_RequiredExportServerSideEncryptionOutputTypeDef",
+    {
+        "Type": ServerSideEncryptionTypesType,
+    },
+)
+_OptionalExportServerSideEncryptionOutputTypeDef = TypedDict(
+    "_OptionalExportServerSideEncryptionOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
+class ExportServerSideEncryptionOutputTypeDef(
+    _RequiredExportServerSideEncryptionOutputTypeDef,
+    _OptionalExportServerSideEncryptionOutputTypeDef,
+):
+    pass
+
 _RequiredExportServerSideEncryptionTypeDef = TypedDict(
     "_RequiredExportServerSideEncryptionTypeDef",
     {
         "Type": ServerSideEncryptionTypesType,
     },
 )
 _OptionalExportServerSideEncryptionTypeDef = TypedDict(
@@ -321,14 +404,22 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -374,14 +465,21 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RevisionPublishedOutputTypeDef = TypedDict(
+    "RevisionPublishedOutputTypeDef",
+    {
+        "DataSetId": str,
+    },
+)
+
 RevisionPublishedTypeDef = TypedDict(
     "RevisionPublishedTypeDef",
     {
         "DataSetId": str,
     },
 )
 
@@ -433,14 +531,34 @@
 )
 
 class RevisionDestinationEntryTypeDef(
     _RequiredRevisionDestinationEntryTypeDef, _OptionalRevisionDestinationEntryTypeDef
 ):
     pass
 
+_RequiredRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_RequiredRevisionDestinationEntryOutputTypeDef",
+    {
+        "Bucket": str,
+        "RevisionId": str,
+    },
+)
+_OptionalRevisionDestinationEntryOutputTypeDef = TypedDict(
+    "_OptionalRevisionDestinationEntryOutputTypeDef",
+    {
+        "KeyPattern": str,
+    },
+    total=False,
+)
+
+class RevisionDestinationEntryOutputTypeDef(
+    _RequiredRevisionDestinationEntryOutputTypeDef, _OptionalRevisionDestinationEntryOutputTypeDef
+):
+    pass
+
 GetAssetRequestRequestTypeDef = TypedDict(
     "GetAssetRequestRequestTypeDef",
     {
         "AssetId": str,
         "DataSetId": str,
         "RevisionId": str,
     },
@@ -587,14 +705,28 @@
 RedshiftDataShareAssetSourceEntryTypeDef = TypedDict(
     "RedshiftDataShareAssetSourceEntryTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
+RedshiftDataShareAssetSourceEntryOutputTypeDef = TypedDict(
+    "RedshiftDataShareAssetSourceEntryOutputTypeDef",
+    {
+        "DataShareArn": str,
+    },
+)
+
+KmsKeyToGrantOutputTypeDef = TypedDict(
+    "KmsKeyToGrantOutputTypeDef",
+    {
+        "KmsKeyArn": str,
+    },
+)
+
 KmsKeyToGrantTypeDef = TypedDict(
     "KmsKeyToGrantTypeDef",
     {
         "KmsKeyArn": str,
     },
 )
 
@@ -952,31 +1084,72 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
+    "ImportAssetsFromS3ResponseDetailsTypeDef",
+    {
+        "AssetSources": List[AssetSourceEntryOutputTypeDef],
+        "DataSetId": str,
+        "RevisionId": str,
+    },
+)
+
 ImportAssetsFromS3RequestDetailsTypeDef = TypedDict(
     "ImportAssetsFromS3RequestDetailsTypeDef",
     {
         "AssetSources": Sequence[AssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-ImportAssetsFromS3ResponseDetailsTypeDef = TypedDict(
-    "ImportAssetsFromS3ResponseDetailsTypeDef",
+_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
+    "_RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    {
+        "RevisionDestination": AutoExportRevisionDestinationEntryOutputTypeDef,
+    },
+)
+_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef = TypedDict(
+    "_OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+class AutoExportRevisionToS3RequestDetailsOutputTypeDef(
+    _RequiredAutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    _OptionalAutoExportRevisionToS3RequestDetailsOutputTypeDef,
+):
+    pass
+
+_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
     {
-        "AssetSources": List[AssetSourceEntryTypeDef],
+        "AssetDestinations": List[AssetDestinationEntryOutputTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
+_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
+    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
+    {
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+class ExportAssetsToS3ResponseDetailsTypeDef(
+    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
+):
+    pass
 
 _RequiredAutoExportRevisionToS3RequestDetailsTypeDef = TypedDict(
     "_RequiredAutoExportRevisionToS3RequestDetailsTypeDef",
     {
         "RevisionDestination": AutoExportRevisionDestinationEntryTypeDef,
     },
 )
@@ -1011,35 +1184,14 @@
 )
 
 class ExportAssetsToS3RequestDetailsTypeDef(
     _RequiredExportAssetsToS3RequestDetailsTypeDef, _OptionalExportAssetsToS3RequestDetailsTypeDef
 ):
     pass
 
-_RequiredExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_RequiredExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "AssetDestinations": List[AssetDestinationEntryTypeDef],
-        "DataSetId": str,
-        "RevisionId": str,
-    },
-)
-_OptionalExportAssetsToS3ResponseDetailsTypeDef = TypedDict(
-    "_OptionalExportAssetsToS3ResponseDetailsTypeDef",
-    {
-        "Encryption": ExportServerSideEncryptionTypeDef,
-    },
-    total=False,
-)
-
-class ExportAssetsToS3ResponseDetailsTypeDef(
-    _RequiredExportAssetsToS3ResponseDetailsTypeDef, _OptionalExportAssetsToS3ResponseDetailsTypeDef
-):
-    pass
-
 CreateDataSetResponseTypeDef = TypedDict(
     "CreateDataSetResponseTypeDef",
     {
         "Arn": str,
         "AssetType": AssetTypeType,
         "CreatedAt": datetime,
         "Description": str,
@@ -1110,49 +1262,73 @@
         "OriginDetails": OriginDetailsTypeDef,
         "SourceId": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[Literal["DESCRIBE"]],
+        "Expression": List[LFTagOutputTypeDef],
+        "Permissions": List[Literal["DESCRIBE"]],
     },
 )
 
 DatabaseLFTagPolicyTypeDef = TypedDict(
     "DatabaseLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagTypeDef],
+        "Expression": List[LFTagOutputTypeDef],
     },
 )
 
-TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsTypeDef",
+TableLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsOutputTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[TableTagPolicyLFPermissionType],
+        "Expression": List[LFTagOutputTypeDef],
+        "Permissions": List[TableTagPolicyLFPermissionType],
     },
 )
 
 TableLFTagPolicyTypeDef = TypedDict(
     "TableLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagTypeDef],
+        "Expression": List[LFTagOutputTypeDef],
+    },
+)
+
+DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[Literal["DESCRIBE"]],
+    },
+)
+
+TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsTypeDef",
+    {
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[TableTagPolicyLFPermissionType],
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
-        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryTypeDef],
+        "ImportAssetsFromS3JobErrorDetails": List[AssetSourceEntryOutputTypeDef],
+    },
+    total=False,
+)
+
+EventOutputTypeDef = TypedDict(
+    "EventOutputTypeDef",
+    {
+        "RevisionPublished": RevisionPublishedOutputTypeDef,
     },
     total=False,
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
@@ -1182,21 +1358,21 @@
 ):
     pass
 
 _RequiredExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_RequiredExportRevisionsToS3ResponseDetailsTypeDef",
     {
         "DataSetId": str,
-        "RevisionDestinations": List[RevisionDestinationEntryTypeDef],
+        "RevisionDestinations": List[RevisionDestinationEntryOutputTypeDef],
     },
 )
 _OptionalExportRevisionsToS3ResponseDetailsTypeDef = TypedDict(
     "_OptionalExportRevisionsToS3ResponseDetailsTypeDef",
     {
-        "Encryption": ExportServerSideEncryptionTypeDef,
+        "Encryption": ExportServerSideEncryptionOutputTypeDef,
         "EventActionArn": str,
     },
     total=False,
 )
 
 class ExportRevisionsToS3ResponseDetailsTypeDef(
     _RequiredExportRevisionsToS3ResponseDetailsTypeDef,
@@ -1212,38 +1388,39 @@
         "RevisionId": str,
     },
 )
 
 ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef = TypedDict(
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
     {
-        "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
+        "AssetSources": List[RedshiftDataShareAssetSourceEntryOutputTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+_RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
     {
         "Bucket": str,
     },
 )
-_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+_OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
     {
-        "KeyPrefixes": Sequence[str],
-        "Keys": Sequence[str],
-        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+        "KeyPrefixes": List[str],
+        "Keys": List[str],
+        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
     },
     total=False,
 )
 
-class S3DataAccessAssetSourceEntryTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+class S3DataAccessAssetSourceEntryOutputTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
+    _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
 ):
     pass
 
 _RequiredS3DataAccessAssetTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetTypeDef",
     {
         "Bucket": str,
@@ -1252,33 +1429,62 @@
 _OptionalS3DataAccessAssetTypeDef = TypedDict(
     "_OptionalS3DataAccessAssetTypeDef",
     {
         "KeyPrefixes": List[str],
         "Keys": List[str],
         "S3AccessPointAlias": str,
         "S3AccessPointArn": str,
-        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
+        "KmsKeysToGrant": List[KmsKeyToGrantOutputTypeDef],
     },
     total=False,
 )
 
 class S3DataAccessAssetTypeDef(
     _RequiredS3DataAccessAssetTypeDef, _OptionalS3DataAccessAssetTypeDef
 ):
     pass
 
+_RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_RequiredS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
+    "_OptionalS3DataAccessAssetSourceEntryTypeDef",
+    {
+        "KeyPrefixes": Sequence[str],
+        "Keys": Sequence[str],
+        "KmsKeysToGrant": Sequence[KmsKeyToGrantTypeDef],
+    },
+    total=False,
+)
+
+class S3DataAccessAssetSourceEntryTypeDef(
+    _RequiredS3DataAccessAssetSourceEntryTypeDef, _OptionalS3DataAccessAssetSourceEntryTypeDef
+):
+    pass
+
 ListDataSetRevisionsResponseTypeDef = TypedDict(
     "ListDataSetRevisionsResponseTypeDef",
     {
         "NextToken": str,
         "Revisions": List[RevisionEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ExportRevisionToS3": AutoExportRevisionToS3RequestDetailsTypeDef,
     },
     total=False,
 )
@@ -1288,71 +1494,71 @@
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
-        "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
-        "Table": TableLFTagPolicyAndPermissionsTypeDef,
+        "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
+        "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
     },
     total=False,
 )
 
-class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
-_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+LFResourceDetailsTypeDef = TypedDict(
+    "LFResourceDetailsTypeDef",
+    {
+        "Database": DatabaseLFTagPolicyTypeDef,
+        "Table": TableLFTagPolicyTypeDef,
+    },
+    total=False,
+)
+
+_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
-class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
-LFResourceDetailsTypeDef = TypedDict(
-    "LFResourceDetailsTypeDef",
-    {
-        "Database": DatabaseLFTagPolicyTypeDef,
-        "Table": TableLFTagPolicyTypeDef,
-    },
-    total=False,
-)
-
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1367,78 +1573,91 @@
     },
     total=False,
 )
 
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
-CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
-        "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
+        "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
+CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateEventActionRequestRequestTypeDef = TypedDict(
-    "CreateEventActionRequestRequestTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Event": EventTypeDef,
-    },
-)
-
 CreateEventActionResponseTypeDef = TypedDict(
     "CreateEventActionResponseTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventActionEntryTypeDef = TypedDict(
     "EventActionEntryTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
     },
 )
 
 GetEventActionResponseTypeDef = TypedDict(
     "GetEventActionResponseTypeDef",
     {
-        "Action": ActionTypeDef,
+        "Action": ActionOutputTypeDef,
         "Arn": str,
         "CreatedAt": datetime,
-        "Event": EventTypeDef,
+        "Event": EventOutputTypeDef,
+        "Id": str,
+        "UpdatedAt": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateEventActionResponseTypeDef = TypedDict(
+    "UpdateEventActionResponseTypeDef",
+    {
+        "Action": ActionOutputTypeDef,
+        "Arn": str,
+        "CreatedAt": datetime,
+        "Event": EventOutputTypeDef,
         "Id": str,
         "UpdatedAt": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateEventActionRequestRequestTypeDef = TypedDict(
+    "CreateEventActionRequestRequestTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "Event": EventTypeDef,
+    },
+)
+
 _RequiredUpdateEventActionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventActionRequestRequestTypeDef",
     {
         "EventActionId": str,
     },
 )
 _OptionalUpdateEventActionRequestRequestTypeDef = TypedDict(
@@ -1450,56 +1669,23 @@
 )
 
 class UpdateEventActionRequestRequestTypeDef(
     _RequiredUpdateEventActionRequestRequestTypeDef, _OptionalUpdateEventActionRequestRequestTypeDef
 ):
     pass
 
-UpdateEventActionResponseTypeDef = TypedDict(
-    "UpdateEventActionResponseTypeDef",
-    {
-        "Action": ActionTypeDef,
-        "Arn": str,
-        "CreatedAt": datetime,
-        "Event": EventTypeDef,
-        "Id": str,
-        "UpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LFTagPolicyDetailsTypeDef = TypedDict(
     "LFTagPolicyDetailsTypeDef",
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
     },
 )
 
-RequestDetailsTypeDef = TypedDict(
-    "RequestDetailsTypeDef",
-    {
-        "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
-        "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
-        "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
-        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
-        "ImportAssetsFromS3": ImportAssetsFromS3RequestDetailsTypeDef,
-        "ImportAssetsFromRedshiftDataShares": (
-            ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef
-        ),
-        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
-        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
-        "ImportAssetsFromLakeFormationTagPolicy": (
-            ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
-        ),
-    },
-    total=False,
-)
-
 ResponseDetailsTypeDef = TypedDict(
     "ResponseDetailsTypeDef",
     {
         "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
         "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
         "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
         "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
@@ -1512,14 +1698,34 @@
         "ImportAssetsFromLakeFormationTagPolicy": (
             ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
         ),
     },
     total=False,
 )
 
+RequestDetailsTypeDef = TypedDict(
+    "RequestDetailsTypeDef",
+    {
+        "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
+        "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
+        "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
+        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
+        "ImportAssetsFromS3": ImportAssetsFromS3RequestDetailsTypeDef,
+        "ImportAssetsFromRedshiftDataShares": (
+            ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef
+        ),
+        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
+        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
+        "ImportAssetsFromLakeFormationTagPolicy": (
+            ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
+        ),
+    },
+    total=False,
+)
+
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1529,22 +1735,14 @@
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
     },
     total=False,
 )
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
-    {
-        "Details": RequestDetailsTypeDef,
-        "Type": TypeType,
-    },
-)
-
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
@@ -1590,14 +1788,22 @@
     },
     total=False,
 )
 
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
+    {
+        "Details": RequestDetailsTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredLakeFormationDataPermissionAssetTypeDef = TypedDict(
     "_RequiredLakeFormationDataPermissionAssetTypeDef",
     {
         "LakeFormationDataPermissionDetails": LakeFormationDataPermissionDetailsTypeDef,
         "LakeFormationDataPermissionType": Literal["LFTagPolicy"],
         "Permissions": List[LFPermissionType],
     },
```

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/PKG-INFO` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dataexchange
-Version: 1.28.0
-Summary: Type annotations for boto3.DataExchange 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-dataexchange"></a>
 
 # mypy-boto3-dataexchange
 
 [![PyPI - mypy-boto3-dataexchange](https://img.shields.io/pypi/v/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dataexchange.svg?color=blue)](https://pypi.org/project/mypy-boto3-dataexchange)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-dataexchange?color=blue)](https://pypistats.org/packages/mypy-boto3-dataexchange)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dataexchange)](https://pepy.tech/project/mypy-boto3-dataexchange)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataExchange 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
+[boto3.DataExchange 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
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
 [mypy-boto3-dataexchange docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dataexchange/).
 
 See how it helps to find and fix potential bugs:
 
@@ -352,47 +352,56 @@
 
 `mypy_boto3_dataexchange.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dataexchange.type_defs import (
     ApiGatewayApiAssetTypeDef,
+    AssetDestinationEntryOutputTypeDef,
     AssetDestinationEntryTypeDef,
     RedshiftDataShareAssetTypeDef,
     S3SnapshotAssetTypeDef,
+    AssetSourceEntryOutputTypeDef,
     AssetSourceEntryTypeDef,
+    AutoExportRevisionDestinationEntryOutputTypeDef,
     AutoExportRevisionDestinationEntryTypeDef,
+    ExportServerSideEncryptionOutputTypeDef,
     ExportServerSideEncryptionTypeDef,
     CancelJobRequestRequestTypeDef,
     CreateDataSetRequestRequestTypeDef,
     OriginDetailsTypeDef,
     CreateRevisionRequestRequestTypeDef,
     CreateRevisionResponseTypeDef,
+    LFTagOutputTypeDef,
     LFTagTypeDef,
     DeleteAssetRequestRequestTypeDef,
     DeleteDataSetRequestRequestTypeDef,
     DeleteEventActionRequestRequestTypeDef,
     DeleteRevisionRequestRequestTypeDef,
     ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
     EmptyResponseMetadataTypeDef,
+    RevisionPublishedOutputTypeDef,
     RevisionPublishedTypeDef,
     ExportAssetToSignedUrlRequestDetailsTypeDef,
     ExportAssetToSignedUrlResponseDetailsTypeDef,
     RevisionDestinationEntryTypeDef,
+    RevisionDestinationEntryOutputTypeDef,
     GetAssetRequestRequestTypeDef,
     GetDataSetRequestRequestTypeDef,
     GetEventActionRequestRequestTypeDef,
     GetJobRequestRequestTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     ImportAssetFromApiGatewayApiRequestDetailsTypeDef,
     ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
     ImportAssetFromSignedUrlRequestDetailsTypeDef,
     ImportAssetFromSignedUrlResponseDetailsTypeDef,
     RedshiftDataShareAssetSourceEntryTypeDef,
+    RedshiftDataShareAssetSourceEntryOutputTypeDef,
+    KmsKeyToGrantOutputTypeDef,
     KmsKeyToGrantTypeDef,
     ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef,
     ListDataSetRevisionsRequestRequestTypeDef,
     RevisionEntryTypeDef,
     ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
     ListEventActionsRequestListEventActionsPaginateTypeDef,
@@ -412,59 +421,65 @@
     StartJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssetRequestRequestTypeDef,
     UpdateDataSetRequestRequestTypeDef,
     UpdateRevisionRequestRequestTypeDef,
     UpdateRevisionResponseTypeDef,
-    ImportAssetsFromS3RequestDetailsTypeDef,
     ImportAssetsFromS3ResponseDetailsTypeDef,
+    ImportAssetsFromS3RequestDetailsTypeDef,
+    AutoExportRevisionToS3RequestDetailsOutputTypeDef,
+    ExportAssetsToS3ResponseDetailsTypeDef,
     AutoExportRevisionToS3RequestDetailsTypeDef,
     ExportAssetsToS3RequestDetailsTypeDef,
-    ExportAssetsToS3ResponseDetailsTypeDef,
     CreateDataSetResponseTypeDef,
     DataSetEntryTypeDef,
     GetDataSetResponseTypeDef,
     UpdateDataSetResponseTypeDef,
-    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
     DatabaseLFTagPolicyTypeDef,
-    TableLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsOutputTypeDef,
     TableLFTagPolicyTypeDef,
+    DatabaseLFTagPolicyAndPermissionsTypeDef,
+    TableLFTagPolicyAndPermissionsTypeDef,
     DetailsTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
     ExportRevisionsToS3RequestDetailsTypeDef,
     ExportRevisionsToS3ResponseDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef,
     ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef,
-    S3DataAccessAssetSourceEntryTypeDef,
+    S3DataAccessAssetSourceEntryOutputTypeDef,
     S3DataAccessAssetTypeDef,
+    S3DataAccessAssetSourceEntryTypeDef,
     ListDataSetRevisionsResponseTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ListDataSetsResponseTypeDef,
-    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
     LFResourceDetailsTypeDef,
+    ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
     JobErrorTypeDef,
-    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
-    CreateEventActionRequestRequestTypeDef,
+    CreateS3DataAccessFromS3BucketRequestDetailsTypeDef,
     CreateEventActionResponseTypeDef,
     EventActionEntryTypeDef,
     GetEventActionResponseTypeDef,
-    UpdateEventActionRequestRequestTypeDef,
     UpdateEventActionResponseTypeDef,
+    CreateEventActionRequestRequestTypeDef,
+    UpdateEventActionRequestRequestTypeDef,
     LFTagPolicyDetailsTypeDef,
-    RequestDetailsTypeDef,
     ResponseDetailsTypeDef,
+    RequestDetailsTypeDef,
     ListEventActionsResponseTypeDef,
     LakeFormationDataPermissionDetailsTypeDef,
-    CreateJobRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     JobEntryTypeDef,
+    CreateJobRequestRequestTypeDef,
     LakeFormationDataPermissionAssetTypeDef,
     ListJobsResponseTypeDef,
     AssetDetailsTypeDef,
     AssetEntryTypeDef,
     GetAssetResponseTypeDef,
     UpdateAssetResponseTypeDef,
     ListRevisionAssetsResponseTypeDef,
```

### Comparing `mypy-boto3-dataexchange-1.28.0/mypy_boto3_dataexchange.egg-info/SOURCES.txt` & `mypy-boto3-dataexchange-1.28.12/mypy_boto3_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dataexchange-1.28.0/setup.py` & `mypy-boto3-dataexchange-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dataexchange",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataExchange 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.DataExchange 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

