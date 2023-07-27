# Comparing `tmp/mypy-boto3-resiliencehub-1.28.0.tar.gz` & `tmp/mypy-boto3-resiliencehub-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resiliencehub-1.28.0.tar", last modified: Thu Jul  6 21:00:26 2023, max compression
+gzip compressed data, was "mypy-boto3-resiliencehub-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
```

## Comparing `mypy-boto3-resiliencehub-1.28.0.tar` & `mypy-boto3-resiliencehub-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.002407 mypy-boto3-resiliencehub-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18723 2023-07-06 21:00:26.002407 mypy-boto3-resiliencehub-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.002407 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-07-06 20:53:12.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-07-06 20:53:12.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60883 2023-07-06 20:53:13.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60778 2023-07-06 20:53:13.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:26.002407 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18723 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:25.000000 mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:26.002407 mypy-boto3-resiliencehub-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-06 20:53:11.000000 mypy-boto3-resiliencehub-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.265213 mypy-boto3-resiliencehub-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-27 11:49:30.261213 mypy-boto3-resiliencehub-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17442 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.257213 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39514 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10983 2023-07-27 11:44:36.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-07-27 11:44:36.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63431 2023-07-27 11:44:38.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63320 2023-07-27 11:44:37.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.261213 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:30.000000 mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.265213 mypy-boto3-resiliencehub-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 11:44:34.000000 mypy-boto3-resiliencehub-1.28.12/setup.py
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/LICENSE` & `mypy-boto3-resiliencehub-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.0/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.0
-Summary: Type annotations for boto3.ResilienceHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,52 +323,49 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
+    EksSourceClusterNamespaceOutputTypeDef,
+    TerraformSourceOutputTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
+    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -376,66 +373,76 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
+    LogicalResourceIdOutputTypeDef,
+    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingTypeDef,
+    ResourceMappingOutputTypeDef,
     UnsupportedResourceTypeDef,
+    ResourceMappingTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -448,28 +455,28 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/README.md` & `mypy-boto3-resiliencehub-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,52 +291,49 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
+    EksSourceClusterNamespaceOutputTypeDef,
+    TerraformSourceOutputTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
+    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -344,66 +341,76 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
+    LogicalResourceIdOutputTypeDef,
+    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingTypeDef,
+    ResourceMappingOutputTypeDef,
     UnsupportedResourceTypeDef,
+    ResourceMappingTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -416,28 +423,28 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/__main__.py` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResilienceHub 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ResilienceHub 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub\nOther"
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

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/client.py` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/client.pyi` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/literals.py` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/literals.pyi` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/type_defs.py` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_resiliencehub.type_defs import RecommendationItemTypeDef
+    from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: RecommendationItemTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -51,52 +51,49 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
-    "EksSourceClusterNamespaceTypeDef",
-    "TerraformSourceTypeDef",
+    "EksSourceClusterNamespaceOutputTypeDef",
+    "TerraformSourceOutputTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
+    "TerraformSourceTypeDef",
     "DeleteAppRequestRequestTypeDef",
-    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
+    "FailurePolicyOutputTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -104,66 +101,76 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
+    "LogicalResourceIdOutputTypeDef",
+    "PhysicalResourceIdOutputTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
-    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishAppVersionResponseTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
-    "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
-    "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "DeleteAppInputSourceRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "ResiliencyPolicyTypeDef",
     "PhysicalResourceTypeDef",
-    "ResourceMappingTypeDef",
+    "ResourceMappingOutputTypeDef",
     "UnsupportedResourceTypeDef",
+    "ResourceMappingTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
@@ -176,26 +183,37 @@
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -266,24 +284,24 @@
 )
 
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
 
-EksSourceClusterNamespaceTypeDef = TypedDict(
-    "EksSourceClusterNamespaceTypeDef",
+EksSourceClusterNamespaceOutputTypeDef = TypedDict(
+    "EksSourceClusterNamespaceOutputTypeDef",
     {
         "eksClusterArn": str,
         "namespace": str,
     },
 )
 
-TerraformSourceTypeDef = TypedDict(
-    "TerraformSourceTypeDef",
+TerraformSourceOutputTypeDef = TypedDict(
+    "TerraformSourceOutputTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
 _RequiredAppSummaryTypeDef = TypedDict(
     "_RequiredAppSummaryTypeDef",
@@ -500,20 +518,26 @@
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
     {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eksClusterArn": str,
+        "namespace": str,
+    },
+)
+
+TerraformSourceTypeDef = TypedDict(
+    "TerraformSourceTypeDef",
+    {
+        "s3StateFileUrl": str,
     },
 )
 
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
@@ -531,22 +555,14 @@
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -584,23 +600,14 @@
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -615,22 +622,14 @@
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -677,88 +676,60 @@
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyArn": str,
     },
 )
 
-DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
-    "DescribeResiliencyPolicyRequestRequestTypeDef",
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
     {
-        "policyArn": str,
+        "eksClusterArn": str,
+        "namespaces": List[str],
     },
 )
 
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
 
+FailurePolicyOutputTypeDef = TypedDict(
+    "FailurePolicyOutputTypeDef",
+    {
+        "rpoInSecs": int,
+        "rtoInSecs": int,
+    },
+)
+
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1041,22 +1012,14 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1097,14 +1060,61 @@
 class ListUnsupportedAppVersionResourcesRequestRequestTypeDef(
     _RequiredListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     _OptionalListUnsupportedAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredLogicalResourceIdOutputTypeDef = TypedDict(
+    "_RequiredLogicalResourceIdOutputTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalLogicalResourceIdOutputTypeDef = TypedDict(
+    "_OptionalLogicalResourceIdOutputTypeDef",
+    {
+        "eksSourceName": str,
+        "logicalStackName": str,
+        "resourceGroupName": str,
+        "terraformSourceName": str,
+    },
+    total=False,
+)
+
+
+class LogicalResourceIdOutputTypeDef(
+    _RequiredLogicalResourceIdOutputTypeDef, _OptionalLogicalResourceIdOutputTypeDef
+):
+    pass
+
+
+_RequiredPhysicalResourceIdOutputTypeDef = TypedDict(
+    "_RequiredPhysicalResourceIdOutputTypeDef",
+    {
+        "identifier": str,
+        "type": PhysicalIdentifierTypeType,
+    },
+)
+_OptionalPhysicalResourceIdOutputTypeDef = TypedDict(
+    "_OptionalPhysicalResourceIdOutputTypeDef",
+    {
+        "awsAccountId": str,
+        "awsRegion": str,
+    },
+    total=False,
+)
+
+
+class PhysicalResourceIdOutputTypeDef(
+    _RequiredPhysicalResourceIdOutputTypeDef, _OptionalPhysicalResourceIdOutputTypeDef
+):
+    pass
+
+
 _RequiredPhysicalResourceIdTypeDef = TypedDict(
     "_RequiredPhysicalResourceIdTypeDef",
     {
         "identifier": str,
         "type": PhysicalIdentifierTypeType,
     },
 )
@@ -1127,40 +1137,22 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1189,63 +1181,32 @@
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
 
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
     },
     total=False,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1349,21 +1310,145 @@
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
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
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1493,146 +1578,121 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceOutputTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
-        "terraformSource": TerraformSourceTypeDef,
+        "terraformSource": TerraformSourceOutputTypeDef,
     },
     total=False,
 )
 
 
 class AppInputSourceTypeDef(_RequiredAppInputSourceTypeDef, _OptionalAppInputSourceTypeDef):
     pass
 
 
-_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
-        "sourceArn": str,
-        "terraformSource": TerraformSourceTypeDef,
-    },
-    total=False,
-)
-
-
-class DeleteAppInputSourceRequestRequestTypeDef(
-    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
-    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
-):
-    pass
-
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1800,30 +1860,14 @@
 class CreateResiliencyPolicyRequestRequestTypeDef(
     _RequiredCreateResiliencyPolicyRequestRequestTypeDef,
     _OptionalCreateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ResiliencyPolicyTypeDef = TypedDict(
-    "ResiliencyPolicyTypeDef",
-    {
-        "creationTime": datetime,
-        "dataLocationConstraint": DataLocationConstraintType,
-        "estimatedCostTier": EstimatedCostTierType,
-        "policy": Dict[DisruptionTypeType, FailurePolicyTypeDef],
-        "policyArn": str,
-        "policyDescription": str,
-        "policyName": str,
-        "tags": Dict[str, str],
-        "tier": ResiliencyPolicyTierType,
-    },
-    total=False,
-)
-
 _RequiredUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -1842,14 +1886,52 @@
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "sourceArn": str,
+        "terraformSource": TerraformSourceTypeDef,
+    },
+    total=False,
+)
+
+
+class DeleteAppInputSourceRequestRequestTypeDef(
+    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
+    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
+):
+    pass
+
+
+ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "eksSources": List[EksSourceOutputTypeDef],
+        "sourceArns": List[str],
+        "status": ResourceImportStatusTypeType,
+        "terraformSources": List[TerraformSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
     "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
@@ -1867,32 +1949,35 @@
 class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
     _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
     _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
 ):
     pass
 
 
-ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
+ResiliencyPolicyTypeDef = TypedDict(
+    "ResiliencyPolicyTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
-        "sourceArns": List[str],
-        "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "creationTime": datetime,
+        "dataLocationConstraint": DataLocationConstraintType,
+        "estimatedCostTier": EstimatedCostTierType,
+        "policy": Dict[DisruptionTypeType, FailurePolicyOutputTypeDef],
+        "policyArn": str,
+        "policyDescription": str,
+        "policyName": str,
+        "tags": Dict[str, str],
+        "tier": ResiliencyPolicyTierType,
     },
+    total=False,
 )
 
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdTypeDef,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "logicalResourceId": LogicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
         "resourceType": str,
     },
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
@@ -1906,44 +1991,46 @@
 )
 
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
 
 
-_RequiredResourceMappingTypeDef = TypedDict(
-    "_RequiredResourceMappingTypeDef",
+_RequiredResourceMappingOutputTypeDef = TypedDict(
+    "_RequiredResourceMappingOutputTypeDef",
     {
         "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
     },
 )
-_OptionalResourceMappingTypeDef = TypedDict(
-    "_OptionalResourceMappingTypeDef",
+_OptionalResourceMappingOutputTypeDef = TypedDict(
+    "_OptionalResourceMappingOutputTypeDef",
     {
         "appRegistryAppName": str,
         "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
 
-class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
+class ResourceMappingOutputTypeDef(
+    _RequiredResourceMappingOutputTypeDef, _OptionalResourceMappingOutputTypeDef
+):
     pass
 
 
 _RequiredUnsupportedResourceTypeDef = TypedDict(
     "_RequiredUnsupportedResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdTypeDef,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "logicalResourceId": LogicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
         "resourceType": str,
     },
 )
 _OptionalUnsupportedResourceTypeDef = TypedDict(
     "_OptionalUnsupportedResourceTypeDef",
     {
         "unsupportedResourceStatus": str,
@@ -1954,14 +2041,39 @@
 
 class UnsupportedResourceTypeDef(
     _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
 ):
     pass
 
 
+_RequiredResourceMappingTypeDef = TypedDict(
+    "_RequiredResourceMappingTypeDef",
+    {
+        "mappingType": ResourceMappingTypeType,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
+    },
+)
+_OptionalResourceMappingTypeDef = TypedDict(
+    "_OptionalResourceMappingTypeDef",
+    {
+        "appRegistryAppName": str,
+        "eksSourceName": str,
+        "logicalStackName": str,
+        "resourceGroupName": str,
+        "resourceName": str,
+        "terraformSourceName": str,
+    },
+    total=False,
+)
+
+
+class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
+    pass
+
+
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
         "recommendationTemplateArn": str,
@@ -2001,69 +2113,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -2072,153 +2184,153 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "resourceMappings": Sequence[ResourceMappingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
-        "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "resourceMappings": Sequence[ResourceMappingTypeDef],
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2252,26 +2364,26 @@
 
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub/type_defs.pyi` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for resiliencehub service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_resiliencehub.type_defs import RecommendationItemTypeDef
+    from mypy_boto3_resiliencehub.type_defs import ResponseMetadataTypeDef
 
-    data: RecommendationItemTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -50,52 +50,49 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "RecommendationItemTypeDef",
     "CostTypeDef",
     "DisruptionComplianceTypeDef",
     "ResiliencyScoreTypeDef",
     "AppComponentTypeDef",
-    "EksSourceClusterNamespaceTypeDef",
-    "TerraformSourceTypeDef",
+    "EksSourceClusterNamespaceOutputTypeDef",
+    "TerraformSourceOutputTypeDef",
     "AppSummaryTypeDef",
     "AppTypeDef",
     "AppVersionSummaryTypeDef",
     "RecommendationDisruptionComplianceTypeDef",
     "CreateAppRequestRequestTypeDef",
     "CreateAppVersionAppComponentRequestRequestTypeDef",
     "LogicalResourceIdTypeDef",
     "CreateRecommendationTemplateRequestRequestTypeDef",
     "FailurePolicyTypeDef",
     "DeleteAppAssessmentRequestRequestTypeDef",
-    "DeleteAppAssessmentResponseTypeDef",
+    "EksSourceClusterNamespaceTypeDef",
+    "TerraformSourceTypeDef",
     "DeleteAppRequestRequestTypeDef",
-    "DeleteAppResponseTypeDef",
     "DeleteAppVersionAppComponentRequestRequestTypeDef",
     "DeleteRecommendationTemplateRequestRequestTypeDef",
-    "DeleteRecommendationTemplateResponseTypeDef",
     "DeleteResiliencyPolicyRequestRequestTypeDef",
-    "DeleteResiliencyPolicyResponseTypeDef",
     "DescribeAppAssessmentRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeAppVersionAppComponentRequestRequestTypeDef",
     "DescribeAppVersionRequestRequestTypeDef",
     "DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef",
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    "DescribeAppVersionResponseTypeDef",
     "DescribeAppVersionTemplateRequestRequestTypeDef",
-    "DescribeAppVersionTemplateResponseTypeDef",
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
     "DescribeResiliencyPolicyRequestRequestTypeDef",
+    "EksSourceOutputTypeDef",
     "EksSourceTypeDef",
+    "FailurePolicyOutputTypeDef",
     "ListAlarmRecommendationsRequestRequestTypeDef",
     "ListAppAssessmentsRequestRequestTypeDef",
     "ListAppComponentCompliancesRequestRequestTypeDef",
     "ListAppComponentRecommendationsRequestRequestTypeDef",
     "ListAppInputSourcesRequestRequestTypeDef",
     "ListAppVersionAppComponentsRequestRequestTypeDef",
     "ListAppVersionResourceMappingsRequestRequestTypeDef",
@@ -103,66 +100,76 @@
     "ListAppVersionsRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
     "ListRecommendationTemplatesRequestRequestTypeDef",
     "ListResiliencyPoliciesRequestRequestTypeDef",
     "ListSopRecommendationsRequestRequestTypeDef",
     "ListSuggestedResiliencyPoliciesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTestRecommendationsRequestRequestTypeDef",
     "ListUnsupportedAppVersionResourcesRequestRequestTypeDef",
+    "LogicalResourceIdOutputTypeDef",
+    "PhysicalResourceIdOutputTypeDef",
     "PhysicalResourceIdTypeDef",
     "PublishAppVersionRequestRequestTypeDef",
-    "PublishAppVersionResponseTypeDef",
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
-    "PutDraftAppVersionTemplateResponseTypeDef",
     "S3LocationTypeDef",
     "RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
     "ResolveAppVersionResourcesRequestRequestTypeDef",
-    "ResolveAppVersionResourcesResponseTypeDef",
     "ResourceErrorTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAppAssessmentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "UpdateAppVersionAppComponentRequestRequestTypeDef",
     "UpdateAppVersionRequestRequestTypeDef",
+    "DeleteAppAssessmentResponseTypeDef",
+    "DeleteAppResponseTypeDef",
+    "DeleteRecommendationTemplateResponseTypeDef",
+    "DeleteResiliencyPolicyResponseTypeDef",
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    "DescribeAppVersionResponseTypeDef",
+    "DescribeAppVersionTemplateResponseTypeDef",
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PublishAppVersionResponseTypeDef",
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    "ResolveAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResponseTypeDef",
     "AlarmRecommendationTypeDef",
     "SopRecommendationTypeDef",
     "TestRecommendationTypeDef",
     "AppAssessmentSummaryTypeDef",
     "AppComponentComplianceTypeDef",
     "CreateAppVersionAppComponentResponseTypeDef",
     "DeleteAppVersionAppComponentResponseTypeDef",
     "DescribeAppVersionAppComponentResponseTypeDef",
     "ListAppVersionAppComponentsResponseTypeDef",
     "UpdateAppVersionAppComponentResponseTypeDef",
     "AppInputSourceTypeDef",
-    "DeleteAppInputSourceRequestRequestTypeDef",
     "ListAppsResponseTypeDef",
     "CreateAppResponseTypeDef",
     "DescribeAppResponseTypeDef",
     "UpdateAppResponseTypeDef",
     "ListAppVersionsResponseTypeDef",
     "ConfigRecommendationTypeDef",
     "CreateAppVersionResourceRequestRequestTypeDef",
     "DeleteAppVersionResourceRequestRequestTypeDef",
     "DescribeAppVersionResourceRequestRequestTypeDef",
     "UpdateAppVersionResourceRequestRequestTypeDef",
     "CreateResiliencyPolicyRequestRequestTypeDef",
-    "ResiliencyPolicyTypeDef",
     "UpdateResiliencyPolicyRequestRequestTypeDef",
-    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "DeleteAppInputSourceRequestRequestTypeDef",
     "ImportResourcesToDraftAppVersionResponseTypeDef",
+    "ImportResourcesToDraftAppVersionRequestRequestTypeDef",
+    "ResiliencyPolicyTypeDef",
     "PhysicalResourceTypeDef",
-    "ResourceMappingTypeDef",
+    "ResourceMappingOutputTypeDef",
     "UnsupportedResourceTypeDef",
+    "ResourceMappingTypeDef",
     "RecommendationTemplateTypeDef",
     "ResourceErrorsDetailsTypeDef",
     "ListAlarmRecommendationsResponseTypeDef",
     "ListSopRecommendationsResponseTypeDef",
     "ListTestRecommendationsResponseTypeDef",
     "ListAppAssessmentsResponseTypeDef",
     "ListAppComponentCompliancesResponseTypeDef",
@@ -175,26 +182,37 @@
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     "UpdateResiliencyPolicyResponseTypeDef",
     "CreateAppVersionResourceResponseTypeDef",
     "DeleteAppVersionResourceResponseTypeDef",
     "DescribeAppVersionResourceResponseTypeDef",
     "ListAppVersionResourcesResponseTypeDef",
     "UpdateAppVersionResourceResponseTypeDef",
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     "ListAppVersionResourceMappingsResponseTypeDef",
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
     "CreateRecommendationTemplateResponseTypeDef",
     "ListRecommendationTemplatesResponseTypeDef",
     "AppAssessmentTypeDef",
     "ListAppComponentRecommendationsResponseTypeDef",
     "DescribeAppAssessmentResponseTypeDef",
     "StartAppAssessmentResponseTypeDef",
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
 RecommendationItemTypeDef = TypedDict(
     "RecommendationItemTypeDef",
     {
         "alreadyImplemented": bool,
         "resourceId": str,
         "targetAccountId": str,
         "targetRegion": str,
@@ -261,24 +279,24 @@
     },
     total=False,
 )
 
 class AppComponentTypeDef(_RequiredAppComponentTypeDef, _OptionalAppComponentTypeDef):
     pass
 
-EksSourceClusterNamespaceTypeDef = TypedDict(
-    "EksSourceClusterNamespaceTypeDef",
+EksSourceClusterNamespaceOutputTypeDef = TypedDict(
+    "EksSourceClusterNamespaceOutputTypeDef",
     {
         "eksClusterArn": str,
         "namespace": str,
     },
 )
 
-TerraformSourceTypeDef = TypedDict(
-    "TerraformSourceTypeDef",
+TerraformSourceOutputTypeDef = TypedDict(
+    "TerraformSourceOutputTypeDef",
     {
         "s3StateFileUrl": str,
     },
 )
 
 _RequiredAppSummaryTypeDef = TypedDict(
     "_RequiredAppSummaryTypeDef",
@@ -479,20 +497,26 @@
 
 class DeleteAppAssessmentRequestRequestTypeDef(
     _RequiredDeleteAppAssessmentRequestRequestTypeDef,
     _OptionalDeleteAppAssessmentRequestRequestTypeDef,
 ):
     pass
 
-DeleteAppAssessmentResponseTypeDef = TypedDict(
-    "DeleteAppAssessmentResponseTypeDef",
+EksSourceClusterNamespaceTypeDef = TypedDict(
+    "EksSourceClusterNamespaceTypeDef",
     {
-        "assessmentArn": str,
-        "assessmentStatus": AssessmentStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eksClusterArn": str,
+        "namespace": str,
+    },
+)
+
+TerraformSourceTypeDef = TypedDict(
+    "TerraformSourceTypeDef",
+    {
+        "s3StateFileUrl": str,
     },
 )
 
 _RequiredDeleteAppRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppRequestRequestTypeDef",
     {
         "appArn": str,
@@ -508,22 +532,14 @@
 )
 
 class DeleteAppRequestRequestTypeDef(
     _RequiredDeleteAppRequestRequestTypeDef, _OptionalDeleteAppRequestRequestTypeDef
 ):
     pass
 
-DeleteAppResponseTypeDef = TypedDict(
-    "DeleteAppResponseTypeDef",
-    {
-        "appArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteAppVersionAppComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAppVersionAppComponentRequestRequestTypeDef",
     {
         "appArn": str,
         "id": str,
     },
 )
@@ -557,23 +573,14 @@
 
 class DeleteRecommendationTemplateRequestRequestTypeDef(
     _RequiredDeleteRecommendationTemplateRequestRequestTypeDef,
     _OptionalDeleteRecommendationTemplateRequestRequestTypeDef,
 ):
     pass
 
-DeleteRecommendationTemplateResponseTypeDef = TypedDict(
-    "DeleteRecommendationTemplateResponseTypeDef",
-    {
-        "recommendationTemplateArn": str,
-        "status": RecommendationTemplateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalDeleteResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -586,22 +593,14 @@
 
 class DeleteResiliencyPolicyRequestRequestTypeDef(
     _RequiredDeleteResiliencyPolicyRequestRequestTypeDef,
     _OptionalDeleteResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteResiliencyPolicyResponseTypeDef = TypedDict(
-    "DeleteResiliencyPolicyResponseTypeDef",
-    {
-        "policyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppAssessmentRequestRequestTypeDef = TypedDict(
     "DescribeAppAssessmentRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 
@@ -646,88 +645,60 @@
 
 class DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef(
     _RequiredDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
     _OptionalDescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
 ):
     pass
 
-DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
-    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAppVersionResponseTypeDef = TypedDict(
-    "DescribeAppVersionResponseTypeDef",
-    {
-        "additionalInfo": Dict[str, List[str]],
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "DescribeAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-DescribeAppVersionTemplateResponseTypeDef = TypedDict(
-    "DescribeAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appTemplateBody": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef = TypedDict(
     "DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
-    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResiliencyPolicyRequestRequestTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "errorMessage": str,
-        "status": ResourceImportStatusTypeType,
-        "statusChangeTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "policyArn": str,
     },
 )
 
-DescribeResiliencyPolicyRequestRequestTypeDef = TypedDict(
-    "DescribeResiliencyPolicyRequestRequestTypeDef",
+EksSourceOutputTypeDef = TypedDict(
+    "EksSourceOutputTypeDef",
     {
-        "policyArn": str,
+        "eksClusterArn": str,
+        "namespaces": List[str],
     },
 )
 
 EksSourceTypeDef = TypedDict(
     "EksSourceTypeDef",
     {
         "eksClusterArn": str,
         "namespaces": Sequence[str],
     },
 )
 
+FailurePolicyOutputTypeDef = TypedDict(
+    "FailurePolicyOutputTypeDef",
+    {
+        "rpoInSecs": int,
+        "rtoInSecs": int,
+    },
+)
+
 _RequiredListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlarmRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListAlarmRecommendationsRequestRequestTypeDef = TypedDict(
@@ -990,22 +961,14 @@
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
 _RequiredListTestRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListTestRecommendationsRequestRequestTypeDef",
     {
         "assessmentArn": str,
     },
 )
 _OptionalListTestRecommendationsRequestRequestTypeDef = TypedDict(
@@ -1042,14 +1005,57 @@
 
 class ListUnsupportedAppVersionResourcesRequestRequestTypeDef(
     _RequiredListUnsupportedAppVersionResourcesRequestRequestTypeDef,
     _OptionalListUnsupportedAppVersionResourcesRequestRequestTypeDef,
 ):
     pass
 
+_RequiredLogicalResourceIdOutputTypeDef = TypedDict(
+    "_RequiredLogicalResourceIdOutputTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalLogicalResourceIdOutputTypeDef = TypedDict(
+    "_OptionalLogicalResourceIdOutputTypeDef",
+    {
+        "eksSourceName": str,
+        "logicalStackName": str,
+        "resourceGroupName": str,
+        "terraformSourceName": str,
+    },
+    total=False,
+)
+
+class LogicalResourceIdOutputTypeDef(
+    _RequiredLogicalResourceIdOutputTypeDef, _OptionalLogicalResourceIdOutputTypeDef
+):
+    pass
+
+_RequiredPhysicalResourceIdOutputTypeDef = TypedDict(
+    "_RequiredPhysicalResourceIdOutputTypeDef",
+    {
+        "identifier": str,
+        "type": PhysicalIdentifierTypeType,
+    },
+)
+_OptionalPhysicalResourceIdOutputTypeDef = TypedDict(
+    "_OptionalPhysicalResourceIdOutputTypeDef",
+    {
+        "awsAccountId": str,
+        "awsRegion": str,
+    },
+    total=False,
+)
+
+class PhysicalResourceIdOutputTypeDef(
+    _RequiredPhysicalResourceIdOutputTypeDef, _OptionalPhysicalResourceIdOutputTypeDef
+):
+    pass
+
 _RequiredPhysicalResourceIdTypeDef = TypedDict(
     "_RequiredPhysicalResourceIdTypeDef",
     {
         "identifier": str,
         "type": PhysicalIdentifierTypeType,
     },
 )
@@ -1070,40 +1076,22 @@
 PublishAppVersionRequestRequestTypeDef = TypedDict(
     "PublishAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 
-PublishAppVersionResponseTypeDef = TypedDict(
-    "PublishAppVersionResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDraftAppVersionTemplateRequestRequestTypeDef = TypedDict(
     "PutDraftAppVersionTemplateRequestRequestTypeDef",
     {
         "appArn": str,
         "appTemplateBody": str,
     },
 )
 
-PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
-    "PutDraftAppVersionTemplateResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -1130,63 +1118,32 @@
 
 class RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef(
     _RequiredRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
     _OptionalRemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
 ):
     pass
 
-RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
-    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveAppVersionResourcesRequestRequestTypeDef = TypedDict(
     "ResolveAppVersionResourcesRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
     },
 )
 
-ResolveAppVersionResourcesResponseTypeDef = TypedDict(
-    "ResolveAppVersionResourcesResponseTypeDef",
-    {
-        "appArn": str,
-        "appVersion": str,
-        "resolutionId": str,
-        "status": ResourceResolutionStatusTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceErrorTypeDef = TypedDict(
     "ResourceErrorTypeDef",
     {
         "logicalResourceId": str,
         "physicalResourceId": str,
         "reason": str,
     },
     total=False,
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
 _RequiredStartAppAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredStartAppAssessmentRequestRequestTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "assessmentName": str,
     },
@@ -1282,21 +1239,145 @@
 )
 
 class UpdateAppVersionRequestRequestTypeDef(
     _RequiredUpdateAppVersionRequestRequestTypeDef, _OptionalUpdateAppVersionRequestRequestTypeDef
 ):
     pass
 
+DeleteAppAssessmentResponseTypeDef = TypedDict(
+    "DeleteAppAssessmentResponseTypeDef",
+    {
+        "assessmentArn": str,
+        "assessmentStatus": AssessmentStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAppResponseTypeDef = TypedDict(
+    "DeleteAppResponseTypeDef",
+    {
+        "appArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRecommendationTemplateResponseTypeDef = TypedDict(
+    "DeleteRecommendationTemplateResponseTypeDef",
+    {
+        "recommendationTemplateArn": str,
+        "status": RecommendationTemplateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteResiliencyPolicyResponseTypeDef = TypedDict(
+    "DeleteResiliencyPolicyResponseTypeDef",
+    {
+        "policyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResourcesResolutionStatusResponseTypeDef = TypedDict(
+    "DescribeAppVersionResourcesResolutionStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionResponseTypeDef = TypedDict(
+    "DescribeAppVersionResponseTypeDef",
+    {
+        "additionalInfo": Dict[str, List[str]],
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppVersionTemplateResponseTypeDef = TypedDict(
+    "DescribeAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appTemplateBody": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDraftAppVersionResourcesImportStatusResponseTypeDef = TypedDict(
+    "DescribeDraftAppVersionResourcesImportStatusResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "errorMessage": str,
+        "status": ResourceImportStatusTypeType,
+        "statusChangeTime": datetime,
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
+PublishAppVersionResponseTypeDef = TypedDict(
+    "PublishAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDraftAppVersionTemplateResponseTypeDef = TypedDict(
+    "PutDraftAppVersionTemplateResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
+    "RemoveDraftAppVersionResourceMappingsResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResolveAppVersionResourcesResponseTypeDef = TypedDict(
+    "ResolveAppVersionResourcesResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "resolutionId": str,
+        "status": ResourceResolutionStatusTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateAppVersionResponseTypeDef = TypedDict(
     "UpdateAppVersionResponseTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
         "appArn": str,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAlarmRecommendationTypeDef = TypedDict(
     "_RequiredAlarmRecommendationTypeDef",
     {
         "name": str,
@@ -1418,142 +1499,119 @@
 
 CreateAppVersionAppComponentResponseTypeDef = TypedDict(
     "CreateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionAppComponentResponseTypeDef = TypedDict(
     "DeleteAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionAppComponentResponseTypeDef = TypedDict(
     "DescribeAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionAppComponentsResponseTypeDef = TypedDict(
     "ListAppVersionAppComponentsResponseTypeDef",
     {
         "appArn": str,
         "appComponents": List[AppComponentTypeDef],
         "appVersion": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionAppComponentResponseTypeDef = TypedDict(
     "UpdateAppVersionAppComponentResponseTypeDef",
     {
         "appArn": str,
         "appComponent": AppComponentTypeDef,
         "appVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppInputSourceTypeDef = TypedDict(
     "_RequiredAppInputSourceTypeDef",
     {
         "importType": ResourceMappingTypeType,
     },
 )
 _OptionalAppInputSourceTypeDef = TypedDict(
     "_OptionalAppInputSourceTypeDef",
     {
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceOutputTypeDef,
         "resourceCount": int,
         "sourceArn": str,
         "sourceName": str,
-        "terraformSource": TerraformSourceTypeDef,
+        "terraformSource": TerraformSourceOutputTypeDef,
     },
     total=False,
 )
 
 class AppInputSourceTypeDef(_RequiredAppInputSourceTypeDef, _OptionalAppInputSourceTypeDef):
     pass
 
-_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "appArn": str,
-    },
-)
-_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
-    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
-        "sourceArn": str,
-        "terraformSource": TerraformSourceTypeDef,
-    },
-    total=False,
-)
-
-class DeleteAppInputSourceRequestRequestTypeDef(
-    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
-    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
-):
-    pass
-
 ListAppsResponseTypeDef = TypedDict(
     "ListAppsResponseTypeDef",
     {
         "appSummaries": List[AppSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppResponseTypeDef = TypedDict(
     "CreateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppResponseTypeDef = TypedDict(
     "DescribeAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppResponseTypeDef = TypedDict(
     "UpdateAppResponseTypeDef",
     {
         "app": AppTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionsResponseTypeDef = TypedDict(
     "ListAppVersionsResponseTypeDef",
     {
         "appVersions": List[AppVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfigRecommendationTypeDef = TypedDict(
     "_RequiredConfigRecommendationTypeDef",
     {
         "name": str,
@@ -1709,30 +1767,14 @@
 
 class CreateResiliencyPolicyRequestRequestTypeDef(
     _RequiredCreateResiliencyPolicyRequestRequestTypeDef,
     _OptionalCreateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
-ResiliencyPolicyTypeDef = TypedDict(
-    "ResiliencyPolicyTypeDef",
-    {
-        "creationTime": datetime,
-        "dataLocationConstraint": DataLocationConstraintType,
-        "estimatedCostTier": EstimatedCostTierType,
-        "policy": Dict[DisruptionTypeType, FailurePolicyTypeDef],
-        "policyArn": str,
-        "policyDescription": str,
-        "policyName": str,
-        "tags": Dict[str, str],
-        "tier": ResiliencyPolicyTierType,
-    },
-    total=False,
-)
-
 _RequiredUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResiliencyPolicyRequestRequestTypeDef",
     {
         "policyArn": str,
     },
 )
 _OptionalUpdateResiliencyPolicyRequestRequestTypeDef = TypedDict(
@@ -1749,14 +1791,50 @@
 
 class UpdateResiliencyPolicyRequestRequestTypeDef(
     _RequiredUpdateResiliencyPolicyRequestRequestTypeDef,
     _OptionalUpdateResiliencyPolicyRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_RequiredDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "appArn": str,
+    },
+)
+_OptionalDeleteAppInputSourceRequestRequestTypeDef = TypedDict(
+    "_OptionalDeleteAppInputSourceRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "eksSourceClusterNamespace": EksSourceClusterNamespaceTypeDef,
+        "sourceArn": str,
+        "terraformSource": TerraformSourceTypeDef,
+    },
+    total=False,
+)
+
+class DeleteAppInputSourceRequestRequestTypeDef(
+    _RequiredDeleteAppInputSourceRequestRequestTypeDef,
+    _OptionalDeleteAppInputSourceRequestRequestTypeDef,
+):
+    pass
+
+ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
+    "ImportResourcesToDraftAppVersionResponseTypeDef",
+    {
+        "appArn": str,
+        "appVersion": str,
+        "eksSources": List[EksSourceOutputTypeDef],
+        "sourceArns": List[str],
+        "status": ResourceImportStatusTypeType,
+        "terraformSources": List[TerraformSourceOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
     "_RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef",
     {
         "appArn": str,
     },
 )
 _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef = TypedDict(
@@ -1772,32 +1850,35 @@
 
 class ImportResourcesToDraftAppVersionRequestRequestTypeDef(
     _RequiredImportResourcesToDraftAppVersionRequestRequestTypeDef,
     _OptionalImportResourcesToDraftAppVersionRequestRequestTypeDef,
 ):
     pass
 
-ImportResourcesToDraftAppVersionResponseTypeDef = TypedDict(
-    "ImportResourcesToDraftAppVersionResponseTypeDef",
+ResiliencyPolicyTypeDef = TypedDict(
+    "ResiliencyPolicyTypeDef",
     {
-        "appArn": str,
-        "appVersion": str,
-        "eksSources": List[EksSourceTypeDef],
-        "sourceArns": List[str],
-        "status": ResourceImportStatusTypeType,
-        "terraformSources": List[TerraformSourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "creationTime": datetime,
+        "dataLocationConstraint": DataLocationConstraintType,
+        "estimatedCostTier": EstimatedCostTierType,
+        "policy": Dict[DisruptionTypeType, FailurePolicyOutputTypeDef],
+        "policyArn": str,
+        "policyDescription": str,
+        "policyName": str,
+        "tags": Dict[str, str],
+        "tier": ResiliencyPolicyTierType,
     },
+    total=False,
 )
 
 _RequiredPhysicalResourceTypeDef = TypedDict(
     "_RequiredPhysicalResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdTypeDef,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "logicalResourceId": LogicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
         "resourceType": str,
     },
 )
 _OptionalPhysicalResourceTypeDef = TypedDict(
     "_OptionalPhysicalResourceTypeDef",
     {
         "additionalInfo": Dict[str, List[str]],
@@ -1809,42 +1890,44 @@
     },
     total=False,
 )
 
 class PhysicalResourceTypeDef(_RequiredPhysicalResourceTypeDef, _OptionalPhysicalResourceTypeDef):
     pass
 
-_RequiredResourceMappingTypeDef = TypedDict(
-    "_RequiredResourceMappingTypeDef",
+_RequiredResourceMappingOutputTypeDef = TypedDict(
+    "_RequiredResourceMappingOutputTypeDef",
     {
         "mappingType": ResourceMappingTypeType,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
     },
 )
-_OptionalResourceMappingTypeDef = TypedDict(
-    "_OptionalResourceMappingTypeDef",
+_OptionalResourceMappingOutputTypeDef = TypedDict(
+    "_OptionalResourceMappingOutputTypeDef",
     {
         "appRegistryAppName": str,
         "eksSourceName": str,
         "logicalStackName": str,
         "resourceGroupName": str,
         "resourceName": str,
         "terraformSourceName": str,
     },
     total=False,
 )
 
-class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
+class ResourceMappingOutputTypeDef(
+    _RequiredResourceMappingOutputTypeDef, _OptionalResourceMappingOutputTypeDef
+):
     pass
 
 _RequiredUnsupportedResourceTypeDef = TypedDict(
     "_RequiredUnsupportedResourceTypeDef",
     {
-        "logicalResourceId": LogicalResourceIdTypeDef,
-        "physicalResourceId": PhysicalResourceIdTypeDef,
+        "logicalResourceId": LogicalResourceIdOutputTypeDef,
+        "physicalResourceId": PhysicalResourceIdOutputTypeDef,
         "resourceType": str,
     },
 )
 _OptionalUnsupportedResourceTypeDef = TypedDict(
     "_OptionalUnsupportedResourceTypeDef",
     {
         "unsupportedResourceStatus": str,
@@ -1853,14 +1936,37 @@
 )
 
 class UnsupportedResourceTypeDef(
     _RequiredUnsupportedResourceTypeDef, _OptionalUnsupportedResourceTypeDef
 ):
     pass
 
+_RequiredResourceMappingTypeDef = TypedDict(
+    "_RequiredResourceMappingTypeDef",
+    {
+        "mappingType": ResourceMappingTypeType,
+        "physicalResourceId": PhysicalResourceIdTypeDef,
+    },
+)
+_OptionalResourceMappingTypeDef = TypedDict(
+    "_OptionalResourceMappingTypeDef",
+    {
+        "appRegistryAppName": str,
+        "eksSourceName": str,
+        "logicalStackName": str,
+        "resourceGroupName": str,
+        "resourceName": str,
+        "terraformSourceName": str,
+    },
+    total=False,
+)
+
+class ResourceMappingTypeDef(_RequiredResourceMappingTypeDef, _OptionalResourceMappingTypeDef):
+    pass
+
 _RequiredRecommendationTemplateTypeDef = TypedDict(
     "_RequiredRecommendationTemplateTypeDef",
     {
         "assessmentArn": str,
         "format": TemplateFormatType,
         "name": str,
         "recommendationTemplateArn": str,
@@ -1898,69 +2004,69 @@
 )
 
 ListAlarmRecommendationsResponseTypeDef = TypedDict(
     "ListAlarmRecommendationsResponseTypeDef",
     {
         "alarmRecommendations": List[AlarmRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSopRecommendationsResponseTypeDef = TypedDict(
     "ListSopRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "sopRecommendations": List[SopRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTestRecommendationsResponseTypeDef = TypedDict(
     "ListTestRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "testRecommendations": List[TestRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAssessmentsResponseTypeDef = TypedDict(
     "ListAppAssessmentsResponseTypeDef",
     {
         "assessmentSummaries": List[AppAssessmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppComponentCompliancesResponseTypeDef = TypedDict(
     "ListAppComponentCompliancesResponseTypeDef",
     {
         "componentCompliances": List[AppComponentComplianceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppInputSourceResponseTypeDef = TypedDict(
     "DeleteAppInputSourceResponseTypeDef",
     {
         "appArn": str,
         "appInputSource": AppInputSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInputSourcesResponseTypeDef = TypedDict(
     "ListAppInputSourcesResponseTypeDef",
     {
         "appInputSources": List[AppInputSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRecommendationTypeDef = TypedDict(
     "ComponentRecommendationTypeDef",
     {
         "appComponentName": str,
@@ -1969,153 +2075,153 @@
     },
 )
 
 CreateResiliencyPolicyResponseTypeDef = TypedDict(
     "CreateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResiliencyPolicyResponseTypeDef = TypedDict(
     "DescribeResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuggestedResiliencyPoliciesResponseTypeDef = TypedDict(
     "ListSuggestedResiliencyPoliciesResponseTypeDef",
     {
         "nextToken": str,
         "resiliencyPolicies": List[ResiliencyPolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResiliencyPolicyResponseTypeDef = TypedDict(
     "UpdateResiliencyPolicyResponseTypeDef",
     {
         "policy": ResiliencyPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppVersionResourceResponseTypeDef = TypedDict(
     "CreateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAppVersionResourceResponseTypeDef = TypedDict(
     "DeleteAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppVersionResourceResponseTypeDef = TypedDict(
     "DescribeAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourcesResponseTypeDef = TypedDict(
     "ListAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "physicalResources": List[PhysicalResourceTypeDef],
         "resolutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppVersionResourceResponseTypeDef = TypedDict(
     "UpdateAppVersionResourceResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
         "physicalResource": PhysicalResourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
-    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
-    {
-        "appArn": str,
-        "resourceMappings": Sequence[ResourceMappingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddDraftAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "AddDraftAppVersionResourceMappingsResponseTypeDef",
     {
         "appArn": str,
         "appVersion": str,
-        "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppVersionResourceMappingsResponseTypeDef = TypedDict(
     "ListAppVersionResourceMappingsResponseTypeDef",
     {
         "nextToken": str,
-        "resourceMappings": List[ResourceMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceMappings": List[ResourceMappingOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUnsupportedAppVersionResourcesResponseTypeDef = TypedDict(
     "ListUnsupportedAppVersionResourcesResponseTypeDef",
     {
         "nextToken": str,
         "resolutionId": str,
         "unsupportedResources": List[UnsupportedResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddDraftAppVersionResourceMappingsRequestRequestTypeDef = TypedDict(
+    "AddDraftAppVersionResourceMappingsRequestRequestTypeDef",
+    {
+        "appArn": str,
+        "resourceMappings": Sequence[ResourceMappingTypeDef],
     },
 )
 
 CreateRecommendationTemplateResponseTypeDef = TypedDict(
     "CreateRecommendationTemplateResponseTypeDef",
     {
         "recommendationTemplate": RecommendationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecommendationTemplatesResponseTypeDef = TypedDict(
     "ListRecommendationTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationTemplates": List[RecommendationTemplateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAppAssessmentTypeDef = TypedDict(
     "_RequiredAppAssessmentTypeDef",
     {
         "assessmentArn": str,
@@ -2147,26 +2253,26 @@
     pass
 
 ListAppComponentRecommendationsResponseTypeDef = TypedDict(
     "ListAppComponentRecommendationsResponseTypeDef",
     {
         "componentRecommendations": List[ComponentRecommendationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppAssessmentResponseTypeDef = TypedDict(
     "DescribeAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAppAssessmentResponseTypeDef = TypedDict(
     "StartAppAssessmentResponseTypeDef",
     {
         "assessment": AppAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/PKG-INFO` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resiliencehub
-Version: 1.28.0
-Summary: Type annotations for boto3.ResilienceHub 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-resiliencehub"></a>
 
 # mypy-boto3-resiliencehub
 
 [![PyPI - mypy-boto3-resiliencehub](https://img.shields.io/pypi/v/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resiliencehub.svg?color=blue)](https://pypi.org/project/mypy-boto3-resiliencehub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-resiliencehub?color=blue)](https://pypistats.org/packages/mypy-boto3-resiliencehub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resiliencehub)](https://pepy.tech/project/mypy-boto3-resiliencehub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResilienceHub 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
+[boto3.ResilienceHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#ResilienceHub)
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
 [mypy-boto3-resiliencehub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resiliencehub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,52 +323,49 @@
 ### Typed dictionaries
 
 `mypy_boto3_resiliencehub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_resiliencehub.type_defs import (
+    ResponseMetadataTypeDef,
     RecommendationItemTypeDef,
     CostTypeDef,
     DisruptionComplianceTypeDef,
     ResiliencyScoreTypeDef,
     AppComponentTypeDef,
-    EksSourceClusterNamespaceTypeDef,
-    TerraformSourceTypeDef,
+    EksSourceClusterNamespaceOutputTypeDef,
+    TerraformSourceOutputTypeDef,
     AppSummaryTypeDef,
     AppTypeDef,
     AppVersionSummaryTypeDef,
     RecommendationDisruptionComplianceTypeDef,
     CreateAppRequestRequestTypeDef,
     CreateAppVersionAppComponentRequestRequestTypeDef,
     LogicalResourceIdTypeDef,
     CreateRecommendationTemplateRequestRequestTypeDef,
     FailurePolicyTypeDef,
     DeleteAppAssessmentRequestRequestTypeDef,
-    DeleteAppAssessmentResponseTypeDef,
+    EksSourceClusterNamespaceTypeDef,
+    TerraformSourceTypeDef,
     DeleteAppRequestRequestTypeDef,
-    DeleteAppResponseTypeDef,
     DeleteAppVersionAppComponentRequestRequestTypeDef,
     DeleteRecommendationTemplateRequestRequestTypeDef,
-    DeleteRecommendationTemplateResponseTypeDef,
     DeleteResiliencyPolicyRequestRequestTypeDef,
-    DeleteResiliencyPolicyResponseTypeDef,
     DescribeAppAssessmentRequestRequestTypeDef,
     DescribeAppRequestRequestTypeDef,
     DescribeAppVersionAppComponentRequestRequestTypeDef,
     DescribeAppVersionRequestRequestTypeDef,
     DescribeAppVersionResourcesResolutionStatusRequestRequestTypeDef,
-    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
-    DescribeAppVersionResponseTypeDef,
     DescribeAppVersionTemplateRequestRequestTypeDef,
-    DescribeAppVersionTemplateResponseTypeDef,
     DescribeDraftAppVersionResourcesImportStatusRequestRequestTypeDef,
-    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
     DescribeResiliencyPolicyRequestRequestTypeDef,
+    EksSourceOutputTypeDef,
     EksSourceTypeDef,
+    FailurePolicyOutputTypeDef,
     ListAlarmRecommendationsRequestRequestTypeDef,
     ListAppAssessmentsRequestRequestTypeDef,
     ListAppComponentCompliancesRequestRequestTypeDef,
     ListAppComponentRecommendationsRequestRequestTypeDef,
     ListAppInputSourcesRequestRequestTypeDef,
     ListAppVersionAppComponentsRequestRequestTypeDef,
     ListAppVersionResourceMappingsRequestRequestTypeDef,
@@ -376,66 +373,76 @@
     ListAppVersionsRequestRequestTypeDef,
     ListAppsRequestRequestTypeDef,
     ListRecommendationTemplatesRequestRequestTypeDef,
     ListResiliencyPoliciesRequestRequestTypeDef,
     ListSopRecommendationsRequestRequestTypeDef,
     ListSuggestedResiliencyPoliciesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTestRecommendationsRequestRequestTypeDef,
     ListUnsupportedAppVersionResourcesRequestRequestTypeDef,
+    LogicalResourceIdOutputTypeDef,
+    PhysicalResourceIdOutputTypeDef,
     PhysicalResourceIdTypeDef,
     PublishAppVersionRequestRequestTypeDef,
-    PublishAppVersionResponseTypeDef,
     PutDraftAppVersionTemplateRequestRequestTypeDef,
-    PutDraftAppVersionTemplateResponseTypeDef,
     S3LocationTypeDef,
     RemoveDraftAppVersionResourceMappingsRequestRequestTypeDef,
-    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
     ResolveAppVersionResourcesRequestRequestTypeDef,
-    ResolveAppVersionResourcesResponseTypeDef,
     ResourceErrorTypeDef,
-    ResponseMetadataTypeDef,
     StartAppAssessmentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAppRequestRequestTypeDef,
     UpdateAppVersionAppComponentRequestRequestTypeDef,
     UpdateAppVersionRequestRequestTypeDef,
+    DeleteAppAssessmentResponseTypeDef,
+    DeleteAppResponseTypeDef,
+    DeleteRecommendationTemplateResponseTypeDef,
+    DeleteResiliencyPolicyResponseTypeDef,
+    DescribeAppVersionResourcesResolutionStatusResponseTypeDef,
+    DescribeAppVersionResponseTypeDef,
+    DescribeAppVersionTemplateResponseTypeDef,
+    DescribeDraftAppVersionResourcesImportStatusResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PublishAppVersionResponseTypeDef,
+    PutDraftAppVersionTemplateResponseTypeDef,
+    RemoveDraftAppVersionResourceMappingsResponseTypeDef,
+    ResolveAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResponseTypeDef,
     AlarmRecommendationTypeDef,
     SopRecommendationTypeDef,
     TestRecommendationTypeDef,
     AppAssessmentSummaryTypeDef,
     AppComponentComplianceTypeDef,
     CreateAppVersionAppComponentResponseTypeDef,
     DeleteAppVersionAppComponentResponseTypeDef,
     DescribeAppVersionAppComponentResponseTypeDef,
     ListAppVersionAppComponentsResponseTypeDef,
     UpdateAppVersionAppComponentResponseTypeDef,
     AppInputSourceTypeDef,
-    DeleteAppInputSourceRequestRequestTypeDef,
     ListAppsResponseTypeDef,
     CreateAppResponseTypeDef,
     DescribeAppResponseTypeDef,
     UpdateAppResponseTypeDef,
     ListAppVersionsResponseTypeDef,
     ConfigRecommendationTypeDef,
     CreateAppVersionResourceRequestRequestTypeDef,
     DeleteAppVersionResourceRequestRequestTypeDef,
     DescribeAppVersionResourceRequestRequestTypeDef,
     UpdateAppVersionResourceRequestRequestTypeDef,
     CreateResiliencyPolicyRequestRequestTypeDef,
-    ResiliencyPolicyTypeDef,
     UpdateResiliencyPolicyRequestRequestTypeDef,
-    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    DeleteAppInputSourceRequestRequestTypeDef,
     ImportResourcesToDraftAppVersionResponseTypeDef,
+    ImportResourcesToDraftAppVersionRequestRequestTypeDef,
+    ResiliencyPolicyTypeDef,
     PhysicalResourceTypeDef,
-    ResourceMappingTypeDef,
+    ResourceMappingOutputTypeDef,
     UnsupportedResourceTypeDef,
+    ResourceMappingTypeDef,
     RecommendationTemplateTypeDef,
     ResourceErrorsDetailsTypeDef,
     ListAlarmRecommendationsResponseTypeDef,
     ListSopRecommendationsResponseTypeDef,
     ListTestRecommendationsResponseTypeDef,
     ListAppAssessmentsResponseTypeDef,
     ListAppComponentCompliancesResponseTypeDef,
@@ -448,28 +455,28 @@
     ListSuggestedResiliencyPoliciesResponseTypeDef,
     UpdateResiliencyPolicyResponseTypeDef,
     CreateAppVersionResourceResponseTypeDef,
     DeleteAppVersionResourceResponseTypeDef,
     DescribeAppVersionResourceResponseTypeDef,
     ListAppVersionResourcesResponseTypeDef,
     UpdateAppVersionResourceResponseTypeDef,
-    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     AddDraftAppVersionResourceMappingsResponseTypeDef,
     ListAppVersionResourceMappingsResponseTypeDef,
     ListUnsupportedAppVersionResourcesResponseTypeDef,
+    AddDraftAppVersionResourceMappingsRequestRequestTypeDef,
     CreateRecommendationTemplateResponseTypeDef,
     ListRecommendationTemplatesResponseTypeDef,
     AppAssessmentTypeDef,
     ListAppComponentRecommendationsResponseTypeDef,
     DescribeAppAssessmentResponseTypeDef,
     StartAppAssessmentResponseTypeDef,
 )
 
 
-def get_structure() -> RecommendationItemTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-resiliencehub-1.28.0/mypy_boto3_resiliencehub.egg-info/SOURCES.txt` & `mypy-boto3-resiliencehub-1.28.12/mypy_boto3_resiliencehub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resiliencehub-1.28.0/setup.py` & `mypy-boto3-resiliencehub-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resiliencehub",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_resiliencehub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResilienceHub 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ResilienceHub 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

