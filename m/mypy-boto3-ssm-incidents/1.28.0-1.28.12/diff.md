# Comparing `tmp/mypy-boto3-ssm-incidents-1.28.0.tar.gz` & `tmp/mypy-boto3-ssm-incidents-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.0.tar", last modified: Thu Jul  6 21:00:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-incidents-1.28.12.tar", last modified: Thu Jul 27 11:49:42 2023, max compression
```

## Comparing `mypy-boto3-ssm-incidents-1.28.0.tar` & `mypy-boto3-ssm-incidents-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.386441 mypy-boto3-ssm-incidents-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-06 21:00:42.386441 mypy-boto3-ssm-incidents-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16784 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.386441 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-06 20:56:35.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-06 20:56:35.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33935 2023-07-06 20:56:39.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33871 2023-07-06 20:56:39.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:42.386441 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18292 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:42.000000 mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:42.386441 mypy-boto3-ssm-incidents-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-06 20:56:34.000000 mypy-boto3-ssm-incidents-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.165325 mypy-boto3-ssm-incidents-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-27 11:49:42.161325 mypy-boto3-ssm-incidents-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17261 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.153325 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25687 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25643 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38387 2023-07-27 11:47:32.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38315 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-27 11:47:31.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.161325 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:41.000000 mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:42.165325 mypy-boto3-ssm-incidents-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 11:47:30.000000 mypy-boto3-ssm-incidents-1.28.12/setup.py
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/LICENSE` & `mypy-boto3-ssm-incidents-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm-incidents
-Version: 1.28.0
-Summary: Type annotations for boto3.SSMIncidents 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,95 +389,109 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
+    ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventReferenceTypeDef,
-    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
+    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
+    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
+    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
+    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
-    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
-    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
+    CreateTimelineEventOutputTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
+    SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
+    IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
+    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
+    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/README.md` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-ssm-incidents
+Version: 1.28.12
+Summary: Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,95 +389,109 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
+    ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventReferenceTypeDef,
-    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
+    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
+    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
+    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
+    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
-    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
-    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
+    CreateTimelineEventOutputTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
+    SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
+    IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
+    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
+    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__init__.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__init__.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/__main__.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSMIncidents 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SSMIncidents 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents\nOther"
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

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/client.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/client.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/literals.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -273,26 +274,28 @@
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

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/literals.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -271,26 +272,28 @@
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

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/paginator.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
         """
 
 
@@ -93,60 +93,60 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 
 class ListRelatedItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
     """
 
     def paginate(
-        self, *, incidentRecordArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, incidentRecordArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRelatedItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
         """
 
 
 class ListReplicationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReplicationSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
         """
 
 
 class ListResponsePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResponsePlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
         """
 
 
@@ -159,13 +159,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/paginator.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 class GetResourcePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetResourcePoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#getresourcepoliciespaginator)
         """
 
 class ListIncidentRecordsPaginator(Paginator):
@@ -88,57 +88,57 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIncidentRecordsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listincidentrecordspaginator)
         """
 
 class ListRelatedItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
     """
 
     def paginate(
-        self, *, incidentRecordArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, incidentRecordArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRelatedItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listrelateditemspaginator)
         """
 
 class ListReplicationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReplicationSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listreplicationsetspaginator)
         """
 
 class ListResponsePlansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResponsePlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listresponseplanspaginator)
         """
 
 class ListTimelineEventsPaginator(Paginator):
@@ -150,13 +150,13 @@
     def paginate(
         self,
         *,
         incidentRecordArn: str,
         filters: Sequence[FilterTypeDef] = ...,
         sortBy: Literal["EVENT_TIME"] = ...,
         sortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTimelineEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/paginators/#listtimelineeventspaginator)
         """
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/type_defs.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -30,100 +30,113 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
+    "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
-    "CreateReplicationSetOutputTypeDef",
-    "CreateResponsePlanOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
-    "CreateTimelineEventOutputTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
+    "DynamicSsmParameterValueOutputTypeDef",
     "DynamicSsmParameterValueTypeDef",
+    "EventReferenceOutputTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
+    "NotificationTargetItemOutputTypeDef",
     "NotificationTargetItemTypeDef",
+    "PagerDutyIncidentDetailOutputTypeDef",
     "PagerDutyIncidentDetailTypeDef",
-    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
-    "ListReplicationSetsOutputTypeDef",
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PagerDutyIncidentConfigurationOutputTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
     "RegionInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "TriggerDetailsTypeDef",
-    "StartIncidentOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
     "ConditionTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
+    "CreateReplicationSetOutputTypeDef",
+    "CreateResponsePlanOutputTypeDef",
+    "CreateTimelineEventOutputTypeDef",
+    "ListReplicationSetsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
-    "EventSummaryTypeDef",
-    "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
+    "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
+    "EventSummaryTypeDef",
+    "TimelineEventTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
+    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
+    "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
+    "ItemValueOutputTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
+    "PagerDutyConfigurationOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
-    "ListTimelineEventsOutputTypeDef",
-    "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "ListTimelineEventsOutputTypeDef",
+    "GetTimelineEventOutputTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
+    "ItemIdentifierOutputTypeDef",
     "ItemIdentifierTypeDef",
+    "IntegrationOutputTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "RelatedItemOutputTypeDef",
     "RelatedItemTypeDef",
-    "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
+    "CreateResponsePlanInputRequestTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -137,19 +150,17 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
-
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -159,14 +170,23 @@
     "AutomationExecutionTypeDef",
     {
         "ssmExecutionArn": str,
     },
     total=False,
 )
 
+ChatChannelOutputTypeDef = TypedDict(
+    "ChatChannelOutputTypeDef",
+    {
+        "chatbotSns": List[str],
+        "empty": Dict[str, Any],
+    },
+    total=False,
+)
+
 ChatChannelTypeDef = TypedDict(
     "ChatChannelTypeDef",
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
@@ -176,48 +196,34 @@
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-CreateReplicationSetOutputTypeDef = TypedDict(
-    "CreateReplicationSetOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResponsePlanOutputTypeDef = TypedDict(
-    "CreateResponsePlanOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EventReferenceTypeDef = TypedDict(
     "EventReferenceTypeDef",
     {
         "relatedItemId": str,
         "resource": str,
     },
     total=False,
 )
 
-CreateTimelineEventOutputTypeDef = TypedDict(
-    "CreateTimelineEventOutputTypeDef",
-    {
-        "eventId": str,
-        "incidentRecordArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIncidentRecordInputRequestTypeDef = TypedDict(
     "DeleteIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -254,22 +260,39 @@
     "DeleteTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 
+DynamicSsmParameterValueOutputTypeDef = TypedDict(
+    "DynamicSsmParameterValueOutputTypeDef",
+    {
+        "variable": VariableTypeType,
+    },
+    total=False,
+)
+
 DynamicSsmParameterValueTypeDef = TypedDict(
     "DynamicSsmParameterValueTypeDef",
     {
         "variable": VariableTypeType,
     },
     total=False,
 )
 
+EventReferenceOutputTypeDef = TypedDict(
+    "EventReferenceOutputTypeDef",
+    {
+        "relatedItemId": str,
+        "resource": str,
+    },
+    total=False,
+)
+
 GetIncidentRecordInputRequestTypeDef = TypedDict(
     "GetIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -285,36 +308,24 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
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
-class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourcePoliciesInputRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputRequestTypeDef = TypedDict(
@@ -322,21 +333,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
-
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -369,73 +378,75 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
-
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
+NotificationTargetItemOutputTypeDef = TypedDict(
+    "NotificationTargetItemOutputTypeDef",
+    {
+        "snsTopicArn": str,
+    },
+    total=False,
+)
 
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
-    "_RequiredPagerDutyIncidentDetailTypeDef",
+_RequiredPagerDutyIncidentDetailOutputTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailOutputTypeDef",
     {
         "id": str,
     },
 )
-_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
-    "_OptionalPagerDutyIncidentDetailTypeDef",
+_OptionalPagerDutyIncidentDetailOutputTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailOutputTypeDef",
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
-
-class PagerDutyIncidentDetailTypeDef(
-    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
+class PagerDutyIncidentDetailOutputTypeDef(
+    _RequiredPagerDutyIncidentDetailOutputTypeDef, _OptionalPagerDutyIncidentDetailOutputTypeDef
 ):
     pass
 
-
-_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailTypeDef",
     {
-        "incidentRecordArn": str,
+        "id": str,
     },
 )
-_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "autoResolve": bool,
+        "secretId": str,
     },
     total=False,
 )
 
-
-class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
-    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+class PagerDutyIncidentDetailTypeDef(
+    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
-
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -443,55 +454,28 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
-
-ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListReplicationSetsOutputTypeDef = TypedDict(
-    "ListReplicationSetsOutputTypeDef",
-    {
-        "nextToken": str,
-        "replicationSetArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResponsePlansInputRequestTypeDef = TypedDict(
     "ListResponsePlansInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -508,69 +492,48 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
-
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+PagerDutyIncidentConfigurationOutputTypeDef = TypedDict(
+    "PagerDutyIncidentConfigurationOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serviceId": str,
     },
 )
 
 PagerDutyIncidentConfigurationTypeDef = TypedDict(
     "PagerDutyIncidentConfigurationTypeDef",
     {
         "serviceId": str,
     },
 )
 
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
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "policyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegionInfoTypeDef = TypedDict(
     "_RequiredRegionInfoTypeDef",
     {
         "status": RegionStatusType,
         "statusUpdateDateTime": datetime,
     },
 )
@@ -579,30 +542,17 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
-
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
-
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
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
 )
@@ -611,27 +561,17 @@
     {
         "rawData": str,
         "triggerArn": str,
     },
     total=False,
 )
 
-
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
-
-StartIncidentOutputTypeDef = TypedDict(
-    "StartIncidentOutputTypeDef",
-    {
-        "incidentRecordArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -655,22 +595,20 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
-
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": Union[datetime, str],
         "before": Union[datetime, str],
         "equals": AttributeValueListTypeDef,
     },
@@ -688,94 +626,101 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTimelineEventInputRequestTypeDef",
+CreateReplicationSetOutputTypeDef = TypedDict(
+    "CreateReplicationSetOutputTypeDef",
     {
-        "eventData": str,
-        "eventTime": Union[datetime, str],
-        "eventType": str,
-        "incidentRecordArn": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTimelineEventInputRequestTypeDef",
+
+CreateResponsePlanOutputTypeDef = TypedDict(
+    "CreateResponsePlanOutputTypeDef",
     {
-        "clientToken": str,
-        "eventReferences": Sequence[EventReferenceTypeDef],
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateTimelineEventInputRequestTypeDef(
-    _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
-):
-    pass
-
-
-_RequiredEventSummaryTypeDef = TypedDict(
-    "_RequiredEventSummaryTypeDef",
+CreateTimelineEventOutputTypeDef = TypedDict(
+    "CreateTimelineEventOutputTypeDef",
     {
         "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
         "incidentRecordArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEventSummaryTypeDef = TypedDict(
-    "_OptionalEventSummaryTypeDef",
+
+ListReplicationSetsOutputTypeDef = TypedDict(
+    "ListReplicationSetsOutputTypeDef",
     {
-        "eventReferences": List[EventReferenceTypeDef],
+        "nextToken": str,
+        "replicationSetArns": List[str],
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
 
-class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
-    pass
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "policyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartIncidentOutputTypeDef = TypedDict(
+    "StartIncidentOutputTypeDef",
+    {
+        "incidentRecordArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredTimelineEventTypeDef = TypedDict(
-    "_RequiredTimelineEventTypeDef",
+_RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
-        "eventId": str,
-        "eventTime": datetime,
+        "eventTime": Union[datetime, str],
         "eventType": str,
-        "eventUpdatedTime": datetime,
         "incidentRecordArn": str,
     },
 )
-_OptionalTimelineEventTypeDef = TypedDict(
-    "_OptionalTimelineEventTypeDef",
+_OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTimelineEventInputRequestTypeDef",
     {
-        "eventReferences": List[EventReferenceTypeDef],
+        "clientToken": str,
+        "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
-
-class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+class CreateTimelineEventInputRequestTypeDef(
+    _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
+):
     pass
 
-
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
@@ -787,30 +732,51 @@
         "eventReferences": Sequence[EventReferenceTypeDef],
         "eventTime": Union[datetime, str],
         "eventType": str,
     },
     total=False,
 )
 
-
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
-
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
 )
 
+_RequiredSsmAutomationOutputTypeDef = TypedDict(
+    "_RequiredSsmAutomationOutputTypeDef",
+    {
+        "documentName": str,
+        "roleArn": str,
+    },
+)
+_OptionalSsmAutomationOutputTypeDef = TypedDict(
+    "_OptionalSsmAutomationOutputTypeDef",
+    {
+        "documentVersion": str,
+        "dynamicParameters": Dict[str, DynamicSsmParameterValueOutputTypeDef],
+        "parameters": Dict[str, List[str]],
+        "targetAccount": SsmTargetAccountType,
+    },
+    total=False,
+)
+
+class SsmAutomationOutputTypeDef(
+    _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
+):
+    pass
+
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -821,18 +787,59 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
-
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
+_RequiredEventSummaryTypeDef = TypedDict(
+    "_RequiredEventSummaryTypeDef",
+    {
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalEventSummaryTypeDef = TypedDict(
+    "_OptionalEventSummaryTypeDef",
+    {
+        "eventReferences": List[EventReferenceOutputTypeDef],
+    },
+    total=False,
+)
+
+class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
+    pass
+
+_RequiredTimelineEventTypeDef = TypedDict(
+    "_RequiredTimelineEventTypeDef",
+    {
+        "eventData": str,
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalTimelineEventTypeDef = TypedDict(
+    "_OptionalTimelineEventTypeDef",
+    {
+        "eventReferences": List[EventReferenceOutputTypeDef],
+    },
+    total=False,
+)
+
+class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+    pass
 
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
@@ -840,50 +847,102 @@
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
+_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "incidentRecordArn": str,
+    },
+)
+_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
+    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+):
+    pass
+
+ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 GetResourcePoliciesOutputTypeDef = TypedDict(
     "GetResourcePoliciesOutputTypeDef",
     {
         "nextToken": str,
         "resourcePolicies": List[ResourcePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncidentRecordSummaryTypeDef = TypedDict(
     "_RequiredIncidentRecordSummaryTypeDef",
     {
         "arn": str,
@@ -898,21 +957,19 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
-
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
-
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -923,26 +980,47 @@
         "title": str,
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
-        "chatChannel": ChatChannelTypeDef,
-        "notificationTargets": List[NotificationTargetItemTypeDef],
+        "chatChannel": ChatChannelOutputTypeDef,
+        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
+_RequiredIncidentTemplateOutputTypeDef = TypedDict(
+    "_RequiredIncidentTemplateOutputTypeDef",
+    {
+        "impact": int,
+        "title": str,
+    },
+)
+_OptionalIncidentTemplateOutputTypeDef = TypedDict(
+    "_OptionalIncidentTemplateOutputTypeDef",
+    {
+        "dedupeString": str,
+        "incidentTags": Dict[str, str],
+        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "summary": str,
+    },
+    total=False,
+)
+
+class IncidentTemplateOutputTypeDef(
+    _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
+):
+    pass
 
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
@@ -954,19 +1032,17 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
-
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
-
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -979,21 +1055,30 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
-
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
+ItemValueOutputTypeDef = TypedDict(
+    "ItemValueOutputTypeDef",
+    {
+        "arn": str,
+        "metricDefinition": str,
+        "pagerDutyIncidentDetail": PagerDutyIncidentDetailOutputTypeDef,
+        "url": str,
+    },
+    total=False,
+)
 
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
@@ -1003,15 +1088,24 @@
 )
 
 ListResponsePlansOutputTypeDef = TypedDict(
     "ListResponsePlansOutputTypeDef",
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PagerDutyConfigurationOutputTypeDef = TypedDict(
+    "PagerDutyConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationOutputTypeDef,
+        "secretId": str,
     },
 )
 
 PagerDutyConfigurationTypeDef = TypedDict(
     "PagerDutyConfigurationTypeDef",
     {
         "name": str,
@@ -1036,44 +1130,25 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
-
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
 
-ListTimelineEventsOutputTypeDef = TypedDict(
-    "ListTimelineEventsOutputTypeDef",
-    {
-        "eventSummaries": List[EventSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTimelineEventOutputTypeDef = TypedDict(
-    "GetTimelineEventOutputTypeDef",
-    {
-        "event": TimelineEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
         "arn": str,
     },
 )
@@ -1081,76 +1156,115 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ssmAutomation": SsmAutomationOutputTypeDef,
+    },
+    total=False,
+)
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
 
+ListTimelineEventsOutputTypeDef = TypedDict(
+    "ListTimelineEventsOutputTypeDef",
+    {
+        "eventSummaries": List[EventSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTimelineEventOutputTypeDef = TypedDict(
+    "GetTimelineEventOutputTypeDef",
+    {
+        "event": TimelineEventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIncidentRecordOutputTypeDef = TypedDict(
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ItemIdentifierOutputTypeDef = TypedDict(
+    "ItemIdentifierOutputTypeDef",
+    {
+        "type": ItemTypeType,
+        "value": ItemValueOutputTypeDef,
     },
 )
 
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
 
+IntegrationOutputTypeDef = TypedDict(
+    "IntegrationOutputTypeDef",
+    {
+        "pagerDutyConfiguration": PagerDutyConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
 
 GetReplicationSetOutputTypeDef = TypedDict(
     "GetReplicationSetOutputTypeDef",
     {
         "replicationSet": ReplicationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef = TypedDict(
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListIncidentRecordsInputRequestTypeDef = TypedDict(
     "ListIncidentRecordsInputRequestTypeDef",
     {
@@ -1169,27 +1283,25 @@
 )
 _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef = TypedDict(
     "_OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1200,20 +1312,38 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
-
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
+_RequiredRelatedItemOutputTypeDef = TypedDict(
+    "_RequiredRelatedItemOutputTypeDef",
+    {
+        "identifier": ItemIdentifierOutputTypeDef,
+    },
+)
+_OptionalRelatedItemOutputTypeDef = TypedDict(
+    "_OptionalRelatedItemOutputTypeDef",
+    {
+        "generatedId": str,
+        "title": str,
+    },
+    total=False,
+)
+
+class RelatedItemOutputTypeDef(
+    _RequiredRelatedItemOutputTypeDef, _OptionalRelatedItemOutputTypeDef
+):
+    pass
 
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
@@ -1222,18 +1352,31 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
-
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationOutputTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
@@ -1248,36 +1391,19 @@
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
-
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateResponsePlanInputRequestTypeDef = TypedDict(
@@ -1295,27 +1421,25 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
-
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
-        "relatedItems": List[RelatedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "relatedItems": List[RelatedItemOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
         "itemToAdd": RelatedItemTypeDef,
@@ -1338,21 +1462,19 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1360,12 +1482,11 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/type_defs.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,99 +30,114 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddRegionActionTypeDef",
     "AttributeValueListTypeDef",
     "AutomationExecutionTypeDef",
+    "ChatChannelOutputTypeDef",
     "ChatChannelTypeDef",
     "RegionMapInputValueTypeDef",
-    "CreateReplicationSetOutputTypeDef",
-    "CreateResponsePlanOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventReferenceTypeDef",
-    "CreateTimelineEventOutputTypeDef",
     "DeleteIncidentRecordInputRequestTypeDef",
     "DeleteRegionActionTypeDef",
     "DeleteReplicationSetInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteResponsePlanInputRequestTypeDef",
     "DeleteTimelineEventInputRequestTypeDef",
+    "DynamicSsmParameterValueOutputTypeDef",
     "DynamicSsmParameterValueTypeDef",
+    "EventReferenceOutputTypeDef",
     "GetIncidentRecordInputRequestTypeDef",
     "GetReplicationSetInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetResourcePoliciesInputRequestTypeDef",
     "ResourcePolicyTypeDef",
     "GetResponsePlanInputRequestTypeDef",
     "GetTimelineEventInputRequestTypeDef",
     "IncidentRecordSourceTypeDef",
+    "NotificationTargetItemOutputTypeDef",
     "NotificationTargetItemTypeDef",
+    "PagerDutyIncidentDetailOutputTypeDef",
     "PagerDutyIncidentDetailTypeDef",
-    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
     "ListRelatedItemsInputRequestTypeDef",
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
     "ListReplicationSetsInputRequestTypeDef",
-    "ListReplicationSetsOutputTypeDef",
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "ListResponsePlansInputRequestTypeDef",
     "ResponsePlanSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "PagerDutyIncidentConfigurationOutputTypeDef",
     "PagerDutyIncidentConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyInputRequestTypeDef",
-    "PutResourcePolicyOutputTypeDef",
     "RegionInfoTypeDef",
-    "ResponseMetadataTypeDef",
     "TriggerDetailsTypeDef",
-    "StartIncidentOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeletionProtectionInputRequestTypeDef",
     "ConditionTypeDef",
     "CreateReplicationSetInputRequestTypeDef",
+    "CreateReplicationSetOutputTypeDef",
+    "CreateResponsePlanOutputTypeDef",
+    "CreateTimelineEventOutputTypeDef",
+    "ListReplicationSetsOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutResourcePolicyOutputTypeDef",
+    "StartIncidentOutputTypeDef",
     "CreateTimelineEventInputRequestTypeDef",
-    "EventSummaryTypeDef",
-    "TimelineEventTypeDef",
     "UpdateTimelineEventInputRequestTypeDef",
     "UpdateReplicationSetActionTypeDef",
+    "SsmAutomationOutputTypeDef",
     "SsmAutomationTypeDef",
+    "EventSummaryTypeDef",
+    "TimelineEventTypeDef",
     "GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     "GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
+    "GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    "ListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
     "GetResourcePoliciesOutputTypeDef",
     "IncidentRecordSummaryTypeDef",
     "IncidentRecordTypeDef",
+    "IncidentTemplateOutputTypeDef",
     "IncidentTemplateTypeDef",
     "UpdateIncidentRecordInputRequestTypeDef",
+    "ItemValueOutputTypeDef",
     "ItemValueTypeDef",
     "ListResponsePlansOutputTypeDef",
+    "PagerDutyConfigurationOutputTypeDef",
     "PagerDutyConfigurationTypeDef",
     "ReplicationSetTypeDef",
     "FilterTypeDef",
-    "ListTimelineEventsOutputTypeDef",
-    "GetTimelineEventOutputTypeDef",
     "UpdateReplicationSetInputRequestTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
+    "ListTimelineEventsOutputTypeDef",
+    "GetTimelineEventOutputTypeDef",
     "ListIncidentRecordsOutputTypeDef",
     "GetIncidentRecordOutputTypeDef",
+    "ItemIdentifierOutputTypeDef",
     "ItemIdentifierTypeDef",
+    "IntegrationOutputTypeDef",
     "IntegrationTypeDef",
     "GetReplicationSetOutputTypeDef",
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     "ListIncidentRecordsInputRequestTypeDef",
     "ListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     "ListTimelineEventsInputRequestTypeDef",
+    "RelatedItemOutputTypeDef",
     "RelatedItemTypeDef",
-    "CreateResponsePlanInputRequestTypeDef",
     "GetResponsePlanOutputTypeDef",
+    "CreateResponsePlanInputRequestTypeDef",
     "UpdateResponsePlanInputRequestTypeDef",
     "ListRelatedItemsOutputTypeDef",
     "RelatedItemsUpdateTypeDef",
     "StartIncidentInputRequestTypeDef",
     "UpdateRelatedItemsInputRequestTypeDef",
 )
 
@@ -136,17 +151,19 @@
     "_OptionalAddRegionActionTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
+
 class AddRegionActionTypeDef(_RequiredAddRegionActionTypeDef, _OptionalAddRegionActionTypeDef):
     pass
 
+
 AttributeValueListTypeDef = TypedDict(
     "AttributeValueListTypeDef",
     {
         "integerValues": Sequence[int],
         "stringValues": Sequence[str],
     },
     total=False,
@@ -156,14 +173,23 @@
     "AutomationExecutionTypeDef",
     {
         "ssmExecutionArn": str,
     },
     total=False,
 )
 
+ChatChannelOutputTypeDef = TypedDict(
+    "ChatChannelOutputTypeDef",
+    {
+        "chatbotSns": List[str],
+        "empty": Dict[str, Any],
+    },
+    total=False,
+)
+
 ChatChannelTypeDef = TypedDict(
     "ChatChannelTypeDef",
     {
         "chatbotSns": Sequence[str],
         "empty": Mapping[str, Any],
     },
     total=False,
@@ -173,48 +199,34 @@
     "RegionMapInputValueTypeDef",
     {
         "sseKmsKeyId": str,
     },
     total=False,
 )
 
-CreateReplicationSetOutputTypeDef = TypedDict(
-    "CreateReplicationSetOutputTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateResponsePlanOutputTypeDef = TypedDict(
-    "CreateResponsePlanOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EventReferenceTypeDef = TypedDict(
     "EventReferenceTypeDef",
     {
         "relatedItemId": str,
         "resource": str,
     },
     total=False,
 )
 
-CreateTimelineEventOutputTypeDef = TypedDict(
-    "CreateTimelineEventOutputTypeDef",
-    {
-        "eventId": str,
-        "incidentRecordArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIncidentRecordInputRequestTypeDef = TypedDict(
     "DeleteIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -251,22 +263,39 @@
     "DeleteTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
 
+DynamicSsmParameterValueOutputTypeDef = TypedDict(
+    "DynamicSsmParameterValueOutputTypeDef",
+    {
+        "variable": VariableTypeType,
+    },
+    total=False,
+)
+
 DynamicSsmParameterValueTypeDef = TypedDict(
     "DynamicSsmParameterValueTypeDef",
     {
         "variable": VariableTypeType,
     },
     total=False,
 )
 
+EventReferenceOutputTypeDef = TypedDict(
+    "EventReferenceOutputTypeDef",
+    {
+        "relatedItemId": str,
+        "resource": str,
+    },
+    total=False,
+)
+
 GetIncidentRecordInputRequestTypeDef = TypedDict(
     "GetIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -282,34 +311,24 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
-    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
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
 
-class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
-    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourcePoliciesInputRequestTypeDef = TypedDict(
     "_RequiredGetResourcePoliciesInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalGetResourcePoliciesInputRequestTypeDef = TypedDict(
@@ -317,19 +336,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class GetResourcePoliciesInputRequestTypeDef(
     _RequiredGetResourcePoliciesInputRequestTypeDef, _OptionalGetResourcePoliciesInputRequestTypeDef
 ):
     pass
 
+
 ResourcePolicyTypeDef = TypedDict(
     "ResourcePolicyTypeDef",
     {
         "policyDocument": str,
         "policyId": str,
         "ramResourceShareRegion": str,
     },
@@ -362,67 +383,81 @@
     {
         "invokedBy": str,
         "resourceArn": str,
     },
     total=False,
 )
 
+
 class IncidentRecordSourceTypeDef(
     _RequiredIncidentRecordSourceTypeDef, _OptionalIncidentRecordSourceTypeDef
 ):
     pass
 
+
+NotificationTargetItemOutputTypeDef = TypedDict(
+    "NotificationTargetItemOutputTypeDef",
+    {
+        "snsTopicArn": str,
+    },
+    total=False,
+)
+
 NotificationTargetItemTypeDef = TypedDict(
     "NotificationTargetItemTypeDef",
     {
         "snsTopicArn": str,
     },
     total=False,
 )
 
-_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
-    "_RequiredPagerDutyIncidentDetailTypeDef",
+_RequiredPagerDutyIncidentDetailOutputTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailOutputTypeDef",
     {
         "id": str,
     },
 )
-_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
-    "_OptionalPagerDutyIncidentDetailTypeDef",
+_OptionalPagerDutyIncidentDetailOutputTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailOutputTypeDef",
     {
         "autoResolve": bool,
         "secretId": str,
     },
     total=False,
 )
 
-class PagerDutyIncidentDetailTypeDef(
-    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
+
+class PagerDutyIncidentDetailOutputTypeDef(
+    _RequiredPagerDutyIncidentDetailOutputTypeDef, _OptionalPagerDutyIncidentDetailOutputTypeDef
 ):
     pass
 
-_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+
+_RequiredPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_RequiredPagerDutyIncidentDetailTypeDef",
     {
-        "incidentRecordArn": str,
+        "id": str,
     },
 )
-_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+_OptionalPagerDutyIncidentDetailTypeDef = TypedDict(
+    "_OptionalPagerDutyIncidentDetailTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "autoResolve": bool,
+        "secretId": str,
     },
     total=False,
 )
 
-class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
-    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
-    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+
+class PagerDutyIncidentDetailTypeDef(
+    _RequiredPagerDutyIncidentDetailTypeDef, _OptionalPagerDutyIncidentDetailTypeDef
 ):
     pass
 
+
 _RequiredListRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredListRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListRelatedItemsInputRequestTypeDef = TypedDict(
@@ -430,53 +465,30 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRelatedItemsInputRequestTypeDef(
     _RequiredListRelatedItemsInputRequestTypeDef, _OptionalListRelatedItemsInputRequestTypeDef
 ):
     pass
 
-ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
-    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListReplicationSetsInputRequestTypeDef = TypedDict(
     "ListReplicationSetsInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListReplicationSetsOutputTypeDef = TypedDict(
-    "ListReplicationSetsOutputTypeDef",
-    {
-        "nextToken": str,
-        "replicationSetArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
-    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResponsePlansInputRequestTypeDef = TypedDict(
     "ListResponsePlansInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -493,67 +505,50 @@
     "_OptionalResponsePlanSummaryTypeDef",
     {
         "displayName": str,
     },
     total=False,
 )
 
+
 class ResponsePlanSummaryTypeDef(
     _RequiredResponsePlanSummaryTypeDef, _OptionalResponsePlanSummaryTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+PagerDutyIncidentConfigurationOutputTypeDef = TypedDict(
+    "PagerDutyIncidentConfigurationOutputTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "serviceId": str,
     },
 )
 
 PagerDutyIncidentConfigurationTypeDef = TypedDict(
     "PagerDutyIncidentConfigurationTypeDef",
     {
         "serviceId": str,
     },
 )
 
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
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
 
-PutResourcePolicyOutputTypeDef = TypedDict(
-    "PutResourcePolicyOutputTypeDef",
-    {
-        "policyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegionInfoTypeDef = TypedDict(
     "_RequiredRegionInfoTypeDef",
     {
         "status": RegionStatusType,
         "statusUpdateDateTime": datetime,
     },
 )
@@ -562,27 +557,18 @@
     {
         "sseKmsKeyId": str,
         "statusMessage": str,
     },
     total=False,
 )
 
+
 class RegionInfoTypeDef(_RequiredRegionInfoTypeDef, _OptionalRegionInfoTypeDef):
     pass
 
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
 
 _RequiredTriggerDetailsTypeDef = TypedDict(
     "_RequiredTriggerDetailsTypeDef",
     {
         "source": str,
         "timestamp": Union[datetime, str],
     },
@@ -592,24 +578,18 @@
     {
         "rawData": str,
         "triggerArn": str,
     },
     total=False,
 )
 
+
 class TriggerDetailsTypeDef(_RequiredTriggerDetailsTypeDef, _OptionalTriggerDetailsTypeDef):
     pass
 
-StartIncidentOutputTypeDef = TypedDict(
-    "StartIncidentOutputTypeDef",
-    {
-        "incidentRecordArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
@@ -634,20 +614,22 @@
     "_OptionalUpdateDeletionProtectionInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDeletionProtectionInputRequestTypeDef(
     _RequiredUpdateDeletionProtectionInputRequestTypeDef,
     _OptionalUpdateDeletionProtectionInputRequestTypeDef,
 ):
     pass
 
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "after": Union[datetime, str],
         "before": Union[datetime, str],
         "equals": AttributeValueListTypeDef,
     },
@@ -665,86 +647,105 @@
     {
         "clientToken": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateReplicationSetInputRequestTypeDef(
     _RequiredCreateReplicationSetInputRequestTypeDef,
     _OptionalCreateReplicationSetInputRequestTypeDef,
 ):
     pass
 
-_RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTimelineEventInputRequestTypeDef",
+
+CreateReplicationSetOutputTypeDef = TypedDict(
+    "CreateReplicationSetOutputTypeDef",
     {
-        "eventData": str,
-        "eventTime": Union[datetime, str],
-        "eventType": str,
-        "incidentRecordArn": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTimelineEventInputRequestTypeDef",
+
+CreateResponsePlanOutputTypeDef = TypedDict(
+    "CreateResponsePlanOutputTypeDef",
     {
-        "clientToken": str,
-        "eventReferences": Sequence[EventReferenceTypeDef],
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateTimelineEventInputRequestTypeDef(
-    _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
-):
-    pass
-
-_RequiredEventSummaryTypeDef = TypedDict(
-    "_RequiredEventSummaryTypeDef",
+CreateTimelineEventOutputTypeDef = TypedDict(
+    "CreateTimelineEventOutputTypeDef",
     {
         "eventId": str,
-        "eventTime": datetime,
-        "eventType": str,
-        "eventUpdatedTime": datetime,
         "incidentRecordArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEventSummaryTypeDef = TypedDict(
-    "_OptionalEventSummaryTypeDef",
+
+ListReplicationSetsOutputTypeDef = TypedDict(
+    "ListReplicationSetsOutputTypeDef",
     {
-        "eventReferences": List[EventReferenceTypeDef],
+        "nextToken": str,
+        "replicationSetArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
-    pass
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredTimelineEventTypeDef = TypedDict(
-    "_RequiredTimelineEventTypeDef",
+PutResourcePolicyOutputTypeDef = TypedDict(
+    "PutResourcePolicyOutputTypeDef",
+    {
+        "policyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartIncidentOutputTypeDef = TypedDict(
+    "StartIncidentOutputTypeDef",
+    {
+        "incidentRecordArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateTimelineEventInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTimelineEventInputRequestTypeDef",
     {
         "eventData": str,
-        "eventId": str,
-        "eventTime": datetime,
+        "eventTime": Union[datetime, str],
         "eventType": str,
-        "eventUpdatedTime": datetime,
         "incidentRecordArn": str,
     },
 )
-_OptionalTimelineEventTypeDef = TypedDict(
-    "_OptionalTimelineEventTypeDef",
+_OptionalCreateTimelineEventInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTimelineEventInputRequestTypeDef",
     {
-        "eventReferences": List[EventReferenceTypeDef],
+        "clientToken": str,
+        "eventReferences": Sequence[EventReferenceTypeDef],
     },
     total=False,
 )
 
-class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+
+class CreateTimelineEventInputRequestTypeDef(
+    _RequiredCreateTimelineEventInputRequestTypeDef, _OptionalCreateTimelineEventInputRequestTypeDef
+):
     pass
 
+
 _RequiredUpdateTimelineEventInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTimelineEventInputRequestTypeDef",
     {
         "eventId": str,
         "incidentRecordArn": str,
     },
 )
@@ -756,28 +757,55 @@
         "eventReferences": Sequence[EventReferenceTypeDef],
         "eventTime": Union[datetime, str],
         "eventType": str,
     },
     total=False,
 )
 
+
 class UpdateTimelineEventInputRequestTypeDef(
     _RequiredUpdateTimelineEventInputRequestTypeDef, _OptionalUpdateTimelineEventInputRequestTypeDef
 ):
     pass
 
+
 UpdateReplicationSetActionTypeDef = TypedDict(
     "UpdateReplicationSetActionTypeDef",
     {
         "addRegionAction": AddRegionActionTypeDef,
         "deleteRegionAction": DeleteRegionActionTypeDef,
     },
     total=False,
 )
 
+_RequiredSsmAutomationOutputTypeDef = TypedDict(
+    "_RequiredSsmAutomationOutputTypeDef",
+    {
+        "documentName": str,
+        "roleArn": str,
+    },
+)
+_OptionalSsmAutomationOutputTypeDef = TypedDict(
+    "_OptionalSsmAutomationOutputTypeDef",
+    {
+        "documentVersion": str,
+        "dynamicParameters": Dict[str, DynamicSsmParameterValueOutputTypeDef],
+        "parameters": Dict[str, List[str]],
+        "targetAccount": SsmTargetAccountType,
+    },
+    total=False,
+)
+
+
+class SsmAutomationOutputTypeDef(
+    _RequiredSsmAutomationOutputTypeDef, _OptionalSsmAutomationOutputTypeDef
+):
+    pass
+
+
 _RequiredSsmAutomationTypeDef = TypedDict(
     "_RequiredSsmAutomationTypeDef",
     {
         "documentName": str,
         "roleArn": str,
     },
 )
@@ -788,63 +816,176 @@
         "dynamicParameters": Mapping[str, DynamicSsmParameterValueTypeDef],
         "parameters": Mapping[str, Sequence[str]],
         "targetAccount": SsmTargetAccountType,
     },
     total=False,
 )
 
+
 class SsmAutomationTypeDef(_RequiredSsmAutomationTypeDef, _OptionalSsmAutomationTypeDef):
     pass
 
+
+_RequiredEventSummaryTypeDef = TypedDict(
+    "_RequiredEventSummaryTypeDef",
+    {
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalEventSummaryTypeDef = TypedDict(
+    "_OptionalEventSummaryTypeDef",
+    {
+        "eventReferences": List[EventReferenceOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class EventSummaryTypeDef(_RequiredEventSummaryTypeDef, _OptionalEventSummaryTypeDef):
+    pass
+
+
+_RequiredTimelineEventTypeDef = TypedDict(
+    "_RequiredTimelineEventTypeDef",
+    {
+        "eventData": str,
+        "eventId": str,
+        "eventTime": datetime,
+        "eventType": str,
+        "eventUpdatedTime": datetime,
+        "incidentRecordArn": str,
+    },
+)
+_OptionalTimelineEventTypeDef = TypedDict(
+    "_OptionalTimelineEventTypeDef",
+    {
+        "eventReferences": List[EventReferenceOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class TimelineEventTypeDef(_RequiredTimelineEventTypeDef, _OptionalTimelineEventTypeDef):
+    pass
+
+
 _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef = TypedDict(
     "_OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef(
     _RequiredGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
     _OptionalGetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
 ):
     pass
 
+
+_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef = TypedDict(
+    "_OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef(
+    _RequiredGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    _OptionalGetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "incidentRecordArn": str,
+    },
+)
+_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRelatedItemsInputListRelatedItemsPaginateTypeDef(
+    _RequiredListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    _OptionalListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+):
+    pass
+
+
+ListReplicationSetsInputListReplicationSetsPaginateTypeDef = TypedDict(
+    "ListReplicationSetsInputListReplicationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResponsePlansInputListResponsePlansPaginateTypeDef = TypedDict(
+    "ListResponsePlansInputListResponsePlansPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetResourcePoliciesOutputTypeDef = TypedDict(
     "GetResourcePoliciesOutputTypeDef",
     {
         "nextToken": str,
         "resourcePolicies": List[ResourcePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncidentRecordSummaryTypeDef = TypedDict(
     "_RequiredIncidentRecordSummaryTypeDef",
     {
         "arn": str,
@@ -859,19 +1000,21 @@
     "_OptionalIncidentRecordSummaryTypeDef",
     {
         "resolvedTime": datetime,
     },
     total=False,
 )
 
+
 class IncidentRecordSummaryTypeDef(
     _RequiredIncidentRecordSummaryTypeDef, _OptionalIncidentRecordSummaryTypeDef
 ):
     pass
 
+
 _RequiredIncidentRecordTypeDef = TypedDict(
     "_RequiredIncidentRecordTypeDef",
     {
         "arn": str,
         "creationTime": datetime,
         "dedupeString": str,
         "impact": int,
@@ -882,25 +1025,52 @@
         "title": str,
     },
 )
 _OptionalIncidentRecordTypeDef = TypedDict(
     "_OptionalIncidentRecordTypeDef",
     {
         "automationExecutions": List[AutomationExecutionTypeDef],
-        "chatChannel": ChatChannelTypeDef,
-        "notificationTargets": List[NotificationTargetItemTypeDef],
+        "chatChannel": ChatChannelOutputTypeDef,
+        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
         "resolvedTime": datetime,
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentRecordTypeDef(_RequiredIncidentRecordTypeDef, _OptionalIncidentRecordTypeDef):
     pass
 
+
+_RequiredIncidentTemplateOutputTypeDef = TypedDict(
+    "_RequiredIncidentTemplateOutputTypeDef",
+    {
+        "impact": int,
+        "title": str,
+    },
+)
+_OptionalIncidentTemplateOutputTypeDef = TypedDict(
+    "_OptionalIncidentTemplateOutputTypeDef",
+    {
+        "dedupeString": str,
+        "incidentTags": Dict[str, str],
+        "notificationTargets": List[NotificationTargetItemOutputTypeDef],
+        "summary": str,
+    },
+    total=False,
+)
+
+
+class IncidentTemplateOutputTypeDef(
+    _RequiredIncidentTemplateOutputTypeDef, _OptionalIncidentTemplateOutputTypeDef
+):
+    pass
+
+
 _RequiredIncidentTemplateTypeDef = TypedDict(
     "_RequiredIncidentTemplateTypeDef",
     {
         "impact": int,
         "title": str,
     },
 )
@@ -911,17 +1081,19 @@
         "incidentTags": Mapping[str, str],
         "notificationTargets": Sequence[NotificationTargetItemTypeDef],
         "summary": str,
     },
     total=False,
 )
 
+
 class IncidentTemplateTypeDef(_RequiredIncidentTemplateTypeDef, _OptionalIncidentTemplateTypeDef):
     pass
 
+
 _RequiredUpdateIncidentRecordInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIncidentRecordInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateIncidentRecordInputRequestTypeDef = TypedDict(
@@ -934,20 +1106,33 @@
         "status": IncidentRecordStatusType,
         "summary": str,
         "title": str,
     },
     total=False,
 )
 
+
 class UpdateIncidentRecordInputRequestTypeDef(
     _RequiredUpdateIncidentRecordInputRequestTypeDef,
     _OptionalUpdateIncidentRecordInputRequestTypeDef,
 ):
     pass
 
+
+ItemValueOutputTypeDef = TypedDict(
+    "ItemValueOutputTypeDef",
+    {
+        "arn": str,
+        "metricDefinition": str,
+        "pagerDutyIncidentDetail": PagerDutyIncidentDetailOutputTypeDef,
+        "url": str,
+    },
+    total=False,
+)
+
 ItemValueTypeDef = TypedDict(
     "ItemValueTypeDef",
     {
         "arn": str,
         "metricDefinition": str,
         "pagerDutyIncidentDetail": PagerDutyIncidentDetailTypeDef,
         "url": str,
@@ -956,15 +1141,24 @@
 )
 
 ListResponsePlansOutputTypeDef = TypedDict(
     "ListResponsePlansOutputTypeDef",
     {
         "nextToken": str,
         "responsePlanSummaries": List[ResponsePlanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PagerDutyConfigurationOutputTypeDef = TypedDict(
+    "PagerDutyConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "pagerDutyIncidentConfiguration": PagerDutyIncidentConfigurationOutputTypeDef,
+        "secretId": str,
     },
 )
 
 PagerDutyConfigurationTypeDef = TypedDict(
     "PagerDutyConfigurationTypeDef",
     {
         "name": str,
@@ -989,42 +1183,27 @@
     "_OptionalReplicationSetTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+
 class ReplicationSetTypeDef(_RequiredReplicationSetTypeDef, _OptionalReplicationSetTypeDef):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "condition": ConditionTypeDef,
         "key": str,
     },
 )
 
-ListTimelineEventsOutputTypeDef = TypedDict(
-    "ListTimelineEventsOutputTypeDef",
-    {
-        "eventSummaries": List[EventSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTimelineEventOutputTypeDef = TypedDict(
-    "GetTimelineEventOutputTypeDef",
-    {
-        "event": TimelineEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateReplicationSetInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationSetInputRequestTypeDef",
     {
         "actions": Sequence[UpdateReplicationSetActionTypeDef],
         "arn": str,
     },
 )
@@ -1032,74 +1211,117 @@
     "_OptionalUpdateReplicationSetInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateReplicationSetInputRequestTypeDef(
     _RequiredUpdateReplicationSetInputRequestTypeDef,
     _OptionalUpdateReplicationSetInputRequestTypeDef,
 ):
     pass
 
+
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "ssmAutomation": SsmAutomationOutputTypeDef,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ssmAutomation": SsmAutomationTypeDef,
     },
     total=False,
 )
 
+ListTimelineEventsOutputTypeDef = TypedDict(
+    "ListTimelineEventsOutputTypeDef",
+    {
+        "eventSummaries": List[EventSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTimelineEventOutputTypeDef = TypedDict(
+    "GetTimelineEventOutputTypeDef",
+    {
+        "event": TimelineEventTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListIncidentRecordsOutputTypeDef = TypedDict(
     "ListIncidentRecordsOutputTypeDef",
     {
         "incidentRecordSummaries": List[IncidentRecordSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIncidentRecordOutputTypeDef = TypedDict(
     "GetIncidentRecordOutputTypeDef",
     {
         "incidentRecord": IncidentRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ItemIdentifierOutputTypeDef = TypedDict(
+    "ItemIdentifierOutputTypeDef",
+    {
+        "type": ItemTypeType,
+        "value": ItemValueOutputTypeDef,
     },
 )
 
 ItemIdentifierTypeDef = TypedDict(
     "ItemIdentifierTypeDef",
     {
         "type": ItemTypeType,
         "value": ItemValueTypeDef,
     },
 )
 
+IntegrationOutputTypeDef = TypedDict(
+    "IntegrationOutputTypeDef",
+    {
+        "pagerDutyConfiguration": PagerDutyConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "pagerDutyConfiguration": PagerDutyConfigurationTypeDef,
     },
     total=False,
 )
 
 GetReplicationSetOutputTypeDef = TypedDict(
     "GetReplicationSetOutputTypeDef",
     {
         "replicationSet": ReplicationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef = TypedDict(
     "ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListIncidentRecordsInputRequestTypeDef = TypedDict(
     "ListIncidentRecordsInputRequestTypeDef",
     {
@@ -1118,25 +1340,27 @@
 )
 _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef = TypedDict(
     "_OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputListTimelineEventsPaginateTypeDef(
     _RequiredListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     _OptionalListTimelineEventsInputListTimelineEventsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListTimelineEventsInputRequestTypeDef = TypedDict(
     "_RequiredListTimelineEventsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
     },
 )
 _OptionalListTimelineEventsInputRequestTypeDef = TypedDict(
@@ -1147,19 +1371,43 @@
         "nextToken": str,
         "sortBy": Literal["EVENT_TIME"],
         "sortOrder": SortOrderType,
     },
     total=False,
 )
 
+
 class ListTimelineEventsInputRequestTypeDef(
     _RequiredListTimelineEventsInputRequestTypeDef, _OptionalListTimelineEventsInputRequestTypeDef
 ):
     pass
 
+
+_RequiredRelatedItemOutputTypeDef = TypedDict(
+    "_RequiredRelatedItemOutputTypeDef",
+    {
+        "identifier": ItemIdentifierOutputTypeDef,
+    },
+)
+_OptionalRelatedItemOutputTypeDef = TypedDict(
+    "_OptionalRelatedItemOutputTypeDef",
+    {
+        "generatedId": str,
+        "title": str,
+    },
+    total=False,
+)
+
+
+class RelatedItemOutputTypeDef(
+    _RequiredRelatedItemOutputTypeDef, _OptionalRelatedItemOutputTypeDef
+):
+    pass
+
+
 _RequiredRelatedItemTypeDef = TypedDict(
     "_RequiredRelatedItemTypeDef",
     {
         "identifier": ItemIdentifierTypeDef,
     },
 )
 _OptionalRelatedItemTypeDef = TypedDict(
@@ -1167,17 +1415,34 @@
     {
         "generatedId": str,
         "title": str,
     },
     total=False,
 )
 
+
 class RelatedItemTypeDef(_RequiredRelatedItemTypeDef, _OptionalRelatedItemTypeDef):
     pass
 
+
+GetResponsePlanOutputTypeDef = TypedDict(
+    "GetResponsePlanOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+        "arn": str,
+        "chatChannel": ChatChannelOutputTypeDef,
+        "displayName": str,
+        "engagements": List[str],
+        "incidentTemplate": IncidentTemplateOutputTypeDef,
+        "integrations": List[IntegrationOutputTypeDef],
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateResponsePlanInputRequestTypeDef",
     {
         "incidentTemplate": IncidentTemplateTypeDef,
         "name": str,
     },
 )
@@ -1191,33 +1456,20 @@
         "engagements": Sequence[str],
         "integrations": Sequence[IntegrationTypeDef],
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateResponsePlanInputRequestTypeDef(
     _RequiredCreateResponsePlanInputRequestTypeDef, _OptionalCreateResponsePlanInputRequestTypeDef
 ):
     pass
 
-GetResponsePlanOutputTypeDef = TypedDict(
-    "GetResponsePlanOutputTypeDef",
-    {
-        "actions": List[ActionTypeDef],
-        "arn": str,
-        "chatChannel": ChatChannelTypeDef,
-        "displayName": str,
-        "engagements": List[str],
-        "incidentTemplate": IncidentTemplateTypeDef,
-        "integrations": List[IntegrationTypeDef],
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateResponsePlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResponsePlanInputRequestTypeDef",
     {
         "arn": str,
     },
 )
@@ -1236,25 +1488,27 @@
         "incidentTemplateTags": Mapping[str, str],
         "incidentTemplateTitle": str,
         "integrations": Sequence[IntegrationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateResponsePlanInputRequestTypeDef(
     _RequiredUpdateResponsePlanInputRequestTypeDef, _OptionalUpdateResponsePlanInputRequestTypeDef
 ):
     pass
 
+
 ListRelatedItemsOutputTypeDef = TypedDict(
     "ListRelatedItemsOutputTypeDef",
     {
         "nextToken": str,
-        "relatedItems": List[RelatedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "relatedItems": List[RelatedItemOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemsUpdateTypeDef = TypedDict(
     "RelatedItemsUpdateTypeDef",
     {
         "itemToAdd": RelatedItemTypeDef,
@@ -1277,19 +1531,21 @@
         "relatedItems": Sequence[RelatedItemTypeDef],
         "title": str,
         "triggerDetails": TriggerDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StartIncidentInputRequestTypeDef(
     _RequiredStartIncidentInputRequestTypeDef, _OptionalStartIncidentInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRelatedItemsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRelatedItemsInputRequestTypeDef",
     {
         "incidentRecordArn": str,
         "relatedItemsUpdate": RelatedItemsUpdateTypeDef,
     },
 )
@@ -1297,11 +1553,12 @@
     "_OptionalUpdateRelatedItemsInputRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateRelatedItemsInputRequestTypeDef(
     _RequiredUpdateRelatedItemsInputRequestTypeDef, _OptionalUpdateRelatedItemsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/waiter.py` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents/waiter.pyi` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/PKG-INFO` & `mypy-boto3-ssm-incidents-1.28.12/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-ssm-incidents
-Version: 1.28.0
-Summary: Type annotations for boto3.SSMIncidents 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 ssm-incidents type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-ssm-incidents"></a>
 
 # mypy-boto3-ssm-incidents
 
 [![PyPI - mypy-boto3-ssm-incidents](https://img.shields.io/pypi/v/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm-incidents.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm-incidents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ssm-incidents?color=blue)](https://pypistats.org/packages/mypy-boto3-ssm-incidents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm-incidents)](https://pepy.tech/project/mypy-boto3-ssm-incidents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSMIncidents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
+[boto3.SSMIncidents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
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
 [mypy-boto3-ssm-incidents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm_incidents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -389,95 +357,109 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm_incidents.type_defs import (
     AddRegionActionTypeDef,
     AttributeValueListTypeDef,
     AutomationExecutionTypeDef,
+    ChatChannelOutputTypeDef,
     ChatChannelTypeDef,
     RegionMapInputValueTypeDef,
-    CreateReplicationSetOutputTypeDef,
-    CreateResponsePlanOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventReferenceTypeDef,
-    CreateTimelineEventOutputTypeDef,
     DeleteIncidentRecordInputRequestTypeDef,
     DeleteRegionActionTypeDef,
     DeleteReplicationSetInputRequestTypeDef,
     DeleteResourcePolicyInputRequestTypeDef,
     DeleteResponsePlanInputRequestTypeDef,
     DeleteTimelineEventInputRequestTypeDef,
+    DynamicSsmParameterValueOutputTypeDef,
     DynamicSsmParameterValueTypeDef,
+    EventReferenceOutputTypeDef,
     GetIncidentRecordInputRequestTypeDef,
     GetReplicationSetInputRequestTypeDef,
     WaiterConfigTypeDef,
-    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetResourcePoliciesInputRequestTypeDef,
     ResourcePolicyTypeDef,
     GetResponsePlanInputRequestTypeDef,
     GetTimelineEventInputRequestTypeDef,
     IncidentRecordSourceTypeDef,
+    NotificationTargetItemOutputTypeDef,
     NotificationTargetItemTypeDef,
+    PagerDutyIncidentDetailOutputTypeDef,
     PagerDutyIncidentDetailTypeDef,
-    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
     ListRelatedItemsInputRequestTypeDef,
-    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
     ListReplicationSetsInputRequestTypeDef,
-    ListReplicationSetsOutputTypeDef,
-    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     ListResponsePlansInputRequestTypeDef,
     ResponsePlanSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    PagerDutyIncidentConfigurationOutputTypeDef,
     PagerDutyIncidentConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyInputRequestTypeDef,
-    PutResourcePolicyOutputTypeDef,
     RegionInfoTypeDef,
-    ResponseMetadataTypeDef,
     TriggerDetailsTypeDef,
-    StartIncidentOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeletionProtectionInputRequestTypeDef,
     ConditionTypeDef,
     CreateReplicationSetInputRequestTypeDef,
+    CreateReplicationSetOutputTypeDef,
+    CreateResponsePlanOutputTypeDef,
+    CreateTimelineEventOutputTypeDef,
+    ListReplicationSetsOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutResourcePolicyOutputTypeDef,
+    StartIncidentOutputTypeDef,
     CreateTimelineEventInputRequestTypeDef,
-    EventSummaryTypeDef,
-    TimelineEventTypeDef,
     UpdateTimelineEventInputRequestTypeDef,
     UpdateReplicationSetActionTypeDef,
+    SsmAutomationOutputTypeDef,
     SsmAutomationTypeDef,
+    EventSummaryTypeDef,
+    TimelineEventTypeDef,
     GetReplicationSetInputWaitForReplicationSetActiveWaitTypeDef,
     GetReplicationSetInputWaitForReplicationSetDeletedWaitTypeDef,
+    GetResourcePoliciesInputGetResourcePoliciesPaginateTypeDef,
+    ListRelatedItemsInputListRelatedItemsPaginateTypeDef,
+    ListReplicationSetsInputListReplicationSetsPaginateTypeDef,
+    ListResponsePlansInputListResponsePlansPaginateTypeDef,
     GetResourcePoliciesOutputTypeDef,
     IncidentRecordSummaryTypeDef,
     IncidentRecordTypeDef,
+    IncidentTemplateOutputTypeDef,
     IncidentTemplateTypeDef,
     UpdateIncidentRecordInputRequestTypeDef,
+    ItemValueOutputTypeDef,
     ItemValueTypeDef,
     ListResponsePlansOutputTypeDef,
+    PagerDutyConfigurationOutputTypeDef,
     PagerDutyConfigurationTypeDef,
     ReplicationSetTypeDef,
     FilterTypeDef,
-    ListTimelineEventsOutputTypeDef,
-    GetTimelineEventOutputTypeDef,
     UpdateReplicationSetInputRequestTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
+    ListTimelineEventsOutputTypeDef,
+    GetTimelineEventOutputTypeDef,
     ListIncidentRecordsOutputTypeDef,
     GetIncidentRecordOutputTypeDef,
+    ItemIdentifierOutputTypeDef,
     ItemIdentifierTypeDef,
+    IntegrationOutputTypeDef,
     IntegrationTypeDef,
     GetReplicationSetOutputTypeDef,
     ListIncidentRecordsInputListIncidentRecordsPaginateTypeDef,
     ListIncidentRecordsInputRequestTypeDef,
     ListTimelineEventsInputListTimelineEventsPaginateTypeDef,
     ListTimelineEventsInputRequestTypeDef,
+    RelatedItemOutputTypeDef,
     RelatedItemTypeDef,
-    CreateResponsePlanInputRequestTypeDef,
     GetResponsePlanOutputTypeDef,
+    CreateResponsePlanInputRequestTypeDef,
     UpdateResponsePlanInputRequestTypeDef,
     ListRelatedItemsOutputTypeDef,
     RelatedItemsUpdateTypeDef,
     StartIncidentInputRequestTypeDef,
     UpdateRelatedItemsInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-ssm-incidents-1.28.0/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt` & `mypy-boto3-ssm-incidents-1.28.12/mypy_boto3_ssm_incidents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-incidents-1.28.0/setup.py` & `mypy-boto3-ssm-incidents-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm-incidents",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ssm_incidents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSMIncidents 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.SSMIncidents 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

