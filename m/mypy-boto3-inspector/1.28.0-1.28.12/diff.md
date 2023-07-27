# Comparing `tmp/mypy-boto3-inspector-1.28.0.tar.gz` & `tmp/mypy-boto3-inspector-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-inspector-1.28.0.tar", last modified: Thu Jul  6 20:59:44 2023, max compression
+gzip compressed data, was "mypy-boto3-inspector-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
```

## Comparing `mypy-boto3-inspector-1.28.0.tar` & `mypy-boto3-inspector-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.378322 mypy-boto3-inspector-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-07-06 20:59:44.378322 mypy-boto3-inspector-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.374322 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40510 2023-07-06 20:43:01.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40445 2023-07-06 20:43:01.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:00.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:44.378322 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:44.000000 mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:44.378322 mypy-boto3-inspector-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:42:59.000000 mypy-boto3-inspector-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.296490 mypy-boto3-inspector-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-27 05:34:47.292490 mypy-boto3-inspector-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17422 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.284490 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31933 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31880 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11276 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41766 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41695 2023-07-27 05:23:34.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.292490 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18917 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:47.000000 mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.296490 mypy-boto3-inspector-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:33.000000 mypy-boto3-inspector-1.28.12/setup.py
```

### Comparing `mypy-boto3-inspector-1.28.0/LICENSE` & `mypy-boto3-inspector-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/PKG-INFO` & `mypy-boto3-inspector-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.0
-Summary: Type annotations for boto3.Inspector 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,17 +380,18 @@
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
+    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateAssessmentTargetResponseTypeDef,
     CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
     CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
     CreateResourceGroupResponseTypeDef,
@@ -430,61 +431,63 @@
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResourceGroupTagOutputTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
-    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    AssessmentTemplateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
     NetworkInterfaceTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    ResourceGroupTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.0/README.md` & `mypy-boto3-inspector-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,17 +348,18 @@
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
+    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateAssessmentTargetResponseTypeDef,
     CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
     CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
     CreateResourceGroupResponseTypeDef,
@@ -398,61 +399,63 @@
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResourceGroupTagOutputTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
-    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    AssessmentTemplateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
     NetworkInterfaceTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    ResourceGroupTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__init__.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__init__.pyi` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/__main__.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Inspector 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Inspector 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/client.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/client.pyi` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/literals.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
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
@@ -307,26 +308,28 @@
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

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/literals.pyi` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
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
@@ -305,26 +306,28 @@
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

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/paginator.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/paginator.pyi` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/type_defs.py` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,17 +47,18 @@
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
+    "AttributeOutputTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
     "CreateAssessmentTargetResponseTypeDef",
     "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
     "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
     "CreateResourceGroupResponseTypeDef",
@@ -97,61 +98,63 @@
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
     "PaginatorConfigTypeDef",
     "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
+    "ResourceGroupTagOutputTypeDef",
     "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
     "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
-    "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
     "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
+    "AssessmentTemplateTypeDef",
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
-    "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
     "NetworkInterfaceTypeDef",
-    "DescribeAssessmentTemplatesResponseTypeDef",
+    "ResourceGroupTypeDef",
+    "SetTagsForResourceRequestRequestTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
-    "DescribeResourceGroupsResponseTypeDef",
+    "DescribeAssessmentTemplatesResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "DescribeResourceGroupsResponseTypeDef",
     "FindingTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -281,14 +284,33 @@
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
+
 AssessmentTargetFilterTypeDef = TypedDict(
     "AssessmentTargetFilterTypeDef",
     {
         "assessmentTargetNamePattern": str,
     },
     total=False,
 )
@@ -311,30 +333,30 @@
 )
 
 
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
 
-_RequiredTagTypeDef = TypedDict(
-    "_RequiredTagTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
         "key": str,
     },
 )
-_OptionalTagTypeDef = TypedDict(
-    "_OptionalTagTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
 
-class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
     pass
 
 
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
@@ -880,25 +902,65 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
     },
 )
 
+_RequiredResourceGroupTagOutputTypeDef = TypedDict(
+    "_RequiredResourceGroupTagOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalResourceGroupTagOutputTypeDef = TypedDict(
+    "_OptionalResourceGroupTagOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class ResourceGroupTagOutputTypeDef(
+    _RequiredResourceGroupTagOutputTypeDef, _OptionalResourceGroupTagOutputTypeDef
+):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredTagTypeDef = TypedDict(
+    "_RequiredTagTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalTagTypeDef = TypedDict(
+    "_OptionalTagTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+
+class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
+    pass
+
+
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
@@ -991,42 +1053,14 @@
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
-_RequiredAssessmentTemplateTypeDef = TypedDict(
-    "_RequiredAssessmentTemplateTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "assessmentTargetArn": str,
-        "durationInSeconds": int,
-        "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeTypeDef],
-        "assessmentRunCount": int,
-        "createdAt": datetime,
-    },
-)
-_OptionalAssessmentTemplateTypeDef = TypedDict(
-    "_OptionalAssessmentTemplateTypeDef",
-    {
-        "lastAssessmentRunArn": str,
-    },
-    total=False,
-)
-
-
-class AssessmentTemplateTypeDef(
-    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
-):
-    pass
-
-
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -1198,15 +1232,15 @@
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
         "durationInSeconds": int,
         "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeTypeDef],
+        "userAttributesForFindings": List[AttributeOutputTypeDef],
         "createdAt": datetime,
         "stateChangedAt": datetime,
         "dataCollected": bool,
         "stateChanges": List[AssessmentRunStateChangeTypeDef],
         "notifications": List[AssessmentRunNotificationTypeDef],
         "findingCounts": Dict[SeverityType, int],
     },
@@ -1221,14 +1255,42 @@
 )
 
 
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
 
+_RequiredAssessmentTemplateTypeDef = TypedDict(
+    "_RequiredAssessmentTemplateTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "assessmentTargetArn": str,
+        "durationInSeconds": int,
+        "rulesPackageArns": List[str],
+        "userAttributesForFindings": List[AttributeOutputTypeDef],
+        "assessmentRunCount": int,
+        "createdAt": datetime,
+    },
+)
+_OptionalAssessmentTemplateTypeDef = TypedDict(
+    "_OptionalAssessmentTemplateTypeDef",
+    {
+        "lastAssessmentRunArn": str,
+    },
+    total=False,
+)
+
+
+class AssessmentTemplateTypeDef(
+    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
+):
+    pass
+
+
 ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1252,57 +1314,26 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredSetTagsForResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalSetTagsForResourceRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class SetTagsForResourceRequestRequestTypeDef(
-    _RequiredSetTagsForResourceRequestRequestTypeDef,
-    _OptionalSetTagsForResourceRequestRequestTypeDef,
-):
-    pass
-
-
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
-ResourceGroupTypeDef = TypedDict(
-    "ResourceGroupTypeDef",
-    {
-        "arn": str,
-        "tags": List[ResourceGroupTagTypeDef],
-        "createdAt": datetime,
-    },
-)
-
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1325,15 +1356,15 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionPreviewTypeDef = TypedDict(
     "_OptionalExclusionPreviewTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
@@ -1348,15 +1379,15 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionTypeDef = TypedDict(
     "_OptionalExclusionTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
@@ -1375,23 +1406,45 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
-DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
-    "DescribeAssessmentTemplatesResponseTypeDef",
+ResourceGroupTypeDef = TypedDict(
+    "ResourceGroupTypeDef",
     {
-        "assessmentTemplates": List[AssessmentTemplateTypeDef],
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "tags": List[ResourceGroupTagOutputTypeDef],
+        "createdAt": datetime,
+    },
+)
+
+_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+
+class SetTagsForResourceRequestRequestTypeDef(
+    _RequiredSetTagsForResourceRequestRequestTypeDef,
+    _OptionalSetTagsForResourceRequestRequestTypeDef,
+):
+    pass
+
+
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1465,18 +1518,18 @@
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeResourceGroupsResponseTypeDef = TypedDict(
-    "DescribeResourceGroupsResponseTypeDef",
+DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
+    "DescribeAssessmentTemplatesResponseTypeDef",
     {
-        "resourceGroups": List[ResourceGroupTypeDef],
+        "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
@@ -1516,31 +1569,40 @@
     "_OptionalAssetAttributesTypeDef",
     {
         "agentId": str,
         "autoScalingGroup": str,
         "amiId": str,
         "hostname": str,
         "ipv4Addresses": List[str],
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
 
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
 
+DescribeResourceGroupsResponseTypeDef = TypedDict(
+    "DescribeResourceGroupsResponseTypeDef",
+    {
+        "resourceGroups": List[ResourceGroupTypeDef],
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
-        "attributes": List[AttributeTypeDef],
-        "userAttributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
+        "userAttributes": List[AttributeOutputTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
```

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector/type_defs.pyi` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,18 @@
     "AgentFilterTypeDef",
     "AgentPreviewTypeDef",
     "TelemetryMetadataTypeDef",
     "DurationRangeTypeDef",
     "TimestampRangeTypeDef",
     "AssessmentRunNotificationTypeDef",
     "AssessmentRunStateChangeTypeDef",
+    "AttributeOutputTypeDef",
     "AssessmentTargetFilterTypeDef",
     "AssessmentTargetTypeDef",
-    "TagTypeDef",
+    "TagOutputTypeDef",
     "CreateAssessmentTargetRequestRequestTypeDef",
     "CreateAssessmentTargetResponseTypeDef",
     "CreateAssessmentTemplateResponseTypeDef",
     "CreateExclusionsPreviewRequestRequestTypeDef",
     "CreateExclusionsPreviewResponseTypeDef",
     "ResourceGroupTagTypeDef",
     "CreateResourceGroupResponseTypeDef",
@@ -96,61 +97,63 @@
     "PrivateIpTypeDef",
     "SecurityGroupTypeDef",
     "PaginatorConfigTypeDef",
     "PreviewAgentsRequestPreviewAgentsPaginateTypeDef",
     "PreviewAgentsRequestRequestTypeDef",
     "RegisterCrossAccountAccessRoleRequestRequestTypeDef",
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
+    "ResourceGroupTagOutputTypeDef",
     "ResponseMetadataTypeDef",
+    "TagTypeDef",
     "StartAssessmentRunRequestRequestTypeDef",
     "StartAssessmentRunResponseTypeDef",
     "StopAssessmentRunRequestRequestTypeDef",
     "SubscribeToEventRequestRequestTypeDef",
     "UnsubscribeFromEventRequestRequestTypeDef",
     "UpdateAssessmentTargetRequestRequestTypeDef",
     "AddAttributesToFindingsRequestRequestTypeDef",
-    "AssessmentTemplateTypeDef",
     "CreateAssessmentTemplateRequestRequestTypeDef",
     "AddAttributesToFindingsResponseTypeDef",
     "RemoveAttributesFromFindingsResponseTypeDef",
     "ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef",
     "ListAssessmentRunAgentsRequestRequestTypeDef",
     "PreviewAgentsResponseTypeDef",
     "AssessmentRunAgentTypeDef",
     "GetTelemetryMetadataResponseTypeDef",
     "AssessmentTemplateFilterTypeDef",
     "AssessmentRunFilterTypeDef",
     "FindingFilterTypeDef",
     "AssessmentRunTypeDef",
+    "AssessmentTemplateTypeDef",
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     "ListAssessmentTargetsRequestRequestTypeDef",
     "DescribeAssessmentTargetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "SetTagsForResourceRequestRequestTypeDef",
     "CreateResourceGroupRequestRequestTypeDef",
-    "ResourceGroupTypeDef",
     "DescribeRulesPackagesResponseTypeDef",
     "SubscriptionTypeDef",
     "ExclusionPreviewTypeDef",
     "ExclusionTypeDef",
     "NetworkInterfaceTypeDef",
-    "DescribeAssessmentTemplatesResponseTypeDef",
+    "ResourceGroupTypeDef",
+    "SetTagsForResourceRequestRequestTypeDef",
     "ListAssessmentRunAgentsResponseTypeDef",
     "ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef",
     "ListAssessmentTemplatesRequestRequestTypeDef",
     "ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef",
     "ListAssessmentRunsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "DescribeAssessmentRunsResponseTypeDef",
-    "DescribeResourceGroupsResponseTypeDef",
+    "DescribeAssessmentTemplatesResponseTypeDef",
     "ListEventSubscriptionsResponseTypeDef",
     "GetExclusionsPreviewResponseTypeDef",
     "DescribeExclusionsResponseTypeDef",
     "AssetAttributesTypeDef",
+    "DescribeResourceGroupsResponseTypeDef",
     "FindingTypeDef",
     "DescribeFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -272,14 +275,31 @@
     "AssessmentRunStateChangeTypeDef",
     {
         "stateChangedAt": datetime,
         "state": AssessmentRunStateType,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
 AssessmentTargetFilterTypeDef = TypedDict(
     "AssessmentTargetFilterTypeDef",
     {
         "assessmentTargetNamePattern": str,
     },
     total=False,
 )
@@ -300,29 +320,29 @@
     },
     total=False,
 )
 
 class AssessmentTargetTypeDef(_RequiredAssessmentTargetTypeDef, _OptionalAssessmentTargetTypeDef):
     pass
 
-_RequiredTagTypeDef = TypedDict(
-    "_RequiredTagTypeDef",
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
     {
         "key": str,
     },
 )
-_OptionalTagTypeDef = TypedDict(
-    "_OptionalTagTypeDef",
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
     pass
 
 _RequiredCreateAssessmentTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTargetRequestRequestTypeDef",
     {
         "assessmentTargetName": str,
     },
@@ -843,25 +863,61 @@
     "RemoveAttributesFromFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributeKeys": Sequence[str],
     },
 )
 
+_RequiredResourceGroupTagOutputTypeDef = TypedDict(
+    "_RequiredResourceGroupTagOutputTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalResourceGroupTagOutputTypeDef = TypedDict(
+    "_OptionalResourceGroupTagOutputTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class ResourceGroupTagOutputTypeDef(
+    _RequiredResourceGroupTagOutputTypeDef, _OptionalResourceGroupTagOutputTypeDef
+):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+_RequiredTagTypeDef = TypedDict(
+    "_RequiredTagTypeDef",
+    {
+        "key": str,
+    },
+)
+_OptionalTagTypeDef = TypedDict(
+    "_OptionalTagTypeDef",
+    {
+        "value": str,
+    },
+    total=False,
+)
+
+class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
+    pass
+
 _RequiredStartAssessmentRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentRunRequestRequestTypeDef",
     {
         "assessmentTemplateArn": str,
     },
 )
 _OptionalStartAssessmentRunRequestRequestTypeDef = TypedDict(
@@ -948,40 +1004,14 @@
     "AddAttributesToFindingsRequestRequestTypeDef",
     {
         "findingArns": Sequence[str],
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
-_RequiredAssessmentTemplateTypeDef = TypedDict(
-    "_RequiredAssessmentTemplateTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "assessmentTargetArn": str,
-        "durationInSeconds": int,
-        "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeTypeDef],
-        "assessmentRunCount": int,
-        "createdAt": datetime,
-    },
-)
-_OptionalAssessmentTemplateTypeDef = TypedDict(
-    "_OptionalAssessmentTemplateTypeDef",
-    {
-        "lastAssessmentRunArn": str,
-    },
-    total=False,
-)
-
-class AssessmentTemplateTypeDef(
-    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
-):
-    pass
-
 _RequiredCreateAssessmentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentTemplateRequestRequestTypeDef",
     {
         "assessmentTargetArn": str,
         "assessmentTemplateName": str,
         "durationInSeconds": int,
         "rulesPackageArns": Sequence[str],
@@ -1145,15 +1175,15 @@
     {
         "arn": str,
         "name": str,
         "assessmentTemplateArn": str,
         "state": AssessmentRunStateType,
         "durationInSeconds": int,
         "rulesPackageArns": List[str],
-        "userAttributesForFindings": List[AttributeTypeDef],
+        "userAttributesForFindings": List[AttributeOutputTypeDef],
         "createdAt": datetime,
         "stateChangedAt": datetime,
         "dataCollected": bool,
         "stateChanges": List[AssessmentRunStateChangeTypeDef],
         "notifications": List[AssessmentRunNotificationTypeDef],
         "findingCounts": Dict[SeverityType, int],
     },
@@ -1166,14 +1196,40 @@
     },
     total=False,
 )
 
 class AssessmentRunTypeDef(_RequiredAssessmentRunTypeDef, _OptionalAssessmentRunTypeDef):
     pass
 
+_RequiredAssessmentTemplateTypeDef = TypedDict(
+    "_RequiredAssessmentTemplateTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "assessmentTargetArn": str,
+        "durationInSeconds": int,
+        "rulesPackageArns": List[str],
+        "userAttributesForFindings": List[AttributeOutputTypeDef],
+        "assessmentRunCount": int,
+        "createdAt": datetime,
+    },
+)
+_OptionalAssessmentTemplateTypeDef = TypedDict(
+    "_OptionalAssessmentTemplateTypeDef",
+    {
+        "lastAssessmentRunArn": str,
+    },
+    total=False,
+)
+
+class AssessmentTemplateTypeDef(
+    _RequiredAssessmentTemplateTypeDef, _OptionalAssessmentTemplateTypeDef
+):
+    pass
+
 ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef = TypedDict(
     "ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef",
     {
         "filter": AssessmentTargetFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1197,55 +1253,26 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredSetTagsForResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalSetTagsForResourceRequestRequestTypeDef",
-    {
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class SetTagsForResourceRequestRequestTypeDef(
-    _RequiredSetTagsForResourceRequestRequestTypeDef,
-    _OptionalSetTagsForResourceRequestRequestTypeDef,
-):
-    pass
-
 CreateResourceGroupRequestRequestTypeDef = TypedDict(
     "CreateResourceGroupRequestRequestTypeDef",
     {
         "resourceGroupTags": Sequence[ResourceGroupTagTypeDef],
     },
 )
 
-ResourceGroupTypeDef = TypedDict(
-    "ResourceGroupTypeDef",
-    {
-        "arn": str,
-        "tags": List[ResourceGroupTagTypeDef],
-        "createdAt": datetime,
-    },
-)
-
 DescribeRulesPackagesResponseTypeDef = TypedDict(
     "DescribeRulesPackagesResponseTypeDef",
     {
         "rulesPackages": List[RulesPackageTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1268,15 +1295,15 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionPreviewTypeDef = TypedDict(
     "_OptionalExclusionPreviewTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 class ExclusionPreviewTypeDef(_RequiredExclusionPreviewTypeDef, _OptionalExclusionPreviewTypeDef):
     pass
 
@@ -1289,15 +1316,15 @@
         "recommendation": str,
         "scopes": List[ScopeTypeDef],
     },
 )
 _OptionalExclusionTypeDef = TypedDict(
     "_OptionalExclusionTypeDef",
     {
-        "attributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
     },
     total=False,
 )
 
 class ExclusionTypeDef(_RequiredExclusionTypeDef, _OptionalExclusionTypeDef):
     pass
 
@@ -1314,23 +1341,43 @@
         "publicIp": str,
         "ipv6Addresses": List[str],
         "securityGroups": List[SecurityGroupTypeDef],
     },
     total=False,
 )
 
-DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
-    "DescribeAssessmentTemplatesResponseTypeDef",
+ResourceGroupTypeDef = TypedDict(
+    "ResourceGroupTypeDef",
     {
-        "assessmentTemplates": List[AssessmentTemplateTypeDef],
-        "failedItems": Dict[str, FailedItemDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "tags": List[ResourceGroupTagOutputTypeDef],
+        "createdAt": datetime,
     },
 )
 
+_RequiredSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredSetTagsForResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalSetTagsForResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalSetTagsForResourceRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class SetTagsForResourceRequestRequestTypeDef(
+    _RequiredSetTagsForResourceRequestRequestTypeDef,
+    _OptionalSetTagsForResourceRequestRequestTypeDef,
+):
+    pass
+
 ListAssessmentRunAgentsResponseTypeDef = TypedDict(
     "ListAssessmentRunAgentsResponseTypeDef",
     {
         "assessmentRunAgents": List[AssessmentRunAgentTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1404,18 +1451,18 @@
     {
         "assessmentRuns": List[AssessmentRunTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeResourceGroupsResponseTypeDef = TypedDict(
-    "DescribeResourceGroupsResponseTypeDef",
+DescribeAssessmentTemplatesResponseTypeDef = TypedDict(
+    "DescribeAssessmentTemplatesResponseTypeDef",
     {
-        "resourceGroups": List[ResourceGroupTypeDef],
+        "assessmentTemplates": List[AssessmentTemplateTypeDef],
         "failedItems": Dict[str, FailedItemDetailsTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListEventSubscriptionsResponseTypeDef = TypedDict(
     "ListEventSubscriptionsResponseTypeDef",
@@ -1455,29 +1502,38 @@
     "_OptionalAssetAttributesTypeDef",
     {
         "agentId": str,
         "autoScalingGroup": str,
         "amiId": str,
         "hostname": str,
         "ipv4Addresses": List[str],
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "networkInterfaces": List[NetworkInterfaceTypeDef],
     },
     total=False,
 )
 
 class AssetAttributesTypeDef(_RequiredAssetAttributesTypeDef, _OptionalAssetAttributesTypeDef):
     pass
 
+DescribeResourceGroupsResponseTypeDef = TypedDict(
+    "DescribeResourceGroupsResponseTypeDef",
+    {
+        "resourceGroups": List[ResourceGroupTypeDef],
+        "failedItems": Dict[str, FailedItemDetailsTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "arn": str,
-        "attributes": List[AttributeTypeDef],
-        "userAttributes": List[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
+        "userAttributes": List[AttributeOutputTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalFindingTypeDef = TypedDict(
     "_OptionalFindingTypeDef",
     {
```

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/PKG-INFO` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-inspector
-Version: 1.28.0
-Summary: Type annotations for boto3.Inspector 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-inspector"></a>
 
 # mypy-boto3-inspector
 
 [![PyPI - mypy-boto3-inspector](https://img.shields.io/pypi/v/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-inspector.svg?color=blue)](https://pypi.org/project/mypy-boto3-inspector)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-inspector?color=blue)](https://pypistats.org/packages/mypy-boto3-inspector)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-inspector)](https://pepy.tech/project/mypy-boto3-inspector)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Inspector 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
+[boto3.Inspector 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector)
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
 [mypy-boto3-inspector docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_inspector/).
 
 See how it helps to find and fix potential bugs:
 
@@ -380,17 +380,18 @@
     AgentFilterTypeDef,
     AgentPreviewTypeDef,
     TelemetryMetadataTypeDef,
     DurationRangeTypeDef,
     TimestampRangeTypeDef,
     AssessmentRunNotificationTypeDef,
     AssessmentRunStateChangeTypeDef,
+    AttributeOutputTypeDef,
     AssessmentTargetFilterTypeDef,
     AssessmentTargetTypeDef,
-    TagTypeDef,
+    TagOutputTypeDef,
     CreateAssessmentTargetRequestRequestTypeDef,
     CreateAssessmentTargetResponseTypeDef,
     CreateAssessmentTemplateResponseTypeDef,
     CreateExclusionsPreviewRequestRequestTypeDef,
     CreateExclusionsPreviewResponseTypeDef,
     ResourceGroupTagTypeDef,
     CreateResourceGroupResponseTypeDef,
@@ -430,61 +431,63 @@
     PrivateIpTypeDef,
     SecurityGroupTypeDef,
     PaginatorConfigTypeDef,
     PreviewAgentsRequestPreviewAgentsPaginateTypeDef,
     PreviewAgentsRequestRequestTypeDef,
     RegisterCrossAccountAccessRoleRequestRequestTypeDef,
     RemoveAttributesFromFindingsRequestRequestTypeDef,
+    ResourceGroupTagOutputTypeDef,
     ResponseMetadataTypeDef,
+    TagTypeDef,
     StartAssessmentRunRequestRequestTypeDef,
     StartAssessmentRunResponseTypeDef,
     StopAssessmentRunRequestRequestTypeDef,
     SubscribeToEventRequestRequestTypeDef,
     UnsubscribeFromEventRequestRequestTypeDef,
     UpdateAssessmentTargetRequestRequestTypeDef,
     AddAttributesToFindingsRequestRequestTypeDef,
-    AssessmentTemplateTypeDef,
     CreateAssessmentTemplateRequestRequestTypeDef,
     AddAttributesToFindingsResponseTypeDef,
     RemoveAttributesFromFindingsResponseTypeDef,
     ListAssessmentRunAgentsRequestListAssessmentRunAgentsPaginateTypeDef,
     ListAssessmentRunAgentsRequestRequestTypeDef,
     PreviewAgentsResponseTypeDef,
     AssessmentRunAgentTypeDef,
     GetTelemetryMetadataResponseTypeDef,
     AssessmentTemplateFilterTypeDef,
     AssessmentRunFilterTypeDef,
     FindingFilterTypeDef,
     AssessmentRunTypeDef,
+    AssessmentTemplateTypeDef,
     ListAssessmentTargetsRequestListAssessmentTargetsPaginateTypeDef,
     ListAssessmentTargetsRequestRequestTypeDef,
     DescribeAssessmentTargetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    SetTagsForResourceRequestRequestTypeDef,
     CreateResourceGroupRequestRequestTypeDef,
-    ResourceGroupTypeDef,
     DescribeRulesPackagesResponseTypeDef,
     SubscriptionTypeDef,
     ExclusionPreviewTypeDef,
     ExclusionTypeDef,
     NetworkInterfaceTypeDef,
-    DescribeAssessmentTemplatesResponseTypeDef,
+    ResourceGroupTypeDef,
+    SetTagsForResourceRequestRequestTypeDef,
     ListAssessmentRunAgentsResponseTypeDef,
     ListAssessmentTemplatesRequestListAssessmentTemplatesPaginateTypeDef,
     ListAssessmentTemplatesRequestRequestTypeDef,
     ListAssessmentRunsRequestListAssessmentRunsPaginateTypeDef,
     ListAssessmentRunsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     DescribeAssessmentRunsResponseTypeDef,
-    DescribeResourceGroupsResponseTypeDef,
+    DescribeAssessmentTemplatesResponseTypeDef,
     ListEventSubscriptionsResponseTypeDef,
     GetExclusionsPreviewResponseTypeDef,
     DescribeExclusionsResponseTypeDef,
     AssetAttributesTypeDef,
+    DescribeResourceGroupsResponseTypeDef,
     FindingTypeDef,
     DescribeFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-inspector-1.28.0/mypy_boto3_inspector.egg-info/SOURCES.txt` & `mypy-boto3-inspector-1.28.12/mypy_boto3_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-inspector-1.28.0/setup.py` & `mypy-boto3-inspector-1.28.12/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-inspector",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Inspector 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Inspector 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

