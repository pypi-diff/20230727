# Comparing `tmp/mypy-boto3-customer-profiles-1.28.11.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.28.12.tar", last modified: Thu Jul 27 05:34:32 2023, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.28.11.tar` & `mypy-boto3-customer-profiles-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.833034 mypy-boto3-customer-profiles-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13003 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 19:46:56.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68581 2023-07-25 19:46:58.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68499 2023-07-25 19:46:57.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.829034 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 19:49:13.000000 mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.833034 mypy-boto3-customer-profiles-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-25 19:46:55.000000 mypy-boto3-customer-profiles-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19129 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.724539 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40360 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40301 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13056 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72206 2023-07-27 05:19:54.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72102 2023-07-27 05:19:53.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:32.000000 mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:32.732539 mypy-boto3-customer-profiles-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:52.000000 mypy-boto3-customer-profiles-1.28.12/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/LICENSE` & `mypy-boto3-customer-profiles-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.11
-Summary: Type annotations for boto3.CustomerProfiles 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CustomerProfiles 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,15 +349,15 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
@@ -371,105 +371,106 @@
     ConsolidationTypeDef,
     RangeOutputTypeDef,
     ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldOutputTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
+    MergeProfilesResponseTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    GetSimilarProfilesResponseTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
@@ -492,15 +493,14 @@
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/README.md` & `mypy-boto3-customer-profiles-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,15 +317,15 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
@@ -339,105 +339,106 @@
     ConsolidationTypeDef,
     RangeOutputTypeDef,
     ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldOutputTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
+    MergeProfilesResponseTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    GetSimilarProfilesResponseTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
@@ -460,15 +461,14 @@
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__init__.pyi` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.28.11\nVersion:         1.28.11\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -331,14 +331,15 @@
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
@@ -417,14 +418,15 @@
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
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,15 @@
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
@@ -415,14 +416,15 @@
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
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/paginator.pyi` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEventStreamsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEventStreamsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEventStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
     """
 
     def paginate(
-        self, *, DomainName: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, DomainName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListEventStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Paginator.ListEventStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/paginators/#listeventstreamspaginator)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfileKeyResponseTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
@@ -74,105 +74,106 @@
     "ConsolidationTypeDef",
     "RangeOutputTypeDef",
     "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
+    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
+    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
     "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
+    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldOutputTypeDef",
     "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetSimilarProfilesRequestRequestTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
+    "MergeProfilesResponseTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
+    "PutProfileObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
-    "AddProfileKeyResponseTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DeleteIntegrationResponseTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
-    "DeleteProfileResponseTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    "GetIntegrationResponseTypeDef",
-    "GetSimilarProfilesResponseTypeDef",
-    "ListRuleBasedMatchesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PutIntegrationResponseTypeDef",
-    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
@@ -195,15 +196,14 @@
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
@@ -245,22 +245,20 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
@@ -278,14 +276,15 @@
         "City": str,
         "County": str,
         "State": str,
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
+    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
@@ -305,23 +304,37 @@
     "BatchTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-AppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "AppflowIntegrationWorkflowAttributesTypeDef",
+_RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
+    },
+)
+_OptionalAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "_OptionalAppflowIntegrationWorkflowAttributesTypeDef",
+    {
         "RoleArn": str,
     },
+    total=False,
 )
 
+
+class AppflowIntegrationWorkflowAttributesTypeDef(
+    _RequiredAppflowIntegrationWorkflowAttributesTypeDef,
+    _OptionalAppflowIntegrationWorkflowAttributesTypeDef,
+):
+    pass
+
+
 AppflowIntegrationWorkflowMetricsTypeDef = TypedDict(
     "AppflowIntegrationWorkflowMetricsTypeDef",
     {
         "RecordsProcessed": int,
         "StepsCompleted": int,
         "TotalSteps": int,
     },
@@ -351,24 +364,37 @@
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
-AttributeTypesSelectorOutputTypeDef = TypedDict(
-    "AttributeTypesSelectorOutputTypeDef",
+_RequiredAttributeTypesSelectorOutputTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorOutputTypeDef",
     {
         "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorOutputTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorOutputTypeDef",
+    {
         "Address": List[str],
         "PhoneNumber": List[str],
         "EmailAddress": List[str],
     },
+    total=False,
 )
 
+
+class AttributeTypesSelectorOutputTypeDef(
+    _RequiredAttributeTypesSelectorOutputTypeDef, _OptionalAttributeTypesSelectorOutputTypeDef
+):
+    pass
+
+
 _RequiredAttributeTypesSelectorTypeDef = TypedDict(
     "_RequiredAttributeTypesSelectorTypeDef",
     {
         "AttributeMatchingModel": AttributeMatchingModelType,
     },
 )
 _OptionalAttributeTypesSelectorTypeDef = TypedDict(
@@ -384,22 +410,35 @@
 
 class AttributeTypesSelectorTypeDef(
     _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
 ):
     pass
 
 
-ConflictResolutionOutputTypeDef = TypedDict(
-    "ConflictResolutionOutputTypeDef",
+_RequiredConflictResolutionOutputTypeDef = TypedDict(
+    "_RequiredConflictResolutionOutputTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
+    },
+)
+_OptionalConflictResolutionOutputTypeDef = TypedDict(
+    "_OptionalConflictResolutionOutputTypeDef",
+    {
         "SourceName": str,
     },
+    total=False,
 )
 
+
+class ConflictResolutionOutputTypeDef(
+    _RequiredConflictResolutionOutputTypeDef, _OptionalConflictResolutionOutputTypeDef
+):
+    pass
+
+
 ConsolidationOutputTypeDef = TypedDict(
     "ConsolidationOutputTypeDef",
     {
         "MatchingAttributesList": List[List[str]],
     },
 )
 
@@ -494,14 +533,40 @@
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
 
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -509,14 +574,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -525,95 +598,175 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
-DestinationSummaryTypeDef = TypedDict(
-    "DestinationSummaryTypeDef",
+_RequiredDestinationSummaryTypeDef = TypedDict(
+    "_RequiredDestinationSummaryTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalDestinationSummaryTypeDef = TypedDict(
+    "_OptionalDestinationSummaryTypeDef",
+    {
         "UnhealthySince": datetime,
     },
+    total=False,
 )
 
+
+class DestinationSummaryTypeDef(
+    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
+):
+    pass
+
+
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
+    total=False,
 )
 
-EventStreamDestinationDetailsTypeDef = TypedDict(
-    "EventStreamDestinationDetailsTypeDef",
+_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_RequiredEventStreamDestinationDetailsTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_OptionalEventStreamDestinationDetailsTypeDef",
+    {
         "UnhealthySince": datetime,
         "Message": str,
     },
+    total=False,
 )
 
-S3ExportingConfigOutputTypeDef = TypedDict(
-    "S3ExportingConfigOutputTypeDef",
+
+class EventStreamDestinationDetailsTypeDef(
+    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
+):
+    pass
+
+
+_RequiredS3ExportingConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ExportingConfigOutputTypeDef",
     {
         "S3BucketName": str,
+    },
+)
+_OptionalS3ExportingConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ExportingConfigOutputTypeDef",
+    {
         "S3KeyName": str,
     },
+    total=False,
 )
 
+
+class S3ExportingConfigOutputTypeDef(
+    _RequiredS3ExportingConfigOutputTypeDef, _OptionalS3ExportingConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -633,14 +786,15 @@
 
 S3ExportingLocationTypeDef = TypedDict(
     "S3ExportingLocationTypeDef",
     {
         "S3BucketName": str,
         "S3KeyName": str,
     },
+    total=False,
 )
 
 FieldSourceProfileIdsTypeDef = TypedDict(
     "FieldSourceProfileIdsTypeDef",
     {
         "AccountNumber": str,
         "AdditionalInformation": str,
@@ -669,14 +823,26 @@
 
 FoundByKeyValueTypeDef = TypedDict(
     "FoundByKeyValueTypeDef",
     {
         "KeyName": str,
         "Values": List[str],
     },
+    total=False,
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
@@ -688,14 +854,25 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -718,24 +895,41 @@
 JobStatsTypeDef = TypedDict(
     "JobStatsTypeDef",
     {
         "NumberOfProfilesReviewed": int,
         "NumberOfMatchesFound": int,
         "NumberOfMergesDone": int,
     },
+    total=False,
 )
 
 GetIntegrationRequestRequestTypeDef = TypedDict(
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -757,14 +951,15 @@
 MatchItemTypeDef = TypedDict(
     "MatchItemTypeDef",
     {
         "MatchId": str,
         "ProfileIds": List[str],
         "ConfidenceScore": float,
     },
+    total=False,
 )
 
 GetProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
@@ -774,22 +969,24 @@
 ObjectTypeFieldOutputTypeDef = TypedDict(
     "ObjectTypeFieldOutputTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
+    total=False,
 )
 
 ObjectTypeKeyOutputTypeDef = TypedDict(
     "ObjectTypeKeyOutputTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
+    total=False,
 )
 
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
@@ -817,14 +1014,27 @@
 class GetSimilarProfilesRequestRequestTypeDef(
     _RequiredGetSimilarProfilesRequestRequestTypeDef,
     _OptionalGetSimilarProfilesRequestRequestTypeDef,
 ):
     pass
 
 
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -896,39 +1106,53 @@
 class ListAccountIntegrationsRequestRequestTypeDef(
     _RequiredListAccountIntegrationsRequestRequestTypeDef,
     _OptionalListAccountIntegrationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListIntegrationItemTypeDef = TypedDict(
-    "ListIntegrationItemTypeDef",
+_RequiredListIntegrationItemTypeDef = TypedDict(
+    "_RequiredListIntegrationItemTypeDef",
     {
         "DomainName": str,
         "Uri": str,
-        "ObjectTypeName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+    },
+)
+_OptionalListIntegrationItemTypeDef = TypedDict(
+    "_OptionalListIntegrationItemTypeDef",
+    {
+        "ObjectTypeName": str,
         "Tags": Dict[str, str],
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
     },
+    total=False,
 )
 
+
+class ListIntegrationItemTypeDef(
+    _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
+):
+    pass
+
+
 ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
 _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -954,14 +1178,15 @@
     "ListCalculatedAttributeForProfileItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "IsDataPartial": str,
         "Value": str,
     },
+    total=False,
 )
 
 _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
     {
         "DomainName": str,
         "ProfileId": str,
@@ -980,43 +1205,66 @@
 class ListCalculatedAttributesForProfileRequestRequestTypeDef(
     _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
     _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
 ):
     pass
 
 
-ListDomainItemTypeDef = TypedDict(
-    "ListDomainItemTypeDef",
+_RequiredListDomainItemTypeDef = TypedDict(
+    "_RequiredListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+    },
+)
+_OptionalListDomainItemTypeDef = TypedDict(
+    "_OptionalListDomainItemTypeDef",
+    {
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+
+class ListDomainItemTypeDef(_RequiredListDomainItemTypeDef, _OptionalListDomainItemTypeDef):
+    pass
+
+
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1077,32 +1325,46 @@
 
 class ListIntegrationsRequestRequestTypeDef(
     _RequiredListIntegrationsRequestRequestTypeDef, _OptionalListIntegrationsRequestRequestTypeDef
 ):
     pass
 
 
-ListProfileObjectTypeItemTypeDef = TypedDict(
-    "ListProfileObjectTypeItemTypeDef",
+_RequiredListProfileObjectTypeItemTypeDef = TypedDict(
+    "_RequiredListProfileObjectTypeItemTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
+    },
+)
+_OptionalListProfileObjectTypeItemTypeDef = TypedDict(
+    "_OptionalListProfileObjectTypeItemTypeDef",
+    {
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+
+class ListProfileObjectTypeItemTypeDef(
+    _RequiredListProfileObjectTypeItemTypeDef, _OptionalListProfileObjectTypeItemTypeDef
+):
+    pass
+
+
 ListProfileObjectTypeTemplateItemTypeDef = TypedDict(
     "ListProfileObjectTypeTemplateItemTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
     },
+    total=False,
 )
 
 ListProfileObjectTypeTemplatesRequestRequestTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1136,14 +1398,15 @@
 ListProfileObjectsItemTypeDef = TypedDict(
     "ListProfileObjectsItemTypeDef",
     {
         "ObjectTypeName": str,
         "ProfileObjectUniqueKey": str,
         "Object": str,
     },
+    total=False,
 )
 
 ObjectFilterTypeDef = TypedDict(
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
@@ -1169,21 +1432,38 @@
 class ListRuleBasedMatchesRequestRequestTypeDef(
     _RequiredListRuleBasedMatchesRequestRequestTypeDef,
     _OptionalListRuleBasedMatchesRequestRequestTypeDef,
 ):
     pass
 
 
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -1235,14 +1515,22 @@
 MatchingRuleTypeDef = TypedDict(
     "MatchingRuleTypeDef",
     {
         "Rule": Sequence[str],
     },
 )
 
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ObjectTypeFieldTypeDef = TypedDict(
     "ObjectTypeFieldTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
@@ -1254,23 +1542,68 @@
     {
         "StandardIdentifiers": Sequence[StandardIdentifierType],
         "FieldNames": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1379,202 +1712,19 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
-    {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSimilarProfilesResponseTypeDef = TypedDict(
-    "GetSimilarProfilesResponseTypeDef",
-    {
-        "ProfileIds": List[str],
-        "MatchId": str,
-        "MatchType": MatchTypeType,
-        "RuleLevel": int,
-        "ConfidenceScore": float,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRuleBasedMatchesResponseTypeDef = TypedDict(
-    "ListRuleBasedMatchesResponseTypeDef",
-    {
-        "MatchIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1644,28 +1794,31 @@
 
 
 WorkflowAttributesTypeDef = TypedDict(
     "WorkflowAttributesTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowAttributesTypeDef,
     },
+    total=False,
 )
 
 WorkflowMetricsTypeDef = TypedDict(
     "WorkflowMetricsTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowMetricsTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepItemTypeDef = TypedDict(
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
+    total=False,
 )
 
 AttributeDetailsOutputTypeDef = TypedDict(
     "AttributeDetailsOutputTypeDef",
     {
         "Attributes": List[AttributeItemOutputTypeDef],
         "Expression": str,
@@ -1676,24 +1829,37 @@
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
-AutoMergingOutputTypeDef = TypedDict(
-    "AutoMergingOutputTypeDef",
+_RequiredAutoMergingOutputTypeDef = TypedDict(
+    "_RequiredAutoMergingOutputTypeDef",
     {
         "Enabled": bool,
+    },
+)
+_OptionalAutoMergingOutputTypeDef = TypedDict(
+    "_OptionalAutoMergingOutputTypeDef",
+    {
         "Consolidation": ConsolidationOutputTypeDef,
         "ConflictResolution": ConflictResolutionOutputTypeDef,
         "MinAllowedConfidenceScoreForMerging": float,
     },
+    total=False,
 )
 
+
+class AutoMergingOutputTypeDef(
+    _RequiredAutoMergingOutputTypeDef, _OptionalAutoMergingOutputTypeDef
+):
+    pass
+
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1738,14 +1904,15 @@
 ConditionsOutputTypeDef = TypedDict(
     "ConditionsOutputTypeDef",
     {
         "Range": RangeOutputTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdOutputTypeDef,
     },
+    total=False,
 )
 
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
@@ -1772,46 +1939,60 @@
 )
 
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
 
-EventStreamSummaryTypeDef = TypedDict(
-    "EventStreamSummaryTypeDef",
+_RequiredEventStreamSummaryTypeDef = TypedDict(
+    "_RequiredEventStreamSummaryTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
         "EventStreamArn": str,
         "State": EventStreamStateType,
+    },
+)
+_OptionalEventStreamSummaryTypeDef = TypedDict(
+    "_OptionalEventStreamSummaryTypeDef",
+    {
         "StoppedSince": datetime,
         "DestinationSummary": DestinationSummaryTypeDef,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+
+class EventStreamSummaryTypeDef(
+    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
+):
+    pass
+
+
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportingConfigOutputTypeDef = TypedDict(
     "ExportingConfigOutputTypeDef",
     {
         "S3Exporting": S3ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
@@ -1819,14 +2000,15 @@
 )
 
 ExportingLocationTypeDef = TypedDict(
     "ExportingLocationTypeDef",
     {
         "S3Exporting": S3ExportingLocationTypeDef,
     },
+    total=False,
 )
 
 _RequiredMergeProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredMergeProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
         "MainProfileId": str,
@@ -1873,24 +2055,25 @@
         "MailingAddress": AddressOutputTypeDef,
         "BillingAddress": AddressOutputTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
+    total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1901,29 +2084,29 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1934,109 +2117,87 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
-
-
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2063,15 +2224,15 @@
 
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2173,26 +2334,26 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2200,15 +2361,15 @@
         "Description": str,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Conditions": ConditionsOutputTypeDef,
         "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2216,15 +2377,15 @@
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsOutputTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2232,15 +2393,15 @@
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsOutputTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2294,40 +2455,42 @@
 
 
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MatchingResponseTypeDef = TypedDict(
     "MatchingResponseTypeDef",
     {
         "Enabled": bool,
         "JobSchedule": JobScheduleOutputTypeDef,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingConfig": ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 RuleBasedMatchingResponseTypeDef = TypedDict(
     "RuleBasedMatchingResponseTypeDef",
     {
         "Enabled": bool,
         "MatchingRules": List[MatchingRuleOutputTypeDef],
         "Status": RuleBasedMatchingStatusType,
         "MaxAllowedRuleLevelForMerging": int,
         "MaxAllowedRuleLevelForMatching": int,
         "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
         "ConflictResolution": ConflictResolutionOutputTypeDef,
         "ExportingConfig": ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
@@ -2383,15 +2546,15 @@
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2399,22 +2562,23 @@
         "Status": IdentityResolutionJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "JobStats": JobStatsTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "Message": str,
     },
+    total=False,
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2462,15 +2626,15 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResponseTypeDef = TypedDict(
     "GetDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -2479,15 +2643,15 @@
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -2495,15 +2659,15 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2556,15 +2720,15 @@
 
 
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfileKeyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfileKeyResponseTypeDef",
     "AdditionalSearchKeyTypeDef",
     "AddressOutputTypeDef",
     "AddressTypeDef",
     "BatchTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
@@ -73,105 +73,106 @@
     "ConsolidationTypeDef",
     "RangeOutputTypeDef",
     "ThresholdOutputTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
+    "CreateEventStreamResponseTypeDef",
+    "CreateIntegrationWorkflowResponseTypeDef",
+    "CreateProfileResponseTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     "DeleteDomainRequestRequestTypeDef",
+    "DeleteDomainResponseTypeDef",
     "DeleteEventStreamRequestRequestTypeDef",
     "DeleteIntegrationRequestRequestTypeDef",
+    "DeleteIntegrationResponseTypeDef",
     "DeleteProfileKeyRequestRequestTypeDef",
+    "DeleteProfileKeyResponseTypeDef",
     "DeleteProfileObjectRequestRequestTypeDef",
+    "DeleteProfileObjectResponseTypeDef",
     "DeleteProfileObjectTypeRequestRequestTypeDef",
+    "DeleteProfileObjectTypeResponseTypeDef",
     "DeleteProfileRequestRequestTypeDef",
+    "DeleteProfileResponseTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "DestinationSummaryTypeDef",
     "DomainStatsTypeDef",
     "EventStreamDestinationDetailsTypeDef",
     "S3ExportingConfigOutputTypeDef",
     "S3ExportingConfigTypeDef",
     "S3ExportingLocationTypeDef",
     "FieldSourceProfileIdsTypeDef",
     "FoundByKeyValueTypeDef",
+    "GetAutoMergingPreviewResponseTypeDef",
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     "GetCalculatedAttributeForProfileRequestRequestTypeDef",
+    "GetCalculatedAttributeForProfileResponseTypeDef",
     "GetDomainRequestRequestTypeDef",
     "GetEventStreamRequestRequestTypeDef",
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
+    "GetIntegrationResponseTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldOutputTypeDef",
     "ObjectTypeKeyOutputTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetSimilarProfilesRequestRequestTypeDef",
+    "GetSimilarProfilesResponseTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleOutputTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
     "ListCalculatedAttributeDefinitionItemTypeDef",
     "ListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     "ListCalculatedAttributeForProfileItemTypeDef",
     "ListCalculatedAttributesForProfileRequestRequestTypeDef",
     "ListDomainItemTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListEventStreamsRequestRequestTypeDef",
     "ListIdentityResolutionJobsRequestRequestTypeDef",
     "ListIntegrationsRequestRequestTypeDef",
     "ListProfileObjectTypeItemTypeDef",
     "ListProfileObjectTypeTemplateItemTypeDef",
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListRuleBasedMatchesRequestRequestTypeDef",
+    "ListRuleBasedMatchesResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowsItemTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "MarketoSourcePropertiesTypeDef",
     "MatchingRuleOutputTypeDef",
     "MatchingRuleTypeDef",
+    "MergeProfilesResponseTypeDef",
     "ObjectTypeFieldTypeDef",
     "ObjectTypeKeyTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutIntegrationResponseTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
+    "PutProfileObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddressTypeDef",
-    "AddProfileKeyResponseTypeDef",
-    "CreateEventStreamResponseTypeDef",
-    "CreateIntegrationWorkflowResponseTypeDef",
-    "CreateProfileResponseTypeDef",
-    "DeleteDomainResponseTypeDef",
-    "DeleteIntegrationResponseTypeDef",
-    "DeleteProfileKeyResponseTypeDef",
-    "DeleteProfileObjectResponseTypeDef",
-    "DeleteProfileObjectTypeResponseTypeDef",
-    "DeleteProfileResponseTypeDef",
-    "GetAutoMergingPreviewResponseTypeDef",
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    "GetIntegrationResponseTypeDef",
-    "GetSimilarProfilesResponseTypeDef",
-    "ListRuleBasedMatchesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "MergeProfilesResponseTypeDef",
-    "PutIntegrationResponseTypeDef",
-    "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
     "AttributeDetailsOutputTypeDef",
@@ -194,15 +195,14 @@
     "GetProfileObjectTypeTemplateResponseTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
-    "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "PutProfileObjectTypeRequestRequestTypeDef",
     "TriggerPropertiesTypeDef",
@@ -244,22 +244,20 @@
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfileKeyResponseTypeDef = TypedDict(
+    "AddProfileKeyResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "KeyName": str,
+        "Values": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AdditionalSearchKeyTypeDef = TypedDict(
     "AdditionalSearchKeyTypeDef",
     {
         "KeyName": str,
@@ -277,14 +275,15 @@
         "City": str,
         "County": str,
         "State": str,
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
+    total=False,
 )
 
 AddressTypeDef = TypedDict(
     "AddressTypeDef",
     {
         "Address1": str,
         "Address2": str,
@@ -304,23 +303,35 @@
     "BatchTypeDef",
     {
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
     },
 )
 
-AppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
-    "AppflowIntegrationWorkflowAttributesTypeDef",
+_RequiredAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "_RequiredAppflowIntegrationWorkflowAttributesTypeDef",
     {
         "SourceConnectorType": SourceConnectorTypeType,
         "ConnectorProfileName": str,
+    },
+)
+_OptionalAppflowIntegrationWorkflowAttributesTypeDef = TypedDict(
+    "_OptionalAppflowIntegrationWorkflowAttributesTypeDef",
+    {
         "RoleArn": str,
     },
+    total=False,
 )
 
+class AppflowIntegrationWorkflowAttributesTypeDef(
+    _RequiredAppflowIntegrationWorkflowAttributesTypeDef,
+    _OptionalAppflowIntegrationWorkflowAttributesTypeDef,
+):
+    pass
+
 AppflowIntegrationWorkflowMetricsTypeDef = TypedDict(
     "AppflowIntegrationWorkflowMetricsTypeDef",
     {
         "RecordsProcessed": int,
         "StepsCompleted": int,
         "TotalSteps": int,
     },
@@ -350,24 +361,35 @@
 AttributeItemTypeDef = TypedDict(
     "AttributeItemTypeDef",
     {
         "Name": str,
     },
 )
 
-AttributeTypesSelectorOutputTypeDef = TypedDict(
-    "AttributeTypesSelectorOutputTypeDef",
+_RequiredAttributeTypesSelectorOutputTypeDef = TypedDict(
+    "_RequiredAttributeTypesSelectorOutputTypeDef",
     {
         "AttributeMatchingModel": AttributeMatchingModelType,
+    },
+)
+_OptionalAttributeTypesSelectorOutputTypeDef = TypedDict(
+    "_OptionalAttributeTypesSelectorOutputTypeDef",
+    {
         "Address": List[str],
         "PhoneNumber": List[str],
         "EmailAddress": List[str],
     },
+    total=False,
 )
 
+class AttributeTypesSelectorOutputTypeDef(
+    _RequiredAttributeTypesSelectorOutputTypeDef, _OptionalAttributeTypesSelectorOutputTypeDef
+):
+    pass
+
 _RequiredAttributeTypesSelectorTypeDef = TypedDict(
     "_RequiredAttributeTypesSelectorTypeDef",
     {
         "AttributeMatchingModel": AttributeMatchingModelType,
     },
 )
 _OptionalAttributeTypesSelectorTypeDef = TypedDict(
@@ -381,22 +403,33 @@
 )
 
 class AttributeTypesSelectorTypeDef(
     _RequiredAttributeTypesSelectorTypeDef, _OptionalAttributeTypesSelectorTypeDef
 ):
     pass
 
-ConflictResolutionOutputTypeDef = TypedDict(
-    "ConflictResolutionOutputTypeDef",
+_RequiredConflictResolutionOutputTypeDef = TypedDict(
+    "_RequiredConflictResolutionOutputTypeDef",
     {
         "ConflictResolvingModel": ConflictResolvingModelType,
+    },
+)
+_OptionalConflictResolutionOutputTypeDef = TypedDict(
+    "_OptionalConflictResolutionOutputTypeDef",
+    {
         "SourceName": str,
     },
+    total=False,
 )
 
+class ConflictResolutionOutputTypeDef(
+    _RequiredConflictResolutionOutputTypeDef, _OptionalConflictResolutionOutputTypeDef
+):
+    pass
+
 ConsolidationOutputTypeDef = TypedDict(
     "ConsolidationOutputTypeDef",
     {
         "MatchingAttributesList": List[List[str]],
     },
 )
 
@@ -487,14 +520,40 @@
 )
 
 class CreateEventStreamRequestRequestTypeDef(
     _RequiredCreateEventStreamRequestRequestTypeDef, _OptionalCreateEventStreamRequestRequestTypeDef
 ):
     pass
 
+CreateEventStreamResponseTypeDef = TypedDict(
+    "CreateEventStreamResponseTypeDef",
+    {
+        "EventStreamArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateIntegrationWorkflowResponseTypeDef = TypedDict(
+    "CreateIntegrationWorkflowResponseTypeDef",
+    {
+        "WorkflowId": str,
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateProfileResponseTypeDef = TypedDict(
+    "CreateProfileResponseTypeDef",
+    {
+        "ProfileId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
     },
 )
@@ -502,14 +561,22 @@
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
+DeleteDomainResponseTypeDef = TypedDict(
+    "DeleteDomainResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteEventStreamRequestRequestTypeDef = TypedDict(
     "DeleteEventStreamRequestRequestTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
     },
 )
@@ -518,95 +585,169 @@
     "DeleteIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+DeleteIntegrationResponseTypeDef = TypedDict(
+    "DeleteIntegrationResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileKeyRequestRequestTypeDef = TypedDict(
     "DeleteProfileKeyRequestRequestTypeDef",
     {
         "ProfileId": str,
         "KeyName": str,
         "Values": Sequence[str],
         "DomainName": str,
     },
 )
 
+DeleteProfileKeyResponseTypeDef = TypedDict(
+    "DeleteProfileKeyResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectRequestRequestTypeDef",
     {
         "ProfileId": str,
         "ProfileObjectUniqueKey": str,
         "ObjectTypeName": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileObjectResponseTypeDef = TypedDict(
+    "DeleteProfileObjectResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "DeleteProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
     },
 )
 
+DeleteProfileObjectTypeResponseTypeDef = TypedDict(
+    "DeleteProfileObjectTypeResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteProfileRequestRequestTypeDef = TypedDict(
     "DeleteProfileRequestRequestTypeDef",
     {
         "ProfileId": str,
         "DomainName": str,
     },
 )
 
+DeleteProfileResponseTypeDef = TypedDict(
+    "DeleteProfileResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteWorkflowRequestRequestTypeDef = TypedDict(
     "DeleteWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
 
-DestinationSummaryTypeDef = TypedDict(
-    "DestinationSummaryTypeDef",
+_RequiredDestinationSummaryTypeDef = TypedDict(
+    "_RequiredDestinationSummaryTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalDestinationSummaryTypeDef = TypedDict(
+    "_OptionalDestinationSummaryTypeDef",
+    {
         "UnhealthySince": datetime,
     },
+    total=False,
 )
 
+class DestinationSummaryTypeDef(
+    _RequiredDestinationSummaryTypeDef, _OptionalDestinationSummaryTypeDef
+):
+    pass
+
 DomainStatsTypeDef = TypedDict(
     "DomainStatsTypeDef",
     {
         "ProfileCount": int,
         "MeteringProfileCount": int,
         "ObjectCount": int,
         "TotalSize": int,
     },
+    total=False,
 )
 
-EventStreamDestinationDetailsTypeDef = TypedDict(
-    "EventStreamDestinationDetailsTypeDef",
+_RequiredEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_RequiredEventStreamDestinationDetailsTypeDef",
     {
         "Uri": str,
         "Status": EventStreamDestinationStatusType,
+    },
+)
+_OptionalEventStreamDestinationDetailsTypeDef = TypedDict(
+    "_OptionalEventStreamDestinationDetailsTypeDef",
+    {
         "UnhealthySince": datetime,
         "Message": str,
     },
+    total=False,
 )
 
-S3ExportingConfigOutputTypeDef = TypedDict(
-    "S3ExportingConfigOutputTypeDef",
+class EventStreamDestinationDetailsTypeDef(
+    _RequiredEventStreamDestinationDetailsTypeDef, _OptionalEventStreamDestinationDetailsTypeDef
+):
+    pass
+
+_RequiredS3ExportingConfigOutputTypeDef = TypedDict(
+    "_RequiredS3ExportingConfigOutputTypeDef",
     {
         "S3BucketName": str,
+    },
+)
+_OptionalS3ExportingConfigOutputTypeDef = TypedDict(
+    "_OptionalS3ExportingConfigOutputTypeDef",
+    {
         "S3KeyName": str,
     },
+    total=False,
 )
 
+class S3ExportingConfigOutputTypeDef(
+    _RequiredS3ExportingConfigOutputTypeDef, _OptionalS3ExportingConfigOutputTypeDef
+):
+    pass
+
 _RequiredS3ExportingConfigTypeDef = TypedDict(
     "_RequiredS3ExportingConfigTypeDef",
     {
         "S3BucketName": str,
     },
 )
 _OptionalS3ExportingConfigTypeDef = TypedDict(
@@ -624,14 +765,15 @@
 
 S3ExportingLocationTypeDef = TypedDict(
     "S3ExportingLocationTypeDef",
     {
         "S3BucketName": str,
         "S3KeyName": str,
     },
+    total=False,
 )
 
 FieldSourceProfileIdsTypeDef = TypedDict(
     "FieldSourceProfileIdsTypeDef",
     {
         "AccountNumber": str,
         "AdditionalInformation": str,
@@ -660,14 +802,26 @@
 
 FoundByKeyValueTypeDef = TypedDict(
     "FoundByKeyValueTypeDef",
     {
         "KeyName": str,
         "Values": List[str],
     },
+    total=False,
+)
+
+GetAutoMergingPreviewResponseTypeDef = TypedDict(
+    "GetAutoMergingPreviewResponseTypeDef",
+    {
+        "DomainName": str,
+        "NumberOfMatchesInSample": int,
+        "NumberOfProfilesInSample": int,
+        "NumberOfProfilesWillBeMerged": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 GetCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
         "CalculatedAttributeName": str,
@@ -679,14 +833,25 @@
     {
         "DomainName": str,
         "ProfileId": str,
         "CalculatedAttributeName": str,
     },
 )
 
+GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
+    "GetCalculatedAttributeForProfileResponseTypeDef",
+    {
+        "CalculatedAttributeName": str,
+        "DisplayName": str,
+        "IsDataPartial": str,
+        "Value": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
@@ -709,24 +874,41 @@
 JobStatsTypeDef = TypedDict(
     "JobStatsTypeDef",
     {
         "NumberOfProfilesReviewed": int,
         "NumberOfMatchesFound": int,
         "NumberOfMergesDone": int,
     },
+    total=False,
 )
 
 GetIntegrationRequestRequestTypeDef = TypedDict(
     "GetIntegrationRequestRequestTypeDef",
     {
         "DomainName": str,
         "Uri": str,
     },
 )
 
+GetIntegrationResponseTypeDef = TypedDict(
+    "GetIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetMatchesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMatchesRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetMatchesRequestRequestTypeDef = TypedDict(
@@ -746,14 +928,15 @@
 MatchItemTypeDef = TypedDict(
     "MatchItemTypeDef",
     {
         "MatchId": str,
         "ProfileIds": List[str],
         "ConfidenceScore": float,
     },
+    total=False,
 )
 
 GetProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
         "ObjectTypeName": str,
@@ -763,22 +946,24 @@
 ObjectTypeFieldOutputTypeDef = TypedDict(
     "ObjectTypeFieldOutputTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
+    total=False,
 )
 
 ObjectTypeKeyOutputTypeDef = TypedDict(
     "ObjectTypeKeyOutputTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
+    total=False,
 )
 
 GetProfileObjectTypeTemplateRequestRequestTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     {
         "TemplateId": str,
     },
@@ -804,14 +989,27 @@
 
 class GetSimilarProfilesRequestRequestTypeDef(
     _RequiredGetSimilarProfilesRequestRequestTypeDef,
     _OptionalGetSimilarProfilesRequestRequestTypeDef,
 ):
     pass
 
+GetSimilarProfilesResponseTypeDef = TypedDict(
+    "GetSimilarProfilesResponseTypeDef",
+    {
+        "ProfileIds": List[str],
+        "MatchId": str,
+        "MatchType": MatchTypeType,
+        "RuleLevel": int,
+        "ConfidenceScore": float,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetWorkflowRequestRequestTypeDef = TypedDict(
     "GetWorkflowRequestRequestTypeDef",
     {
         "DomainName": str,
         "WorkflowId": str,
     },
 )
@@ -879,39 +1077,51 @@
 
 class ListAccountIntegrationsRequestRequestTypeDef(
     _RequiredListAccountIntegrationsRequestRequestTypeDef,
     _OptionalListAccountIntegrationsRequestRequestTypeDef,
 ):
     pass
 
-ListIntegrationItemTypeDef = TypedDict(
-    "ListIntegrationItemTypeDef",
+_RequiredListIntegrationItemTypeDef = TypedDict(
+    "_RequiredListIntegrationItemTypeDef",
     {
         "DomainName": str,
         "Uri": str,
-        "ObjectTypeName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+    },
+)
+_OptionalListIntegrationItemTypeDef = TypedDict(
+    "_OptionalListIntegrationItemTypeDef",
+    {
+        "ObjectTypeName": str,
         "Tags": Dict[str, str],
         "ObjectTypeNames": Dict[str, str],
         "WorkflowId": str,
         "IsUnstructured": bool,
     },
+    total=False,
 )
 
+class ListIntegrationItemTypeDef(
+    _RequiredListIntegrationItemTypeDef, _OptionalListIntegrationItemTypeDef
+):
+    pass
+
 ListCalculatedAttributeDefinitionItemTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
 _RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributeDefinitionsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
@@ -935,14 +1145,15 @@
     "ListCalculatedAttributeForProfileItemTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "IsDataPartial": str,
         "Value": str,
     },
+    total=False,
 )
 
 _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListCalculatedAttributesForProfileRequestRequestTypeDef",
     {
         "DomainName": str,
         "ProfileId": str,
@@ -959,43 +1170,62 @@
 
 class ListCalculatedAttributesForProfileRequestRequestTypeDef(
     _RequiredListCalculatedAttributesForProfileRequestRequestTypeDef,
     _OptionalListCalculatedAttributesForProfileRequestRequestTypeDef,
 ):
     pass
 
-ListDomainItemTypeDef = TypedDict(
-    "ListDomainItemTypeDef",
+_RequiredListDomainItemTypeDef = TypedDict(
+    "_RequiredListDomainItemTypeDef",
     {
         "DomainName": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
+    },
+)
+_OptionalListDomainItemTypeDef = TypedDict(
+    "_OptionalListDomainItemTypeDef",
+    {
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+class ListDomainItemTypeDef(_RequiredListDomainItemTypeDef, _OptionalListDomainItemTypeDef):
+    pass
+
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DomainName": str,
+    },
+)
+_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
+    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
+    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
+    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
+):
+    pass
+
 _RequiredListEventStreamsRequestRequestTypeDef = TypedDict(
     "_RequiredListEventStreamsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalListEventStreamsRequestRequestTypeDef = TypedDict(
@@ -1050,32 +1280,44 @@
 )
 
 class ListIntegrationsRequestRequestTypeDef(
     _RequiredListIntegrationsRequestRequestTypeDef, _OptionalListIntegrationsRequestRequestTypeDef
 ):
     pass
 
-ListProfileObjectTypeItemTypeDef = TypedDict(
-    "ListProfileObjectTypeItemTypeDef",
+_RequiredListProfileObjectTypeItemTypeDef = TypedDict(
+    "_RequiredListProfileObjectTypeItemTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
+    },
+)
+_OptionalListProfileObjectTypeItemTypeDef = TypedDict(
+    "_OptionalListProfileObjectTypeItemTypeDef",
+    {
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+class ListProfileObjectTypeItemTypeDef(
+    _RequiredListProfileObjectTypeItemTypeDef, _OptionalListProfileObjectTypeItemTypeDef
+):
+    pass
+
 ListProfileObjectTypeTemplateItemTypeDef = TypedDict(
     "ListProfileObjectTypeTemplateItemTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
     },
+    total=False,
 )
 
 ListProfileObjectTypeTemplatesRequestRequestTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -1107,14 +1349,15 @@
 ListProfileObjectsItemTypeDef = TypedDict(
     "ListProfileObjectsItemTypeDef",
     {
         "ObjectTypeName": str,
         "ProfileObjectUniqueKey": str,
         "Object": str,
     },
+    total=False,
 )
 
 ObjectFilterTypeDef = TypedDict(
     "ObjectFilterTypeDef",
     {
         "KeyName": str,
         "Values": Sequence[str],
@@ -1138,21 +1381,38 @@
 
 class ListRuleBasedMatchesRequestRequestTypeDef(
     _RequiredListRuleBasedMatchesRequestRequestTypeDef,
     _OptionalListRuleBasedMatchesRequestRequestTypeDef,
 ):
     pass
 
+ListRuleBasedMatchesResponseTypeDef = TypedDict(
+    "ListRuleBasedMatchesResponseTypeDef",
+    {
+        "MatchIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListWorkflowsItemTypeDef = TypedDict(
     "ListWorkflowsItemTypeDef",
     {
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "WorkflowId": str,
         "Status": StatusType,
         "StatusDescription": str,
@@ -1202,14 +1462,22 @@
 MatchingRuleTypeDef = TypedDict(
     "MatchingRuleTypeDef",
     {
         "Rule": Sequence[str],
     },
 )
 
+MergeProfilesResponseTypeDef = TypedDict(
+    "MergeProfilesResponseTypeDef",
+    {
+        "Message": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ObjectTypeFieldTypeDef = TypedDict(
     "ObjectTypeFieldTypeDef",
     {
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
@@ -1221,23 +1489,68 @@
     {
         "StandardIdentifiers": Sequence[StandardIdentifierType],
         "FieldNames": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PutIntegrationResponseTypeDef = TypedDict(
+    "PutIntegrationResponseTypeDef",
+    {
+        "DomainName": str,
+        "Uri": str,
+        "ObjectTypeName": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Tags": Dict[str, str],
+        "ObjectTypeNames": Dict[str, str],
+        "WorkflowId": str,
+        "IsUnstructured": bool,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
 )
 
+PutProfileObjectResponseTypeDef = TypedDict(
+    "PutProfileObjectResponseTypeDef",
+    {
+        "ProfileObjectUniqueKey": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
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
 _RequiredS3SourcePropertiesTypeDef = TypedDict(
     "_RequiredS3SourcePropertiesTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3SourcePropertiesTypeDef = TypedDict(
@@ -1340,202 +1653,19 @@
         "Province": str,
         "Country": str,
         "PostalCode": str,
     },
     total=False,
 )
 
-AddProfileKeyResponseTypeDef = TypedDict(
-    "AddProfileKeyResponseTypeDef",
-    {
-        "KeyName": str,
-        "Values": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateEventStreamResponseTypeDef = TypedDict(
-    "CreateEventStreamResponseTypeDef",
-    {
-        "EventStreamArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateIntegrationWorkflowResponseTypeDef = TypedDict(
-    "CreateIntegrationWorkflowResponseTypeDef",
-    {
-        "WorkflowId": str,
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateProfileResponseTypeDef = TypedDict(
-    "CreateProfileResponseTypeDef",
-    {
-        "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteDomainResponseTypeDef = TypedDict(
-    "DeleteDomainResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteIntegrationResponseTypeDef = TypedDict(
-    "DeleteIntegrationResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileKeyResponseTypeDef = TypedDict(
-    "DeleteProfileKeyResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectResponseTypeDef = TypedDict(
-    "DeleteProfileObjectResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileObjectTypeResponseTypeDef = TypedDict(
-    "DeleteProfileObjectTypeResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteProfileResponseTypeDef = TypedDict(
-    "DeleteProfileResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAutoMergingPreviewResponseTypeDef = TypedDict(
-    "GetAutoMergingPreviewResponseTypeDef",
-    {
-        "DomainName": str,
-        "NumberOfMatchesInSample": int,
-        "NumberOfProfilesInSample": int,
-        "NumberOfProfilesWillBeMerged": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCalculatedAttributeForProfileResponseTypeDef = TypedDict(
-    "GetCalculatedAttributeForProfileResponseTypeDef",
-    {
-        "CalculatedAttributeName": str,
-        "DisplayName": str,
-        "IsDataPartial": str,
-        "Value": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetIntegrationResponseTypeDef = TypedDict(
-    "GetIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSimilarProfilesResponseTypeDef = TypedDict(
-    "GetSimilarProfilesResponseTypeDef",
-    {
-        "ProfileIds": List[str],
-        "MatchId": str,
-        "MatchType": MatchTypeType,
-        "RuleLevel": int,
-        "ConfidenceScore": float,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListRuleBasedMatchesResponseTypeDef = TypedDict(
-    "ListRuleBasedMatchesResponseTypeDef",
-    {
-        "MatchIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MergeProfilesResponseTypeDef = TypedDict(
-    "MergeProfilesResponseTypeDef",
-    {
-        "Message": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutIntegrationResponseTypeDef = TypedDict(
-    "PutIntegrationResponseTypeDef",
-    {
-        "DomainName": str,
-        "Uri": str,
-        "ObjectTypeName": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Tags": Dict[str, str],
-        "ObjectTypeNames": Dict[str, str],
-        "WorkflowId": str,
-        "IsUnstructured": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutProfileObjectResponseTypeDef = TypedDict(
-    "PutProfileObjectResponseTypeDef",
-    {
-        "ProfileObjectUniqueKey": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateProfileResponseTypeDef = TypedDict(
     "UpdateProfileResponseTypeDef",
     {
         "ProfileId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSearchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -1601,28 +1731,31 @@
     pass
 
 WorkflowAttributesTypeDef = TypedDict(
     "WorkflowAttributesTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowAttributesTypeDef,
     },
+    total=False,
 )
 
 WorkflowMetricsTypeDef = TypedDict(
     "WorkflowMetricsTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowMetricsTypeDef,
     },
+    total=False,
 )
 
 WorkflowStepItemTypeDef = TypedDict(
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
+    total=False,
 )
 
 AttributeDetailsOutputTypeDef = TypedDict(
     "AttributeDetailsOutputTypeDef",
     {
         "Attributes": List[AttributeItemOutputTypeDef],
         "Expression": str,
@@ -1633,24 +1766,35 @@
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
-AutoMergingOutputTypeDef = TypedDict(
-    "AutoMergingOutputTypeDef",
+_RequiredAutoMergingOutputTypeDef = TypedDict(
+    "_RequiredAutoMergingOutputTypeDef",
     {
         "Enabled": bool,
+    },
+)
+_OptionalAutoMergingOutputTypeDef = TypedDict(
+    "_OptionalAutoMergingOutputTypeDef",
+    {
         "Consolidation": ConsolidationOutputTypeDef,
         "ConflictResolution": ConflictResolutionOutputTypeDef,
         "MinAllowedConfidenceScoreForMerging": float,
     },
+    total=False,
 )
 
+class AutoMergingOutputTypeDef(
+    _RequiredAutoMergingOutputTypeDef, _OptionalAutoMergingOutputTypeDef
+):
+    pass
+
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1691,14 +1835,15 @@
 ConditionsOutputTypeDef = TypedDict(
     "ConditionsOutputTypeDef",
     {
         "Range": RangeOutputTypeDef,
         "ObjectCount": int,
         "Threshold": ThresholdOutputTypeDef,
     },
+    total=False,
 )
 
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "Range": RangeTypeDef,
         "ObjectCount": int,
@@ -1723,46 +1868,58 @@
     },
     total=False,
 )
 
 class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-EventStreamSummaryTypeDef = TypedDict(
-    "EventStreamSummaryTypeDef",
+_RequiredEventStreamSummaryTypeDef = TypedDict(
+    "_RequiredEventStreamSummaryTypeDef",
     {
         "DomainName": str,
         "EventStreamName": str,
         "EventStreamArn": str,
         "State": EventStreamStateType,
+    },
+)
+_OptionalEventStreamSummaryTypeDef = TypedDict(
+    "_OptionalEventStreamSummaryTypeDef",
+    {
         "StoppedSince": datetime,
         "DestinationSummary": DestinationSummaryTypeDef,
         "Tags": Dict[str, str],
     },
+    total=False,
 )
 
+class EventStreamSummaryTypeDef(
+    _RequiredEventStreamSummaryTypeDef, _OptionalEventStreamSummaryTypeDef
+):
+    pass
+
 GetEventStreamResponseTypeDef = TypedDict(
     "GetEventStreamResponseTypeDef",
     {
         "DomainName": str,
         "EventStreamArn": str,
         "CreatedAt": datetime,
         "State": EventStreamStateType,
         "StoppedSince": datetime,
         "DestinationDetails": EventStreamDestinationDetailsTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ExportingConfigOutputTypeDef = TypedDict(
     "ExportingConfigOutputTypeDef",
     {
         "S3Exporting": S3ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 ExportingConfigTypeDef = TypedDict(
     "ExportingConfigTypeDef",
     {
         "S3Exporting": S3ExportingConfigTypeDef,
     },
@@ -1770,14 +1927,15 @@
 )
 
 ExportingLocationTypeDef = TypedDict(
     "ExportingLocationTypeDef",
     {
         "S3Exporting": S3ExportingLocationTypeDef,
     },
+    total=False,
 )
 
 _RequiredMergeProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredMergeProfilesRequestRequestTypeDef",
     {
         "DomainName": str,
         "MainProfileId": str,
@@ -1822,24 +1980,25 @@
         "MailingAddress": AddressOutputTypeDef,
         "BillingAddress": AddressOutputTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
         "PartyTypeString": str,
         "GenderString": str,
     },
+    total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
         "NextToken": str,
         "MatchGenerationDate": datetime,
         "PotentialMatches": int,
         "Matches": List[MatchItemTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeResponseTypeDef = TypedDict(
     "GetProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1850,29 +2009,29 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetProfileObjectTypeTemplateResponseTypeDef = TypedDict(
     "GetProfileObjectTypeTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
@@ -1883,107 +2042,87 @@
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldOutputTypeDef],
         "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountIntegrationsResponseTypeDef = TypedDict(
     "ListAccountIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListIntegrationsResponseTypeDef = TypedDict(
     "ListIntegrationsResponseTypeDef",
     {
         "Items": List[ListIntegrationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCalculatedAttributeDefinitionsResponseTypeDef = TypedDict(
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeDefinitionItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCalculatedAttributesForProfileResponseTypeDef = TypedDict(
     "ListCalculatedAttributesForProfileResponseTypeDef",
     {
         "Items": List[ListCalculatedAttributeForProfileItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "Items": List[ListDomainItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "DomainName": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef = TypedDict(
-    "_OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListEventStreamsRequestListEventStreamsPaginateTypeDef(
-    _RequiredListEventStreamsRequestListEventStreamsPaginateTypeDef,
-    _OptionalListEventStreamsRequestListEventStreamsPaginateTypeDef,
-):
-    pass
 
 ListProfileObjectTypesResponseTypeDef = TypedDict(
     "ListProfileObjectTypesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectTypeTemplatesResponseTypeDef = TypedDict(
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     {
         "Items": List[ListProfileObjectTypeTemplateItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListProfileObjectsResponseTypeDef = TypedDict(
     "ListProfileObjectsResponseTypeDef",
     {
         "Items": List[ListProfileObjectsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListProfileObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredListProfileObjectsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2008,15 +2147,15 @@
     pass
 
 ListWorkflowsResponseTypeDef = TypedDict(
     "ListWorkflowsResponseTypeDef",
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
     "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2114,26 +2253,26 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Status": StatusType,
         "ErrorDescription": str,
         "StartDate": datetime,
         "LastUpdatedAt": datetime,
         "Attributes": WorkflowAttributesTypeDef,
         "Metrics": WorkflowMetricsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetWorkflowStepsResponseTypeDef = TypedDict(
     "GetWorkflowStepsResponseTypeDef",
     {
         "WorkflowId": str,
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2141,15 +2280,15 @@
         "Description": str,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Conditions": ConditionsOutputTypeDef,
         "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2157,15 +2296,15 @@
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsOutputTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
@@ -2173,15 +2312,15 @@
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsOutputTypeDef,
         "AttributeDetails": AttributeDetailsOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2231,40 +2370,42 @@
     pass
 
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
     {
         "Items": List[EventStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 MatchingResponseTypeDef = TypedDict(
     "MatchingResponseTypeDef",
     {
         "Enabled": bool,
         "JobSchedule": JobScheduleOutputTypeDef,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingConfig": ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 RuleBasedMatchingResponseTypeDef = TypedDict(
     "RuleBasedMatchingResponseTypeDef",
     {
         "Enabled": bool,
         "MatchingRules": List[MatchingRuleOutputTypeDef],
         "Status": RuleBasedMatchingStatusType,
         "MaxAllowedRuleLevelForMerging": int,
         "MaxAllowedRuleLevelForMatching": int,
         "AttributeTypesSelector": AttributeTypesSelectorOutputTypeDef,
         "ConflictResolution": ConflictResolutionOutputTypeDef,
         "ExportingConfig": ExportingConfigOutputTypeDef,
     },
+    total=False,
 )
 
 _RequiredMatchingRequestTypeDef = TypedDict(
     "_RequiredMatchingRequestTypeDef",
     {
         "Enabled": bool,
     },
@@ -2316,15 +2457,15 @@
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
         "AutoMerging": AutoMergingOutputTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
     "IdentityResolutionJobTypeDef",
     {
         "DomainName": str,
@@ -2332,22 +2473,23 @@
         "Status": IdentityResolutionJobStatusType,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "JobStats": JobStatsTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "Message": str,
     },
+    total=False,
 )
 
 SearchProfilesResponseTypeDef = TypedDict(
     "SearchProfilesResponseTypeDef",
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredTriggerConfigTypeDef = TypedDict(
     "_RequiredTriggerConfigTypeDef",
     {
         "TriggerType": TriggerTypeType,
@@ -2391,15 +2533,15 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDomainResponseTypeDef = TypedDict(
     "GetDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -2408,15 +2550,15 @@
         "DeadLetterQueueUrl": str,
         "Stats": DomainStatsTypeDef,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "DomainName": str,
@@ -2424,15 +2566,15 @@
         "DefaultEncryptionKey": str,
         "DeadLetterQueueUrl": str,
         "Matching": MatchingResponseTypeDef,
         "RuleBasedMatching": RuleBasedMatchingResponseTypeDef,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -2481,15 +2623,15 @@
     pass
 
 ListIdentityResolutionJobsResponseTypeDef = TypedDict(
     "ListIdentityResolutionJobsResponseTypeDef",
     {
         "IdentityResolutionJobsList": List[IdentityResolutionJobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredFlowDefinitionTypeDef = TypedDict(
     "_RequiredFlowDefinitionTypeDef",
     {
         "FlowName": str,
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.28.11
-Summary: Type annotations for boto3.CustomerProfiles 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CustomerProfiles 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-customer-profiles"></a>
 
 # mypy-boto3-customer-profiles
 
 [![PyPI - mypy-boto3-customer-profiles](https://img.shields.io/pypi/v/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-customer-profiles)](https://pepy.tech/project/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,15 +349,15 @@
 
 `mypy_boto3_customer_profiles.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_customer_profiles.type_defs import (
     AddProfileKeyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfileKeyResponseTypeDef,
     AdditionalSearchKeyTypeDef,
     AddressOutputTypeDef,
     AddressTypeDef,
     BatchTypeDef,
     AppflowIntegrationWorkflowAttributesTypeDef,
     AppflowIntegrationWorkflowMetricsTypeDef,
     AppflowIntegrationWorkflowStepTypeDef,
@@ -371,105 +371,106 @@
     ConsolidationTypeDef,
     RangeOutputTypeDef,
     ThresholdOutputTypeDef,
     RangeTypeDef,
     ThresholdTypeDef,
     ConnectorOperatorTypeDef,
     CreateEventStreamRequestRequestTypeDef,
+    CreateEventStreamResponseTypeDef,
+    CreateIntegrationWorkflowResponseTypeDef,
+    CreateProfileResponseTypeDef,
     DeleteCalculatedAttributeDefinitionRequestRequestTypeDef,
     DeleteDomainRequestRequestTypeDef,
+    DeleteDomainResponseTypeDef,
     DeleteEventStreamRequestRequestTypeDef,
     DeleteIntegrationRequestRequestTypeDef,
+    DeleteIntegrationResponseTypeDef,
     DeleteProfileKeyRequestRequestTypeDef,
+    DeleteProfileKeyResponseTypeDef,
     DeleteProfileObjectRequestRequestTypeDef,
+    DeleteProfileObjectResponseTypeDef,
     DeleteProfileObjectTypeRequestRequestTypeDef,
+    DeleteProfileObjectTypeResponseTypeDef,
     DeleteProfileRequestRequestTypeDef,
+    DeleteProfileResponseTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     DestinationSummaryTypeDef,
     DomainStatsTypeDef,
     EventStreamDestinationDetailsTypeDef,
     S3ExportingConfigOutputTypeDef,
     S3ExportingConfigTypeDef,
     S3ExportingLocationTypeDef,
     FieldSourceProfileIdsTypeDef,
     FoundByKeyValueTypeDef,
+    GetAutoMergingPreviewResponseTypeDef,
     GetCalculatedAttributeDefinitionRequestRequestTypeDef,
     GetCalculatedAttributeForProfileRequestRequestTypeDef,
+    GetCalculatedAttributeForProfileResponseTypeDef,
     GetDomainRequestRequestTypeDef,
     GetEventStreamRequestRequestTypeDef,
     GetIdentityResolutionJobRequestRequestTypeDef,
     JobStatsTypeDef,
     GetIntegrationRequestRequestTypeDef,
+    GetIntegrationResponseTypeDef,
     GetMatchesRequestRequestTypeDef,
     MatchItemTypeDef,
     GetProfileObjectTypeRequestRequestTypeDef,
     ObjectTypeFieldOutputTypeDef,
     ObjectTypeKeyOutputTypeDef,
     GetProfileObjectTypeTemplateRequestRequestTypeDef,
     GetSimilarProfilesRequestRequestTypeDef,
+    GetSimilarProfilesResponseTypeDef,
     GetWorkflowRequestRequestTypeDef,
     GetWorkflowStepsRequestRequestTypeDef,
     IncrementalPullConfigTypeDef,
     JobScheduleOutputTypeDef,
     JobScheduleTypeDef,
     ListAccountIntegrationsRequestRequestTypeDef,
     ListIntegrationItemTypeDef,
     ListCalculatedAttributeDefinitionItemTypeDef,
     ListCalculatedAttributeDefinitionsRequestRequestTypeDef,
     ListCalculatedAttributeForProfileItemTypeDef,
     ListCalculatedAttributesForProfileRequestRequestTypeDef,
     ListDomainItemTypeDef,
     ListDomainsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListEventStreamsRequestRequestTypeDef,
     ListIdentityResolutionJobsRequestRequestTypeDef,
     ListIntegrationsRequestRequestTypeDef,
     ListProfileObjectTypeItemTypeDef,
     ListProfileObjectTypeTemplateItemTypeDef,
     ListProfileObjectTypeTemplatesRequestRequestTypeDef,
     ListProfileObjectTypesRequestRequestTypeDef,
     ListProfileObjectsItemTypeDef,
     ObjectFilterTypeDef,
     ListRuleBasedMatchesRequestRequestTypeDef,
+    ListRuleBasedMatchesResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListWorkflowsItemTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     MarketoSourcePropertiesTypeDef,
     MatchingRuleOutputTypeDef,
     MatchingRuleTypeDef,
+    MergeProfilesResponseTypeDef,
     ObjectTypeFieldTypeDef,
     ObjectTypeKeyTypeDef,
+    PaginatorConfigTypeDef,
+    PutIntegrationResponseTypeDef,
     PutProfileObjectRequestRequestTypeDef,
+    PutProfileObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     S3SourcePropertiesTypeDef,
     SalesforceSourcePropertiesTypeDef,
     ScheduledTriggerPropertiesTypeDef,
     ServiceNowSourcePropertiesTypeDef,
     ZendeskSourcePropertiesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAddressTypeDef,
-    AddProfileKeyResponseTypeDef,
-    CreateEventStreamResponseTypeDef,
-    CreateIntegrationWorkflowResponseTypeDef,
-    CreateProfileResponseTypeDef,
-    DeleteDomainResponseTypeDef,
-    DeleteIntegrationResponseTypeDef,
-    DeleteProfileKeyResponseTypeDef,
-    DeleteProfileObjectResponseTypeDef,
-    DeleteProfileObjectTypeResponseTypeDef,
-    DeleteProfileResponseTypeDef,
-    GetAutoMergingPreviewResponseTypeDef,
-    GetCalculatedAttributeForProfileResponseTypeDef,
-    GetIntegrationResponseTypeDef,
-    GetSimilarProfilesResponseTypeDef,
-    ListRuleBasedMatchesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    MergeProfilesResponseTypeDef,
-    PutIntegrationResponseTypeDef,
-    PutProfileObjectResponseTypeDef,
     UpdateProfileResponseTypeDef,
     SearchProfilesRequestRequestTypeDef,
     CreateProfileRequestRequestTypeDef,
     WorkflowAttributesTypeDef,
     WorkflowMetricsTypeDef,
     WorkflowStepItemTypeDef,
     AttributeDetailsOutputTypeDef,
@@ -492,15 +493,14 @@
     GetProfileObjectTypeTemplateResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     ListAccountIntegrationsResponseTypeDef,
     ListIntegrationsResponseTypeDef,
     ListCalculatedAttributeDefinitionsResponseTypeDef,
     ListCalculatedAttributesForProfileResponseTypeDef,
     ListDomainsResponseTypeDef,
-    ListEventStreamsRequestListEventStreamsPaginateTypeDef,
     ListProfileObjectTypesResponseTypeDef,
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListProfileObjectsResponseTypeDef,
     ListProfileObjectsRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
     PutProfileObjectTypeRequestRequestTypeDef,
     TriggerPropertiesTypeDef,
```

### Comparing `mypy-boto3-customer-profiles-1.28.11/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.28.12/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.28.11/setup.py` & `mypy-boto3-customer-profiles-1.28.12/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.28.11 service generated with"
-        " mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.CustomerProfiles 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

