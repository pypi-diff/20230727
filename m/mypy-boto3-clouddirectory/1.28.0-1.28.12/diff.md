# Comparing `tmp/mypy-boto3-clouddirectory-1.28.0.tar.gz` & `tmp/mypy-boto3-clouddirectory-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-clouddirectory-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-clouddirectory-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
```

## Comparing `mypy-boto3-clouddirectory-1.28.0.tar` & `mypy-boto3-clouddirectory-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.058243 mypy-boto3-clouddirectory-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25871 2023-07-06 20:59:09.054243 mypy-boto3-clouddirectory-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24358 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.046243 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-06 20:35:01.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-06 20:35:01.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-06 20:35:01.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-07-06 20:35:01.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-06 20:35:01.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86497 2023-07-06 20:35:04.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86370 2023-07-06 20:35:03.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.054243 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25871 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:59:08.000000 mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.058243 mypy-boto3-clouddirectory-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:35:00.000000 mypy-boto3-clouddirectory-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.000563 mypy-boto3-clouddirectory-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56752 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56660 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-07-27 05:18:28.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-27 05:18:28.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24367 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    91171 2023-07-27 05:18:30.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91038 2023-07-27 05:18:29.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.992563 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26363 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:24.000000 mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.000563 mypy-boto3-clouddirectory-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:18:27.000000 mypy-boto3-clouddirectory-1.28.12/setup.py
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/LICENSE` & `mypy-boto3-clouddirectory-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudDirectory 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudDirectory 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,22 +423,25 @@
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
+    AttributeKeyOutputTypeDef,
+    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
+    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
@@ -458,15 +461,17 @@
     DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
     EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
@@ -493,27 +498,30 @@
     ListObjectPoliciesResponseTypeDef,
     ListPolicyAttachmentsResponseTypeDef,
     ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
     ListPublishedSchemaArnsResponseTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     ListTypedLinkFacetNamesResponseTypeDef,
+    ObjectReferenceOutputTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
     PutSchemaFromJsonResponseTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
+    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
@@ -550,95 +558,101 @@
     ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
     ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
     ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TagResourceRequestRequestTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    CreateObjectRequestRequestTypeDef,
     AttachTypedLinkRequestRequestTypeDef,
     BatchAttachTypedLinkTypeDef,
     TypedLinkSpecifierTypeDef,
     LinkAttributeUpdateTypeDef,
     ObjectAttributeUpdateTypeDef,
     ObjectAttributeRangeTypeDef,
     TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
+    FacetAttributeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
+    ListFacetAttributesResponseTypeDef,
     CreateFacetRequestRequestTypeDef,
     FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
     BatchWriteOperationResponseTypeDef,
     BatchReadSuccessfulResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchReadOperationTypeDef,
     UpdateFacetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/README.md` & `mypy-boto3-clouddirectory-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,22 +391,25 @@
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
+    AttributeKeyOutputTypeDef,
+    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
+    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
@@ -426,15 +429,17 @@
     DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
     EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
@@ -461,27 +466,30 @@
     ListObjectPoliciesResponseTypeDef,
     ListPolicyAttachmentsResponseTypeDef,
     ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
     ListPublishedSchemaArnsResponseTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     ListTypedLinkFacetNamesResponseTypeDef,
+    ObjectReferenceOutputTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
     PutSchemaFromJsonResponseTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
+    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
@@ -518,95 +526,101 @@
     ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
     ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
     ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TagResourceRequestRequestTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    CreateObjectRequestRequestTypeDef,
     AttachTypedLinkRequestRequestTypeDef,
     BatchAttachTypedLinkTypeDef,
     TypedLinkSpecifierTypeDef,
     LinkAttributeUpdateTypeDef,
     ObjectAttributeUpdateTypeDef,
     ObjectAttributeRangeTypeDef,
     TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
+    FacetAttributeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
+    ListFacetAttributesResponseTypeDef,
     CreateFacetRequestRequestTypeDef,
     FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
     BatchWriteOperationResponseTypeDef,
     BatchReadSuccessfulResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchReadOperationTypeDef,
     UpdateFacetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__init__.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__init__.pyi` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/__main__.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudDirectory 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudDirectory 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory\nOther"
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

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/client.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/client.pyi` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/literals.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
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
@@ -302,26 +303,28 @@
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

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/literals.pyi` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/paginator.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/paginator.pyi` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/type_defs.py` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,22 +40,25 @@
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ApplySchemaResponseTypeDef",
     "AttachObjectResponseTypeDef",
     "AttachToIndexResponseTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
+    "AttributeKeyOutputTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
+    "SchemaFacetOutputTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
@@ -75,15 +78,17 @@
     "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
     "DisableDirectoryResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
     "EnableDirectoryResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "FacetAttributeReferenceOutputTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
@@ -110,27 +115,30 @@
     "ListObjectPoliciesResponseTypeDef",
     "ListPolicyAttachmentsResponseTypeDef",
     "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     "ListPublishedSchemaArnsResponseTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesResponseTypeDef",
+    "ObjectReferenceOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
     "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
     "PutSchemaFromJsonResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "TagTypeDef",
+    "TypedLinkSchemaAndFacetNameOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
@@ -167,95 +175,101 @@
     "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
     "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
-    "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "GetObjectInformationResponseTypeDef",
     "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
+    "BatchGetObjectInformationResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
+    "FacetAttributeDefinitionOutputTypeDef",
+    "TypedLinkAttributeDefinitionOutputTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
-    "CreateObjectRequestRequestTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
+    "TypedLinkSpecifierOutputTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "CreateObjectRequestRequestTypeDef",
     "AttachTypedLinkRequestRequestTypeDef",
     "BatchAttachTypedLinkTypeDef",
     "TypedLinkSpecifierTypeDef",
     "LinkAttributeUpdateTypeDef",
     "ObjectAttributeUpdateTypeDef",
     "ObjectAttributeRangeTypeDef",
     "TypedLinkAttributeRangeTypeDef",
-    "FacetAttributeTypeDef",
+    "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
+    "FacetAttributeTypeDef",
     "TypedLinkFacetAttributeUpdateTypeDef",
     "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
-    "BatchDetachTypedLinkTypeDef",
-    "BatchGetLinkAttributesTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
-    "DetachTypedLinkRequestRequestTypeDef",
-    "GetLinkAttributesRequestRequestTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "BatchDetachTypedLinkTypeDef",
+    "BatchGetLinkAttributesTypeDef",
+    "DetachTypedLinkRequestRequestTypeDef",
+    "GetLinkAttributesRequestRequestTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
+    "ListFacetAttributesResponseTypeDef",
     "CreateFacetRequestRequestTypeDef",
     "FacetAttributeUpdateTypeDef",
-    "ListFacetAttributesResponseTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
     "BatchWriteOperationResponseTypeDef",
     "BatchReadSuccessfulResponseTypeDef",
     "BatchWriteOperationTypeDef",
     "BatchReadOperationTypeDef",
     "UpdateFacetRequestRequestTypeDef",
@@ -320,14 +334,35 @@
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
         "TypedLinkName": str,
     },
 )
 
+AttributeKeyOutputTypeDef = TypedDict(
+    "AttributeKeyOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "FacetName": str,
+        "Name": str,
+    },
+)
+
+TypedAttributeValueOutputTypeDef = TypedDict(
+    "TypedAttributeValueOutputTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": bytes,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": datetime,
+    },
+    total=False,
+)
+
 AttributeKeyTypeDef = TypedDict(
     "AttributeKeyTypeDef",
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
@@ -389,14 +424,23 @@
     "BatchDetachObjectResponseTypeDef",
     {
         "detachedObjectIdentifier": str,
     },
     total=False,
 )
 
+SchemaFacetOutputTypeDef = TypedDict(
+    "SchemaFacetOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "FacetName": str,
+    },
+    total=False,
+)
+
 BatchListObjectChildrenResponseTypeDef = TypedDict(
     "BatchListObjectChildrenResponseTypeDef",
     {
         "Children": Dict[str, str],
         "NextToken": str,
     },
     total=False,
@@ -611,23 +655,40 @@
     "EnableDirectoryResponseTypeDef",
     {
         "DirectoryArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "Type": RuleTypeType,
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+FacetAttributeReferenceOutputTypeDef = TypedDict(
+    "FacetAttributeReferenceOutputTypeDef",
+    {
+        "TargetFacetName": str,
+        "TargetAttributeName": str,
+    },
+)
+
 FacetAttributeReferenceTypeDef = TypedDict(
     "FacetAttributeReferenceTypeDef",
     {
         "TargetFacetName": str,
         "TargetAttributeName": str,
     },
 )
@@ -1029,16 +1090,16 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -1139,14 +1200,22 @@
     {
         "FacetNames": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ObjectReferenceOutputTypeDef = TypedDict(
+    "ObjectReferenceOutputTypeDef",
+    {
+        "Selector": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1217,14 +1286,31 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+TypedLinkSchemaAndFacetNameOutputTypeDef = TypedDict(
+    "TypedLinkSchemaAndFacetNameOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "TypedLinkName": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1929,23 +2015,14 @@
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
-BatchGetObjectInformationResponseTypeDef = TypedDict(
-    "BatchGetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
 _RequiredBatchListObjectAttributesTypeDef = TypedDict(
     "_RequiredBatchListObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectAttributesTypeDef = TypedDict(
@@ -1994,23 +2071,14 @@
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -2063,14 +2131,30 @@
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
+    {
+        "Key": AttributeKeyOutputTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
 )
@@ -2166,14 +2250,32 @@
 
 class TypedAttributeValueRangeTypeDef(
     _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
 
+BatchGetObjectInformationResponseTypeDef = TypedDict(
+    "BatchGetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetOutputTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetOutputTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -2220,14 +2322,63 @@
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionOutputTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionOutputTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
+        "IsImmutable": bool,
+        "Rules": Dict[str, RuleOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class FacetAttributeDefinitionOutputTypeDef(
+    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
+):
+    pass
+
+
+_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+)
+_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
+        "IsImmutable": bool,
+        "Rules": Dict[str, RuleOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class TypedLinkAttributeDefinitionOutputTypeDef(
+    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
+    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
+):
+    pass
+
+
 _RequiredFacetAttributeDefinitionTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionTypeDef",
     {
         "Type": FacetAttributeTypeType,
     },
 )
 _OptionalFacetAttributeDefinitionTypeDef = TypedDict(
@@ -2279,37 +2430,106 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
 
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+GetLinkAttributesResponseTypeDef = TypedDict(
+    "GetLinkAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetObjectAttributesResponseTypeDef = TypedDict(
+    "GetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+IndexAttachmentTypeDef = TypedDict(
+    "IndexAttachmentTypeDef",
+    {
+        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
+ListObjectAttributesResponseTypeDef = TypedDict(
+    "ListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TypedLinkSpecifierOutputTypeDef = TypedDict(
+    "TypedLinkSpecifierOutputTypeDef",
+    {
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameOutputTypeDef,
+        "SourceObjectReference": ObjectReferenceOutputTypeDef,
+        "TargetObjectReference": ObjectReferenceOutputTypeDef,
+        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
+    },
+)
+
 _RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -2358,39 +2578,14 @@
 
 class BatchCreateObjectTypeDef(
     _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
 ):
     pass
 
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-    },
-    total=False,
-)
-
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-    },
-    total=False,
-)
-
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
 _RequiredCreateObjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
@@ -2407,48 +2602,14 @@
 
 class CreateObjectRequestRequestTypeDef(
     _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
 ):
     pass
 
 
-GetLinkAttributesResponseTypeDef = TypedDict(
-    "GetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetObjectAttributesResponseTypeDef = TypedDict(
-    "GetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IndexAttachmentTypeDef = TypedDict(
-    "IndexAttachmentTypeDef",
-    {
-        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-ListObjectAttributesResponseTypeDef = TypedDict(
-    "ListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
@@ -2468,15 +2629,15 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
     },
 )
 
 LinkAttributeUpdateTypeDef = TypedDict(
     "LinkAttributeUpdateTypeDef",
     {
         "AttributeKey": AttributeKeyTypeDef,
@@ -2520,44 +2681,67 @@
 
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
 
-_RequiredFacetAttributeTypeDef = TypedDict(
-    "_RequiredFacetAttributeTypeDef",
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalFacetAttributeTypeDef = TypedDict(
-    "_OptionalFacetAttributeTypeDef",
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
     {
-        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceOutputTypeDef,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
 
-class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+):
     pass
 
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
-        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFacetAttributeTypeDef = TypedDict(
+    "_RequiredFacetAttributeTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeTypeDef = TypedDict(
+    "_OptionalFacetAttributeTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+    total=False,
+)
+
+
+class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+    pass
+
+
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
 )
@@ -2624,58 +2808,76 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
     },
     total=False,
 )
 
-BatchDetachTypedLinkTypeDef = TypedDict(
-    "BatchDetachTypedLinkTypeDef",
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-BatchGetLinkAttributesTypeDef = TypedDict(
-    "BatchGetLinkAttributesTypeDef",
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "AttributeNames": Sequence[str],
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchDetachTypedLinkTypeDef = TypedDict(
+    "BatchDetachTypedLinkTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+    },
+)
+
+BatchGetLinkAttributesTypeDef = TypedDict(
+    "BatchGetLinkAttributesTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "AttributeNames": Sequence[str],
     },
-    total=False,
 )
 
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2701,32 +2903,14 @@
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
 
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
-    {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -2978,14 +3162,23 @@
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
 
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -3011,23 +3204,14 @@
     {
         "Attribute": FacetAttributeTypeDef,
         "Action": UpdateActionTypeType,
     },
     total=False,
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[FacetAttributeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
         "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
         "IdentityAttributeOrder": Sequence[str],
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory/type_defs.pyi` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -39,22 +39,25 @@
     "ObjectReferenceTypeDef",
     "SchemaFacetTypeDef",
     "ApplySchemaRequestRequestTypeDef",
     "ApplySchemaResponseTypeDef",
     "AttachObjectResponseTypeDef",
     "AttachToIndexResponseTypeDef",
     "TypedLinkSchemaAndFacetNameTypeDef",
+    "AttributeKeyOutputTypeDef",
+    "TypedAttributeValueOutputTypeDef",
     "AttributeKeyTypeDef",
     "TypedAttributeValueTypeDef",
     "BatchAttachObjectResponseTypeDef",
     "BatchAttachToIndexResponseTypeDef",
     "BatchCreateIndexResponseTypeDef",
     "BatchCreateObjectResponseTypeDef",
     "BatchDetachFromIndexResponseTypeDef",
     "BatchDetachObjectResponseTypeDef",
+    "SchemaFacetOutputTypeDef",
     "BatchListObjectChildrenResponseTypeDef",
     "PathToObjectIdentifiersTypeDef",
     "ObjectIdentifierAndLinkNameTupleTypeDef",
     "BatchListObjectPoliciesResponseTypeDef",
     "BatchListPolicyAttachmentsResponseTypeDef",
     "BatchReadExceptionTypeDef",
     "BatchUpdateObjectAttributesResponseTypeDef",
@@ -74,15 +77,17 @@
     "DetachObjectResponseTypeDef",
     "DirectoryTypeDef",
     "DisableDirectoryRequestRequestTypeDef",
     "DisableDirectoryResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableDirectoryRequestRequestTypeDef",
     "EnableDirectoryResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
+    "FacetAttributeReferenceOutputTypeDef",
     "FacetAttributeReferenceTypeDef",
     "FacetTypeDef",
     "GetAppliedSchemaVersionRequestRequestTypeDef",
     "GetAppliedSchemaVersionResponseTypeDef",
     "GetDirectoryRequestRequestTypeDef",
     "GetFacetRequestRequestTypeDef",
     "GetSchemaAsJsonRequestRequestTypeDef",
@@ -109,27 +114,30 @@
     "ListObjectPoliciesResponseTypeDef",
     "ListPolicyAttachmentsResponseTypeDef",
     "ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef",
     "ListPublishedSchemaArnsRequestRequestTypeDef",
     "ListPublishedSchemaArnsResponseTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef",
     "ListTypedLinkFacetAttributesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef",
     "ListTypedLinkFacetNamesRequestRequestTypeDef",
     "ListTypedLinkFacetNamesResponseTypeDef",
+    "ObjectReferenceOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PolicyAttachmentTypeDef",
     "PublishSchemaRequestRequestTypeDef",
     "PublishSchemaResponseTypeDef",
     "PutSchemaFromJsonRequestRequestTypeDef",
     "PutSchemaFromJsonResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "TagTypeDef",
+    "TypedLinkSchemaAndFacetNameOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateObjectAttributesResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
     "UpdateSchemaResponseTypeDef",
     "UpgradeAppliedSchemaRequestRequestTypeDef",
     "UpgradeAppliedSchemaResponseTypeDef",
     "UpgradePublishedSchemaRequestRequestTypeDef",
@@ -166,95 +174,101 @@
     "ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef",
     "ListObjectPoliciesRequestRequestTypeDef",
     "ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef",
     "ListPolicyAttachmentsRequestRequestTypeDef",
     "LookupPolicyRequestLookupPolicyPaginateTypeDef",
     "LookupPolicyRequestRequestTypeDef",
     "BatchGetObjectAttributesTypeDef",
-    "BatchGetObjectInformationResponseTypeDef",
     "BatchListObjectAttributesTypeDef",
     "BatchRemoveFacetFromObjectTypeDef",
     "GetObjectAttributesRequestRequestTypeDef",
-    "GetObjectInformationResponseTypeDef",
     "ListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     "ListObjectAttributesRequestRequestTypeDef",
     "RemoveFacetFromObjectRequestRequestTypeDef",
+    "AttributeKeyAndValueOutputTypeDef",
+    "AttributeNameAndValueOutputTypeDef",
     "BatchCreateIndexTypeDef",
     "CreateIndexRequestRequestTypeDef",
     "AttributeKeyAndValueTypeDef",
     "AttributeNameAndValueTypeDef",
     "LinkAttributeActionTypeDef",
     "ObjectAttributeActionTypeDef",
     "TypedAttributeValueRangeTypeDef",
+    "BatchGetObjectInformationResponseTypeDef",
+    "GetObjectInformationResponseTypeDef",
     "BatchListObjectParentPathsResponseTypeDef",
     "ListObjectParentPathsResponseTypeDef",
     "BatchListObjectParentsResponseTypeDef",
     "ListObjectParentsResponseTypeDef",
     "GetDirectoryResponseTypeDef",
     "ListDirectoriesResponseTypeDef",
+    "FacetAttributeDefinitionOutputTypeDef",
+    "TypedLinkAttributeDefinitionOutputTypeDef",
     "FacetAttributeDefinitionTypeDef",
     "TypedLinkAttributeDefinitionTypeDef",
     "GetFacetResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "PolicyToPathTypeDef",
-    "AddFacetToObjectRequestRequestTypeDef",
-    "BatchAddFacetToObjectTypeDef",
-    "BatchCreateObjectTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "BatchGetLinkAttributesResponseTypeDef",
     "BatchGetObjectAttributesResponseTypeDef",
     "BatchListObjectAttributesResponseTypeDef",
-    "CreateObjectRequestRequestTypeDef",
     "GetLinkAttributesResponseTypeDef",
     "GetObjectAttributesResponseTypeDef",
     "IndexAttachmentTypeDef",
     "ListObjectAttributesResponseTypeDef",
+    "TypedLinkSpecifierOutputTypeDef",
+    "AddFacetToObjectRequestRequestTypeDef",
+    "BatchAddFacetToObjectTypeDef",
+    "BatchCreateObjectTypeDef",
+    "CreateObjectRequestRequestTypeDef",
     "AttachTypedLinkRequestRequestTypeDef",
     "BatchAttachTypedLinkTypeDef",
     "TypedLinkSpecifierTypeDef",
     "LinkAttributeUpdateTypeDef",
     "ObjectAttributeUpdateTypeDef",
     "ObjectAttributeRangeTypeDef",
     "TypedLinkAttributeRangeTypeDef",
-    "FacetAttributeTypeDef",
+    "FacetAttributeOutputTypeDef",
     "ListTypedLinkFacetAttributesResponseTypeDef",
+    "FacetAttributeTypeDef",
     "TypedLinkFacetAttributeUpdateTypeDef",
     "TypedLinkFacetTypeDef",
     "BatchLookupPolicyResponseTypeDef",
     "LookupPolicyResponseTypeDef",
     "BatchListAttachedIndicesResponseTypeDef",
     "BatchListIndexResponseTypeDef",
     "ListAttachedIndicesResponseTypeDef",
     "ListIndexResponseTypeDef",
     "AttachTypedLinkResponseTypeDef",
     "BatchAttachTypedLinkResponseTypeDef",
-    "BatchDetachTypedLinkTypeDef",
-    "BatchGetLinkAttributesTypeDef",
     "BatchListIncomingTypedLinksResponseTypeDef",
     "BatchListOutgoingTypedLinksResponseTypeDef",
-    "DetachTypedLinkRequestRequestTypeDef",
-    "GetLinkAttributesRequestRequestTypeDef",
     "ListIncomingTypedLinksResponseTypeDef",
     "ListOutgoingTypedLinksResponseTypeDef",
+    "BatchDetachTypedLinkTypeDef",
+    "BatchGetLinkAttributesTypeDef",
+    "DetachTypedLinkRequestRequestTypeDef",
+    "GetLinkAttributesRequestRequestTypeDef",
     "BatchUpdateLinkAttributesTypeDef",
     "UpdateLinkAttributesRequestRequestTypeDef",
     "BatchUpdateObjectAttributesTypeDef",
     "UpdateObjectAttributesRequestRequestTypeDef",
     "BatchListIndexTypeDef",
     "ListIndexRequestListIndexPaginateTypeDef",
     "ListIndexRequestRequestTypeDef",
     "BatchListIncomingTypedLinksTypeDef",
     "BatchListOutgoingTypedLinksTypeDef",
     "ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef",
     "ListIncomingTypedLinksRequestRequestTypeDef",
     "ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef",
     "ListOutgoingTypedLinksRequestRequestTypeDef",
+    "ListFacetAttributesResponseTypeDef",
     "CreateFacetRequestRequestTypeDef",
     "FacetAttributeUpdateTypeDef",
-    "ListFacetAttributesResponseTypeDef",
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     "CreateTypedLinkFacetRequestRequestTypeDef",
     "BatchWriteOperationResponseTypeDef",
     "BatchReadSuccessfulResponseTypeDef",
     "BatchWriteOperationTypeDef",
     "BatchReadOperationTypeDef",
     "UpdateFacetRequestRequestTypeDef",
@@ -319,14 +333,35 @@
     "TypedLinkSchemaAndFacetNameTypeDef",
     {
         "SchemaArn": str,
         "TypedLinkName": str,
     },
 )
 
+AttributeKeyOutputTypeDef = TypedDict(
+    "AttributeKeyOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "FacetName": str,
+        "Name": str,
+    },
+)
+
+TypedAttributeValueOutputTypeDef = TypedDict(
+    "TypedAttributeValueOutputTypeDef",
+    {
+        "StringValue": str,
+        "BinaryValue": bytes,
+        "BooleanValue": bool,
+        "NumberValue": str,
+        "DatetimeValue": datetime,
+    },
+    total=False,
+)
+
 AttributeKeyTypeDef = TypedDict(
     "AttributeKeyTypeDef",
     {
         "SchemaArn": str,
         "FacetName": str,
         "Name": str,
     },
@@ -388,14 +423,23 @@
     "BatchDetachObjectResponseTypeDef",
     {
         "detachedObjectIdentifier": str,
     },
     total=False,
 )
 
+SchemaFacetOutputTypeDef = TypedDict(
+    "SchemaFacetOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "FacetName": str,
+    },
+    total=False,
+)
+
 BatchListObjectChildrenResponseTypeDef = TypedDict(
     "BatchListObjectChildrenResponseTypeDef",
     {
         "Children": Dict[str, str],
         "NextToken": str,
     },
     total=False,
@@ -610,23 +654,40 @@
     "EnableDirectoryResponseTypeDef",
     {
         "DirectoryArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "Type": RuleTypeType,
+        "Parameters": Dict[str, str],
+    },
+    total=False,
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "Type": RuleTypeType,
         "Parameters": Mapping[str, str],
     },
     total=False,
 )
 
+FacetAttributeReferenceOutputTypeDef = TypedDict(
+    "FacetAttributeReferenceOutputTypeDef",
+    {
+        "TargetFacetName": str,
+        "TargetAttributeName": str,
+    },
+)
+
 FacetAttributeReferenceTypeDef = TypedDict(
     "FacetAttributeReferenceTypeDef",
     {
         "TargetFacetName": str,
         "TargetAttributeName": str,
     },
 )
@@ -1012,16 +1073,16 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -1114,14 +1175,22 @@
     {
         "FacetNames": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ObjectReferenceOutputTypeDef = TypedDict(
+    "ObjectReferenceOutputTypeDef",
+    {
+        "Selector": str,
+    },
+    total=False,
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -1190,14 +1259,31 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+TagTypeDef = TypedDict(
+    "TagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
+TypedLinkSchemaAndFacetNameOutputTypeDef = TypedDict(
+    "TypedLinkSchemaAndFacetNameOutputTypeDef",
+    {
+        "SchemaArn": str,
+        "TypedLinkName": str,
+    },
+)
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1856,23 +1942,14 @@
     {
         "ObjectReference": ObjectReferenceTypeDef,
         "SchemaFacet": SchemaFacetTypeDef,
         "AttributeNames": Sequence[str],
     },
 )
 
-BatchGetObjectInformationResponseTypeDef = TypedDict(
-    "BatchGetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
 _RequiredBatchListObjectAttributesTypeDef = TypedDict(
     "_RequiredBatchListObjectAttributesTypeDef",
     {
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 _OptionalBatchListObjectAttributesTypeDef = TypedDict(
@@ -1917,23 +1994,14 @@
 
 class GetObjectAttributesRequestRequestTypeDef(
     _RequiredGetObjectAttributesRequestRequestTypeDef,
     _OptionalGetObjectAttributesRequestRequestTypeDef,
 ):
     pass
 
-GetObjectInformationResponseTypeDef = TypedDict(
-    "GetObjectInformationResponseTypeDef",
-    {
-        "SchemaFacets": List[SchemaFacetTypeDef],
-        "ObjectIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef = TypedDict(
     "_RequiredListObjectAttributesRequestListObjectAttributesPaginateTypeDef",
     {
         "DirectoryArn": str,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
@@ -1982,14 +2050,30 @@
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
 )
 
+AttributeKeyAndValueOutputTypeDef = TypedDict(
+    "AttributeKeyAndValueOutputTypeDef",
+    {
+        "Key": AttributeKeyOutputTypeDef,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
+AttributeNameAndValueOutputTypeDef = TypedDict(
+    "AttributeNameAndValueOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Value": TypedAttributeValueOutputTypeDef,
+    },
+)
+
 _RequiredBatchCreateIndexTypeDef = TypedDict(
     "_RequiredBatchCreateIndexTypeDef",
     {
         "OrderedIndexedAttributeList": Sequence[AttributeKeyTypeDef],
         "IsUnique": bool,
     },
 )
@@ -2079,14 +2163,32 @@
 )
 
 class TypedAttributeValueRangeTypeDef(
     _RequiredTypedAttributeValueRangeTypeDef, _OptionalTypedAttributeValueRangeTypeDef
 ):
     pass
 
+BatchGetObjectInformationResponseTypeDef = TypedDict(
+    "BatchGetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetOutputTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
+GetObjectInformationResponseTypeDef = TypedDict(
+    "GetObjectInformationResponseTypeDef",
+    {
+        "SchemaFacets": List[SchemaFacetOutputTypeDef],
+        "ObjectIdentifier": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 BatchListObjectParentPathsResponseTypeDef = TypedDict(
     "BatchListObjectParentPathsResponseTypeDef",
     {
         "PathToObjectIdentifiersList": List[PathToObjectIdentifiersTypeDef],
         "NextToken": str,
     },
     total=False,
@@ -2133,14 +2235,59 @@
     {
         "Directories": List[DirectoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeDefinitionOutputTypeDef",
+    {
+        "Type": FacetAttributeTypeType,
+    },
+)
+_OptionalFacetAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeDefinitionOutputTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
+        "IsImmutable": bool,
+        "Rules": Dict[str, RuleOutputTypeDef],
+    },
+    total=False,
+)
+
+class FacetAttributeDefinitionOutputTypeDef(
+    _RequiredFacetAttributeDefinitionOutputTypeDef, _OptionalFacetAttributeDefinitionOutputTypeDef
+):
+    pass
+
+_RequiredTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_RequiredTypedLinkAttributeDefinitionOutputTypeDef",
+    {
+        "Name": str,
+        "Type": FacetAttributeTypeType,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+)
+_OptionalTypedLinkAttributeDefinitionOutputTypeDef = TypedDict(
+    "_OptionalTypedLinkAttributeDefinitionOutputTypeDef",
+    {
+        "DefaultValue": TypedAttributeValueOutputTypeDef,
+        "IsImmutable": bool,
+        "Rules": Dict[str, RuleOutputTypeDef],
+    },
+    total=False,
+)
+
+class TypedLinkAttributeDefinitionOutputTypeDef(
+    _RequiredTypedLinkAttributeDefinitionOutputTypeDef,
+    _OptionalTypedLinkAttributeDefinitionOutputTypeDef,
+):
+    pass
+
 _RequiredFacetAttributeDefinitionTypeDef = TypedDict(
     "_RequiredFacetAttributeDefinitionTypeDef",
     {
         "Type": FacetAttributeTypeType,
     },
 )
 _OptionalFacetAttributeDefinitionTypeDef = TypedDict(
@@ -2188,37 +2335,106 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PolicyToPathTypeDef = TypedDict(
+    "PolicyToPathTypeDef",
+    {
+        "Path": str,
+        "Policies": List[PolicyAttachmentTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-PolicyToPathTypeDef = TypedDict(
-    "PolicyToPathTypeDef",
+BatchGetLinkAttributesResponseTypeDef = TypedDict(
+    "BatchGetLinkAttributesResponseTypeDef",
     {
-        "Path": str,
-        "Policies": List[PolicyAttachmentTypeDef],
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+    },
+    total=False,
+)
+
+BatchGetObjectAttributesResponseTypeDef = TypedDict(
+    "BatchGetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
     },
     total=False,
 )
 
+BatchListObjectAttributesResponseTypeDef = TypedDict(
+    "BatchListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+GetLinkAttributesResponseTypeDef = TypedDict(
+    "GetLinkAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetObjectAttributesResponseTypeDef = TypedDict(
+    "GetObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+IndexAttachmentTypeDef = TypedDict(
+    "IndexAttachmentTypeDef",
+    {
+        "IndexedAttributes": List[AttributeKeyAndValueOutputTypeDef],
+        "ObjectIdentifier": str,
+    },
+    total=False,
+)
+
+ListObjectAttributesResponseTypeDef = TypedDict(
+    "ListObjectAttributesResponseTypeDef",
+    {
+        "Attributes": List[AttributeKeyAndValueOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+TypedLinkSpecifierOutputTypeDef = TypedDict(
+    "TypedLinkSpecifierOutputTypeDef",
+    {
+        "TypedLinkFacet": TypedLinkSchemaAndFacetNameOutputTypeDef,
+        "SourceObjectReference": ObjectReferenceOutputTypeDef,
+        "TargetObjectReference": ObjectReferenceOutputTypeDef,
+        "IdentityAttributeValues": List[AttributeNameAndValueOutputTypeDef],
+    },
+)
+
 _RequiredAddFacetToObjectRequestRequestTypeDef = TypedDict(
     "_RequiredAddFacetToObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SchemaFacet": SchemaFacetTypeDef,
         "ObjectReference": ObjectReferenceTypeDef,
     },
@@ -2263,39 +2479,14 @@
 )
 
 class BatchCreateObjectTypeDef(
     _RequiredBatchCreateObjectTypeDef, _OptionalBatchCreateObjectTypeDef
 ):
     pass
 
-BatchGetLinkAttributesResponseTypeDef = TypedDict(
-    "BatchGetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-    },
-    total=False,
-)
-
-BatchGetObjectAttributesResponseTypeDef = TypedDict(
-    "BatchGetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-    },
-    total=False,
-)
-
-BatchListObjectAttributesResponseTypeDef = TypedDict(
-    "BatchListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
-    },
-    total=False,
-)
-
 _RequiredCreateObjectRequestRequestTypeDef = TypedDict(
     "_RequiredCreateObjectRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SchemaFacets": Sequence[SchemaFacetTypeDef],
     },
 )
@@ -2310,48 +2501,14 @@
 )
 
 class CreateObjectRequestRequestTypeDef(
     _RequiredCreateObjectRequestRequestTypeDef, _OptionalCreateObjectRequestRequestTypeDef
 ):
     pass
 
-GetLinkAttributesResponseTypeDef = TypedDict(
-    "GetLinkAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetObjectAttributesResponseTypeDef = TypedDict(
-    "GetObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-IndexAttachmentTypeDef = TypedDict(
-    "IndexAttachmentTypeDef",
-    {
-        "IndexedAttributes": List[AttributeKeyAndValueTypeDef],
-        "ObjectIdentifier": str,
-    },
-    total=False,
-)
-
-ListObjectAttributesResponseTypeDef = TypedDict(
-    "ListObjectAttributesResponseTypeDef",
-    {
-        "Attributes": List[AttributeKeyAndValueTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttachTypedLinkRequestRequestTypeDef = TypedDict(
     "AttachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
@@ -2371,15 +2528,15 @@
 
 TypedLinkSpecifierTypeDef = TypedDict(
     "TypedLinkSpecifierTypeDef",
     {
         "TypedLinkFacet": TypedLinkSchemaAndFacetNameTypeDef,
         "SourceObjectReference": ObjectReferenceTypeDef,
         "TargetObjectReference": ObjectReferenceTypeDef,
-        "IdentityAttributeValues": List[AttributeNameAndValueTypeDef],
+        "IdentityAttributeValues": Sequence[AttributeNameAndValueTypeDef],
     },
 )
 
 LinkAttributeUpdateTypeDef = TypedDict(
     "LinkAttributeUpdateTypeDef",
     {
         "AttributeKey": AttributeKeyTypeDef,
@@ -2421,42 +2578,63 @@
 )
 
 class TypedLinkAttributeRangeTypeDef(
     _RequiredTypedLinkAttributeRangeTypeDef, _OptionalTypedLinkAttributeRangeTypeDef
 ):
     pass
 
-_RequiredFacetAttributeTypeDef = TypedDict(
-    "_RequiredFacetAttributeTypeDef",
+_RequiredFacetAttributeOutputTypeDef = TypedDict(
+    "_RequiredFacetAttributeOutputTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalFacetAttributeTypeDef = TypedDict(
-    "_OptionalFacetAttributeTypeDef",
+_OptionalFacetAttributeOutputTypeDef = TypedDict(
+    "_OptionalFacetAttributeOutputTypeDef",
     {
-        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
-        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "AttributeDefinition": FacetAttributeDefinitionOutputTypeDef,
+        "AttributeReference": FacetAttributeReferenceOutputTypeDef,
         "RequiredBehavior": RequiredAttributeBehaviorType,
     },
     total=False,
 )
 
-class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+class FacetAttributeOutputTypeDef(
+    _RequiredFacetAttributeOutputTypeDef, _OptionalFacetAttributeOutputTypeDef
+):
     pass
 
 ListTypedLinkFacetAttributesResponseTypeDef = TypedDict(
     "ListTypedLinkFacetAttributesResponseTypeDef",
     {
-        "Attributes": List[TypedLinkAttributeDefinitionTypeDef],
+        "Attributes": List[TypedLinkAttributeDefinitionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFacetAttributeTypeDef = TypedDict(
+    "_RequiredFacetAttributeTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalFacetAttributeTypeDef = TypedDict(
+    "_OptionalFacetAttributeTypeDef",
+    {
+        "AttributeDefinition": FacetAttributeDefinitionTypeDef,
+        "AttributeReference": FacetAttributeReferenceTypeDef,
+        "RequiredBehavior": RequiredAttributeBehaviorType,
+    },
+    total=False,
+)
+
+class FacetAttributeTypeDef(_RequiredFacetAttributeTypeDef, _OptionalFacetAttributeTypeDef):
+    pass
+
 TypedLinkFacetAttributeUpdateTypeDef = TypedDict(
     "TypedLinkFacetAttributeUpdateTypeDef",
     {
         "Attribute": TypedLinkAttributeDefinitionTypeDef,
         "Action": UpdateActionTypeType,
     },
 )
@@ -2523,58 +2701,76 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AttachTypedLinkResponseTypeDef = TypedDict(
     "AttachTypedLinkResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchAttachTypedLinkResponseTypeDef = TypedDict(
     "BatchAttachTypedLinkResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "TypedLinkSpecifier": TypedLinkSpecifierOutputTypeDef,
     },
     total=False,
 )
 
-BatchDetachTypedLinkTypeDef = TypedDict(
-    "BatchDetachTypedLinkTypeDef",
+BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListIncomingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-BatchGetLinkAttributesTypeDef = TypedDict(
-    "BatchGetLinkAttributesTypeDef",
+BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "BatchListOutgoingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
-        "AttributeNames": Sequence[str],
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
+        "NextToken": str,
     },
+    total=False,
 )
 
-BatchListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListIncomingTypedLinksResponseTypeDef",
+ListIncomingTypedLinksResponseTypeDef = TypedDict(
+    "ListIncomingTypedLinksResponseTypeDef",
     {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "LinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-BatchListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "BatchListOutgoingTypedLinksResponseTypeDef",
+ListOutgoingTypedLinksResponseTypeDef = TypedDict(
+    "ListOutgoingTypedLinksResponseTypeDef",
     {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
+        "TypedLinkSpecifiers": List[TypedLinkSpecifierOutputTypeDef],
         "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+BatchDetachTypedLinkTypeDef = TypedDict(
+    "BatchDetachTypedLinkTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+    },
+)
+
+BatchGetLinkAttributesTypeDef = TypedDict(
+    "BatchGetLinkAttributesTypeDef",
+    {
+        "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
+        "AttributeNames": Sequence[str],
     },
-    total=False,
 )
 
 DetachTypedLinkRequestRequestTypeDef = TypedDict(
     "DetachTypedLinkRequestRequestTypeDef",
     {
         "DirectoryArn": str,
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
@@ -2598,32 +2794,14 @@
 )
 
 class GetLinkAttributesRequestRequestTypeDef(
     _RequiredGetLinkAttributesRequestRequestTypeDef, _OptionalGetLinkAttributesRequestRequestTypeDef
 ):
     pass
 
-ListIncomingTypedLinksResponseTypeDef = TypedDict(
-    "ListIncomingTypedLinksResponseTypeDef",
-    {
-        "LinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOutgoingTypedLinksResponseTypeDef = TypedDict(
-    "ListOutgoingTypedLinksResponseTypeDef",
-    {
-        "TypedLinkSpecifiers": List[TypedLinkSpecifierTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateLinkAttributesTypeDef = TypedDict(
     "BatchUpdateLinkAttributesTypeDef",
     {
         "TypedLinkSpecifier": TypedLinkSpecifierTypeDef,
         "AttributeUpdates": Sequence[LinkAttributeUpdateTypeDef],
     },
 )
@@ -2857,14 +3035,23 @@
 
 class ListOutgoingTypedLinksRequestRequestTypeDef(
     _RequiredListOutgoingTypedLinksRequestRequestTypeDef,
     _OptionalListOutgoingTypedLinksRequestRequestTypeDef,
 ):
     pass
 
+ListFacetAttributesResponseTypeDef = TypedDict(
+    "ListFacetAttributesResponseTypeDef",
+    {
+        "Attributes": List[FacetAttributeOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFacetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
     },
 )
@@ -2888,23 +3075,14 @@
     {
         "Attribute": FacetAttributeTypeDef,
         "Action": UpdateActionTypeType,
     },
     total=False,
 )
 
-ListFacetAttributesResponseTypeDef = TypedDict(
-    "ListFacetAttributesResponseTypeDef",
-    {
-        "Attributes": List[FacetAttributeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTypedLinkFacetRequestRequestTypeDef = TypedDict(
     "UpdateTypedLinkFacetRequestRequestTypeDef",
     {
         "SchemaArn": str,
         "Name": str,
         "AttributeUpdates": Sequence[TypedLinkFacetAttributeUpdateTypeDef],
         "IdentityAttributeOrder": Sequence[str],
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/PKG-INFO` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-clouddirectory
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudDirectory 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudDirectory 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-clouddirectory"></a>
 
 # mypy-boto3-clouddirectory
 
 [![PyPI - mypy-boto3-clouddirectory](https://img.shields.io/pypi/v/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-clouddirectory.svg?color=blue)](https://pypi.org/project/mypy-boto3-clouddirectory)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-clouddirectory?color=blue)](https://pypistats.org/packages/mypy-boto3-clouddirectory)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-clouddirectory)](https://pepy.tech/project/mypy-boto3-clouddirectory)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudDirectory 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
+[boto3.CloudDirectory 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#CloudDirectory)
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
 [mypy-boto3-clouddirectory docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_clouddirectory/).
 
 See how it helps to find and fix potential bugs:
 
@@ -423,22 +423,25 @@
     ObjectReferenceTypeDef,
     SchemaFacetTypeDef,
     ApplySchemaRequestRequestTypeDef,
     ApplySchemaResponseTypeDef,
     AttachObjectResponseTypeDef,
     AttachToIndexResponseTypeDef,
     TypedLinkSchemaAndFacetNameTypeDef,
+    AttributeKeyOutputTypeDef,
+    TypedAttributeValueOutputTypeDef,
     AttributeKeyTypeDef,
     TypedAttributeValueTypeDef,
     BatchAttachObjectResponseTypeDef,
     BatchAttachToIndexResponseTypeDef,
     BatchCreateIndexResponseTypeDef,
     BatchCreateObjectResponseTypeDef,
     BatchDetachFromIndexResponseTypeDef,
     BatchDetachObjectResponseTypeDef,
+    SchemaFacetOutputTypeDef,
     BatchListObjectChildrenResponseTypeDef,
     PathToObjectIdentifiersTypeDef,
     ObjectIdentifierAndLinkNameTupleTypeDef,
     BatchListObjectPoliciesResponseTypeDef,
     BatchListPolicyAttachmentsResponseTypeDef,
     BatchReadExceptionTypeDef,
     BatchUpdateObjectAttributesResponseTypeDef,
@@ -458,15 +461,17 @@
     DetachObjectResponseTypeDef,
     DirectoryTypeDef,
     DisableDirectoryRequestRequestTypeDef,
     DisableDirectoryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDirectoryRequestRequestTypeDef,
     EnableDirectoryResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
+    FacetAttributeReferenceOutputTypeDef,
     FacetAttributeReferenceTypeDef,
     FacetTypeDef,
     GetAppliedSchemaVersionRequestRequestTypeDef,
     GetAppliedSchemaVersionResponseTypeDef,
     GetDirectoryRequestRequestTypeDef,
     GetFacetRequestRequestTypeDef,
     GetSchemaAsJsonRequestRequestTypeDef,
@@ -493,27 +498,30 @@
     ListObjectPoliciesResponseTypeDef,
     ListPolicyAttachmentsResponseTypeDef,
     ListPublishedSchemaArnsRequestListPublishedSchemaArnsPaginateTypeDef,
     ListPublishedSchemaArnsRequestRequestTypeDef,
     ListPublishedSchemaArnsResponseTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     ListTypedLinkFacetAttributesRequestListTypedLinkFacetAttributesPaginateTypeDef,
     ListTypedLinkFacetAttributesRequestRequestTypeDef,
     ListTypedLinkFacetNamesRequestListTypedLinkFacetNamesPaginateTypeDef,
     ListTypedLinkFacetNamesRequestRequestTypeDef,
     ListTypedLinkFacetNamesResponseTypeDef,
+    ObjectReferenceOutputTypeDef,
     PaginatorConfigTypeDef,
     PolicyAttachmentTypeDef,
     PublishSchemaRequestRequestTypeDef,
     PublishSchemaResponseTypeDef,
     PutSchemaFromJsonRequestRequestTypeDef,
     PutSchemaFromJsonResponseTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
+    TypedLinkSchemaAndFacetNameOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateObjectAttributesResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
     UpdateSchemaResponseTypeDef,
     UpgradeAppliedSchemaRequestRequestTypeDef,
     UpgradeAppliedSchemaResponseTypeDef,
     UpgradePublishedSchemaRequestRequestTypeDef,
@@ -550,95 +558,101 @@
     ListObjectPoliciesRequestListObjectPoliciesPaginateTypeDef,
     ListObjectPoliciesRequestRequestTypeDef,
     ListPolicyAttachmentsRequestListPolicyAttachmentsPaginateTypeDef,
     ListPolicyAttachmentsRequestRequestTypeDef,
     LookupPolicyRequestLookupPolicyPaginateTypeDef,
     LookupPolicyRequestRequestTypeDef,
     BatchGetObjectAttributesTypeDef,
-    BatchGetObjectInformationResponseTypeDef,
     BatchListObjectAttributesTypeDef,
     BatchRemoveFacetFromObjectTypeDef,
     GetObjectAttributesRequestRequestTypeDef,
-    GetObjectInformationResponseTypeDef,
     ListObjectAttributesRequestListObjectAttributesPaginateTypeDef,
     ListObjectAttributesRequestRequestTypeDef,
     RemoveFacetFromObjectRequestRequestTypeDef,
+    AttributeKeyAndValueOutputTypeDef,
+    AttributeNameAndValueOutputTypeDef,
     BatchCreateIndexTypeDef,
     CreateIndexRequestRequestTypeDef,
     AttributeKeyAndValueTypeDef,
     AttributeNameAndValueTypeDef,
     LinkAttributeActionTypeDef,
     ObjectAttributeActionTypeDef,
     TypedAttributeValueRangeTypeDef,
+    BatchGetObjectInformationResponseTypeDef,
+    GetObjectInformationResponseTypeDef,
     BatchListObjectParentPathsResponseTypeDef,
     ListObjectParentPathsResponseTypeDef,
     BatchListObjectParentsResponseTypeDef,
     ListObjectParentsResponseTypeDef,
     GetDirectoryResponseTypeDef,
     ListDirectoriesResponseTypeDef,
+    FacetAttributeDefinitionOutputTypeDef,
+    TypedLinkAttributeDefinitionOutputTypeDef,
     FacetAttributeDefinitionTypeDef,
     TypedLinkAttributeDefinitionTypeDef,
     GetFacetResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
     PolicyToPathTypeDef,
-    AddFacetToObjectRequestRequestTypeDef,
-    BatchAddFacetToObjectTypeDef,
-    BatchCreateObjectTypeDef,
+    TagResourceRequestRequestTypeDef,
     BatchGetLinkAttributesResponseTypeDef,
     BatchGetObjectAttributesResponseTypeDef,
     BatchListObjectAttributesResponseTypeDef,
-    CreateObjectRequestRequestTypeDef,
     GetLinkAttributesResponseTypeDef,
     GetObjectAttributesResponseTypeDef,
     IndexAttachmentTypeDef,
     ListObjectAttributesResponseTypeDef,
+    TypedLinkSpecifierOutputTypeDef,
+    AddFacetToObjectRequestRequestTypeDef,
+    BatchAddFacetToObjectTypeDef,
+    BatchCreateObjectTypeDef,
+    CreateObjectRequestRequestTypeDef,
     AttachTypedLinkRequestRequestTypeDef,
     BatchAttachTypedLinkTypeDef,
     TypedLinkSpecifierTypeDef,
     LinkAttributeUpdateTypeDef,
     ObjectAttributeUpdateTypeDef,
     ObjectAttributeRangeTypeDef,
     TypedLinkAttributeRangeTypeDef,
-    FacetAttributeTypeDef,
+    FacetAttributeOutputTypeDef,
     ListTypedLinkFacetAttributesResponseTypeDef,
+    FacetAttributeTypeDef,
     TypedLinkFacetAttributeUpdateTypeDef,
     TypedLinkFacetTypeDef,
     BatchLookupPolicyResponseTypeDef,
     LookupPolicyResponseTypeDef,
     BatchListAttachedIndicesResponseTypeDef,
     BatchListIndexResponseTypeDef,
     ListAttachedIndicesResponseTypeDef,
     ListIndexResponseTypeDef,
     AttachTypedLinkResponseTypeDef,
     BatchAttachTypedLinkResponseTypeDef,
-    BatchDetachTypedLinkTypeDef,
-    BatchGetLinkAttributesTypeDef,
     BatchListIncomingTypedLinksResponseTypeDef,
     BatchListOutgoingTypedLinksResponseTypeDef,
-    DetachTypedLinkRequestRequestTypeDef,
-    GetLinkAttributesRequestRequestTypeDef,
     ListIncomingTypedLinksResponseTypeDef,
     ListOutgoingTypedLinksResponseTypeDef,
+    BatchDetachTypedLinkTypeDef,
+    BatchGetLinkAttributesTypeDef,
+    DetachTypedLinkRequestRequestTypeDef,
+    GetLinkAttributesRequestRequestTypeDef,
     BatchUpdateLinkAttributesTypeDef,
     UpdateLinkAttributesRequestRequestTypeDef,
     BatchUpdateObjectAttributesTypeDef,
     UpdateObjectAttributesRequestRequestTypeDef,
     BatchListIndexTypeDef,
     ListIndexRequestListIndexPaginateTypeDef,
     ListIndexRequestRequestTypeDef,
     BatchListIncomingTypedLinksTypeDef,
     BatchListOutgoingTypedLinksTypeDef,
     ListIncomingTypedLinksRequestListIncomingTypedLinksPaginateTypeDef,
     ListIncomingTypedLinksRequestRequestTypeDef,
     ListOutgoingTypedLinksRequestListOutgoingTypedLinksPaginateTypeDef,
     ListOutgoingTypedLinksRequestRequestTypeDef,
+    ListFacetAttributesResponseTypeDef,
     CreateFacetRequestRequestTypeDef,
     FacetAttributeUpdateTypeDef,
-    ListFacetAttributesResponseTypeDef,
     UpdateTypedLinkFacetRequestRequestTypeDef,
     CreateTypedLinkFacetRequestRequestTypeDef,
     BatchWriteOperationResponseTypeDef,
     BatchReadSuccessfulResponseTypeDef,
     BatchWriteOperationTypeDef,
     BatchReadOperationTypeDef,
     UpdateFacetRequestRequestTypeDef,
```

### Comparing `mypy-boto3-clouddirectory-1.28.0/mypy_boto3_clouddirectory.egg-info/SOURCES.txt` & `mypy-boto3-clouddirectory-1.28.12/mypy_boto3_clouddirectory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-clouddirectory-1.28.0/setup.py` & `mypy-boto3-clouddirectory-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-clouddirectory",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_clouddirectory"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudDirectory 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudDirectory 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

