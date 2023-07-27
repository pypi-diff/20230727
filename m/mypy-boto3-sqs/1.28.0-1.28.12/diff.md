# Comparing `tmp/mypy-boto3-sqs-1.28.0.tar.gz` & `tmp/mypy-boto3-sqs-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.28.0.tar", last modified: Thu Jul  6 21:00:42 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.28.0.tar` & `mypy-boto3-sqs-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.010440 mypy-boto3-sqs-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:15.000000 mypy-boto3-sqs-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-07-06 21:00:42.010440 mypy-boto3-sqs-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-07-06 20:56:15.000000 mypy-boto3-sqs-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:41.998440 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-06 20:56:15.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-07-06 20:56:16.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24536 2023-07-06 20:56:17.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-06 20:56:17.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:15.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.010440 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17725 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:41.000000 mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:42.010440 mypy-boto3-sqs-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:56:15.000000 mypy-boto3-sqs-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.593320 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-27 11:47:14.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-27 11:47:14.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25207 2023-07-27 11:47:15.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25168 2023-07-27 11:47:15.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17752 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:41.000000 mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.601320 mypy-boto3-sqs-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:12.000000 mypy-boto3-sqs-1.28.12/setup.py
```

### Comparing `mypy-boto3-sqs-1.28.0/LICENSE` & `mypy-boto3-sqs-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/PKG-INFO` & `mypy-boto3-sqs-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.0
-Summary: Type annotations for boto3.SQS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,65 +416,66 @@
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
-    CancelMessageMoveTaskResultTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
-    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
```

### Comparing `mypy-boto3-sqs-1.28.0/README.md` & `mypy-boto3-sqs-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -384,65 +384,66 @@
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
-    CancelMessageMoveTaskResultTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
-    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SQS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
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

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,14 +220,15 @@
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
@@ -306,26 +307,28 @@
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

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,15 @@
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
@@ -304,26 +305,28 @@
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

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
@@ -155,15 +156,15 @@
     """
 
     message_id: str
     md5_of_body: str
     body: str
     attributes: Dict[MessageSystemAttributeNameType, str]
     md5_of_message_attributes: str
-    message_attributes: Dict[str, MessageAttributeValueTypeDef]
+    message_attributes: Dict[str, MessageAttributeValueOutputTypeDef]
     queue_url: str
     receipt_handle: str
 
     def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     QueueAttributeNameType,
 )
 from .type_defs import (
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
 )
 
@@ -141,15 +142,15 @@
     """
 
     message_id: str
     md5_of_body: str
     body: str
     attributes: Dict[MessageSystemAttributeNameType, str]
     md5_of_message_attributes: str
-    message_attributes: Dict[str, MessageAttributeValueTypeDef]
+    message_attributes: Dict[str, MessageAttributeValueOutputTypeDef]
     queue_url: str
     receipt_handle: str
 
     def Queue(self) -> "_Queue":
         """
         Creates a Queue resource.
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,65 +33,66 @@
 
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
-    "CancelMessageMoveTaskResultTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
-    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
-    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResultTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
-    "StartMessageMoveTaskResultTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
+    "CancelMessageMoveTaskResultTypeDef",
+    "CreateQueueResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetQueueAttributesResultTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesResultTypeDef",
+    "SendMessageResultTypeDef",
+    "StartMessageMoveTaskResultTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
@@ -144,19 +145,22 @@
 CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
     "CancelMessageMoveTaskRequestRequestTypeDef",
     {
         "TaskHandle": str,
     },
 )
 
-CancelMessageMoveTaskResultTypeDef = TypedDict(
-    "CancelMessageMoveTaskResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApproximateNumberOfMessagesMoved": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -243,22 +247,14 @@
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
 
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -281,21 +277,14 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -310,22 +299,14 @@
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -361,44 +342,24 @@
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
 
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -414,23 +375,14 @@
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
 
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListMessageMoveTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListMessageMoveTasksRequestRequestTypeDef",
     {
         "SourceArn": str,
     },
 )
 _OptionalListMessageMoveTasksRequestRequestTypeDef = TypedDict(
@@ -468,63 +420,61 @@
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
+_RequiredMessageAttributeValueOutputTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueOutputTypeDef",
     {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataType": str,
+    },
+)
+_OptionalMessageAttributeValueOutputTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueOutputTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": bytes,
+        "StringListValues": List[str],
+        "BinaryListValues": List[bytes],
     },
+    total=False,
 )
 
+
+class MessageAttributeValueOutputTypeDef(
+    _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
+):
+    pass
+
+
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
     "_OptionalMessageAttributeValueTypeDef",
     {
         "StringValue": str,
-        "BinaryValue": bytes,
-        "StringListValues": List[str],
-        "BinaryListValues": List[bytes],
+        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
     total=False,
 )
 
 
 class MessageAttributeValueTypeDef(
     _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
@@ -552,24 +502,14 @@
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -623,25 +563,14 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -659,26 +588,14 @@
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
 
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -709,22 +626,14 @@
 class StartMessageMoveTaskRequestRequestTypeDef(
     _RequiredStartMessageMoveTaskRequestRequestTypeDef,
     _OptionalStartMessageMoveTaskRequestRequestTypeDef,
 ):
     pass
 
 
-StartMessageMoveTaskResultTypeDef = TypedDict(
-    "StartMessageMoveTaskResultTypeDef",
-    {
-        "TaskHandle": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagQueueRequestRequestTypeDef = TypedDict(
     "TagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -733,14 +642,99 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CancelMessageMoveTaskResultTypeDef = TypedDict(
+    "CancelMessageMoveTaskResultTypeDef",
+    {
+        "ApproximateNumberOfMessagesMoved": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMessageMoveTaskResultTypeDef = TypedDict(
+    "StartMessageMoveTaskResultTypeDef",
+    {
+        "TaskHandle": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     {
         "Entries": Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],
     },
 )
 
@@ -753,15 +747,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -777,36 +771,67 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListMessageMoveTasksResultTypeDef = TypedDict(
     "ListMessageMoveTasksResultTypeDef",
     {
         "Results": List[ListMessageMoveTasksResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
@@ -892,23 +917,23 @@
 
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -32,65 +32,66 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CancelMessageMoveTaskRequestRequestTypeDef",
-    "CancelMessageMoveTaskResultTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
-    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
-    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
     "ListMessageMoveTasksRequestRequestTypeDef",
     "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
-    "ListQueuesResultTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
-    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
-    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
     "StartMessageMoveTaskRequestRequestTypeDef",
-    "StartMessageMoveTaskResultTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
+    "CancelMessageMoveTaskResultTypeDef",
+    "CreateQueueResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetQueueAttributesResultTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesResultTypeDef",
+    "SendMessageResultTypeDef",
+    "StartMessageMoveTaskResultTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
@@ -141,19 +142,22 @@
 CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
     "CancelMessageMoveTaskRequestRequestTypeDef",
     {
         "TaskHandle": str,
     },
 )
 
-CancelMessageMoveTaskResultTypeDef = TypedDict(
-    "CancelMessageMoveTaskResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApproximateNumberOfMessagesMoved": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -234,22 +238,14 @@
 
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -272,21 +268,14 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -299,22 +288,14 @@
 
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -346,42 +327,24 @@
 
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -395,23 +358,14 @@
 
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListMessageMoveTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListMessageMoveTasksRequestRequestTypeDef",
     {
         "SourceArn": str,
     },
 )
 _OptionalListMessageMoveTasksRequestRequestTypeDef = TypedDict(
@@ -447,63 +401,59 @@
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
+_RequiredMessageAttributeValueOutputTypeDef = TypedDict(
+    "_RequiredMessageAttributeValueOutputTypeDef",
     {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataType": str,
     },
 )
+_OptionalMessageAttributeValueOutputTypeDef = TypedDict(
+    "_OptionalMessageAttributeValueOutputTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": bytes,
+        "StringListValues": List[str],
+        "BinaryListValues": List[bytes],
+    },
+    total=False,
+)
+
+class MessageAttributeValueOutputTypeDef(
+    _RequiredMessageAttributeValueOutputTypeDef, _OptionalMessageAttributeValueOutputTypeDef
+):
+    pass
 
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
     "_OptionalMessageAttributeValueTypeDef",
     {
         "StringValue": str,
-        "BinaryValue": bytes,
-        "StringListValues": List[str],
-        "BinaryListValues": List[bytes],
+        "BinaryValue": Union[str, bytes, IO[Any], StreamingBody],
+        "StringListValues": Sequence[str],
+        "BinaryListValues": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
     },
     total=False,
 )
 
 class MessageAttributeValueTypeDef(
     _RequiredMessageAttributeValueTypeDef, _OptionalMessageAttributeValueTypeDef
 ):
@@ -527,24 +477,14 @@
 )
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -596,25 +536,14 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -630,26 +559,14 @@
 )
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -678,22 +595,14 @@
 
 class StartMessageMoveTaskRequestRequestTypeDef(
     _RequiredStartMessageMoveTaskRequestRequestTypeDef,
     _OptionalStartMessageMoveTaskRequestRequestTypeDef,
 ):
     pass
 
-StartMessageMoveTaskResultTypeDef = TypedDict(
-    "StartMessageMoveTaskResultTypeDef",
-    {
-        "TaskHandle": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagQueueRequestRequestTypeDef = TypedDict(
     "TagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -702,14 +611,99 @@
     "UntagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CancelMessageMoveTaskResultTypeDef = TypedDict(
+    "CancelMessageMoveTaskResultTypeDef",
+    {
+        "ApproximateNumberOfMessagesMoved": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMessageMoveTaskResultTypeDef = TypedDict(
+    "StartMessageMoveTaskResultTypeDef",
+    {
+        "TaskHandle": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     {
         "Entries": Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],
     },
 )
 
@@ -722,15 +716,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -746,36 +740,65 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListMessageMoveTasksResultTypeDef = TypedDict(
     "ListMessageMoveTasksResultTypeDef",
     {
         "Results": List[ListMessageMoveTasksResultEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
         "Body": str,
         "Attributes": Dict[MessageSystemAttributeNameType, str],
         "MD5OfMessageAttributes": str,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
     },
     total=False,
 )
 
 _RequiredSendMessageBatchRequestEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchRequestEntryTypeDef",
     {
@@ -855,23 +878,23 @@
     pass
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.28.0
-Summary: Type annotations for boto3.SQS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sqs"></a>
 
 # mypy-boto3-sqs
 
 [![PyPI - mypy-boto3-sqs](https://img.shields.io/pypi/v/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sqs)](https://pepy.tech/project/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
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
 [mypy-boto3-sqs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -416,65 +416,66 @@
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
     CancelMessageMoveTaskRequestRequestTypeDef,
-    CancelMessageMoveTaskResultTypeDef,
+    ResponseMetadataTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
-    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
-    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
     ListMessageMoveTasksRequestRequestTypeDef,
     ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
-    ListQueuesResultTypeDef,
+    MessageAttributeValueOutputTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
-    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
-    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
     StartMessageMoveTaskRequestRequestTypeDef,
-    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
+    CreateQueueResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetQueueAttributesResultTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesResultTypeDef,
+    SendMessageResultTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
```

### Comparing `mypy-boto3-sqs-1.28.0/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.28.12/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.28.0/setup.py` & `mypy-boto3-sqs-1.28.12/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SQS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

