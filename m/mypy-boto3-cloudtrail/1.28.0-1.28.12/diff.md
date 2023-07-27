# Comparing `tmp/mypy-boto3-cloudtrail-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudtrail-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudtrail-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudtrail-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
```

## Comparing `mypy-boto3-cloudtrail-1.28.0.tar` & `mypy-boto3-cloudtrail-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.386250 mypy-boto3-cloudtrail-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-06 20:59:12.382250 mypy-boto3-cloudtrail-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.378250 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39017 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10111 2023-07-06 20:35:33.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39814 2023-07-06 20:35:34.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39779 2023-07-06 20:35:33.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.378250 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:12.000000 mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.386250 mypy-boto3-cloudtrail-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:31.000000 mypy-boto3-cloudtrail-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16557 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:26.992556 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39076 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39017 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10187 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42799 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42758 2023-07-27 05:18:48.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:26.000000 mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.004557 mypy-boto3-cloudtrail-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:47.000000 mypy-boto3-cloudtrail-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/LICENSE` & `mypy-boto3-cloudtrail-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudTrail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,20 +348,24 @@
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    DestinationOutputTypeDef,
+    TagOutputTypeDef,
     CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -372,25 +376,27 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorTypeDef,
+    InsightSelectorOutputTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
     GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
+    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
+    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
     ListPublicKeysRequestListPublicKeysPaginateTypeDef,
@@ -418,55 +424,58 @@
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
     UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    ResourceTagTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
+    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/README.md` & `mypy-boto3-cloudtrail-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,20 +316,24 @@
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    DestinationOutputTypeDef,
+    TagOutputTypeDef,
     CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -340,25 +344,27 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorTypeDef,
+    InsightSelectorOutputTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
     GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
+    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
+    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
     ListPublicKeysRequestListPublicKeysPaginateTypeDef,
@@ -386,55 +392,58 @@
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
     UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    ResourceTagTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
+    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__init__.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__init__.pyi` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/__main__.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudTrail 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudTrail 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/client.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/client.pyi` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/literals.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
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
@@ -288,26 +289,28 @@
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

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/literals.pyi` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -200,14 +200,15 @@
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
@@ -286,26 +287,28 @@
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

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/paginator.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/paginator.pyi` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/type_defs.py` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,20 +35,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
+    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
+    "DestinationOutputTypeDef",
+    "TagOutputTypeDef",
     "CreateTrailResponseTypeDef",
+    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -59,25 +63,27 @@
     "GetChannelRequestRequestTypeDef",
     "IngestionStatusTypeDef",
     "GetEventDataStoreRequestRequestTypeDef",
     "GetEventSelectorsRequestRequestTypeDef",
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
-    "InsightSelectorTypeDef",
+    "InsightSelectorOutputTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
     "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
+    "S3ImportSourceOutputTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
+    "InsightSelectorTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
     "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
@@ -105,55 +111,58 @@
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
     "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResourceTagTypeDef",
+    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "ResourceTagTypeDef",
+    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
-    "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
+    "ImportSourceOutputTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
+    "PutInsightSelectorsRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "GetEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
@@ -169,14 +178,40 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
+_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Field": str,
+    },
+)
+_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Equals": List[str],
+        "StartsWith": List[str],
+        "EndsWith": List[str],
+        "NotEquals": List[str],
+        "NotStartsWith": List[str],
+        "NotEndsWith": List[str],
+    },
+    total=False,
+)
+
+
+class AdvancedFieldSelectorOutputTypeDef(
+    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
+):
+    pass
+
+
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -242,14 +277,41 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "Type": DestinationTypeType,
+        "Location": str,
+    },
+)
+
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
 CreateTrailResponseTypeDef = TypedDict(
     "CreateTrailResponseTypeDef",
     {
         "Name": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "SnsTopicName": str,
@@ -262,19 +324,28 @@
         "CloudWatchLogsRoleArn": str,
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataResourceOutputTypeDef = TypedDict(
+    "DataResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -428,16 +499,16 @@
 GetInsightSelectorsRequestRequestTypeDef = TypedDict(
     "GetInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
     },
 )
 
-InsightSelectorTypeDef = TypedDict(
-    "InsightSelectorTypeDef",
+InsightSelectorOutputTypeDef = TypedDict(
+    "InsightSelectorOutputTypeDef",
     {
         "InsightType": InsightTypeType,
     },
     total=False,
 )
 
 _RequiredGetQueryResultsRequestRequestTypeDef = TypedDict(
@@ -535,14 +606,23 @@
         "ErrorType": str,
         "ErrorMessage": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+S3ImportSourceOutputTypeDef = TypedDict(
+    "S3ImportSourceOutputTypeDef",
+    {
+        "S3LocationUri": str,
+        "S3BucketRegion": str,
+        "S3BucketAccessRoleArn": str,
+    },
+)
+
 S3ImportSourceTypeDef = TypedDict(
     "S3ImportSourceTypeDef",
     {
         "S3LocationUri": str,
         "S3BucketRegion": str,
         "S3BucketAccessRoleArn": str,
     },
@@ -556,14 +636,22 @@
         "Destinations": List[str],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+InsightSelectorTypeDef = TypedDict(
+    "InsightSelectorTypeDef",
+    {
+        "InsightType": InsightTypeType,
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -985,23 +1073,35 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
+_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedEventSelectorOutputTypeDef",
     {
-        "ResourceId": str,
-        "TagsList": List[TagTypeDef],
+        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
+    },
+)
+_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedEventSelectorOutputTypeDef",
+    {
+        "Name": str,
     },
     total=False,
 )
 
+
+class AdvancedEventSelectorOutputTypeDef(
+    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
+):
+    pass
+
+
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -1047,26 +1147,14 @@
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "Name": str,
-        "Source": str,
-        "Destinations": List[DestinationTypeDef],
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1087,26 +1175,58 @@
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
-        "Destinations": List[DestinationTypeDef],
+        "Destinations": List[DestinationOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "Name": str,
+        "Source": str,
+        "Destinations": List[DestinationOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "ResourceId": str,
+        "TagsList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+EventSelectorOutputTypeDef = TypedDict(
+    "EventSelectorOutputTypeDef",
+    {
+        "ReadWriteType": ReadWriteTypeType,
+        "IncludeManagementEvents": bool,
+        "DataResources": List[DataResourceOutputTypeDef],
+        "ExcludeManagementEventSources": List[str],
+    },
+    total=False,
+)
+
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceTypeDef],
-        "ExcludeManagementEventSources": List[str],
+        "DataResources": Sequence[DataResourceTypeDef],
+        "ExcludeManagementEventSources": Sequence[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
@@ -1153,32 +1273,24 @@
     total=False,
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorTypeDef],
+        "InsightSelectors": List[InsightSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutInsightSelectorsRequestRequestTypeDef = TypedDict(
-    "PutInsightSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-        "InsightSelectors": Sequence[InsightSelectorTypeDef],
-    },
-)
-
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorTypeDef],
+        "InsightSelectors": List[InsightSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
@@ -1196,14 +1308,21 @@
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImportSourceOutputTypeDef = TypedDict(
+    "ImportSourceOutputTypeDef",
+    {
+        "S3": S3ImportSourceOutputTypeDef,
+    },
+)
+
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
     },
 )
 
@@ -1212,14 +1331,22 @@
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutInsightSelectorsRequestRequestTypeDef = TypedDict(
+    "PutInsightSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+        "InsightSelectors": Sequence[InsightSelectorTypeDef],
+    },
+)
+
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1264,79 +1391,41 @@
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "ResourceTagList": List[ResourceTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
-        "TagsList": List[TagTypeDef],
+        "TagsList": List[TagOutputTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1344,15 +1433,15 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1362,15 +1451,15 @@
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1378,19 +1467,66 @@
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+    },
+    total=False,
+)
+
+UpdateEventDataStoreResponseTypeDef = TypedDict(
+    "UpdateEventDataStoreResponseTypeDef",
+    {
+        "EventDataStoreArn": str,
+        "Name": str,
+        "Status": EventDataStoreStatusType,
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "KmsKeyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
     },
     total=False,
 )
 
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 _OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
@@ -1411,38 +1547,39 @@
 class UpdateEventDataStoreRequestRequestTypeDef(
     _RequiredUpdateEventDataStoreRequestRequestTypeDef,
     _OptionalUpdateEventDataStoreRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateEventDataStoreResponseTypeDef = TypedDict(
-    "UpdateEventDataStoreResponseTypeDef",
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
     {
-        "EventDataStoreArn": str,
-        "Name": str,
-        "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "KmsKeyId": str,
+        "ResourceTagList": List[ResourceTagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutEventSelectorsResponseTypeDef = TypedDict(
+    "PutEventSelectorsResponseTypeDef",
+    {
+        "TrailARN": str,
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
@@ -1461,92 +1598,82 @@
 
 class PutEventSelectorsRequestRequestTypeDef(
     _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
 ):
     pass
 
 
-PutEventSelectorsResponseTypeDef = TypedDict(
-    "PutEventSelectorsResponseTypeDef",
-    {
-        "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartImportRequestRequestTypeDef = TypedDict(
-    "StartImportRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[str],
-        "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
-        "ImportId": str,
-    },
-    total=False,
-)
-
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartImportRequestRequestTypeDef = TypedDict(
+    "StartImportRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[str],
+        "ImportSource": ImportSourceTypeDef,
+        "StartEventTime": Union[datetime, str],
+        "EndEventTime": Union[datetime, str],
+        "ImportId": str,
+    },
+    total=False,
+)
+
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1555,12 +1682,12 @@
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
-        "Destinations": List[DestinationTypeDef],
+        "Destinations": List[DestinationOutputTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail/type_defs.pyi` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
+    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
+    "DestinationOutputTypeDef",
+    "TagOutputTypeDef",
     "CreateTrailResponseTypeDef",
+    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -58,25 +62,27 @@
     "GetChannelRequestRequestTypeDef",
     "IngestionStatusTypeDef",
     "GetEventDataStoreRequestRequestTypeDef",
     "GetEventSelectorsRequestRequestTypeDef",
     "GetImportRequestRequestTypeDef",
     "ImportStatisticsTypeDef",
     "GetInsightSelectorsRequestRequestTypeDef",
-    "InsightSelectorTypeDef",
+    "InsightSelectorOutputTypeDef",
     "GetQueryResultsRequestRequestTypeDef",
     "QueryStatisticsTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetTrailRequestRequestTypeDef",
     "GetTrailStatusRequestRequestTypeDef",
     "GetTrailStatusResponseTypeDef",
     "ImportFailureListItemTypeDef",
+    "S3ImportSourceOutputTypeDef",
     "S3ImportSourceTypeDef",
     "ImportsListItemTypeDef",
+    "InsightSelectorTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListEventDataStoresRequestRequestTypeDef",
     "ListImportFailuresRequestListImportFailuresPaginateTypeDef",
     "ListImportFailuresRequestRequestTypeDef",
     "ListImportsRequestListImportsPaginateTypeDef",
     "ListImportsRequestRequestTypeDef",
     "ListPublicKeysRequestListPublicKeysPaginateTypeDef",
@@ -104,55 +110,58 @@
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
     "UpdateTrailResponseTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
-    "ResourceTagTypeDef",
+    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "ResourceTagTypeDef",
+    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
-    "PutInsightSelectorsRequestRequestTypeDef",
     "PutInsightSelectorsResponseTypeDef",
     "GetQueryResultsResponseTypeDef",
     "ListImportFailuresResponseTypeDef",
+    "ImportSourceOutputTypeDef",
     "ImportSourceTypeDef",
     "ListImportsResponseTypeDef",
+    "PutInsightSelectorsRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "GetEventSelectorsResponseTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
-    "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
+    "StartImportRequestRequestTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
@@ -166,14 +175,38 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
+_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Field": str,
+    },
+)
+_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedFieldSelectorOutputTypeDef",
+    {
+        "Equals": List[str],
+        "StartsWith": List[str],
+        "EndsWith": List[str],
+        "NotEquals": List[str],
+        "NotStartsWith": List[str],
+        "NotEndsWith": List[str],
+    },
+    total=False,
+)
+
+class AdvancedFieldSelectorOutputTypeDef(
+    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
+):
+    pass
+
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -235,14 +268,39 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
+DestinationOutputTypeDef = TypedDict(
+    "DestinationOutputTypeDef",
+    {
+        "Type": DestinationTypeType,
+        "Location": str,
+    },
+)
+
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
 CreateTrailResponseTypeDef = TypedDict(
     "CreateTrailResponseTypeDef",
     {
         "Name": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "SnsTopicName": str,
@@ -255,19 +313,28 @@
         "CloudWatchLogsRoleArn": str,
         "KmsKeyId": str,
         "IsOrganizationTrail": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DataResourceOutputTypeDef = TypedDict(
+    "DataResourceOutputTypeDef",
+    {
+        "Type": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": List[str],
+        "Values": Sequence[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -421,16 +488,16 @@
 GetInsightSelectorsRequestRequestTypeDef = TypedDict(
     "GetInsightSelectorsRequestRequestTypeDef",
     {
         "TrailName": str,
     },
 )
 
-InsightSelectorTypeDef = TypedDict(
-    "InsightSelectorTypeDef",
+InsightSelectorOutputTypeDef = TypedDict(
+    "InsightSelectorOutputTypeDef",
     {
         "InsightType": InsightTypeType,
     },
     total=False,
 )
 
 _RequiredGetQueryResultsRequestRequestTypeDef = TypedDict(
@@ -526,14 +593,23 @@
         "ErrorType": str,
         "ErrorMessage": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+S3ImportSourceOutputTypeDef = TypedDict(
+    "S3ImportSourceOutputTypeDef",
+    {
+        "S3LocationUri": str,
+        "S3BucketRegion": str,
+        "S3BucketAccessRoleArn": str,
+    },
+)
+
 S3ImportSourceTypeDef = TypedDict(
     "S3ImportSourceTypeDef",
     {
         "S3LocationUri": str,
         "S3BucketRegion": str,
         "S3BucketAccessRoleArn": str,
     },
@@ -547,14 +623,22 @@
         "Destinations": List[str],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+InsightSelectorTypeDef = TypedDict(
+    "InsightSelectorTypeDef",
+    {
+        "InsightType": InsightTypeType,
+    },
+    total=False,
+)
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -962,23 +1046,33 @@
     "RemoveTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagsList": Sequence[TagTypeDef],
     },
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
+_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_RequiredAdvancedEventSelectorOutputTypeDef",
     {
-        "ResourceId": str,
-        "TagsList": List[TagTypeDef],
+        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
+    },
+)
+_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
+    "_OptionalAdvancedEventSelectorOutputTypeDef",
+    {
+        "Name": str,
     },
     total=False,
 )
 
+class AdvancedEventSelectorOutputTypeDef(
+    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
+):
+    pass
+
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -1020,26 +1114,14 @@
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "Name": str,
-        "Source": str,
-        "Destinations": List[DestinationTypeDef],
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "Channel": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1058,26 +1140,58 @@
 
 UpdateChannelResponseTypeDef = TypedDict(
     "UpdateChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
-        "Destinations": List[DestinationTypeDef],
+        "Destinations": List[DestinationOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "Name": str,
+        "Source": str,
+        "Destinations": List[DestinationOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "ResourceId": str,
+        "TagsList": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+EventSelectorOutputTypeDef = TypedDict(
+    "EventSelectorOutputTypeDef",
+    {
+        "ReadWriteType": ReadWriteTypeType,
+        "IncludeManagementEvents": bool,
+        "DataResources": List[DataResourceOutputTypeDef],
+        "ExcludeManagementEventSources": List[str],
+    },
+    total=False,
+)
+
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceTypeDef],
-        "ExcludeManagementEventSources": List[str],
+        "DataResources": Sequence[DataResourceTypeDef],
+        "ExcludeManagementEventSources": Sequence[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
@@ -1124,32 +1238,24 @@
     total=False,
 )
 
 GetInsightSelectorsResponseTypeDef = TypedDict(
     "GetInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorTypeDef],
+        "InsightSelectors": List[InsightSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutInsightSelectorsRequestRequestTypeDef = TypedDict(
-    "PutInsightSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-        "InsightSelectors": Sequence[InsightSelectorTypeDef],
-    },
-)
-
 PutInsightSelectorsResponseTypeDef = TypedDict(
     "PutInsightSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "InsightSelectors": List[InsightSelectorTypeDef],
+        "InsightSelectors": List[InsightSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetQueryResultsResponseTypeDef = TypedDict(
     "GetQueryResultsResponseTypeDef",
     {
@@ -1167,14 +1273,21 @@
     {
         "Failures": List[ImportFailureListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ImportSourceOutputTypeDef = TypedDict(
+    "ImportSourceOutputTypeDef",
+    {
+        "S3": S3ImportSourceOutputTypeDef,
+    },
+)
+
 ImportSourceTypeDef = TypedDict(
     "ImportSourceTypeDef",
     {
         "S3": S3ImportSourceTypeDef,
     },
 )
 
@@ -1183,14 +1296,22 @@
     {
         "Imports": List[ImportsListItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutInsightSelectorsRequestRequestTypeDef = TypedDict(
+    "PutInsightSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+        "InsightSelectors": Sequence[InsightSelectorTypeDef],
+    },
+)
+
 ListPublicKeysResponseTypeDef = TypedDict(
     "ListPublicKeysResponseTypeDef",
     {
         "PublicKeyList": List[PublicKeyTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1235,77 +1356,41 @@
         "EventCategory": Literal["insight"],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "ResourceTagList": List[ResourceTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
-        "TagsList": List[TagTypeDef],
+        "TagsList": List[TagOutputTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1313,15 +1398,15 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1331,15 +1416,15 @@
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1347,19 +1432,64 @@
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
     },
     total=False,
 )
 
+UpdateEventDataStoreResponseTypeDef = TypedDict(
+    "UpdateEventDataStoreResponseTypeDef",
+    {
+        "EventDataStoreArn": str,
+        "Name": str,
+        "Status": EventDataStoreStatusType,
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "KmsKeyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
     {
         "EventDataStore": str,
     },
 )
 _OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
@@ -1378,38 +1508,39 @@
 
 class UpdateEventDataStoreRequestRequestTypeDef(
     _RequiredUpdateEventDataStoreRequestRequestTypeDef,
     _OptionalUpdateEventDataStoreRequestRequestTypeDef,
 ):
     pass
 
-UpdateEventDataStoreResponseTypeDef = TypedDict(
-    "UpdateEventDataStoreResponseTypeDef",
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
     {
-        "EventDataStoreArn": str,
-        "Name": str,
-        "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "KmsKeyId": str,
+        "ResourceTagList": List[ResourceTagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PutEventSelectorsResponseTypeDef = TypedDict(
+    "PutEventSelectorsResponseTypeDef",
+    {
+        "TrailARN": str,
+        "EventSelectors": List[EventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
     "_RequiredPutEventSelectorsRequestRequestTypeDef",
     {
@@ -1426,92 +1557,82 @@
 )
 
 class PutEventSelectorsRequestRequestTypeDef(
     _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
 ):
     pass
 
-PutEventSelectorsResponseTypeDef = TypedDict(
-    "PutEventSelectorsResponseTypeDef",
-    {
-        "TrailARN": str,
-        "EventSelectors": List[EventSelectorTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetImportResponseTypeDef = TypedDict(
     "GetImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StartImportRequestRequestTypeDef = TypedDict(
-    "StartImportRequestRequestTypeDef",
-    {
-        "Destinations": Sequence[str],
-        "ImportSource": ImportSourceTypeDef,
-        "StartEventTime": Union[datetime, str],
-        "EndEventTime": Union[datetime, str],
-        "ImportId": str,
-    },
-    total=False,
-)
-
 StartImportResponseTypeDef = TypedDict(
     "StartImportResponseTypeDef",
     {
         "ImportId": str,
         "Destinations": List[str],
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StopImportResponseTypeDef = TypedDict(
     "StopImportResponseTypeDef",
     {
         "ImportId": str,
-        "ImportSource": ImportSourceTypeDef,
+        "ImportSource": ImportSourceOutputTypeDef,
         "Destinations": List[str],
         "ImportStatus": ImportStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "StartEventTime": datetime,
         "EndEventTime": datetime,
         "ImportStatistics": ImportStatisticsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StartImportRequestRequestTypeDef = TypedDict(
+    "StartImportRequestRequestTypeDef",
+    {
+        "Destinations": Sequence[str],
+        "ImportSource": ImportSourceTypeDef,
+        "StartEventTime": Union[datetime, str],
+        "EndEventTime": Union[datetime, str],
+        "ImportId": str,
+    },
+    total=False,
+)
+
 ListEventDataStoresResponseTypeDef = TypedDict(
     "ListEventDataStoresResponseTypeDef",
     {
         "EventDataStores": List[EventDataStoreTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1520,12 +1641,12 @@
 GetChannelResponseTypeDef = TypedDict(
     "GetChannelResponseTypeDef",
     {
         "ChannelArn": str,
         "Name": str,
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
-        "Destinations": List[DestinationTypeDef],
+        "Destinations": List[DestinationOutputTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/PKG-INFO` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudtrail
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudTrail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudtrail"></a>
 
 # mypy-boto3-cloudtrail
 
 [![PyPI - mypy-boto3-cloudtrail](https://img.shields.io/pypi/v/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudtrail.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudtrail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudtrail?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudtrail)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudtrail)](https://pepy.tech/project/mypy-boto3-cloudtrail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudTrail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
+[boto3.CloudTrail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
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
 [mypy-boto3-cloudtrail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudtrail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,20 +348,24 @@
 
 `mypy_boto3_cloudtrail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudtrail.type_defs import (
     TagTypeDef,
+    AdvancedFieldSelectorOutputTypeDef,
     AdvancedFieldSelectorTypeDef,
     CancelQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     ChannelTypeDef,
     DestinationTypeDef,
+    DestinationOutputTypeDef,
+    TagOutputTypeDef,
     CreateTrailResponseTypeDef,
+    DataResourceOutputTypeDef,
     DataResourceTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteEventDataStoreRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteTrailRequestRequestTypeDef,
     DeregisterOrganizationDelegatedAdminRequestRequestTypeDef,
     DescribeQueryRequestRequestTypeDef,
@@ -372,25 +376,27 @@
     GetChannelRequestRequestTypeDef,
     IngestionStatusTypeDef,
     GetEventDataStoreRequestRequestTypeDef,
     GetEventSelectorsRequestRequestTypeDef,
     GetImportRequestRequestTypeDef,
     ImportStatisticsTypeDef,
     GetInsightSelectorsRequestRequestTypeDef,
-    InsightSelectorTypeDef,
+    InsightSelectorOutputTypeDef,
     GetQueryResultsRequestRequestTypeDef,
     QueryStatisticsTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
     GetResourcePolicyResponseTypeDef,
     GetTrailRequestRequestTypeDef,
     GetTrailStatusRequestRequestTypeDef,
     GetTrailStatusResponseTypeDef,
     ImportFailureListItemTypeDef,
+    S3ImportSourceOutputTypeDef,
     S3ImportSourceTypeDef,
     ImportsListItemTypeDef,
+    InsightSelectorTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListEventDataStoresRequestRequestTypeDef,
     ListImportFailuresRequestListImportFailuresPaginateTypeDef,
     ListImportFailuresRequestRequestTypeDef,
     ListImportsRequestListImportsPaginateTypeDef,
     ListImportsRequestRequestTypeDef,
     ListPublicKeysRequestListPublicKeysPaginateTypeDef,
@@ -418,55 +424,58 @@
     StopImportRequestRequestTypeDef,
     StopLoggingRequestRequestTypeDef,
     UpdateTrailRequestRequestTypeDef,
     UpdateTrailResponseTypeDef,
     AddTagsRequestRequestTypeDef,
     CreateTrailRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
-    ResourceTagTypeDef,
+    AdvancedEventSelectorOutputTypeDef,
     AdvancedEventSelectorTypeDef,
     ListChannelsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
     UpdateChannelResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    ResourceTagTypeDef,
+    EventSelectorOutputTypeDef,
     EventSelectorTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     GetTrailResponseTypeDef,
     EventTypeDef,
     GetInsightSelectorsResponseTypeDef,
-    PutInsightSelectorsRequestRequestTypeDef,
     PutInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     ListImportFailuresResponseTypeDef,
+    ImportSourceOutputTypeDef,
     ImportSourceTypeDef,
     ListImportsResponseTypeDef,
+    PutInsightSelectorsRequestRequestTypeDef,
     ListPublicKeysResponseTypeDef,
     ListQueriesResponseTypeDef,
     ListTrailsResponseTypeDef,
     LookupEventsRequestLookupEventsPaginateTypeDef,
     LookupEventsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    CreateEventDataStoreRequestRequestTypeDef,
     CreateEventDataStoreResponseTypeDef,
     EventDataStoreTypeDef,
     GetEventDataStoreResponseTypeDef,
     RestoreEventDataStoreResponseTypeDef,
     SourceConfigTypeDef,
-    UpdateEventDataStoreRequestRequestTypeDef,
     UpdateEventDataStoreResponseTypeDef,
+    CreateEventDataStoreRequestRequestTypeDef,
+    UpdateEventDataStoreRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
-    PutEventSelectorsRequestRequestTypeDef,
     PutEventSelectorsResponseTypeDef,
+    PutEventSelectorsRequestRequestTypeDef,
     LookupEventsResponseTypeDef,
     GetImportResponseTypeDef,
-    StartImportRequestRequestTypeDef,
     StartImportResponseTypeDef,
     StopImportResponseTypeDef,
+    StartImportRequestRequestTypeDef,
     ListEventDataStoresResponseTypeDef,
     GetChannelResponseTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudtrail-1.28.0/mypy_boto3_cloudtrail.egg-info/SOURCES.txt` & `mypy-boto3-cloudtrail-1.28.12/mypy_boto3_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudtrail-1.28.0/setup.py` & `mypy-boto3-cloudtrail-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudtrail",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudTrail 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudTrail 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

