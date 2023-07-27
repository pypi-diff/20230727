# Comparing `tmp/mypy-boto3-omics-1.28.0.tar.gz` & `tmp/mypy-boto3-omics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.28.0.tar", last modified: Thu Jul  6 21:00:14 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
```

## Comparing `mypy-boto3-omics-1.28.0.tar` & `mypy-boto3-omics-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.434384 mypy-boto3-omics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28974 2023-07-06 21:00:14.430384 mypy-boto3-omics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27497 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.418384 mypy-boto3-omics-1.28.0/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61309 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15770 2023-07-06 20:48:31.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-07-06 20:48:31.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22007 2023-07-06 20:48:31.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97546 2023-07-06 20:48:34.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97390 2023-07-06 20:48:32.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:30.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-06 20:48:31.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-06 20:48:31.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:14.430384 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28974 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:14.000000 mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:14.434384 mypy-boto3-omics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:48:29.000000 mypy-boto3-omics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29272 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61309 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100219 2023-07-27 05:44:02.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100059 2023-07-27 05:44:01.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29272 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:43:58.000000 mypy-boto3-omics-1.28.12/setup.py
```

### Comparing `mypy-boto3-omics-1.28.0/LICENSE` & `mypy-boto3-omics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/PKG-INFO` & `mypy-boto3-omics-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.0
-Summary: Type annotations for boto3.Omics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-omics"></a>
 
 # mypy-boto3-omics
 
 [![PyPI - mypy-boto3-omics](https://img.shields.io/pypi/v/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,155 +514,154 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
+    ReferenceItemOutputTypeDef,
+    SseConfigOutputTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
+    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
+    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesTypeDef,
+    SourceFilesOutputTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
     ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
     ReadSetFilterTypeDef,
     ReferenceStoreFilterTypeDef,
     ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
+    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
     AnnotationStoreItemTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
+    ReferenceStoreDetailTypeDef,
+    SequenceStoreDetailTypeDef,
+    VariantStoreItemTypeDef,
+    BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
+    CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
     GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
     GetSequenceStoreResponseTypeDef,
     GetVariantStoreResponseTypeDef,
-    ReferenceStoreDetailTypeDef,
-    SequenceStoreDetailTypeDef,
-    VariantStoreItemTypeDef,
-    BatchDeleteReadSetResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
@@ -678,24 +677,31 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
     ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
     ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
     ListReadSetsRequestListReadSetsPaginateTypeDef,
@@ -712,33 +718,37 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
+    StartReadSetImportJobRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-omics-1.28.0/README.md` & `mypy-boto3-omics-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-omics"></a>
 
 # mypy-boto3-omics
 
 [![PyPI - mypy-boto3-omics](https://img.shields.io/pypi/v/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -482,155 +482,154 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
+    ReferenceItemOutputTypeDef,
+    SseConfigOutputTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
+    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
+    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesTypeDef,
+    SourceFilesOutputTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
     ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
     ReadSetFilterTypeDef,
     ReferenceStoreFilterTypeDef,
     ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
+    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
     AnnotationStoreItemTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
+    ReferenceStoreDetailTypeDef,
+    SequenceStoreDetailTypeDef,
+    VariantStoreItemTypeDef,
+    BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
+    CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
     GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
     GetSequenceStoreResponseTypeDef,
     GetVariantStoreResponseTypeDef,
-    ReferenceStoreDetailTypeDef,
-    SequenceStoreDetailTypeDef,
-    VariantStoreItemTypeDef,
-    BatchDeleteReadSetResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
@@ -646,24 +645,31 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
     ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
     ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
     ListReadSetsRequestListReadSetsPaginateTypeDef,
@@ -680,33 +686,37 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
+    StartReadSetImportJobRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Omics 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,14 +319,15 @@
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
@@ -405,26 +406,28 @@
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

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -317,14 +317,15 @@
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
@@ -403,26 +404,28 @@
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

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listannotationimportjobspaginator)
         """
 
 
@@ -151,30 +151,30 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listannotationstorespaginator)
         """
 
 
 class ListMultipartReadSetUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
-        self, *, sequenceStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
 
@@ -185,15 +185,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
 
@@ -204,15 +204,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetexportjobspaginator)
         """
 
 
@@ -223,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetimportjobspaginator)
         """
 
 
@@ -244,15 +244,15 @@
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
 
@@ -263,15 +263,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetspaginator)
         """
 
 
@@ -282,15 +282,15 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferenceimportjobspaginator)
         """
 
 
@@ -300,15 +300,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencestorespaginator)
         """
 
 
@@ -319,30 +319,30 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencespaginator)
         """
 
 
 class ListRunGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrungroupspaginator)
         """
 
 
@@ -353,15 +353,15 @@
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listruntaskspaginator)
         """
 
 
@@ -373,15 +373,15 @@
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrunspaginator)
         """
 
 
@@ -391,15 +391,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listsequencestorespaginator)
         """
 
 
@@ -410,15 +410,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listvariantimportjobspaginator)
         """
 
 
@@ -429,15 +429,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listvariantstorespaginator)
         """
 
 
@@ -448,13 +448,13 @@
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnnotationImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listannotationimportjobspaginator)
         """
 
 class ListAnnotationStoresPaginator(Paginator):
@@ -147,29 +147,29 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListAnnotationStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAnnotationStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListAnnotationStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listannotationstorespaginator)
         """
 
 class ListMultipartReadSetUploadsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listmultipartreadsetuploadspaginator)
     """
 
     def paginate(
-        self, *, sequenceStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, sequenceStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMultipartReadSetUploadsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListMultipartReadSetUploads.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listmultipartreadsetuploadspaginator)
         """
 
 class ListReadSetActivationJobsPaginator(Paginator):
@@ -179,15 +179,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ActivateReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetActivationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetActivationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetactivationjobspaginator)
         """
 
 class ListReadSetExportJobsPaginator(Paginator):
@@ -197,15 +197,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ExportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetExportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetexportjobspaginator)
         """
 
 class ListReadSetImportJobsPaginator(Paginator):
@@ -215,15 +215,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ImportReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetimportjobspaginator)
         """
 
 class ListReadSetUploadPartsPaginator(Paginator):
@@ -235,15 +235,15 @@
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         uploadId: str,
         partSource: ReadSetPartSourceType,
         filter: ReadSetUploadPartListFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetUploadPartsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSetUploadParts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetuploadpartspaginator)
         """
 
 class ListReadSetsPaginator(Paginator):
@@ -253,15 +253,15 @@
     """
 
     def paginate(
         self,
         *,
         sequenceStoreId: str,
         filter: ReadSetFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReadSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReadSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreadsetspaginator)
         """
 
 class ListReferenceImportJobsPaginator(Paginator):
@@ -271,15 +271,15 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ImportReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferenceImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferenceimportjobspaginator)
         """
 
 class ListReferenceStoresPaginator(Paginator):
@@ -288,15 +288,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: ReferenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferenceStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencestorespaginator)
         """
 
 class ListReferencesPaginator(Paginator):
@@ -306,29 +306,29 @@
     """
 
     def paginate(
         self,
         *,
         referenceStoreId: str,
         filter: ReferenceFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListReferences.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listreferencespaginator)
         """
 
 class ListRunGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrungroupspaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrungroupspaginator)
         """
 
 class ListRunTasksPaginator(Paginator):
@@ -338,15 +338,15 @@
     """
 
     def paginate(
         self,
         *,
         id: str,
         status: TaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRunTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listruntaskspaginator)
         """
 
 class ListRunsPaginator(Paginator):
@@ -357,15 +357,15 @@
 
     def paginate(
         self,
         *,
         name: str = ...,
         runGroupId: str = ...,
         status: RunStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRunsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListRuns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listrunspaginator)
         """
 
 class ListSequenceStoresPaginator(Paginator):
@@ -374,15 +374,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listsequencestorespaginator)
     """
 
     def paginate(
         self,
         *,
         filter: SequenceStoreFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSequenceStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListSequenceStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listsequencestorespaginator)
         """
 
 class ListVariantImportJobsPaginator(Paginator):
@@ -392,15 +392,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantImportJobsFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVariantImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listvariantimportjobspaginator)
         """
 
 class ListVariantStoresPaginator(Paginator):
@@ -410,15 +410,15 @@
     """
 
     def paginate(
         self,
         *,
         ids: Sequence[str] = ...,
         filter: ListVariantStoresFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVariantStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListVariantStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listvariantstorespaginator)
         """
 
 class ListWorkflowsPaginator(Paginator):
@@ -428,13 +428,13 @@
     """
 
     def paginate(
         self,
         *,
         type: WorkflowTypeType = ...,
         name: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkflowsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Paginator.ListWorkflows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/paginators/#listworkflowspaginator)
         """
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,155 +60,154 @@
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     "ActivateReadSetFilterTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
-    "ReferenceItemTypeDef",
-    "SseConfigTypeDef",
+    "ReferenceItemOutputTypeDef",
+    "SseConfigOutputTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "ReferenceItemTypeDef",
+    "SseConfigTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
-    "CreateRunGroupResponseTypeDef",
     "WorkflowParameterTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
-    "DeleteAnnotationStoreResponseTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
-    "DeleteVariantStoreResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
+    "VcfOptionsOutputTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
     "GetReadSetMetadataRequestRequestTypeDef",
     "SequenceInformationTypeDef",
     "GetReadSetRequestRequestTypeDef",
-    "GetReadSetResponseTypeDef",
     "GetReferenceImportJobRequestRequestTypeDef",
     "ImportReferenceSourceItemTypeDef",
     "GetReferenceMetadataRequestRequestTypeDef",
     "GetReferenceRequestRequestTypeDef",
-    "GetReferenceResponseTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
-    "GetRunGroupResponseTypeDef",
     "GetRunRequestRequestTypeDef",
-    "GetRunResponseTypeDef",
     "GetRunTaskRequestRequestTypeDef",
-    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
+    "WorkflowParameterOutputTypeDef",
     "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
-    "SourceFilesTypeDef",
+    "SourceFilesOutputTypeDef",
     "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
-    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
     "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
     "ReadSetFilterTypeDef",
     "ReferenceStoreFilterTypeDef",
     "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
-    "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
     "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ReadOptionsOutputTypeDef",
     "ReadOptionsTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartAnnotationImportResponseTypeDef",
+    "SourceFilesTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
-    "StartReadSetActivationJobResponseTypeDef",
-    "StartReadSetExportJobResponseTypeDef",
-    "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
-    "StartReferenceImportJobResponseTypeDef",
     "StartRunRequestRequestTypeDef",
-    "StartRunResponseTypeDef",
     "VariantImportItemSourceTypeDef",
-    "StartVariantImportResponseTypeDef",
+    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
-    "UploadReadSetPartResponseTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
-    "ListReadSetActivationJobsResponseTypeDef",
-    "GetReadSetActivationJobResponseTypeDef",
-    "ListAnnotationImportJobsResponseTypeDef",
-    "CreateVariantStoreResponseTypeDef",
-    "UpdateVariantStoreResponseTypeDef",
     "AnnotationStoreItemTypeDef",
-    "CreateReferenceStoreRequestRequestTypeDef",
+    "ReferenceStoreDetailTypeDef",
+    "SequenceStoreDetailTypeDef",
+    "VariantStoreItemTypeDef",
+    "BatchDeleteReadSetResponseTypeDef",
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateReferenceStoreResponseTypeDef",
-    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateRunGroupResponseTypeDef",
     "CreateSequenceStoreResponseTypeDef",
-    "CreateVariantStoreRequestRequestTypeDef",
+    "CreateVariantStoreResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DeleteAnnotationStoreResponseTypeDef",
+    "DeleteVariantStoreResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetReadSetActivationJobResponseTypeDef",
+    "GetReadSetResponseTypeDef",
+    "GetReferenceResponseTypeDef",
     "GetReferenceStoreResponseTypeDef",
+    "GetRunGroupResponseTypeDef",
+    "GetRunResponseTypeDef",
+    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreResponseTypeDef",
     "GetVariantStoreResponseTypeDef",
-    "ReferenceStoreDetailTypeDef",
-    "SequenceStoreDetailTypeDef",
-    "VariantStoreItemTypeDef",
-    "BatchDeleteReadSetResponseTypeDef",
+    "ListAnnotationImportJobsResponseTypeDef",
+    "ListReadSetActivationJobsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartAnnotationImportResponseTypeDef",
+    "StartReadSetActivationJobResponseTypeDef",
+    "StartReadSetExportJobResponseTypeDef",
+    "StartReadSetImportJobResponseTypeDef",
+    "StartReferenceImportJobResponseTypeDef",
+    "StartRunResponseTypeDef",
+    "StartVariantImportResponseTypeDef",
+    "UpdateVariantStoreResponseTypeDef",
+    "UploadReadSetPartResponseTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
+    "CreateReferenceStoreRequestRequestTypeDef",
+    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateVariantStoreRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
-    "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
@@ -224,24 +223,31 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "GetWorkflowResponseTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
-    "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
+    "ListRunTasksRequestListRunTasksPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
     "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
     "ListReadSetsRequestListReadSetsPaginateTypeDef",
@@ -258,33 +264,37 @@
     "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TsvOptionsOutputTypeDef",
     "TsvOptionsTypeDef",
+    "StartReadSetImportJobSourceItemTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
+    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
-    "StartReadSetImportJobRequestRequestTypeDef",
+    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
+    "StartReadSetImportJobRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -388,38 +398,38 @@
 
 class AnnotationImportJobItemTypeDef(
     _RequiredAnnotationImportJobItemTypeDef, _OptionalAnnotationImportJobItemTypeDef
 ):
     pass
 
 
-ReferenceItemTypeDef = TypedDict(
-    "ReferenceItemTypeDef",
+ReferenceItemOutputTypeDef = TypedDict(
+    "ReferenceItemOutputTypeDef",
     {
         "referenceArn": str,
     },
     total=False,
 )
 
-_RequiredSseConfigTypeDef = TypedDict(
-    "_RequiredSseConfigTypeDef",
+_RequiredSseConfigOutputTypeDef = TypedDict(
+    "_RequiredSseConfigOutputTypeDef",
     {
         "type": Literal["KMS"],
     },
 )
-_OptionalSseConfigTypeDef = TypedDict(
-    "_OptionalSseConfigTypeDef",
+_OptionalSseConfigOutputTypeDef = TypedDict(
+    "_OptionalSseConfigOutputTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
 
-class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
+class SseConfigOutputTypeDef(_RequiredSseConfigOutputTypeDef, _OptionalSseConfigOutputTypeDef):
     pass
 
 
 BatchDeleteReadSetRequestRequestTypeDef = TypedDict(
     "BatchDeleteReadSetRequestRequestTypeDef",
     {
         "ids": Sequence[str],
@@ -432,14 +442,25 @@
     {
         "id": str,
         "code": str,
         "message": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -462,22 +483,41 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CompleteMultipartReadSetUploadResponseTypeDef",
+ReferenceItemTypeDef = TypedDict(
+    "ReferenceItemTypeDef",
     {
-        "readSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "referenceArn": str,
+    },
+    total=False,
+)
+
+_RequiredSseConfigTypeDef = TypedDict(
+    "_RequiredSseConfigTypeDef",
+    {
+        "type": Literal["KMS"],
+    },
+)
+_OptionalSseConfigTypeDef = TypedDict(
+    "_OptionalSseConfigTypeDef",
+    {
+        "keyArn": str,
     },
+    total=False,
 )
 
+
+class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
+    pass
+
+
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -500,32 +540,14 @@
 class CreateMultipartReadSetUploadRequestRequestTypeDef(
     _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef,
     _OptionalCreateMultipartReadSetUploadRequestRequestTypeDef,
 ):
     pass
 
 
-CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CreateMultipartReadSetUploadResponseTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "generatedFrom": str,
-        "referenceArn": str,
-        "name": str,
-        "description": str,
-        "tags": Dict[str, str],
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRunGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRunGroupRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateRunGroupRequestRequestTypeDef = TypedDict(
@@ -544,44 +566,23 @@
 
 class CreateRunGroupRequestRequestTypeDef(
     _RequiredCreateRunGroupRequestRequestTypeDef, _OptionalCreateRunGroupRequestRequestTypeDef
 ):
     pass
 
 
-CreateRunGroupResponseTypeDef = TypedDict(
-    "CreateRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowParameterTypeDef = TypedDict(
     "WorkflowParameterTypeDef",
     {
         "description": str,
         "optional": bool,
     },
     total=False,
 )
 
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnnotationStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
@@ -596,22 +597,14 @@
 class DeleteAnnotationStoreRequestRequestTypeDef(
     _RequiredDeleteAnnotationStoreRequestRequestTypeDef,
     _OptionalDeleteAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteAnnotationStoreResponseTypeDef = TypedDict(
-    "DeleteAnnotationStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReferenceRequestRequestTypeDef = TypedDict(
     "DeleteReferenceRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -662,36 +655,21 @@
 class DeleteVariantStoreRequestRequestTypeDef(
     _RequiredDeleteVariantStoreRequestRequestTypeDef,
     _OptionalDeleteVariantStoreRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteVariantStoreResponseTypeDef = TypedDict(
-    "DeleteVariantStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportReadSetDetailTypeDef = TypedDict(
     "_RequiredExportReadSetDetailTypeDef",
     {
         "id": str,
         "status": ReadSetExportJobItemStatusType,
     },
 )
@@ -758,14 +736,23 @@
         "totalParts": int,
         "partSize": int,
         "contentLength": int,
     },
     total=False,
 )
 
+VcfOptionsOutputTypeDef = TypedDict(
+    "VcfOptionsOutputTypeDef",
+    {
+        "ignoreQualField": bool,
+        "ignoreFilterField": bool,
+    },
+    total=False,
+)
+
 VcfOptionsTypeDef = TypedDict(
     "VcfOptionsTypeDef",
     {
         "ignoreQualField": bool,
         "ignoreFilterField": bool,
     },
     total=False,
@@ -856,22 +843,14 @@
 
 class GetReadSetRequestRequestTypeDef(
     _RequiredGetReadSetRequestRequestTypeDef, _OptionalGetReadSetRequestRequestTypeDef
 ):
     pass
 
 
-GetReadSetResponseTypeDef = TypedDict(
-    "GetReadSetResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceImportJobRequestRequestTypeDef = TypedDict(
     "GetReferenceImportJobRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -929,52 +908,28 @@
 
 class GetReferenceRequestRequestTypeDef(
     _RequiredGetReferenceRequestRequestTypeDef, _OptionalGetReferenceRequestRequestTypeDef
 ):
     pass
 
 
-GetReferenceResponseTypeDef = TypedDict(
-    "GetReferenceResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceStoreRequestRequestTypeDef = TypedDict(
     "GetReferenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
 GetRunGroupRequestRequestTypeDef = TypedDict(
     "GetRunGroupRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetRunGroupResponseTypeDef = TypedDict(
-    "GetRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "maxCpus": int,
-        "maxRuns": int,
-        "maxDuration": int,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "maxGpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetRunRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetRunRequestRequestTypeDef = TypedDict(
@@ -988,71 +943,22 @@
 
 class GetRunRequestRequestTypeDef(
     _RequiredGetRunRequestRequestTypeDef, _OptionalGetRunRequestRequestTypeDef
 ):
     pass
 
 
-GetRunResponseTypeDef = TypedDict(
-    "GetRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "workflowId": str,
-        "workflowType": WorkflowTypeType,
-        "runId": str,
-        "roleArn": str,
-        "name": str,
-        "runGroupId": str,
-        "priority": int,
-        "definition": str,
-        "digest": str,
-        "parameters": Dict[str, Any],
-        "storageCapacity": int,
-        "outputUri": str,
-        "logLevel": RunLogLevelType,
-        "resourceDigests": Dict[str, str],
-        "startedBy": str,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRunTaskRequestRequestTypeDef = TypedDict(
     "GetRunTaskRequestRequestTypeDef",
     {
         "id": str,
         "taskId": str,
     },
 )
 
-GetRunTaskResponseTypeDef = TypedDict(
-    "GetRunTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "status": TaskStatusType,
-        "name": str,
-        "cpus": int,
-        "memory": int,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "logStream": str,
-        "gpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1110,14 +1016,23 @@
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
 
+WorkflowParameterOutputTypeDef = TypedDict(
+    "WorkflowParameterOutputTypeDef",
+    {
+        "description": str,
+        "optional": bool,
+    },
+    total=False,
+)
+
 ImportReadSetFilterTypeDef = TypedDict(
     "ImportReadSetFilterTypeDef",
     {
         "status": ReadSetImportJobStatusType,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
     },
@@ -1145,30 +1060,32 @@
 
 class ImportReadSetJobItemTypeDef(
     _RequiredImportReadSetJobItemTypeDef, _OptionalImportReadSetJobItemTypeDef
 ):
     pass
 
 
-_RequiredSourceFilesTypeDef = TypedDict(
-    "_RequiredSourceFilesTypeDef",
+_RequiredSourceFilesOutputTypeDef = TypedDict(
+    "_RequiredSourceFilesOutputTypeDef",
     {
         "source1": str,
     },
 )
-_OptionalSourceFilesTypeDef = TypedDict(
-    "_OptionalSourceFilesTypeDef",
+_OptionalSourceFilesOutputTypeDef = TypedDict(
+    "_OptionalSourceFilesOutputTypeDef",
     {
         "source2": str,
     },
     total=False,
 )
 
 
-class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
+class SourceFilesOutputTypeDef(
+    _RequiredSourceFilesOutputTypeDef, _OptionalSourceFilesOutputTypeDef
+):
     pass
 
 
 ImportReferenceFilterTypeDef = TypedDict(
     "ImportReferenceFilterTypeDef",
     {
         "status": ReferenceImportJobStatusType,
@@ -1208,44 +1125,32 @@
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
 )
 
-ListAnnotationStoresFilterTypeDef = TypedDict(
-    "ListAnnotationStoresFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StoreStatusType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+ListAnnotationStoresFilterTypeDef = TypedDict(
+    "ListAnnotationStoresFilterTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": StoreStatusType,
     },
     total=False,
 )
 
-
-class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
-    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartReadSetUploadsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
@@ -1389,23 +1294,14 @@
 
 class ReferenceListItemTypeDef(
     _RequiredReferenceListItemTypeDef, _OptionalReferenceListItemTypeDef
 ):
     pass
 
 
-ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunGroupsRequestRequestTypeDef = TypedDict(
     "ListRunGroupsRequestRequestTypeDef",
     {
         "name": str,
         "startingToken": str,
         "maxResults": int,
     },
@@ -1423,37 +1319,14 @@
         "maxDuration": int,
         "creationTime": datetime,
         "maxGpus": int,
     },
     total=False,
 )
 
-_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRunTasksRequestListRunTasksPaginateTypeDef(
-    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
-    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRunTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListRunTasksRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalListRunTasksRequestRequestTypeDef = TypedDict(
@@ -1485,25 +1358,14 @@
         "startTime": datetime,
         "stopTime": datetime,
         "gpus": int,
     },
     total=False,
 )
 
-ListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "ListRunsRequestListRunsPaginateTypeDef",
-    {
-        "name": str,
-        "runGroupId": str,
-        "status": RunStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunsRequestRequestTypeDef = TypedDict(
     "ListRunsRequestRequestTypeDef",
     {
         "name": str,
         "runGroupId": str,
         "startingToken": str,
         "maxResults": int,
@@ -1542,22 +1404,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVariantImportJobsFilterTypeDef = TypedDict(
     "ListVariantImportJobsFilterTypeDef",
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
@@ -1595,24 +1449,14 @@
     "ListVariantStoresFilterTypeDef",
     {
         "status": StoreStatusType,
     },
     total=False,
 )
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "type": WorkflowTypeType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "type": WorkflowTypeType,
         "name": str,
         "startingToken": str,
         "maxResults": int,
@@ -1631,20 +1475,26 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ReadOptionsOutputTypeDef = TypedDict(
+    "ReadOptionsOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "sep": str,
+        "encoding": str,
+        "quote": str,
+        "quoteAll": bool,
+        "escape": str,
+        "escapeQuotes": bool,
+        "comment": str,
+        "header": bool,
+        "lineSep": str,
     },
     total=False,
 )
 
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
@@ -1657,72 +1507,37 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredSourceFilesTypeDef = TypedDict(
+    "_RequiredSourceFilesTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "source1": str,
     },
 )
-
-StartAnnotationImportResponseTypeDef = TypedDict(
-    "StartAnnotationImportResponseTypeDef",
+_OptionalSourceFilesTypeDef = TypedDict(
+    "_OptionalSourceFilesTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "source2": str,
     },
+    total=False,
 )
 
-StartReadSetActivationJobSourceItemTypeDef = TypedDict(
-    "StartReadSetActivationJobSourceItemTypeDef",
-    {
-        "readSetId": str,
-    },
-)
 
-StartReadSetActivationJobResponseTypeDef = TypedDict(
-    "StartReadSetActivationJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
+    pass
 
-StartReadSetExportJobResponseTypeDef = TypedDict(
-    "StartReadSetExportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "destination": str,
-        "status": ReadSetExportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-StartReadSetImportJobResponseTypeDef = TypedDict(
-    "StartReadSetImportJobResponseTypeDef",
+StartReadSetActivationJobSourceItemTypeDef = TypedDict(
+    "StartReadSetActivationJobSourceItemTypeDef",
     {
-        "id": str,
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "status": ReadSetImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "readSetId": str,
     },
 )
 
 _RequiredStartReferenceImportJobSourceItemTypeDef = TypedDict(
     "_RequiredStartReferenceImportJobSourceItemTypeDef",
     {
         "sourceFile": str,
@@ -1742,26 +1557,14 @@
 class StartReferenceImportJobSourceItemTypeDef(
     _RequiredStartReferenceImportJobSourceItemTypeDef,
     _OptionalStartReferenceImportJobSourceItemTypeDef,
 ):
     pass
 
 
-StartReferenceImportJobResponseTypeDef = TypedDict(
-    "StartReferenceImportJobResponseTypeDef",
-    {
-        "id": str,
-        "referenceStoreId": str,
-        "roleArn": str,
-        "status": ReferenceImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartRunRequestRequestTypeDef",
     {
         "roleArn": str,
         "requestId": str,
     },
 )
@@ -1786,38 +1589,29 @@
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
 ):
     pass
 
 
-StartRunResponseTypeDef = TypedDict(
-    "StartRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-StartVariantImportResponseTypeDef = TypedDict(
-    "StartVariantImportResponseTypeDef",
+TsvStoreOptionsOutputTypeDef = TypedDict(
+    "TsvStoreOptionsOutputTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationType": AnnotationTypeType,
+        "formatToHeader": Dict[FormatToHeaderKeyType, str],
+        "schema": List[Dict[str, SchemaValueTypeType]],
     },
+    total=False,
 )
 
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
@@ -1940,45 +1734,14 @@
         "uploadId": str,
         "partSource": ReadSetPartSourceType,
         "partNumber": int,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-UploadReadSetPartResponseTypeDef = TypedDict(
-    "UploadReadSetPartResponseTypeDef",
-    {
-        "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
@@ -1995,324 +1758,565 @@
 class ListReadSetActivationJobsRequestRequestTypeDef(
     _RequiredListReadSetActivationJobsRequestRequestTypeDef,
     _OptionalListReadSetActivationJobsRequestRequestTypeDef,
 ):
     pass
 
 
-ListReadSetActivationJobsResponseTypeDef = TypedDict(
-    "ListReadSetActivationJobsResponseTypeDef",
+AnnotationStoreItemTypeDef = TypedDict(
+    "AnnotationStoreItemTypeDef",
     {
-        "nextToken": str,
-        "activationJobs": List[ActivateReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "reference": ReferenceItemOutputTypeDef,
+        "status": StoreStatusType,
+        "storeArn": str,
+        "name": str,
+        "storeFormat": StoreFormatType,
+        "description": str,
+        "sseConfig": SseConfigOutputTypeDef,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "statusMessage": str,
+        "storeSizeBytes": int,
     },
 )
 
-GetReadSetActivationJobResponseTypeDef = TypedDict(
-    "GetReadSetActivationJobResponseTypeDef",
+_RequiredReferenceStoreDetailTypeDef = TypedDict(
+    "_RequiredReferenceStoreDetailTypeDef",
     {
+        "arn": str,
         "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "statusMessage": str,
         "creationTime": datetime,
-        "completionTime": datetime,
-        "sources": List[ActivateReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-ListAnnotationImportJobsResponseTypeDef = TypedDict(
-    "ListAnnotationImportJobsResponseTypeDef",
+_OptionalReferenceStoreDetailTypeDef = TypedDict(
+    "_OptionalReferenceStoreDetailTypeDef",
     {
-        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigOutputTypeDef,
     },
+    total=False,
 )
 
-CreateVariantStoreResponseTypeDef = TypedDict(
-    "CreateVariantStoreResponseTypeDef",
+
+class ReferenceStoreDetailTypeDef(
+    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
+):
+    pass
+
+
+_RequiredSequenceStoreDetailTypeDef = TypedDict(
+    "_RequiredSequenceStoreDetailTypeDef",
     {
+        "arn": str,
         "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
-        "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-UpdateVariantStoreResponseTypeDef = TypedDict(
-    "UpdateVariantStoreResponseTypeDef",
+_OptionalSequenceStoreDetailTypeDef = TypedDict(
+    "_OptionalSequenceStoreDetailTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
         "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sseConfig": SseConfigOutputTypeDef,
+        "fallbackLocation": str,
     },
+    total=False,
 )
 
-AnnotationStoreItemTypeDef = TypedDict(
-    "AnnotationStoreItemTypeDef",
+
+class SequenceStoreDetailTypeDef(
+    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
+):
+    pass
+
+
+VariantStoreItemTypeDef = TypedDict(
+    "VariantStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
-        "storeFormat": StoreFormatType,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
-_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+BatchDeleteReadSetResponseTypeDef = TypedDict(
+    "BatchDeleteReadSetResponseTypeDef",
     {
-        "name": str,
+        "errors": List[ReadSetBatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+
+CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CompleteMultipartReadSetUploadResponseTypeDef",
     {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
+        "readSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateReferenceStoreRequestRequestTypeDef(
-    _RequiredCreateReferenceStoreRequestRequestTypeDef,
-    _OptionalCreateReferenceStoreRequestRequestTypeDef,
-):
-    pass
-
+CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "generatedFrom": str,
+        "referenceArn": str,
+        "name": str,
+        "description": str,
+        "tags": Dict[str, str],
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateReferenceStoreResponseTypeDef = TypedDict(
     "CreateReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+CreateRunGroupResponseTypeDef = TypedDict(
+    "CreateRunGroupResponseTypeDef",
     {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-        "fallbackLocation": str,
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateSequenceStoreRequestRequestTypeDef(
-    _RequiredCreateSequenceStoreRequestRequestTypeDef,
-    _OptionalCreateSequenceStoreRequestRequestTypeDef,
-):
-    pass
-
-
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+CreateVariantStoreResponseTypeDef = TypedDict(
+    "CreateVariantStoreResponseTypeDef",
     {
-        "reference": ReferenceItemTypeDef,
+        "id": str,
+        "reference": ReferenceItemOutputTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteAnnotationStoreResponseTypeDef = TypedDict(
+    "DeleteAnnotationStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateVariantStoreRequestRequestTypeDef(
-    _RequiredCreateVariantStoreRequestRequestTypeDef,
-    _OptionalCreateVariantStoreRequestRequestTypeDef,
-):
-    pass
+DeleteVariantStoreResponseTypeDef = TypedDict(
+    "DeleteVariantStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadSetActivationJobResponseTypeDef = TypedDict(
+    "GetReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "statusMessage": str,
+        "creationTime": datetime,
+        "completionTime": datetime,
+        "sources": List[ActivateReadSetSourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadSetResponseTypeDef = TypedDict(
+    "GetReadSetResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceResponseTypeDef = TypedDict(
+    "GetReferenceResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetReferenceStoreResponseTypeDef = TypedDict(
     "GetReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunGroupResponseTypeDef = TypedDict(
+    "GetRunGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "maxCpus": int,
+        "maxRuns": int,
+        "maxDuration": int,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "maxGpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunResponseTypeDef = TypedDict(
+    "GetRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "workflowId": str,
+        "workflowType": WorkflowTypeType,
+        "runId": str,
+        "roleArn": str,
+        "name": str,
+        "runGroupId": str,
+        "priority": int,
+        "definition": str,
+        "digest": str,
+        "parameters": Dict[str, Any],
+        "storageCapacity": int,
+        "outputUri": str,
+        "logLevel": RunLogLevelType,
+        "resourceDigests": Dict[str, str],
+        "startedBy": str,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunTaskResponseTypeDef = TypedDict(
+    "GetRunTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "status": TaskStatusType,
+        "name": str,
+        "cpus": int,
+        "memory": int,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "logStream": str,
+        "gpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSequenceStoreResponseTypeDef = TypedDict(
     "GetSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReferenceStoreDetailTypeDef = TypedDict(
-    "_RequiredReferenceStoreDetailTypeDef",
+ListAnnotationImportJobsResponseTypeDef = TypedDict(
+    "ListAnnotationImportJobsResponseTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "creationTime": datetime,
+        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalReferenceStoreDetailTypeDef = TypedDict(
-    "_OptionalReferenceStoreDetailTypeDef",
+
+ListReadSetActivationJobsResponseTypeDef = TypedDict(
+    "ListReadSetActivationJobsResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "nextToken": str,
+        "activationJobs": List[ActivateReadSetJobItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ReferenceStoreDetailTypeDef(
-    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
-):
-    pass
+StartAnnotationImportResponseTypeDef = TypedDict(
+    "StartAnnotationImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartReadSetActivationJobResponseTypeDef = TypedDict(
+    "StartReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredSequenceStoreDetailTypeDef = TypedDict(
-    "_RequiredSequenceStoreDetailTypeDef",
+StartReadSetExportJobResponseTypeDef = TypedDict(
+    "StartReadSetExportJobResponseTypeDef",
     {
-        "arn": str,
         "id": str,
+        "sequenceStoreId": str,
+        "destination": str,
+        "status": ReadSetExportJobStatusType,
         "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSequenceStoreDetailTypeDef = TypedDict(
-    "_OptionalSequenceStoreDetailTypeDef",
+
+StartReadSetImportJobResponseTypeDef = TypedDict(
+    "StartReadSetImportJobResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "fallbackLocation": str,
+        "id": str,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "status": ReadSetImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+StartReferenceImportJobResponseTypeDef = TypedDict(
+    "StartReferenceImportJobResponseTypeDef",
+    {
+        "id": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "status": ReferenceImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class SequenceStoreDetailTypeDef(
-    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
-):
-    pass
+StartRunResponseTypeDef = TypedDict(
+    "StartRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartVariantImportResponseTypeDef = TypedDict(
+    "StartVariantImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VariantStoreItemTypeDef = TypedDict(
-    "VariantStoreItemTypeDef",
+UpdateVariantStoreResponseTypeDef = TypedDict(
+    "UpdateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
-        "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
-        "statusMessage": str,
-        "storeSizeBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeleteReadSetResponseTypeDef = TypedDict(
-    "BatchDeleteReadSetResponseTypeDef",
+UploadReadSetPartResponseTypeDef = TypedDict(
+    "UploadReadSetPartResponseTypeDef",
     {
-        "errors": List[ReadSetBatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
 )
 
+_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateReferenceStoreRequestRequestTypeDef(
+    _RequiredCreateReferenceStoreRequestRequestTypeDef,
+    _OptionalCreateReferenceStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+        "fallbackLocation": str,
+    },
+    total=False,
+)
+
+
+class CreateSequenceStoreRequestRequestTypeDef(
+    _RequiredCreateSequenceStoreRequestRequestTypeDef,
+    _OptionalCreateSequenceStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+    },
+)
+_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateVariantStoreRequestRequestTypeDef(
+    _RequiredCreateVariantStoreRequestRequestTypeDef,
+    _OptionalCreateVariantStoreRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2335,75 +2339,28 @@
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-GetWorkflowResponseTypeDef = TypedDict(
-    "GetWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "type": WorkflowTypeType,
-        "name": str,
-        "description": str,
-        "engine": WorkflowEngineType,
-        "definition": str,
-        "main": str,
-        "digest": str,
-        "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
-        "storageCapacity": int,
-        "creationTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "metadata": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
 
 _RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetExportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
@@ -2426,15 +2383,15 @@
 
 
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetExportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2853,15 +2810,15 @@
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReferenceSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantImportResponseTypeDef = TypedDict(
     "GetVariantImportResponseTypeDef",
     {
         "id": str,
@@ -2871,41 +2828,42 @@
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+GetWorkflowResponseTypeDef = TypedDict(
+    "GetWorkflowResponseTypeDef",
     {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "type": WorkflowTypeType,
+        "name": str,
+        "description": str,
+        "engine": WorkflowEngineType,
+        "definition": str,
+        "main": str,
+        "digest": str,
+        "parameterTemplate": Dict[str, WorkflowParameterOutputTypeDef],
+        "storageCapacity": int,
+        "creationTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "metadata": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetImportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
@@ -2927,22 +2885,22 @@
 
 
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
-        "sourceFiles": SourceFilesTypeDef,
+        "sourceFiles": SourceFilesOutputTypeDef,
         "sourceFileType": FileTypeType,
         "status": ReadSetImportJobItemStatusType,
         "subjectId": str,
         "sampleId": str,
     },
 )
 _OptionalImportReadSetSourceItemTypeDef = TypedDict(
@@ -2961,125 +2919,241 @@
 
 class ImportReadSetSourceItemTypeDef(
     _RequiredImportReadSetSourceItemTypeDef, _OptionalImportReadSetSourceItemTypeDef
 ):
     pass
 
 
-_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
     {
-        "sourceFiles": SourceFilesTypeDef,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "referenceArn": str,
+        "referenceStoreId": str,
     },
 )
-_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
     {
-        "generatedFrom": str,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReferenceFilterTypeDef,
     },
     total=False,
 )
 
 
-class StartReadSetImportJobSourceItemTypeDef(
-    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+
+ListReferenceImportJobsResponseTypeDef = TypedDict(
+    "ListReferenceImportJobsResponseTypeDef",
+    {
+        "nextToken": str,
+        "importJobs": List[ImportReferenceJobItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "ids": Sequence[str],
+        "nextToken": str,
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+    },
+    total=False,
+)
+
+ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    {
+        "ids": Sequence[str],
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
+    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
 ):
     pass
 
 
 _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
     "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
         "referenceStoreId": str,
     },
 )
 _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
     "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
         "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
     _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
-        "referenceStoreId": str,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
+
+_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
+        "id": str,
+    },
+)
+_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
+    {
+        "status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+class ListRunTasksRequestListRunTasksPaginateTypeDef(
+    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
+    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
 ):
     pass
 
 
-ListReferenceImportJobsResponseTypeDef = TypedDict(
-    "ListReferenceImportJobsResponseTypeDef",
-    {
-        "nextToken": str,
-        "importJobs": List[ImportReferenceJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+ListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "ListRunsRequestListRunsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListAnnotationImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "name": str,
+        "runGroupId": str,
+        "status": RunStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestRequestTypeDef",
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     {
-        "maxResults": int,
-        "ids": Sequence[str],
-        "nextToken": str,
-        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "type": WorkflowTypeType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListAnnotationStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestRequestTypeDef = TypedDict(
     "ListAnnotationStoresRequestRequestTypeDef",
     {
@@ -3092,15 +3166,15 @@
 )
 
 ListMultipartReadSetUploadsResponseTypeDef = TypedDict(
     "ListMultipartReadSetUploadsResponseTypeDef",
     {
         "nextToken": str,
         "uploads": List[MultipartReadSetUploadListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
     "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
         "sequenceStoreId": str,
@@ -3108,15 +3182,15 @@
         "partSource": ReadSetPartSourceType,
     },
 )
 _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
     "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
         "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
     _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
@@ -3152,29 +3226,29 @@
 
 
 ListReadSetUploadPartsResponseTypeDef = TypedDict(
     "ListReadSetUploadPartsResponseTypeDef",
     {
         "nextToken": str,
         "parts": List[ReadSetUploadPartListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
     "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
     "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
     {
         "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListReadSetsRequestListReadSetsPaginateTypeDef(
     _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
@@ -3206,15 +3280,15 @@
     pass
 
 
 ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
     "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
     {
         "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReferenceStoresRequestRequestTypeDef = TypedDict(
     "ListReferenceStoresRequestRequestTypeDef",
     {
@@ -3231,15 +3305,15 @@
         "referenceStoreId": str,
     },
 )
 _OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
     "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
     {
         "filter": ReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListReferencesRequestListReferencesPaginateTypeDef(
     _RequiredListReferencesRequestListReferencesPaginateTypeDef,
@@ -3272,50 +3346,50 @@
 
 
 ListReferencesResponseTypeDef = TypedDict(
     "ListReferencesResponseTypeDef",
     {
         "nextToken": str,
         "references": List[ReferenceListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunGroupsResponseTypeDef = TypedDict(
     "ListRunGroupsResponseTypeDef",
     {
         "items": List[RunGroupListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunTasksResponseTypeDef = TypedDict(
     "ListRunTasksResponseTypeDef",
     {
         "items": List[TaskListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunsResponseTypeDef = TypedDict(
     "ListRunsResponseTypeDef",
     {
         "items": List[RunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
     "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
     {
         "filter": SequenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSequenceStoresRequestRequestTypeDef = TypedDict(
     "ListSequenceStoresRequestRequestTypeDef",
     {
@@ -3327,15 +3401,15 @@
 )
 
 ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantImportJobsRequestRequestTypeDef = TypedDict(
     "ListVariantImportJobsRequestRequestTypeDef",
     {
@@ -3348,24 +3422,24 @@
 )
 
 ListVariantImportJobsResponseTypeDef = TypedDict(
     "ListVariantImportJobsResponseTypeDef",
     {
         "variantImportJobs": List[VariantImportJobItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantStoresRequestRequestTypeDef = TypedDict(
     "ListVariantStoresRequestRequestTypeDef",
     {
@@ -3378,26 +3452,62 @@
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TsvOptionsOutputTypeDef = TypedDict(
+    "TsvOptionsOutputTypeDef",
+    {
+        "readOptions": ReadOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 TsvOptionsTypeDef = TypedDict(
     "TsvOptionsTypeDef",
     {
         "readOptions": ReadOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+    {
+        "sourceFiles": SourceFilesTypeDef,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "referenceArn": str,
+    },
+)
+_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+    {
+        "generatedFrom": str,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartReadSetImportJobSourceItemTypeDef(
+    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+):
+    pass
+
+
 _RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
@@ -3462,55 +3572,63 @@
 class StartVariantImportRequestRequestTypeDef(
     _RequiredStartVariantImportRequestRequestTypeDef,
     _OptionalStartVariantImportRequestRequestTypeDef,
 ):
     pass
 
 
+StoreOptionsOutputTypeDef = TypedDict(
+    "StoreOptionsOutputTypeDef",
+    {
+        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 StoreOptionsTypeDef = TypedDict(
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
         "annotationStores": List[AnnotationStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReferenceStoresResponseTypeDef = TypedDict(
     "ListReferenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "referenceStores": List[ReferenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresResponseTypeDef = TypedDict(
     "ListSequenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "sequenceStores": List[SequenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresResponseTypeDef = TypedDict(
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetMetadataResponseTypeDef = TypedDict(
     "GetReadSetMetadataResponseTypeDef",
     {
         "id": str,
@@ -3523,15 +3641,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
         "id": str,
@@ -3540,169 +3658,178 @@
         "md5": str,
         "status": ReferenceStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetImportJobResponseTypeDef = TypedDict(
     "GetReadSetImportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobRequestRequestTypeDef",
-    {
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
-    },
-)
-_OptionalStartReadSetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobRequestRequestTypeDef",
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
     {
-        "clientToken": str,
+        "tsvOptions": TsvOptionsOutputTypeDef,
+        "vcfOptions": VcfOptionsOutputTypeDef,
     },
     total=False,
 )
 
-
-class StartReadSetImportJobRequestRequestTypeDef(
-    _RequiredStartReadSetImportJobRequestRequestTypeDef,
-    _OptionalStartReadSetImportJobRequestRequestTypeDef,
-):
-    pass
-
-
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+_RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
-        "storeFormat": StoreFormatType,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
     },
 )
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+_OptionalStartReadSetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobRequestRequestTypeDef",
     {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+class StartReadSetImportJobRequestRequestTypeDef(
+    _RequiredStartReadSetImportJobRequestRequestTypeDef,
+    _OptionalStartReadSetImportJobRequestRequestTypeDef,
 ):
     pass
 
 
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeFormat": StoreFormatType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
         "storeFormat": StoreFormatType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
+
 
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
-        "formatOptions": FormatOptionsTypeDef,
+        "formatOptions": FormatOptionsOutputTypeDef,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
     {
         "destinationName": str,
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,155 +59,154 @@
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     "ActivateReadSetFilterTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
-    "ReferenceItemTypeDef",
-    "SseConfigTypeDef",
+    "ReferenceItemOutputTypeDef",
+    "SseConfigOutputTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "ReferenceItemTypeDef",
+    "SseConfigTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
-    "CreateRunGroupResponseTypeDef",
     "WorkflowParameterTypeDef",
-    "CreateWorkflowResponseTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
-    "DeleteAnnotationStoreResponseTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
     "DeleteRunRequestRequestTypeDef",
     "DeleteSequenceStoreRequestRequestTypeDef",
     "DeleteVariantStoreRequestRequestTypeDef",
-    "DeleteVariantStoreResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
+    "VcfOptionsOutputTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
     "GetReadSetMetadataRequestRequestTypeDef",
     "SequenceInformationTypeDef",
     "GetReadSetRequestRequestTypeDef",
-    "GetReadSetResponseTypeDef",
     "GetReferenceImportJobRequestRequestTypeDef",
     "ImportReferenceSourceItemTypeDef",
     "GetReferenceMetadataRequestRequestTypeDef",
     "GetReferenceRequestRequestTypeDef",
-    "GetReferenceResponseTypeDef",
     "GetReferenceStoreRequestRequestTypeDef",
     "GetRunGroupRequestRequestTypeDef",
-    "GetRunGroupResponseTypeDef",
     "GetRunRequestRequestTypeDef",
-    "GetRunResponseTypeDef",
     "GetRunTaskRequestRequestTypeDef",
-    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
+    "WorkflowParameterOutputTypeDef",
     "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
-    "SourceFilesTypeDef",
+    "SourceFilesOutputTypeDef",
     "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
-    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
     "ReadSetUploadPartListFilterTypeDef",
     "ReadSetUploadPartListItemTypeDef",
     "ReadSetFilterTypeDef",
     "ReferenceStoreFilterTypeDef",
     "ReferenceFilterTypeDef",
     "ReferenceListItemTypeDef",
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     "ListRunGroupsRequestRequestTypeDef",
     "RunGroupListItemTypeDef",
-    "ListRunTasksRequestListRunTasksPaginateTypeDef",
     "ListRunTasksRequestRequestTypeDef",
     "TaskListItemTypeDef",
-    "ListRunsRequestListRunsPaginateTypeDef",
     "ListRunsRequestRequestTypeDef",
     "RunListItemTypeDef",
     "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "PaginatorConfigTypeDef",
+    "ReadOptionsOutputTypeDef",
     "ReadOptionsTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartAnnotationImportResponseTypeDef",
+    "SourceFilesTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
-    "StartReadSetActivationJobResponseTypeDef",
-    "StartReadSetExportJobResponseTypeDef",
-    "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
-    "StartReferenceImportJobResponseTypeDef",
     "StartRunRequestRequestTypeDef",
-    "StartRunResponseTypeDef",
     "VariantImportItemSourceTypeDef",
-    "StartVariantImportResponseTypeDef",
+    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
-    "UploadReadSetPartResponseTypeDef",
-    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
-    "ListReadSetActivationJobsResponseTypeDef",
-    "GetReadSetActivationJobResponseTypeDef",
-    "ListAnnotationImportJobsResponseTypeDef",
-    "CreateVariantStoreResponseTypeDef",
-    "UpdateVariantStoreResponseTypeDef",
     "AnnotationStoreItemTypeDef",
-    "CreateReferenceStoreRequestRequestTypeDef",
+    "ReferenceStoreDetailTypeDef",
+    "SequenceStoreDetailTypeDef",
+    "VariantStoreItemTypeDef",
+    "BatchDeleteReadSetResponseTypeDef",
+    "CompleteMultipartReadSetUploadResponseTypeDef",
+    "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateReferenceStoreResponseTypeDef",
-    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateRunGroupResponseTypeDef",
     "CreateSequenceStoreResponseTypeDef",
-    "CreateVariantStoreRequestRequestTypeDef",
+    "CreateVariantStoreResponseTypeDef",
+    "CreateWorkflowResponseTypeDef",
+    "DeleteAnnotationStoreResponseTypeDef",
+    "DeleteVariantStoreResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetReadSetActivationJobResponseTypeDef",
+    "GetReadSetResponseTypeDef",
+    "GetReferenceResponseTypeDef",
     "GetReferenceStoreResponseTypeDef",
+    "GetRunGroupResponseTypeDef",
+    "GetRunResponseTypeDef",
+    "GetRunTaskResponseTypeDef",
     "GetSequenceStoreResponseTypeDef",
     "GetVariantStoreResponseTypeDef",
-    "ReferenceStoreDetailTypeDef",
-    "SequenceStoreDetailTypeDef",
-    "VariantStoreItemTypeDef",
-    "BatchDeleteReadSetResponseTypeDef",
+    "ListAnnotationImportJobsResponseTypeDef",
+    "ListReadSetActivationJobsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartAnnotationImportResponseTypeDef",
+    "StartReadSetActivationJobResponseTypeDef",
+    "StartReadSetExportJobResponseTypeDef",
+    "StartReadSetImportJobResponseTypeDef",
+    "StartReferenceImportJobResponseTypeDef",
+    "StartRunResponseTypeDef",
+    "StartVariantImportResponseTypeDef",
+    "UpdateVariantStoreResponseTypeDef",
+    "UploadReadSetPartResponseTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
+    "CreateReferenceStoreRequestRequestTypeDef",
+    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateVariantStoreRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
-    "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
-    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
     "GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef",
@@ -223,24 +222,31 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "GetWorkflowResponseTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
-    "StartReadSetImportJobSourceItemTypeDef",
-    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    "ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
+    "ListRunTasksRequestListRunTasksPaginateTypeDef",
+    "ListRunsRequestListRunsPaginateTypeDef",
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     "ListAnnotationStoresRequestRequestTypeDef",
     "ListMultipartReadSetUploadsResponseTypeDef",
     "ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     "ListReadSetUploadPartsRequestRequestTypeDef",
     "ListReadSetUploadPartsResponseTypeDef",
     "ListReadSetsRequestListReadSetsPaginateTypeDef",
@@ -257,33 +263,37 @@
     "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
+    "TsvOptionsOutputTypeDef",
     "TsvOptionsTypeDef",
+    "StartReadSetImportJobSourceItemTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
+    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
-    "StartReadSetImportJobRequestRequestTypeDef",
+    "FormatOptionsOutputTypeDef",
     "FormatOptionsTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
+    "StartReadSetImportJobRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -381,37 +391,37 @@
 )
 
 class AnnotationImportJobItemTypeDef(
     _RequiredAnnotationImportJobItemTypeDef, _OptionalAnnotationImportJobItemTypeDef
 ):
     pass
 
-ReferenceItemTypeDef = TypedDict(
-    "ReferenceItemTypeDef",
+ReferenceItemOutputTypeDef = TypedDict(
+    "ReferenceItemOutputTypeDef",
     {
         "referenceArn": str,
     },
     total=False,
 )
 
-_RequiredSseConfigTypeDef = TypedDict(
-    "_RequiredSseConfigTypeDef",
+_RequiredSseConfigOutputTypeDef = TypedDict(
+    "_RequiredSseConfigOutputTypeDef",
     {
         "type": Literal["KMS"],
     },
 )
-_OptionalSseConfigTypeDef = TypedDict(
-    "_OptionalSseConfigTypeDef",
+_OptionalSseConfigOutputTypeDef = TypedDict(
+    "_OptionalSseConfigOutputTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
+class SseConfigOutputTypeDef(_RequiredSseConfigOutputTypeDef, _OptionalSseConfigOutputTypeDef):
     pass
 
 BatchDeleteReadSetRequestRequestTypeDef = TypedDict(
     "BatchDeleteReadSetRequestRequestTypeDef",
     {
         "ids": Sequence[str],
         "sequenceStoreId": str,
@@ -423,14 +433,25 @@
     {
         "id": str,
         "code": str,
         "message": str,
     },
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 CancelAnnotationImportRequestRequestTypeDef = TypedDict(
     "CancelAnnotationImportRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -453,22 +474,39 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CompleteMultipartReadSetUploadResponseTypeDef",
+ReferenceItemTypeDef = TypedDict(
+    "ReferenceItemTypeDef",
     {
-        "readSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "referenceArn": str,
     },
+    total=False,
 )
 
+_RequiredSseConfigTypeDef = TypedDict(
+    "_RequiredSseConfigTypeDef",
+    {
+        "type": Literal["KMS"],
+    },
+)
+_OptionalSseConfigTypeDef = TypedDict(
+    "_OptionalSseConfigTypeDef",
+    {
+        "keyArn": str,
+    },
+    total=False,
+)
+
+class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
+    pass
+
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -489,32 +527,14 @@
 
 class CreateMultipartReadSetUploadRequestRequestTypeDef(
     _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef,
     _OptionalCreateMultipartReadSetUploadRequestRequestTypeDef,
 ):
     pass
 
-CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
-    "CreateMultipartReadSetUploadResponseTypeDef",
-    {
-        "sequenceStoreId": str,
-        "uploadId": str,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "generatedFrom": str,
-        "referenceArn": str,
-        "name": str,
-        "description": str,
-        "tags": Dict[str, str],
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRunGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRunGroupRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateRunGroupRequestRequestTypeDef = TypedDict(
@@ -531,44 +551,23 @@
 )
 
 class CreateRunGroupRequestRequestTypeDef(
     _RequiredCreateRunGroupRequestRequestTypeDef, _OptionalCreateRunGroupRequestRequestTypeDef
 ):
     pass
 
-CreateRunGroupResponseTypeDef = TypedDict(
-    "CreateRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkflowParameterTypeDef = TypedDict(
     "WorkflowParameterTypeDef",
     {
         "description": str,
         "optional": bool,
     },
     total=False,
 )
 
-CreateWorkflowResponseTypeDef = TypedDict(
-    "CreateWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnnotationStoreRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalDeleteAnnotationStoreRequestRequestTypeDef = TypedDict(
@@ -581,22 +580,14 @@
 
 class DeleteAnnotationStoreRequestRequestTypeDef(
     _RequiredDeleteAnnotationStoreRequestRequestTypeDef,
     _OptionalDeleteAnnotationStoreRequestRequestTypeDef,
 ):
     pass
 
-DeleteAnnotationStoreResponseTypeDef = TypedDict(
-    "DeleteAnnotationStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReferenceRequestRequestTypeDef = TypedDict(
     "DeleteReferenceRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -645,36 +636,21 @@
 
 class DeleteVariantStoreRequestRequestTypeDef(
     _RequiredDeleteVariantStoreRequestRequestTypeDef,
     _OptionalDeleteVariantStoreRequestRequestTypeDef,
 ):
     pass
 
-DeleteVariantStoreResponseTypeDef = TypedDict(
-    "DeleteVariantStoreResponseTypeDef",
-    {
-        "status": StoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportReadSetDetailTypeDef = TypedDict(
     "_RequiredExportReadSetDetailTypeDef",
     {
         "id": str,
         "status": ReadSetExportJobItemStatusType,
     },
 )
@@ -737,14 +713,23 @@
         "totalParts": int,
         "partSize": int,
         "contentLength": int,
     },
     total=False,
 )
 
+VcfOptionsOutputTypeDef = TypedDict(
+    "VcfOptionsOutputTypeDef",
+    {
+        "ignoreQualField": bool,
+        "ignoreFilterField": bool,
+    },
+    total=False,
+)
+
 VcfOptionsTypeDef = TypedDict(
     "VcfOptionsTypeDef",
     {
         "ignoreQualField": bool,
         "ignoreFilterField": bool,
     },
     total=False,
@@ -833,22 +818,14 @@
 )
 
 class GetReadSetRequestRequestTypeDef(
     _RequiredGetReadSetRequestRequestTypeDef, _OptionalGetReadSetRequestRequestTypeDef
 ):
     pass
 
-GetReadSetResponseTypeDef = TypedDict(
-    "GetReadSetResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceImportJobRequestRequestTypeDef = TypedDict(
     "GetReferenceImportJobRequestRequestTypeDef",
     {
         "id": str,
         "referenceStoreId": str,
     },
 )
@@ -902,52 +879,28 @@
 )
 
 class GetReferenceRequestRequestTypeDef(
     _RequiredGetReferenceRequestRequestTypeDef, _OptionalGetReferenceRequestRequestTypeDef
 ):
     pass
 
-GetReferenceResponseTypeDef = TypedDict(
-    "GetReferenceResponseTypeDef",
-    {
-        "payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReferenceStoreRequestRequestTypeDef = TypedDict(
     "GetReferenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
 GetRunGroupRequestRequestTypeDef = TypedDict(
     "GetRunGroupRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetRunGroupResponseTypeDef = TypedDict(
-    "GetRunGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "maxCpus": int,
-        "maxRuns": int,
-        "maxDuration": int,
-        "creationTime": datetime,
-        "tags": Dict[str, str],
-        "maxGpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRunRequestRequestTypeDef = TypedDict(
     "_RequiredGetRunRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetRunRequestRequestTypeDef = TypedDict(
@@ -959,71 +912,22 @@
 )
 
 class GetRunRequestRequestTypeDef(
     _RequiredGetRunRequestRequestTypeDef, _OptionalGetRunRequestRequestTypeDef
 ):
     pass
 
-GetRunResponseTypeDef = TypedDict(
-    "GetRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "workflowId": str,
-        "workflowType": WorkflowTypeType,
-        "runId": str,
-        "roleArn": str,
-        "name": str,
-        "runGroupId": str,
-        "priority": int,
-        "definition": str,
-        "digest": str,
-        "parameters": Dict[str, Any],
-        "storageCapacity": int,
-        "outputUri": str,
-        "logLevel": RunLogLevelType,
-        "resourceDigests": Dict[str, str],
-        "startedBy": str,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRunTaskRequestRequestTypeDef = TypedDict(
     "GetRunTaskRequestRequestTypeDef",
     {
         "id": str,
         "taskId": str,
     },
 )
 
-GetRunTaskResponseTypeDef = TypedDict(
-    "GetRunTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "status": TaskStatusType,
-        "name": str,
-        "cpus": int,
-        "memory": int,
-        "creationTime": datetime,
-        "startTime": datetime,
-        "stopTime": datetime,
-        "statusMessage": str,
-        "logStream": str,
-        "gpus": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSequenceStoreRequestRequestTypeDef = TypedDict(
     "GetSequenceStoreRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -1077,14 +981,23 @@
 )
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
+WorkflowParameterOutputTypeDef = TypedDict(
+    "WorkflowParameterOutputTypeDef",
+    {
+        "description": str,
+        "optional": bool,
+    },
+    total=False,
+)
+
 ImportReadSetFilterTypeDef = TypedDict(
     "ImportReadSetFilterTypeDef",
     {
         "status": ReadSetImportJobStatusType,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
     },
@@ -1110,29 +1023,31 @@
 )
 
 class ImportReadSetJobItemTypeDef(
     _RequiredImportReadSetJobItemTypeDef, _OptionalImportReadSetJobItemTypeDef
 ):
     pass
 
-_RequiredSourceFilesTypeDef = TypedDict(
-    "_RequiredSourceFilesTypeDef",
+_RequiredSourceFilesOutputTypeDef = TypedDict(
+    "_RequiredSourceFilesOutputTypeDef",
     {
         "source1": str,
     },
 )
-_OptionalSourceFilesTypeDef = TypedDict(
-    "_OptionalSourceFilesTypeDef",
+_OptionalSourceFilesOutputTypeDef = TypedDict(
+    "_OptionalSourceFilesOutputTypeDef",
     {
         "source2": str,
     },
     total=False,
 )
 
-class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
+class SourceFilesOutputTypeDef(
+    _RequiredSourceFilesOutputTypeDef, _OptionalSourceFilesOutputTypeDef
+):
     pass
 
 ImportReferenceFilterTypeDef = TypedDict(
     "ImportReferenceFilterTypeDef",
     {
         "status": ReferenceImportJobStatusType,
         "createdAfter": Union[datetime, str],
@@ -1169,42 +1084,32 @@
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
 )
 
-ListAnnotationStoresFilterTypeDef = TypedDict(
-    "ListAnnotationStoresFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": StoreStatusType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
-    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+ListAnnotationStoresFilterTypeDef = TypedDict(
+    "ListAnnotationStoresFilterTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "status": StoreStatusType,
     },
     total=False,
 )
 
-class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
-    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
     "_RequiredListMultipartReadSetUploadsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListMultipartReadSetUploadsRequestRequestTypeDef = TypedDict(
@@ -1340,23 +1245,14 @@
 )
 
 class ReferenceListItemTypeDef(
     _RequiredReferenceListItemTypeDef, _OptionalReferenceListItemTypeDef
 ):
     pass
 
-ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
-    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunGroupsRequestRequestTypeDef = TypedDict(
     "ListRunGroupsRequestRequestTypeDef",
     {
         "name": str,
         "startingToken": str,
         "maxResults": int,
     },
@@ -1374,35 +1270,14 @@
         "maxDuration": int,
         "creationTime": datetime,
         "maxGpus": int,
     },
     total=False,
 )
 
-_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
-    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
-    {
-        "status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRunTasksRequestListRunTasksPaginateTypeDef(
-    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
-    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
-):
-    pass
-
 _RequiredListRunTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListRunTasksRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalListRunTasksRequestRequestTypeDef = TypedDict(
@@ -1432,25 +1307,14 @@
         "startTime": datetime,
         "stopTime": datetime,
         "gpus": int,
     },
     total=False,
 )
 
-ListRunsRequestListRunsPaginateTypeDef = TypedDict(
-    "ListRunsRequestListRunsPaginateTypeDef",
-    {
-        "name": str,
-        "runGroupId": str,
-        "status": RunStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRunsRequestRequestTypeDef = TypedDict(
     "ListRunsRequestRequestTypeDef",
     {
         "name": str,
         "runGroupId": str,
         "startingToken": str,
         "maxResults": int,
@@ -1489,22 +1353,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVariantImportJobsFilterTypeDef = TypedDict(
     "ListVariantImportJobsFilterTypeDef",
     {
         "status": JobStatusType,
         "storeName": str,
     },
     total=False,
@@ -1540,24 +1396,14 @@
     "ListVariantStoresFilterTypeDef",
     {
         "status": StoreStatusType,
     },
     total=False,
 )
 
-ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
-    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
-    {
-        "type": WorkflowTypeType,
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkflowsRequestRequestTypeDef = TypedDict(
     "ListWorkflowsRequestRequestTypeDef",
     {
         "type": WorkflowTypeType,
         "name": str,
         "startingToken": str,
         "maxResults": int,
@@ -1576,20 +1422,26 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ReadOptionsOutputTypeDef = TypedDict(
+    "ReadOptionsOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "sep": str,
+        "encoding": str,
+        "quote": str,
+        "quoteAll": bool,
+        "escape": str,
+        "escapeQuotes": bool,
+        "comment": str,
+        "header": bool,
+        "lineSep": str,
     },
     total=False,
 )
 
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
@@ -1602,75 +1454,38 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredSourceFilesTypeDef = TypedDict(
+    "_RequiredSourceFilesTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "source1": str,
     },
 )
-
-StartAnnotationImportResponseTypeDef = TypedDict(
-    "StartAnnotationImportResponseTypeDef",
+_OptionalSourceFilesTypeDef = TypedDict(
+    "_OptionalSourceFilesTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "source2": str,
     },
+    total=False,
 )
 
+class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
+    pass
+
 StartReadSetActivationJobSourceItemTypeDef = TypedDict(
     "StartReadSetActivationJobSourceItemTypeDef",
     {
         "readSetId": str,
     },
 )
 
-StartReadSetActivationJobResponseTypeDef = TypedDict(
-    "StartReadSetActivationJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetExportJobResponseTypeDef = TypedDict(
-    "StartReadSetExportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "destination": str,
-        "status": ReadSetExportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartReadSetImportJobResponseTypeDef = TypedDict(
-    "StartReadSetImportJobResponseTypeDef",
-    {
-        "id": str,
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "status": ReadSetImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartReferenceImportJobSourceItemTypeDef = TypedDict(
     "_RequiredStartReferenceImportJobSourceItemTypeDef",
     {
         "sourceFile": str,
         "name": str,
     },
 )
@@ -1685,26 +1500,14 @@
 
 class StartReferenceImportJobSourceItemTypeDef(
     _RequiredStartReferenceImportJobSourceItemTypeDef,
     _OptionalStartReferenceImportJobSourceItemTypeDef,
 ):
     pass
 
-StartReferenceImportJobResponseTypeDef = TypedDict(
-    "StartReferenceImportJobResponseTypeDef",
-    {
-        "id": str,
-        "referenceStoreId": str,
-        "roleArn": str,
-        "status": ReferenceImportJobStatusType,
-        "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartRunRequestRequestTypeDef",
     {
         "roleArn": str,
         "requestId": str,
     },
 )
@@ -1727,38 +1530,29 @@
 )
 
 class StartRunRequestRequestTypeDef(
     _RequiredStartRunRequestRequestTypeDef, _OptionalStartRunRequestRequestTypeDef
 ):
     pass
 
-StartRunResponseTypeDef = TypedDict(
-    "StartRunResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": RunStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-StartVariantImportResponseTypeDef = TypedDict(
-    "StartVariantImportResponseTypeDef",
+TsvStoreOptionsOutputTypeDef = TypedDict(
+    "TsvStoreOptionsOutputTypeDef",
     {
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "annotationType": AnnotationTypeType,
+        "formatToHeader": Dict[FormatToHeaderKeyType, str],
+        "schema": List[Dict[str, SchemaValueTypeType]],
     },
+    total=False,
 )
 
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
@@ -1873,43 +1667,14 @@
         "uploadId": str,
         "partSource": ReadSetPartSourceType,
         "partNumber": int,
         "payload": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-UploadReadSetPartResponseTypeDef = TypedDict(
-    "UploadReadSetPartResponseTypeDef",
-    {
-        "checksum": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
-    {
-        "filter": ActivateReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
-    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetActivationJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetActivationJobsRequestRequestTypeDef = TypedDict(
@@ -1924,314 +1689,555 @@
 
 class ListReadSetActivationJobsRequestRequestTypeDef(
     _RequiredListReadSetActivationJobsRequestRequestTypeDef,
     _OptionalListReadSetActivationJobsRequestRequestTypeDef,
 ):
     pass
 
-ListReadSetActivationJobsResponseTypeDef = TypedDict(
-    "ListReadSetActivationJobsResponseTypeDef",
+AnnotationStoreItemTypeDef = TypedDict(
+    "AnnotationStoreItemTypeDef",
     {
-        "nextToken": str,
-        "activationJobs": List[ActivateReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "reference": ReferenceItemOutputTypeDef,
+        "status": StoreStatusType,
+        "storeArn": str,
+        "name": str,
+        "storeFormat": StoreFormatType,
+        "description": str,
+        "sseConfig": SseConfigOutputTypeDef,
+        "creationTime": datetime,
+        "updateTime": datetime,
+        "statusMessage": str,
+        "storeSizeBytes": int,
     },
 )
 
-GetReadSetActivationJobResponseTypeDef = TypedDict(
-    "GetReadSetActivationJobResponseTypeDef",
+_RequiredReferenceStoreDetailTypeDef = TypedDict(
+    "_RequiredReferenceStoreDetailTypeDef",
     {
+        "arn": str,
         "id": str,
-        "sequenceStoreId": str,
-        "status": ReadSetActivationJobStatusType,
-        "statusMessage": str,
         "creationTime": datetime,
-        "completionTime": datetime,
-        "sources": List[ActivateReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-ListAnnotationImportJobsResponseTypeDef = TypedDict(
-    "ListAnnotationImportJobsResponseTypeDef",
+_OptionalReferenceStoreDetailTypeDef = TypedDict(
+    "_OptionalReferenceStoreDetailTypeDef",
     {
-        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "description": str,
+        "sseConfig": SseConfigOutputTypeDef,
     },
+    total=False,
 )
 
-CreateVariantStoreResponseTypeDef = TypedDict(
-    "CreateVariantStoreResponseTypeDef",
+class ReferenceStoreDetailTypeDef(
+    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
+):
+    pass
+
+_RequiredSequenceStoreDetailTypeDef = TypedDict(
+    "_RequiredSequenceStoreDetailTypeDef",
     {
+        "arn": str,
         "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
-        "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-
-UpdateVariantStoreResponseTypeDef = TypedDict(
-    "UpdateVariantStoreResponseTypeDef",
+_OptionalSequenceStoreDetailTypeDef = TypedDict(
+    "_OptionalSequenceStoreDetailTypeDef",
     {
-        "id": str,
-        "reference": ReferenceItemTypeDef,
-        "status": StoreStatusType,
         "name": str,
         "description": str,
-        "creationTime": datetime,
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "sseConfig": SseConfigOutputTypeDef,
+        "fallbackLocation": str,
     },
+    total=False,
 )
 
-AnnotationStoreItemTypeDef = TypedDict(
-    "AnnotationStoreItemTypeDef",
+class SequenceStoreDetailTypeDef(
+    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
+):
+    pass
+
+VariantStoreItemTypeDef = TypedDict(
+    "VariantStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
-        "storeFormat": StoreFormatType,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
-_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+BatchDeleteReadSetResponseTypeDef = TypedDict(
+    "BatchDeleteReadSetResponseTypeDef",
     {
-        "name": str,
+        "errors": List[ReadSetBatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+
+CompleteMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CompleteMultipartReadSetUploadResponseTypeDef",
     {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
+        "readSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateReferenceStoreRequestRequestTypeDef(
-    _RequiredCreateReferenceStoreRequestRequestTypeDef,
-    _OptionalCreateReferenceStoreRequestRequestTypeDef,
-):
-    pass
+CreateMultipartReadSetUploadResponseTypeDef = TypedDict(
+    "CreateMultipartReadSetUploadResponseTypeDef",
+    {
+        "sequenceStoreId": str,
+        "uploadId": str,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "generatedFrom": str,
+        "referenceArn": str,
+        "name": str,
+        "description": str,
+        "tags": Dict[str, str],
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateReferenceStoreResponseTypeDef = TypedDict(
     "CreateReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+CreateRunGroupResponseTypeDef = TypedDict(
+    "CreateRunGroupResponseTypeDef",
     {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-        "fallbackLocation": str,
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateSequenceStoreRequestRequestTypeDef(
-    _RequiredCreateSequenceStoreRequestRequestTypeDef,
-    _OptionalCreateSequenceStoreRequestRequestTypeDef,
-):
-    pass
-
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+CreateVariantStoreResponseTypeDef = TypedDict(
+    "CreateVariantStoreResponseTypeDef",
     {
-        "reference": ReferenceItemTypeDef,
+        "id": str,
+        "reference": ReferenceItemOutputTypeDef,
+        "status": StoreStatusType,
+        "name": str,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+
+CreateWorkflowResponseTypeDef = TypedDict(
+    "CreateWorkflowResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateVariantStoreRequestRequestTypeDef(
-    _RequiredCreateVariantStoreRequestRequestTypeDef,
-    _OptionalCreateVariantStoreRequestRequestTypeDef,
-):
-    pass
+DeleteAnnotationStoreResponseTypeDef = TypedDict(
+    "DeleteAnnotationStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVariantStoreResponseTypeDef = TypedDict(
+    "DeleteVariantStoreResponseTypeDef",
+    {
+        "status": StoreStatusType,
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
+GetReadSetActivationJobResponseTypeDef = TypedDict(
+    "GetReadSetActivationJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
+        "statusMessage": str,
+        "creationTime": datetime,
+        "completionTime": datetime,
+        "sources": List[ActivateReadSetSourceItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReadSetResponseTypeDef = TypedDict(
+    "GetReadSetResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetReferenceResponseTypeDef = TypedDict(
+    "GetReferenceResponseTypeDef",
+    {
+        "payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetReferenceStoreResponseTypeDef = TypedDict(
     "GetReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunGroupResponseTypeDef = TypedDict(
+    "GetRunGroupResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "maxCpus": int,
+        "maxRuns": int,
+        "maxDuration": int,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "maxGpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunResponseTypeDef = TypedDict(
+    "GetRunResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "workflowId": str,
+        "workflowType": WorkflowTypeType,
+        "runId": str,
+        "roleArn": str,
+        "name": str,
+        "runGroupId": str,
+        "priority": int,
+        "definition": str,
+        "digest": str,
+        "parameters": Dict[str, Any],
+        "storageCapacity": int,
+        "outputUri": str,
+        "logLevel": RunLogLevelType,
+        "resourceDigests": Dict[str, str],
+        "startedBy": str,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRunTaskResponseTypeDef = TypedDict(
+    "GetRunTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "status": TaskStatusType,
+        "name": str,
+        "cpus": int,
+        "memory": int,
+        "creationTime": datetime,
+        "startTime": datetime,
+        "stopTime": datetime,
+        "statusMessage": str,
+        "logStream": str,
+        "gpus": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSequenceStoreResponseTypeDef = TypedDict(
     "GetSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReferenceStoreDetailTypeDef = TypedDict(
-    "_RequiredReferenceStoreDetailTypeDef",
+ListAnnotationImportJobsResponseTypeDef = TypedDict(
+    "ListAnnotationImportJobsResponseTypeDef",
+    {
+        "annotationImportJobs": List[AnnotationImportJobItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListReadSetActivationJobsResponseTypeDef = TypedDict(
+    "ListReadSetActivationJobsResponseTypeDef",
+    {
+        "nextToken": str,
+        "activationJobs": List[ActivateReadSetJobItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAnnotationImportResponseTypeDef = TypedDict(
+    "StartAnnotationImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartReadSetActivationJobResponseTypeDef = TypedDict(
+    "StartReadSetActivationJobResponseTypeDef",
     {
-        "arn": str,
         "id": str,
+        "sequenceStoreId": str,
+        "status": ReadSetActivationJobStatusType,
         "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalReferenceStoreDetailTypeDef = TypedDict(
-    "_OptionalReferenceStoreDetailTypeDef",
+
+StartReadSetExportJobResponseTypeDef = TypedDict(
+    "StartReadSetExportJobResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "id": str,
+        "sequenceStoreId": str,
+        "destination": str,
+        "status": ReadSetExportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ReferenceStoreDetailTypeDef(
-    _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
-):
-    pass
+StartReadSetImportJobResponseTypeDef = TypedDict(
+    "StartReadSetImportJobResponseTypeDef",
+    {
+        "id": str,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "status": ReadSetImportJobStatusType,
+        "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredSequenceStoreDetailTypeDef = TypedDict(
-    "_RequiredSequenceStoreDetailTypeDef",
+StartReferenceImportJobResponseTypeDef = TypedDict(
+    "StartReferenceImportJobResponseTypeDef",
     {
-        "arn": str,
         "id": str,
+        "referenceStoreId": str,
+        "roleArn": str,
+        "status": ReferenceImportJobStatusType,
         "creationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalSequenceStoreDetailTypeDef = TypedDict(
-    "_OptionalSequenceStoreDetailTypeDef",
+
+StartRunResponseTypeDef = TypedDict(
+    "StartRunResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "fallbackLocation": str,
+        "arn": str,
+        "id": str,
+        "status": RunStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SequenceStoreDetailTypeDef(
-    _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
-):
-    pass
+StartVariantImportResponseTypeDef = TypedDict(
+    "StartVariantImportResponseTypeDef",
+    {
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-VariantStoreItemTypeDef = TypedDict(
-    "VariantStoreItemTypeDef",
+UpdateVariantStoreResponseTypeDef = TypedDict(
+    "UpdateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
-        "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
-        "statusMessage": str,
-        "storeSizeBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeleteReadSetResponseTypeDef = TypedDict(
-    "BatchDeleteReadSetResponseTypeDef",
+UploadReadSetPartResponseTypeDef = TypedDict(
+    "UploadReadSetPartResponseTypeDef",
     {
-        "errors": List[ReadSetBatchErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "checksum": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
 )
 
+_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateReferenceStoreRequestRequestTypeDef(
+    _RequiredCreateReferenceStoreRequestRequestTypeDef,
+    _OptionalCreateReferenceStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+        "fallbackLocation": str,
+    },
+    total=False,
+)
+
+class CreateSequenceStoreRequestRequestTypeDef(
+    _RequiredCreateSequenceStoreRequestRequestTypeDef,
+    _OptionalCreateSequenceStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+    },
+)
+_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateVariantStoreRequestRequestTypeDef(
+    _RequiredCreateVariantStoreRequestRequestTypeDef,
+    _OptionalCreateVariantStoreRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2252,74 +2258,29 @@
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
-GetWorkflowResponseTypeDef = TypedDict(
-    "GetWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "type": WorkflowTypeType,
-        "name": str,
-        "description": str,
-        "engine": WorkflowEngineType,
-        "definition": str,
-        "main": str,
-        "digest": str,
-        "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
-        "storageCapacity": int,
-        "creationTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "metadata": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "readSets": List[ExportReadSetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
-    {
-        "filter": ExportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
-    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListReadSetExportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetExportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetExportJobsRequestRequestTypeDef = TypedDict(
@@ -2339,15 +2300,15 @@
     pass
 
 ListReadSetExportJobsResponseTypeDef = TypedDict(
     "ListReadSetExportJobsResponseTypeDef",
     {
         "nextToken": str,
         "exportJobs": List[ExportReadSetJobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartReadSetExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetExportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
@@ -2732,15 +2693,15 @@
         "referenceStoreId": str,
         "roleArn": str,
         "status": ReferenceImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReferenceSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantImportResponseTypeDef = TypedDict(
     "GetVariantImportResponseTypeDef",
     {
         "id": str,
@@ -2750,39 +2711,42 @@
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
-    {
-        "sequenceStoreId": str,
-    },
-)
-_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+GetWorkflowResponseTypeDef = TypedDict(
+    "GetWorkflowResponseTypeDef",
     {
-        "filter": ImportReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "type": WorkflowTypeType,
+        "name": str,
+        "description": str,
+        "engine": WorkflowEngineType,
+        "definition": str,
+        "main": str,
+        "digest": str,
+        "parameterTemplate": Dict[str, WorkflowParameterOutputTypeDef],
+        "storageCapacity": int,
+        "creationTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "metadata": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
-    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetImportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
@@ -2802,22 +2766,22 @@
     pass
 
 ListReadSetImportJobsResponseTypeDef = TypedDict(
     "ListReadSetImportJobsResponseTypeDef",
     {
         "nextToken": str,
         "importJobs": List[ImportReadSetJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
-        "sourceFiles": SourceFilesTypeDef,
+        "sourceFiles": SourceFilesOutputTypeDef,
         "sourceFileType": FileTypeType,
         "status": ReadSetImportJobItemStatusType,
         "subjectId": str,
         "sampleId": str,
     },
 )
 _OptionalImportReadSetSourceItemTypeDef = TypedDict(
@@ -2834,119 +2798,227 @@
 )
 
 class ImportReadSetSourceItemTypeDef(
     _RequiredImportReadSetSourceItemTypeDef, _OptionalImportReadSetSourceItemTypeDef
 ):
     pass
 
-_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
     {
-        "sourceFiles": SourceFilesTypeDef,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "referenceArn": str,
+        "referenceStoreId": str,
     },
 )
-_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
     {
-        "generatedFrom": str,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
+        "maxResults": int,
+        "nextToken": str,
+        "filter": ImportReferenceFilterTypeDef,
     },
     total=False,
 )
 
-class StartReadSetImportJobSourceItemTypeDef(
-    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+class ListReferenceImportJobsRequestRequestTypeDef(
+    _RequiredListReferenceImportJobsRequestRequestTypeDef,
+    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+):
+    pass
+
+ListReferenceImportJobsResponseTypeDef = TypedDict(
+    "ListReferenceImportJobsResponseTypeDef",
+    {
+        "nextToken": str,
+        "importJobs": List[ImportReferenceJobItemTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "ids": Sequence[str],
+        "nextToken": str,
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+    },
+    total=False,
+)
+
+ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
+    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+    {
+        "ids": Sequence[str],
+        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef = TypedDict(
+    "_OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef(
+    _RequiredListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    _OptionalListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
+    {
+        "filter": ActivateReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef(
+    _RequiredListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    _OptionalListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
+    {
+        "filter": ExportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef(
+    _RequiredListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    _OptionalListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "sequenceStoreId": str,
+    },
+)
+_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
+    {
+        "filter": ImportReadSetFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef(
+    _RequiredListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    _OptionalListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
 ):
     pass
 
 _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
     "_RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
         "referenceStoreId": str,
     },
 )
 _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef = TypedDict(
     "_OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef",
     {
         "filter": ImportReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef(
     _RequiredListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     _OptionalListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
 ):
     pass
 
-_RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListReferenceImportJobsRequestRequestTypeDef",
+ListRunGroupsRequestListRunGroupsPaginateTypeDef = TypedDict(
+    "ListRunGroupsRequestListRunGroupsPaginateTypeDef",
     {
-        "referenceStoreId": str,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListReferenceImportJobsRequestRequestTypeDef",
+
+_RequiredListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_RequiredListRunTasksRequestListRunTasksPaginateTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "filter": ImportReferenceFilterTypeDef,
+        "id": str,
+    },
+)
+_OptionalListRunTasksRequestListRunTasksPaginateTypeDef = TypedDict(
+    "_OptionalListRunTasksRequestListRunTasksPaginateTypeDef",
+    {
+        "status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListReferenceImportJobsRequestRequestTypeDef(
-    _RequiredListReferenceImportJobsRequestRequestTypeDef,
-    _OptionalListReferenceImportJobsRequestRequestTypeDef,
+class ListRunTasksRequestListRunTasksPaginateTypeDef(
+    _RequiredListRunTasksRequestListRunTasksPaginateTypeDef,
+    _OptionalListRunTasksRequestListRunTasksPaginateTypeDef,
 ):
     pass
 
-ListReferenceImportJobsResponseTypeDef = TypedDict(
-    "ListReferenceImportJobsResponseTypeDef",
-    {
-        "nextToken": str,
-        "importJobs": List[ImportReferenceJobItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
+ListRunsRequestListRunsPaginateTypeDef = TypedDict(
+    "ListRunsRequestListRunsPaginateTypeDef",
     {
-        "ids": Sequence[str],
-        "filter": ListAnnotationImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "name": str,
+        "runGroupId": str,
+        "status": RunStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListAnnotationImportJobsRequestRequestTypeDef = TypedDict(
-    "ListAnnotationImportJobsRequestRequestTypeDef",
+ListWorkflowsRequestListWorkflowsPaginateTypeDef = TypedDict(
+    "ListWorkflowsRequestListWorkflowsPaginateTypeDef",
     {
-        "maxResults": int,
-        "ids": Sequence[str],
-        "nextToken": str,
-        "filter": ListAnnotationImportJobsFilterTypeDef,
+        "type": WorkflowTypeType,
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef = TypedDict(
     "ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListAnnotationStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresRequestRequestTypeDef = TypedDict(
     "ListAnnotationStoresRequestRequestTypeDef",
     {
@@ -2959,15 +3031,15 @@
 )
 
 ListMultipartReadSetUploadsResponseTypeDef = TypedDict(
     "ListMultipartReadSetUploadsResponseTypeDef",
     {
         "nextToken": str,
         "uploads": List[MultipartReadSetUploadListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
     "_RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
         "sequenceStoreId": str,
@@ -2975,15 +3047,15 @@
         "partSource": ReadSetPartSourceType,
     },
 )
 _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef = TypedDict(
     "_OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef",
     {
         "filter": ReadSetUploadPartListFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef(
     _RequiredListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
     _OptionalListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
@@ -3015,29 +3087,29 @@
     pass
 
 ListReadSetUploadPartsResponseTypeDef = TypedDict(
     "ListReadSetUploadPartsResponseTypeDef",
     {
         "nextToken": str,
         "parts": List[ReadSetUploadPartListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
     "_RequiredListReadSetsRequestListReadSetsPaginateTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetsRequestListReadSetsPaginateTypeDef = TypedDict(
     "_OptionalListReadSetsRequestListReadSetsPaginateTypeDef",
     {
         "filter": ReadSetFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListReadSetsRequestListReadSetsPaginateTypeDef(
     _RequiredListReadSetsRequestListReadSetsPaginateTypeDef,
     _OptionalListReadSetsRequestListReadSetsPaginateTypeDef,
@@ -3065,15 +3137,15 @@
 ):
     pass
 
 ListReferenceStoresRequestListReferenceStoresPaginateTypeDef = TypedDict(
     "ListReferenceStoresRequestListReferenceStoresPaginateTypeDef",
     {
         "filter": ReferenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListReferenceStoresRequestRequestTypeDef = TypedDict(
     "ListReferenceStoresRequestRequestTypeDef",
     {
@@ -3090,15 +3162,15 @@
         "referenceStoreId": str,
     },
 )
 _OptionalListReferencesRequestListReferencesPaginateTypeDef = TypedDict(
     "_OptionalListReferencesRequestListReferencesPaginateTypeDef",
     {
         "filter": ReferenceFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListReferencesRequestListReferencesPaginateTypeDef(
     _RequiredListReferencesRequestListReferencesPaginateTypeDef,
     _OptionalListReferencesRequestListReferencesPaginateTypeDef,
@@ -3127,50 +3199,50 @@
     pass
 
 ListReferencesResponseTypeDef = TypedDict(
     "ListReferencesResponseTypeDef",
     {
         "nextToken": str,
         "references": List[ReferenceListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunGroupsResponseTypeDef = TypedDict(
     "ListRunGroupsResponseTypeDef",
     {
         "items": List[RunGroupListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunTasksResponseTypeDef = TypedDict(
     "ListRunTasksResponseTypeDef",
     {
         "items": List[TaskListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRunsResponseTypeDef = TypedDict(
     "ListRunsResponseTypeDef",
     {
         "items": List[RunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresRequestListSequenceStoresPaginateTypeDef = TypedDict(
     "ListSequenceStoresRequestListSequenceStoresPaginateTypeDef",
     {
         "filter": SequenceStoreFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListSequenceStoresRequestRequestTypeDef = TypedDict(
     "ListSequenceStoresRequestRequestTypeDef",
     {
@@ -3182,15 +3254,15 @@
 )
 
 ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef = TypedDict(
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantImportJobsFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantImportJobsRequestRequestTypeDef = TypedDict(
     "ListVariantImportJobsRequestRequestTypeDef",
     {
@@ -3203,24 +3275,24 @@
 )
 
 ListVariantImportJobsResponseTypeDef = TypedDict(
     "ListVariantImportJobsResponseTypeDef",
     {
         "variantImportJobs": List[VariantImportJobItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresRequestListVariantStoresPaginateTypeDef = TypedDict(
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     {
         "ids": Sequence[str],
         "filter": ListVariantStoresFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListVariantStoresRequestRequestTypeDef = TypedDict(
     "ListVariantStoresRequestRequestTypeDef",
     {
@@ -3233,26 +3305,60 @@
 )
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TsvOptionsOutputTypeDef = TypedDict(
+    "TsvOptionsOutputTypeDef",
+    {
+        "readOptions": ReadOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 TsvOptionsTypeDef = TypedDict(
     "TsvOptionsTypeDef",
     {
         "readOptions": ReadOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+    {
+        "sourceFiles": SourceFilesTypeDef,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "referenceArn": str,
+    },
+)
+_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+    {
+        "generatedFrom": str,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartReadSetImportJobSourceItemTypeDef(
+    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+):
+    pass
+
 _RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
@@ -3311,55 +3417,63 @@
 
 class StartVariantImportRequestRequestTypeDef(
     _RequiredStartVariantImportRequestRequestTypeDef,
     _OptionalStartVariantImportRequestRequestTypeDef,
 ):
     pass
 
+StoreOptionsOutputTypeDef = TypedDict(
+    "StoreOptionsOutputTypeDef",
+    {
+        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 StoreOptionsTypeDef = TypedDict(
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
 
 ListAnnotationStoresResponseTypeDef = TypedDict(
     "ListAnnotationStoresResponseTypeDef",
     {
         "annotationStores": List[AnnotationStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReferenceStoresResponseTypeDef = TypedDict(
     "ListReferenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "referenceStores": List[ReferenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSequenceStoresResponseTypeDef = TypedDict(
     "ListSequenceStoresResponseTypeDef",
     {
         "nextToken": str,
         "sequenceStores": List[SequenceStoreDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVariantStoresResponseTypeDef = TypedDict(
     "ListVariantStoresResponseTypeDef",
     {
         "variantStores": List[VariantStoreItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetMetadataResponseTypeDef = TypedDict(
     "GetReadSetMetadataResponseTypeDef",
     {
         "id": str,
@@ -3372,15 +3486,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
         "id": str,
@@ -3389,165 +3503,174 @@
         "md5": str,
         "status": ReferenceStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "files": ReferenceFilesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReadSetsResponseTypeDef = TypedDict(
     "ListReadSetsResponseTypeDef",
     {
         "nextToken": str,
         "readSets": List[ReadSetListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReadSetImportJobResponseTypeDef = TypedDict(
     "GetReadSetImportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "roleArn": str,
         "status": ReadSetImportJobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobRequestRequestTypeDef",
+FormatOptionsOutputTypeDef = TypedDict(
+    "FormatOptionsOutputTypeDef",
     {
-        "sequenceStoreId": str,
-        "roleArn": str,
-        "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
-    },
-)
-_OptionalStartReadSetImportJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobRequestRequestTypeDef",
-    {
-        "clientToken": str,
+        "tsvOptions": TsvOptionsOutputTypeDef,
+        "vcfOptions": VcfOptionsOutputTypeDef,
     },
     total=False,
 )
 
-class StartReadSetImportJobRequestRequestTypeDef(
-    _RequiredStartReadSetImportJobRequestRequestTypeDef,
-    _OptionalStartReadSetImportJobRequestRequestTypeDef,
-):
-    pass
-
 FormatOptionsTypeDef = TypedDict(
     "FormatOptionsTypeDef",
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+_RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
-        "storeFormat": StoreFormatType,
+        "sequenceStoreId": str,
+        "roleArn": str,
+        "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
     },
 )
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+_OptionalStartReadSetImportJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobRequestRequestTypeDef",
     {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
+        "clientToken": str,
     },
     total=False,
 )
 
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+class StartReadSetImportJobRequestRequestTypeDef(
+    _RequiredStartReadSetImportJobRequestRequestTypeDef,
+    _OptionalStartReadSetImportJobRequestRequestTypeDef,
 ):
     pass
 
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigTypeDef,
+        "sseConfig": SseConfigOutputTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemTypeDef,
+        "reference": ReferenceItemOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsTypeDef,
+        "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "storeFormat": StoreFormatType,
+    },
+)
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
+
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
-        "formatOptions": FormatOptionsTypeDef,
+        "formatOptions": FormatOptionsOutputTypeDef,
         "annotationFields": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
     {
         "destinationName": str,
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.0
-Summary: Type annotations for boto3.Omics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-omics"></a>
 
 # mypy-boto3-omics
 
 [![PyPI - mypy-boto3-omics](https://img.shields.io/pypi/v/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-omics?color=blue)](https://pypistats.org/packages/mypy-boto3-omics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,155 +514,154 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
+    ReferenceItemOutputTypeDef,
+    SseConfigOutputTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
+    ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    CompleteMultipartReadSetUploadResponseTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
-    CreateMultipartReadSetUploadResponseTypeDef,
     CreateRunGroupRequestRequestTypeDef,
-    CreateRunGroupResponseTypeDef,
     WorkflowParameterTypeDef,
-    CreateWorkflowResponseTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
-    DeleteAnnotationStoreResponseTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
     DeleteRunRequestRequestTypeDef,
     DeleteSequenceStoreRequestRequestTypeDef,
     DeleteVariantStoreRequestRequestTypeDef,
-    DeleteVariantStoreResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
+    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
     GetReadSetMetadataRequestRequestTypeDef,
     SequenceInformationTypeDef,
     GetReadSetRequestRequestTypeDef,
-    GetReadSetResponseTypeDef,
     GetReferenceImportJobRequestRequestTypeDef,
     ImportReferenceSourceItemTypeDef,
     GetReferenceMetadataRequestRequestTypeDef,
     GetReferenceRequestRequestTypeDef,
-    GetReferenceResponseTypeDef,
     GetReferenceStoreRequestRequestTypeDef,
     GetRunGroupRequestRequestTypeDef,
-    GetRunGroupResponseTypeDef,
     GetRunRequestRequestTypeDef,
-    GetRunResponseTypeDef,
     GetRunTaskRequestRequestTypeDef,
-    GetRunTaskResponseTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
+    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesTypeDef,
+    SourceFilesOutputTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
+    PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
-    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
     ReadSetUploadPartListFilterTypeDef,
     ReadSetUploadPartListItemTypeDef,
     ReadSetFilterTypeDef,
     ReferenceStoreFilterTypeDef,
     ReferenceFilterTypeDef,
     ReferenceListItemTypeDef,
-    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
     ListRunGroupsRequestRequestTypeDef,
     RunGroupListItemTypeDef,
-    ListRunTasksRequestListRunTasksPaginateTypeDef,
     ListRunTasksRequestRequestTypeDef,
     TaskListItemTypeDef,
-    ListRunsRequestListRunsPaginateTypeDef,
     ListRunsRequestRequestTypeDef,
     RunListItemTypeDef,
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
-    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    PaginatorConfigTypeDef,
+    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    StartAnnotationImportResponseTypeDef,
+    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
-    StartReadSetActivationJobResponseTypeDef,
-    StartReadSetExportJobResponseTypeDef,
-    StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
-    StartReferenceImportJobResponseTypeDef,
     StartRunRequestRequestTypeDef,
-    StartRunResponseTypeDef,
     VariantImportItemSourceTypeDef,
-    StartVariantImportResponseTypeDef,
+    TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
-    UploadReadSetPartResponseTypeDef,
-    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
-    ListReadSetActivationJobsResponseTypeDef,
-    GetReadSetActivationJobResponseTypeDef,
-    ListAnnotationImportJobsResponseTypeDef,
-    CreateVariantStoreResponseTypeDef,
-    UpdateVariantStoreResponseTypeDef,
     AnnotationStoreItemTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
+    ReferenceStoreDetailTypeDef,
+    SequenceStoreDetailTypeDef,
+    VariantStoreItemTypeDef,
+    BatchDeleteReadSetResponseTypeDef,
+    CompleteMultipartReadSetUploadResponseTypeDef,
+    CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
+    CreateRunGroupResponseTypeDef,
     CreateSequenceStoreResponseTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
+    CreateVariantStoreResponseTypeDef,
+    CreateWorkflowResponseTypeDef,
+    DeleteAnnotationStoreResponseTypeDef,
+    DeleteVariantStoreResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetReadSetActivationJobResponseTypeDef,
+    GetReadSetResponseTypeDef,
+    GetReferenceResponseTypeDef,
     GetReferenceStoreResponseTypeDef,
+    GetRunGroupResponseTypeDef,
+    GetRunResponseTypeDef,
+    GetRunTaskResponseTypeDef,
     GetSequenceStoreResponseTypeDef,
     GetVariantStoreResponseTypeDef,
-    ReferenceStoreDetailTypeDef,
-    SequenceStoreDetailTypeDef,
-    VariantStoreItemTypeDef,
-    BatchDeleteReadSetResponseTypeDef,
+    ListAnnotationImportJobsResponseTypeDef,
+    ListReadSetActivationJobsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartAnnotationImportResponseTypeDef,
+    StartReadSetActivationJobResponseTypeDef,
+    StartReadSetExportJobResponseTypeDef,
+    StartReadSetImportJobResponseTypeDef,
+    StartReferenceImportJobResponseTypeDef,
+    StartRunResponseTypeDef,
+    StartVariantImportResponseTypeDef,
+    UpdateVariantStoreResponseTypeDef,
+    UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
-    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
-    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
     GetAnnotationStoreRequestAnnotationStoreCreatedWaitTypeDef,
@@ -678,24 +677,31 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
-    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
-    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
+    ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
+    ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
+    ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
+    ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
+    ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef,
+    ListReferenceImportJobsRequestListReferenceImportJobsPaginateTypeDef,
+    ListRunGroupsRequestListRunGroupsPaginateTypeDef,
+    ListRunTasksRequestListRunTasksPaginateTypeDef,
+    ListRunsRequestListRunsPaginateTypeDef,
+    ListWorkflowsRequestListWorkflowsPaginateTypeDef,
     ListAnnotationStoresRequestListAnnotationStoresPaginateTypeDef,
     ListAnnotationStoresRequestRequestTypeDef,
     ListMultipartReadSetUploadsResponseTypeDef,
     ListReadSetUploadPartsRequestListReadSetUploadPartsPaginateTypeDef,
     ListReadSetUploadPartsRequestRequestTypeDef,
     ListReadSetUploadPartsResponseTypeDef,
     ListReadSetsRequestListReadSetsPaginateTypeDef,
@@ -712,33 +718,37 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
+    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
+    StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsOutputTypeDef,
     FormatOptionsTypeDef,
-    CreateAnnotationStoreRequestRequestTypeDef,
+    StartReadSetImportJobRequestRequestTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
+    CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
 
 
 def get_structure() -> AbortMultipartReadSetUploadRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-omics-1.28.0/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.0/setup.py` & `mypy-boto3-omics-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

