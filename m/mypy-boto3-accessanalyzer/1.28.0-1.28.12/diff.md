# Comparing `tmp/mypy-boto3-accessanalyzer-1.28.0.tar.gz` & `tmp/mypy-boto3-accessanalyzer-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.0.tar", last modified: Thu Jul  6 20:58:51 2023, max compression
+gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
```

## Comparing `mypy-boto3-accessanalyzer-1.28.0.tar` & `mypy-boto3-accessanalyzer-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.658206 mypy-boto3-accessanalyzer-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-06 20:58:51.654206 mypy-boto3-accessanalyzer-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.650206 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-06 20:32:26.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12048 2023-07-06 20:32:26.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-07-06 20:32:26.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-06 20:32:26.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-06 20:32:26.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42667 2023-07-06 20:32:28.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42588 2023-07-06 20:32:27.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:51.654206 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:58:51.000000 mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:51.658206 mypy-boto3-accessanalyzer-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:32:25.000000 mypy-boto3-accessanalyzer-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.852594 mypy-boto3-accessanalyzer-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49396 2023-07-27 05:16:52.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49315 2023-07-27 05:16:51.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.852594 mypy-boto3-accessanalyzer-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/setup.py
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/LICENSE` & `mypy-boto3-accessanalyzer-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.0
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,120 +371,143 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
+    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
-    CriterionTypeDef,
+    CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
+    EbsSnapshotConfigurationOutputTypeDef,
+    EcrRepositoryConfigurationOutputTypeDef,
+    EfsFileSystemConfigurationOutputTypeDef,
+    IamRoleConfigurationOutputTypeDef,
+    SecretsManagerSecretConfigurationOutputTypeDef,
+    SnsTopicConfigurationOutputTypeDef,
+    SqsQueueConfigurationOutputTypeDef,
     EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
     GetAnalyzedResourceRequestRequestTypeDef,
     GetAnalyzerRequestRequestTypeDef,
     GetArchiveRuleRequestRequestTypeDef,
     GetFindingRequestRequestTypeDef,
     GetGeneratedPolicyRequestRequestTypeDef,
     JobErrorTypeDef,
+    KmsGrantConstraintsOutputTypeDef,
     KmsGrantConstraintsTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPreviewsRequestRequestTypeDef,
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
+    RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
+    RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
+    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
+    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
-    InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    InlineArchiveRuleTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
+    KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
     ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
+    NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
+    RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
+    RdsDbSnapshotConfigurationOutputTypeDef,
     RdsDbSnapshotConfigurationTypeDef,
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
-    CreateAnalyzerRequestRequestTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
+    KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
+    S3AccessPointConfigurationOutputTypeDef,
     S3AccessPointConfigurationTypeDef,
     LocationTypeDef,
     GeneratedPolicyResultTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListFindingsResponseTypeDef,
     GetFindingResponseTypeDef,
+    S3BucketConfigurationOutputTypeDef,
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
     CreateAccessPreviewRequestRequestTypeDef,
     GetAccessPreviewResponseTypeDef,
 )
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/README.md` & `mypy-boto3-accessanalyzer-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,120 +339,143 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
+    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
-    CriterionTypeDef,
+    CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
+    EbsSnapshotConfigurationOutputTypeDef,
+    EcrRepositoryConfigurationOutputTypeDef,
+    EfsFileSystemConfigurationOutputTypeDef,
+    IamRoleConfigurationOutputTypeDef,
+    SecretsManagerSecretConfigurationOutputTypeDef,
+    SnsTopicConfigurationOutputTypeDef,
+    SqsQueueConfigurationOutputTypeDef,
     EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
     GetAnalyzedResourceRequestRequestTypeDef,
     GetAnalyzerRequestRequestTypeDef,
     GetArchiveRuleRequestRequestTypeDef,
     GetFindingRequestRequestTypeDef,
     GetGeneratedPolicyRequestRequestTypeDef,
     JobErrorTypeDef,
+    KmsGrantConstraintsOutputTypeDef,
     KmsGrantConstraintsTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPreviewsRequestRequestTypeDef,
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
+    RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
+    RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
+    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
+    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
-    InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    InlineArchiveRuleTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
+    KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
     ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
+    NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
+    RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
+    RdsDbSnapshotConfigurationOutputTypeDef,
     RdsDbSnapshotConfigurationTypeDef,
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
-    CreateAnalyzerRequestRequestTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
+    KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
+    S3AccessPointConfigurationOutputTypeDef,
     S3AccessPointConfigurationTypeDef,
     LocationTypeDef,
     GeneratedPolicyResultTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListFindingsResponseTypeDef,
     GetFindingResponseTypeDef,
+    S3BucketConfigurationOutputTypeDef,
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
     CreateAccessPreviewRequestRequestTypeDef,
     GetAccessPreviewResponseTypeDef,
 )
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__init__.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__init__.pyi` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/__main__.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AccessAnalyzer 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.AccessAnalyzer 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
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

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/client.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/client.pyi` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/literals.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
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
@@ -331,26 +332,28 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/literals.pyi` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,15 @@
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
@@ -329,26 +330,28 @@
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

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/paginator.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/paginator.pyi` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/type_defs.py` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,134 +41,166 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessPreviewStatusReasonTypeDef",
+    "AclGranteeOutputTypeDef",
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
-    "CriterionTypeDef",
+    "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
+    "EbsSnapshotConfigurationOutputTypeDef",
+    "EcrRepositoryConfigurationOutputTypeDef",
+    "EfsFileSystemConfigurationOutputTypeDef",
+    "IamRoleConfigurationOutputTypeDef",
+    "SecretsManagerSecretConfigurationOutputTypeDef",
+    "SnsTopicConfigurationOutputTypeDef",
+    "SqsQueueConfigurationOutputTypeDef",
     "EbsSnapshotConfigurationTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
     "SnsTopicConfigurationTypeDef",
     "SqsQueueConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "CriterionTypeDef",
     "DeleteAnalyzerRequestRequestTypeDef",
     "DeleteArchiveRuleRequestRequestTypeDef",
     "FindingSourceDetailTypeDef",
     "GeneratedPolicyTypeDef",
     "GetAccessPreviewRequestRequestTypeDef",
     "GetAnalyzedResourceRequestRequestTypeDef",
     "GetAnalyzerRequestRequestTypeDef",
     "GetArchiveRuleRequestRequestTypeDef",
     "GetFindingRequestRequestTypeDef",
     "GetGeneratedPolicyRequestRequestTypeDef",
     "JobErrorTypeDef",
+    "KmsGrantConstraintsOutputTypeDef",
     "KmsGrantConstraintsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPreviewsRequestRequestTypeDef",
     "ListAnalyzedResourcesRequestRequestTypeDef",
     "ListAnalyzersRequestRequestTypeDef",
     "ListArchiveRulesRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "ListPolicyGenerationsRequestRequestTypeDef",
     "PolicyGenerationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "SubstringTypeDef",
     "PolicyGenerationDetailsTypeDef",
     "PositionTypeDef",
+    "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
     "RdsDbClusterSnapshotAttributeValueTypeDef",
+    "RdsDbSnapshotAttributeValueOutputTypeDef",
     "RdsDbSnapshotAttributeValueTypeDef",
+    "S3PublicAccessBlockConfigurationOutputTypeDef",
     "S3PublicAccessBlockConfigurationTypeDef",
     "StartResourceScanRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "ValidatePolicyRequestRequestTypeDef",
     "AccessPreviewSummaryTypeDef",
+    "S3BucketAclGrantConfigurationOutputTypeDef",
     "S3BucketAclGrantConfigurationTypeDef",
     "AnalyzerSummaryTypeDef",
     "ArchiveRuleSummaryTypeDef",
-    "CreateArchiveRuleRequestRequestTypeDef",
-    "InlineArchiveRuleTypeDef",
-    "ListAccessPreviewFindingsRequestRequestTypeDef",
-    "UpdateArchiveRuleRequestRequestTypeDef",
     "CloudTrailDetailsTypeDef",
     "CloudTrailPropertiesTypeDef",
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAnalyzedResourceResponseTypeDef",
     "ListAnalyzedResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPolicyGenerationResponseTypeDef",
+    "CreateArchiveRuleRequestRequestTypeDef",
+    "InlineArchiveRuleTypeDef",
+    "ListAccessPreviewFindingsRequestRequestTypeDef",
+    "UpdateArchiveRuleRequestRequestTypeDef",
     "FindingSourceTypeDef",
     "JobDetailsTypeDef",
+    "KmsGrantConfigurationOutputTypeDef",
     "KmsGrantConfigurationTypeDef",
     "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     "ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     "ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef",
     "ListAnalyzersRequestListAnalyzersPaginateTypeDef",
     "ListArchiveRulesRequestListArchiveRulesPaginateTypeDef",
     "ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef",
     "ValidatePolicyRequestValidatePolicyPaginateTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "ListPolicyGenerationsResponseTypeDef",
+    "NetworkOriginConfigurationOutputTypeDef",
     "NetworkOriginConfigurationTypeDef",
     "PathElementTypeDef",
     "SpanTypeDef",
+    "RdsDbClusterSnapshotConfigurationOutputTypeDef",
     "RdsDbClusterSnapshotConfigurationTypeDef",
+    "RdsDbSnapshotConfigurationOutputTypeDef",
     "RdsDbSnapshotConfigurationTypeDef",
     "ListAccessPreviewsResponseTypeDef",
     "GetAnalyzerResponseTypeDef",
     "ListAnalyzersResponseTypeDef",
     "GetArchiveRuleResponseTypeDef",
     "ListArchiveRulesResponseTypeDef",
-    "CreateAnalyzerRequestRequestTypeDef",
     "StartPolicyGenerationRequestRequestTypeDef",
     "GeneratedPolicyPropertiesTypeDef",
+    "CreateAnalyzerRequestRequestTypeDef",
     "AccessPreviewFindingTypeDef",
     "FindingSummaryTypeDef",
     "FindingTypeDef",
+    "KmsKeyConfigurationOutputTypeDef",
     "KmsKeyConfigurationTypeDef",
+    "S3AccessPointConfigurationOutputTypeDef",
     "S3AccessPointConfigurationTypeDef",
     "LocationTypeDef",
     "GeneratedPolicyResultTypeDef",
     "ListAccessPreviewFindingsResponseTypeDef",
     "ListFindingsResponseTypeDef",
     "GetFindingResponseTypeDef",
+    "S3BucketConfigurationOutputTypeDef",
     "S3BucketConfigurationTypeDef",
     "ValidatePolicyFindingTypeDef",
     "GetGeneratedPolicyResponseTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ValidatePolicyResponseTypeDef",
     "AccessPreviewTypeDef",
     "CreateAccessPreviewRequestRequestTypeDef",
     "GetAccessPreviewResponseTypeDef",
 )
 
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
 )
 
+AclGranteeOutputTypeDef = TypedDict(
+    "AclGranteeOutputTypeDef",
+    {
+        "id": str,
+        "uri": str,
+    },
+    total=False,
+)
+
 AclGranteeTypeDef = TypedDict(
     "AclGranteeTypeDef",
     {
         "id": str,
         "uri": str,
     },
     total=False,
@@ -236,20 +268,20 @@
 
 class ApplyArchiveRuleRequestRequestTypeDef(
     _RequiredApplyArchiveRuleRequestRequestTypeDef, _OptionalApplyArchiveRuleRequestRequestTypeDef
 ):
     pass
 
 
-CriterionTypeDef = TypedDict(
-    "CriterionTypeDef",
+CriterionOutputTypeDef = TypedDict(
+    "CriterionOutputTypeDef",
     {
-        "eq": Sequence[str],
-        "neq": Sequence[str],
-        "contains": Sequence[str],
+        "eq": List[str],
+        "neq": List[str],
+        "contains": List[str],
         "exists": bool,
     },
     total=False,
 )
 
 CancelPolicyGenerationRequestRequestTypeDef = TypedDict(
     "CancelPolicyGenerationRequestRequestTypeDef",
@@ -294,14 +326,73 @@
 )
 
 
 class TrailPropertiesTypeDef(_RequiredTrailPropertiesTypeDef, _OptionalTrailPropertiesTypeDef):
     pass
 
 
+EbsSnapshotConfigurationOutputTypeDef = TypedDict(
+    "EbsSnapshotConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "groups": List[str],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+EcrRepositoryConfigurationOutputTypeDef = TypedDict(
+    "EcrRepositoryConfigurationOutputTypeDef",
+    {
+        "repositoryPolicy": str,
+    },
+    total=False,
+)
+
+EfsFileSystemConfigurationOutputTypeDef = TypedDict(
+    "EfsFileSystemConfigurationOutputTypeDef",
+    {
+        "fileSystemPolicy": str,
+    },
+    total=False,
+)
+
+IamRoleConfigurationOutputTypeDef = TypedDict(
+    "IamRoleConfigurationOutputTypeDef",
+    {
+        "trustPolicy": str,
+    },
+    total=False,
+)
+
+SecretsManagerSecretConfigurationOutputTypeDef = TypedDict(
+    "SecretsManagerSecretConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+        "secretPolicy": str,
+    },
+    total=False,
+)
+
+SnsTopicConfigurationOutputTypeDef = TypedDict(
+    "SnsTopicConfigurationOutputTypeDef",
+    {
+        "topicPolicy": str,
+    },
+    total=False,
+)
+
+SqsQueueConfigurationOutputTypeDef = TypedDict(
+    "SqsQueueConfigurationOutputTypeDef",
+    {
+        "queuePolicy": str,
+    },
+    total=False,
+)
+
 EbsSnapshotConfigurationTypeDef = TypedDict(
     "EbsSnapshotConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "groups": Sequence[str],
         "kmsKeyId": str,
     },
@@ -364,14 +455,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+CriterionTypeDef = TypedDict(
+    "CriterionTypeDef",
+    {
+        "eq": Sequence[str],
+        "neq": Sequence[str],
+        "contains": Sequence[str],
+        "exists": bool,
+    },
+    total=False,
+)
+
 _RequiredDeleteAnalyzerRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnalyzerRequestRequestTypeDef",
     {
         "analyzerName": str,
     },
 )
 _OptionalDeleteAnalyzerRequestRequestTypeDef = TypedDict(
@@ -493,14 +595,23 @@
     "JobErrorTypeDef",
     {
         "code": JobErrorCodeType,
         "message": str,
     },
 )
 
+KmsGrantConstraintsOutputTypeDef = TypedDict(
+    "KmsGrantConstraintsOutputTypeDef",
+    {
+        "encryptionContextEquals": Dict[str, str],
+        "encryptionContextSubset": Dict[str, str],
+    },
+    total=False,
+)
+
 KmsGrantConstraintsTypeDef = TypedDict(
     "KmsGrantConstraintsTypeDef",
     {
         "encryptionContextEquals": Mapping[str, str],
         "encryptionContextSubset": Mapping[str, str],
     },
     total=False,
@@ -639,14 +750,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "vpcId": str,
     },
 )
 
@@ -670,30 +788,54 @@
     {
         "line": int,
         "column": int,
         "offset": int,
     },
 )
 
+RdsDbClusterSnapshotAttributeValueOutputTypeDef = TypedDict(
+    "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
+    {
+        "accountIds": List[str],
+    },
+    total=False,
+)
+
 RdsDbClusterSnapshotAttributeValueTypeDef = TypedDict(
     "RdsDbClusterSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+RdsDbSnapshotAttributeValueOutputTypeDef = TypedDict(
+    "RdsDbSnapshotAttributeValueOutputTypeDef",
+    {
+        "accountIds": List[str],
+    },
+    total=False,
+)
+
 RdsDbSnapshotAttributeValueTypeDef = TypedDict(
     "RdsDbSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+S3PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "S3PublicAccessBlockConfigurationOutputTypeDef",
+    {
+        "ignorePublicAcls": bool,
+        "restrictPublicBuckets": bool,
+    },
+)
+
 S3PublicAccessBlockConfigurationTypeDef = TypedDict(
     "S3PublicAccessBlockConfigurationTypeDef",
     {
         "ignorePublicAcls": bool,
         "restrictPublicBuckets": bool,
     },
 )
@@ -805,14 +947,22 @@
 
 class AccessPreviewSummaryTypeDef(
     _RequiredAccessPreviewSummaryTypeDef, _OptionalAccessPreviewSummaryTypeDef
 ):
     pass
 
 
+S3BucketAclGrantConfigurationOutputTypeDef = TypedDict(
+    "S3BucketAclGrantConfigurationOutputTypeDef",
+    {
+        "permission": AclPermissionType,
+        "grantee": AclGranteeOutputTypeDef,
+    },
+)
+
 S3BucketAclGrantConfigurationTypeDef = TypedDict(
     "S3BucketAclGrantConfigurationTypeDef",
     {
         "permission": AclPermissionType,
         "grantee": AclGranteeTypeDef,
     },
 )
@@ -843,99 +993,20 @@
     pass
 
 
 ArchiveRuleSummaryTypeDef = TypedDict(
     "ArchiveRuleSummaryTypeDef",
     {
         "ruleName": str,
-        "filter": Dict[str, CriterionTypeDef],
+        "filter": Dict[str, CriterionOutputTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 
-_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateArchiveRuleRequestRequestTypeDef(
-    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
-
-InlineArchiveRuleTypeDef = TypedDict(
-    "InlineArchiveRuleTypeDef",
-    {
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-
-_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, CriterionTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListAccessPreviewFindingsRequestRequestTypeDef(
-    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
-    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class UpdateArchiveRuleRequestRequestTypeDef(
-    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCloudTrailDetailsTypeDef = TypedDict(
     "_RequiredCloudTrailDetailsTypeDef",
     {
         "trails": Sequence[TrailTypeDef],
         "accessRole": str,
         "startTime": Union[datetime, str],
     },
@@ -1016,14 +1087,93 @@
     "StartPolicyGenerationResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateArchiveRuleRequestRequestTypeDef(
+    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+
+InlineArchiveRuleTypeDef = TypedDict(
+    "InlineArchiveRuleTypeDef",
+    {
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+
+_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+
+class ListAccessPreviewFindingsRequestRequestTypeDef(
+    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
+    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateArchiveRuleRequestRequestTypeDef(
+    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredFindingSourceTypeDef = TypedDict(
     "_RequiredFindingSourceTypeDef",
     {
         "type": FindingSourceTypeType,
     },
 )
 _OptionalFindingSourceTypeDef = TypedDict(
@@ -1057,14 +1207,38 @@
 )
 
 
 class JobDetailsTypeDef(_RequiredJobDetailsTypeDef, _OptionalJobDetailsTypeDef):
     pass
 
 
+_RequiredKmsGrantConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKmsGrantConfigurationOutputTypeDef",
+    {
+        "operations": List[KmsGrantOperationType],
+        "granteePrincipal": str,
+        "issuingAccount": str,
+    },
+)
+_OptionalKmsGrantConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKmsGrantConfigurationOutputTypeDef",
+    {
+        "retiringPrincipal": str,
+        "constraints": KmsGrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class KmsGrantConfigurationOutputTypeDef(
+    _RequiredKmsGrantConfigurationOutputTypeDef, _OptionalKmsGrantConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredKmsGrantConfigurationTypeDef = TypedDict(
     "_RequiredKmsGrantConfigurationTypeDef",
     {
         "operations": Sequence[KmsGrantOperationType],
         "granteePrincipal": str,
         "issuingAccount": str,
     },
@@ -1272,14 +1446,23 @@
     {
         "policyGenerations": List[PolicyGenerationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkOriginConfigurationOutputTypeDef = TypedDict(
+    "NetworkOriginConfigurationOutputTypeDef",
+    {
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "internetConfiguration": Dict[str, Any],
+    },
+    total=False,
+)
+
 NetworkOriginConfigurationTypeDef = TypedDict(
     "NetworkOriginConfigurationTypeDef",
     {
         "vpcConfiguration": VpcConfigurationTypeDef,
         "internetConfiguration": Mapping[str, Any],
     },
     total=False,
@@ -1300,23 +1483,41 @@
     "SpanTypeDef",
     {
         "start": PositionTypeDef,
         "end": PositionTypeDef,
     },
 )
 
+RdsDbClusterSnapshotConfigurationOutputTypeDef = TypedDict(
+    "RdsDbClusterSnapshotConfigurationOutputTypeDef",
+    {
+        "attributes": Dict[str, RdsDbClusterSnapshotAttributeValueOutputTypeDef],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 RdsDbClusterSnapshotConfigurationTypeDef = TypedDict(
     "RdsDbClusterSnapshotConfigurationTypeDef",
     {
         "attributes": Mapping[str, RdsDbClusterSnapshotAttributeValueTypeDef],
         "kmsKeyId": str,
     },
     total=False,
 )
 
+RdsDbSnapshotConfigurationOutputTypeDef = TypedDict(
+    "RdsDbSnapshotConfigurationOutputTypeDef",
+    {
+        "attributes": Dict[str, RdsDbSnapshotAttributeValueOutputTypeDef],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 RdsDbSnapshotConfigurationTypeDef = TypedDict(
     "RdsDbSnapshotConfigurationTypeDef",
     {
         "attributes": Mapping[str, RdsDbSnapshotAttributeValueTypeDef],
         "kmsKeyId": str,
     },
     total=False,
@@ -1361,38 +1562,14 @@
     {
         "archiveRules": List[ArchiveRuleSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnalyzerRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "type": TypeType,
-    },
-)
-_OptionalCreateAnalyzerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnalyzerRequestRequestTypeDef",
-    {
-        "archiveRules": Sequence[InlineArchiveRuleTypeDef],
-        "tags": Mapping[str, str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateAnalyzerRequestRequestTypeDef(
-    _RequiredCreateAnalyzerRequestRequestTypeDef, _OptionalCreateAnalyzerRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredStartPolicyGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartPolicyGenerationRequestRequestTypeDef",
     {
         "policyGenerationDetails": PolicyGenerationDetailsTypeDef,
     },
 )
 _OptionalStartPolicyGenerationRequestRequestTypeDef = TypedDict(
@@ -1430,14 +1607,38 @@
 
 class GeneratedPolicyPropertiesTypeDef(
     _RequiredGeneratedPolicyPropertiesTypeDef, _OptionalGeneratedPolicyPropertiesTypeDef
 ):
     pass
 
 
+_RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnalyzerRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "type": TypeType,
+    },
+)
+_OptionalCreateAnalyzerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnalyzerRequestRequestTypeDef",
+    {
+        "archiveRules": Sequence[InlineArchiveRuleTypeDef],
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateAnalyzerRequestRequestTypeDef(
+    _RequiredCreateAnalyzerRequestRequestTypeDef, _OptionalCreateAnalyzerRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredAccessPreviewFindingTypeDef = TypedDict(
     "_RequiredAccessPreviewFindingTypeDef",
     {
         "id": str,
         "resourceType": ResourceTypeType,
         "createdAt": datetime,
         "changeType": FindingChangeTypeType,
@@ -1526,23 +1727,42 @@
 )
 
 
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
 
+KmsKeyConfigurationOutputTypeDef = TypedDict(
+    "KmsKeyConfigurationOutputTypeDef",
+    {
+        "keyPolicies": Dict[str, str],
+        "grants": List[KmsGrantConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 KmsKeyConfigurationTypeDef = TypedDict(
     "KmsKeyConfigurationTypeDef",
     {
         "keyPolicies": Mapping[str, str],
         "grants": Sequence[KmsGrantConfigurationTypeDef],
     },
     total=False,
 )
 
+S3AccessPointConfigurationOutputTypeDef = TypedDict(
+    "S3AccessPointConfigurationOutputTypeDef",
+    {
+        "accessPointPolicy": str,
+        "publicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "networkOrigin": NetworkOriginConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 S3AccessPointConfigurationTypeDef = TypedDict(
     "S3AccessPointConfigurationTypeDef",
     {
         "accessPointPolicy": str,
         "publicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "networkOrigin": NetworkOriginConfigurationTypeDef,
     },
@@ -1600,14 +1820,25 @@
     "GetFindingResponseTypeDef",
     {
         "finding": FindingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+S3BucketConfigurationOutputTypeDef = TypedDict(
+    "S3BucketConfigurationOutputTypeDef",
+    {
+        "bucketPolicy": str,
+        "bucketAclGrants": List[S3BucketAclGrantConfigurationOutputTypeDef],
+        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "accessPoints": Dict[str, S3AccessPointConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
     {
         "bucketPolicy": str,
         "bucketAclGrants": Sequence[S3BucketAclGrantConfigurationTypeDef],
         "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "accessPoints": Mapping[str, S3AccessPointConfigurationTypeDef],
@@ -1631,14 +1862,32 @@
     {
         "jobDetails": JobDetailsTypeDef,
         "generatedPolicyResult": GeneratedPolicyResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "ebsSnapshot": EbsSnapshotConfigurationOutputTypeDef,
+        "ecrRepository": EcrRepositoryConfigurationOutputTypeDef,
+        "iamRole": IamRoleConfigurationOutputTypeDef,
+        "efsFileSystem": EfsFileSystemConfigurationOutputTypeDef,
+        "kmsKey": KmsKeyConfigurationOutputTypeDef,
+        "rdsDbClusterSnapshot": RdsDbClusterSnapshotConfigurationOutputTypeDef,
+        "rdsDbSnapshot": RdsDbSnapshotConfigurationOutputTypeDef,
+        "secretsManagerSecret": SecretsManagerSecretConfigurationOutputTypeDef,
+        "s3Bucket": S3BucketConfigurationOutputTypeDef,
+        "snsTopic": SnsTopicConfigurationOutputTypeDef,
+        "sqsQueue": SqsQueueConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "ebsSnapshot": EbsSnapshotConfigurationTypeDef,
         "ecrRepository": EcrRepositoryConfigurationTypeDef,
         "iamRole": IamRoleConfigurationTypeDef,
         "efsFileSystem": EfsFileSystemConfigurationTypeDef,
@@ -1663,15 +1912,15 @@
 )
 
 _RequiredAccessPreviewTypeDef = TypedDict(
     "_RequiredAccessPreviewTypeDef",
     {
         "id": str,
         "analyzerArn": str,
-        "configurations": Dict[str, ConfigurationTypeDef],
+        "configurations": Dict[str, ConfigurationOutputTypeDef],
         "createdAt": datetime,
         "status": AccessPreviewStatusType,
     },
 )
 _OptionalAccessPreviewTypeDef = TypedDict(
     "_OptionalAccessPreviewTypeDef",
     {
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer/type_defs.pyi` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -40,134 +40,166 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessPreviewStatusReasonTypeDef",
+    "AclGranteeOutputTypeDef",
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
-    "CriterionTypeDef",
+    "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
+    "EbsSnapshotConfigurationOutputTypeDef",
+    "EcrRepositoryConfigurationOutputTypeDef",
+    "EfsFileSystemConfigurationOutputTypeDef",
+    "IamRoleConfigurationOutputTypeDef",
+    "SecretsManagerSecretConfigurationOutputTypeDef",
+    "SnsTopicConfigurationOutputTypeDef",
+    "SqsQueueConfigurationOutputTypeDef",
     "EbsSnapshotConfigurationTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
     "SnsTopicConfigurationTypeDef",
     "SqsQueueConfigurationTypeDef",
     "ResponseMetadataTypeDef",
+    "CriterionTypeDef",
     "DeleteAnalyzerRequestRequestTypeDef",
     "DeleteArchiveRuleRequestRequestTypeDef",
     "FindingSourceDetailTypeDef",
     "GeneratedPolicyTypeDef",
     "GetAccessPreviewRequestRequestTypeDef",
     "GetAnalyzedResourceRequestRequestTypeDef",
     "GetAnalyzerRequestRequestTypeDef",
     "GetArchiveRuleRequestRequestTypeDef",
     "GetFindingRequestRequestTypeDef",
     "GetGeneratedPolicyRequestRequestTypeDef",
     "JobErrorTypeDef",
+    "KmsGrantConstraintsOutputTypeDef",
     "KmsGrantConstraintsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccessPreviewsRequestRequestTypeDef",
     "ListAnalyzedResourcesRequestRequestTypeDef",
     "ListAnalyzersRequestRequestTypeDef",
     "ListArchiveRulesRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "ListPolicyGenerationsRequestRequestTypeDef",
     "PolicyGenerationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "SubstringTypeDef",
     "PolicyGenerationDetailsTypeDef",
     "PositionTypeDef",
+    "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
     "RdsDbClusterSnapshotAttributeValueTypeDef",
+    "RdsDbSnapshotAttributeValueOutputTypeDef",
     "RdsDbSnapshotAttributeValueTypeDef",
+    "S3PublicAccessBlockConfigurationOutputTypeDef",
     "S3PublicAccessBlockConfigurationTypeDef",
     "StartResourceScanRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "ValidatePolicyRequestRequestTypeDef",
     "AccessPreviewSummaryTypeDef",
+    "S3BucketAclGrantConfigurationOutputTypeDef",
     "S3BucketAclGrantConfigurationTypeDef",
     "AnalyzerSummaryTypeDef",
     "ArchiveRuleSummaryTypeDef",
-    "CreateArchiveRuleRequestRequestTypeDef",
-    "InlineArchiveRuleTypeDef",
-    "ListAccessPreviewFindingsRequestRequestTypeDef",
-    "UpdateArchiveRuleRequestRequestTypeDef",
     "CloudTrailDetailsTypeDef",
     "CloudTrailPropertiesTypeDef",
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetAnalyzedResourceResponseTypeDef",
     "ListAnalyzedResourcesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartPolicyGenerationResponseTypeDef",
+    "CreateArchiveRuleRequestRequestTypeDef",
+    "InlineArchiveRuleTypeDef",
+    "ListAccessPreviewFindingsRequestRequestTypeDef",
+    "UpdateArchiveRuleRequestRequestTypeDef",
     "FindingSourceTypeDef",
     "JobDetailsTypeDef",
+    "KmsGrantConfigurationOutputTypeDef",
     "KmsGrantConfigurationTypeDef",
     "ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef",
     "ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef",
     "ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef",
     "ListAnalyzersRequestListAnalyzersPaginateTypeDef",
     "ListArchiveRulesRequestListArchiveRulesPaginateTypeDef",
     "ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef",
     "ValidatePolicyRequestValidatePolicyPaginateTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "ListPolicyGenerationsResponseTypeDef",
+    "NetworkOriginConfigurationOutputTypeDef",
     "NetworkOriginConfigurationTypeDef",
     "PathElementTypeDef",
     "SpanTypeDef",
+    "RdsDbClusterSnapshotConfigurationOutputTypeDef",
     "RdsDbClusterSnapshotConfigurationTypeDef",
+    "RdsDbSnapshotConfigurationOutputTypeDef",
     "RdsDbSnapshotConfigurationTypeDef",
     "ListAccessPreviewsResponseTypeDef",
     "GetAnalyzerResponseTypeDef",
     "ListAnalyzersResponseTypeDef",
     "GetArchiveRuleResponseTypeDef",
     "ListArchiveRulesResponseTypeDef",
-    "CreateAnalyzerRequestRequestTypeDef",
     "StartPolicyGenerationRequestRequestTypeDef",
     "GeneratedPolicyPropertiesTypeDef",
+    "CreateAnalyzerRequestRequestTypeDef",
     "AccessPreviewFindingTypeDef",
     "FindingSummaryTypeDef",
     "FindingTypeDef",
+    "KmsKeyConfigurationOutputTypeDef",
     "KmsKeyConfigurationTypeDef",
+    "S3AccessPointConfigurationOutputTypeDef",
     "S3AccessPointConfigurationTypeDef",
     "LocationTypeDef",
     "GeneratedPolicyResultTypeDef",
     "ListAccessPreviewFindingsResponseTypeDef",
     "ListFindingsResponseTypeDef",
     "GetFindingResponseTypeDef",
+    "S3BucketConfigurationOutputTypeDef",
     "S3BucketConfigurationTypeDef",
     "ValidatePolicyFindingTypeDef",
     "GetGeneratedPolicyResponseTypeDef",
+    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ValidatePolicyResponseTypeDef",
     "AccessPreviewTypeDef",
     "CreateAccessPreviewRequestRequestTypeDef",
     "GetAccessPreviewResponseTypeDef",
 )
 
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
 )
 
+AclGranteeOutputTypeDef = TypedDict(
+    "AclGranteeOutputTypeDef",
+    {
+        "id": str,
+        "uri": str,
+    },
+    total=False,
+)
+
 AclGranteeTypeDef = TypedDict(
     "AclGranteeTypeDef",
     {
         "id": str,
         "uri": str,
     },
     total=False,
@@ -231,20 +263,20 @@
 )
 
 class ApplyArchiveRuleRequestRequestTypeDef(
     _RequiredApplyArchiveRuleRequestRequestTypeDef, _OptionalApplyArchiveRuleRequestRequestTypeDef
 ):
     pass
 
-CriterionTypeDef = TypedDict(
-    "CriterionTypeDef",
+CriterionOutputTypeDef = TypedDict(
+    "CriterionOutputTypeDef",
     {
-        "eq": Sequence[str],
-        "neq": Sequence[str],
-        "contains": Sequence[str],
+        "eq": List[str],
+        "neq": List[str],
+        "contains": List[str],
         "exists": bool,
     },
     total=False,
 )
 
 CancelPolicyGenerationRequestRequestTypeDef = TypedDict(
     "CancelPolicyGenerationRequestRequestTypeDef",
@@ -285,14 +317,73 @@
     },
     total=False,
 )
 
 class TrailPropertiesTypeDef(_RequiredTrailPropertiesTypeDef, _OptionalTrailPropertiesTypeDef):
     pass
 
+EbsSnapshotConfigurationOutputTypeDef = TypedDict(
+    "EbsSnapshotConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "groups": List[str],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
+EcrRepositoryConfigurationOutputTypeDef = TypedDict(
+    "EcrRepositoryConfigurationOutputTypeDef",
+    {
+        "repositoryPolicy": str,
+    },
+    total=False,
+)
+
+EfsFileSystemConfigurationOutputTypeDef = TypedDict(
+    "EfsFileSystemConfigurationOutputTypeDef",
+    {
+        "fileSystemPolicy": str,
+    },
+    total=False,
+)
+
+IamRoleConfigurationOutputTypeDef = TypedDict(
+    "IamRoleConfigurationOutputTypeDef",
+    {
+        "trustPolicy": str,
+    },
+    total=False,
+)
+
+SecretsManagerSecretConfigurationOutputTypeDef = TypedDict(
+    "SecretsManagerSecretConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+        "secretPolicy": str,
+    },
+    total=False,
+)
+
+SnsTopicConfigurationOutputTypeDef = TypedDict(
+    "SnsTopicConfigurationOutputTypeDef",
+    {
+        "topicPolicy": str,
+    },
+    total=False,
+)
+
+SqsQueueConfigurationOutputTypeDef = TypedDict(
+    "SqsQueueConfigurationOutputTypeDef",
+    {
+        "queuePolicy": str,
+    },
+    total=False,
+)
+
 EbsSnapshotConfigurationTypeDef = TypedDict(
     "EbsSnapshotConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "groups": Sequence[str],
         "kmsKeyId": str,
     },
@@ -355,14 +446,25 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+CriterionTypeDef = TypedDict(
+    "CriterionTypeDef",
+    {
+        "eq": Sequence[str],
+        "neq": Sequence[str],
+        "contains": Sequence[str],
+        "exists": bool,
+    },
+    total=False,
+)
+
 _RequiredDeleteAnalyzerRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteAnalyzerRequestRequestTypeDef",
     {
         "analyzerName": str,
     },
 )
 _OptionalDeleteAnalyzerRequestRequestTypeDef = TypedDict(
@@ -478,14 +580,23 @@
     "JobErrorTypeDef",
     {
         "code": JobErrorCodeType,
         "message": str,
     },
 )
 
+KmsGrantConstraintsOutputTypeDef = TypedDict(
+    "KmsGrantConstraintsOutputTypeDef",
+    {
+        "encryptionContextEquals": Dict[str, str],
+        "encryptionContextSubset": Dict[str, str],
+    },
+    total=False,
+)
+
 KmsGrantConstraintsTypeDef = TypedDict(
     "KmsGrantConstraintsTypeDef",
     {
         "encryptionContextEquals": Mapping[str, str],
         "encryptionContextSubset": Mapping[str, str],
     },
     total=False,
@@ -616,14 +727,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
+    {
+        "vpcId": str,
+    },
+)
+
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "vpcId": str,
     },
 )
 
@@ -647,30 +765,54 @@
     {
         "line": int,
         "column": int,
         "offset": int,
     },
 )
 
+RdsDbClusterSnapshotAttributeValueOutputTypeDef = TypedDict(
+    "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
+    {
+        "accountIds": List[str],
+    },
+    total=False,
+)
+
 RdsDbClusterSnapshotAttributeValueTypeDef = TypedDict(
     "RdsDbClusterSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+RdsDbSnapshotAttributeValueOutputTypeDef = TypedDict(
+    "RdsDbSnapshotAttributeValueOutputTypeDef",
+    {
+        "accountIds": List[str],
+    },
+    total=False,
+)
+
 RdsDbSnapshotAttributeValueTypeDef = TypedDict(
     "RdsDbSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
+S3PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "S3PublicAccessBlockConfigurationOutputTypeDef",
+    {
+        "ignorePublicAcls": bool,
+        "restrictPublicBuckets": bool,
+    },
+)
+
 S3PublicAccessBlockConfigurationTypeDef = TypedDict(
     "S3PublicAccessBlockConfigurationTypeDef",
     {
         "ignorePublicAcls": bool,
         "restrictPublicBuckets": bool,
     },
 )
@@ -774,14 +916,22 @@
 )
 
 class AccessPreviewSummaryTypeDef(
     _RequiredAccessPreviewSummaryTypeDef, _OptionalAccessPreviewSummaryTypeDef
 ):
     pass
 
+S3BucketAclGrantConfigurationOutputTypeDef = TypedDict(
+    "S3BucketAclGrantConfigurationOutputTypeDef",
+    {
+        "permission": AclPermissionType,
+        "grantee": AclGranteeOutputTypeDef,
+    },
+)
+
 S3BucketAclGrantConfigurationTypeDef = TypedDict(
     "S3BucketAclGrantConfigurationTypeDef",
     {
         "permission": AclPermissionType,
         "grantee": AclGranteeTypeDef,
     },
 )
@@ -810,93 +960,20 @@
 class AnalyzerSummaryTypeDef(_RequiredAnalyzerSummaryTypeDef, _OptionalAnalyzerSummaryTypeDef):
     pass
 
 ArchiveRuleSummaryTypeDef = TypedDict(
     "ArchiveRuleSummaryTypeDef",
     {
         "ruleName": str,
-        "filter": Dict[str, CriterionTypeDef],
+        "filter": Dict[str, CriterionOutputTypeDef],
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 
-_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateArchiveRuleRequestRequestTypeDef(
-    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
-InlineArchiveRuleTypeDef = TypedDict(
-    "InlineArchiveRuleTypeDef",
-    {
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-
-_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "accessPreviewId": str,
-        "analyzerArn": str,
-    },
-)
-_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
-    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
-    {
-        "filter": Mapping[str, CriterionTypeDef],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListAccessPreviewFindingsRequestRequestTypeDef(
-    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
-    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "ruleName": str,
-        "filter": Mapping[str, CriterionTypeDef],
-    },
-)
-_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class UpdateArchiveRuleRequestRequestTypeDef(
-    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
-):
-    pass
-
 _RequiredCloudTrailDetailsTypeDef = TypedDict(
     "_RequiredCloudTrailDetailsTypeDef",
     {
         "trails": Sequence[TrailTypeDef],
         "accessRole": str,
         "startTime": Union[datetime, str],
     },
@@ -975,14 +1052,87 @@
     "StartPolicyGenerationResponseTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+_OptionalCreateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateArchiveRuleRequestRequestTypeDef(
+    _RequiredCreateArchiveRuleRequestRequestTypeDef, _OptionalCreateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
+InlineArchiveRuleTypeDef = TypedDict(
+    "InlineArchiveRuleTypeDef",
+    {
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+
+_RequiredListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_RequiredListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "accessPreviewId": str,
+        "analyzerArn": str,
+    },
+)
+_OptionalListAccessPreviewFindingsRequestRequestTypeDef = TypedDict(
+    "_OptionalListAccessPreviewFindingsRequestRequestTypeDef",
+    {
+        "filter": Mapping[str, CriterionTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+class ListAccessPreviewFindingsRequestRequestTypeDef(
+    _RequiredListAccessPreviewFindingsRequestRequestTypeDef,
+    _OptionalListAccessPreviewFindingsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "ruleName": str,
+        "filter": Mapping[str, CriterionTypeDef],
+    },
+)
+_OptionalUpdateArchiveRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateArchiveRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateArchiveRuleRequestRequestTypeDef(
+    _RequiredUpdateArchiveRuleRequestRequestTypeDef, _OptionalUpdateArchiveRuleRequestRequestTypeDef
+):
+    pass
+
 _RequiredFindingSourceTypeDef = TypedDict(
     "_RequiredFindingSourceTypeDef",
     {
         "type": FindingSourceTypeType,
     },
 )
 _OptionalFindingSourceTypeDef = TypedDict(
@@ -1012,14 +1162,36 @@
     },
     total=False,
 )
 
 class JobDetailsTypeDef(_RequiredJobDetailsTypeDef, _OptionalJobDetailsTypeDef):
     pass
 
+_RequiredKmsGrantConfigurationOutputTypeDef = TypedDict(
+    "_RequiredKmsGrantConfigurationOutputTypeDef",
+    {
+        "operations": List[KmsGrantOperationType],
+        "granteePrincipal": str,
+        "issuingAccount": str,
+    },
+)
+_OptionalKmsGrantConfigurationOutputTypeDef = TypedDict(
+    "_OptionalKmsGrantConfigurationOutputTypeDef",
+    {
+        "retiringPrincipal": str,
+        "constraints": KmsGrantConstraintsOutputTypeDef,
+    },
+    total=False,
+)
+
+class KmsGrantConfigurationOutputTypeDef(
+    _RequiredKmsGrantConfigurationOutputTypeDef, _OptionalKmsGrantConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredKmsGrantConfigurationTypeDef = TypedDict(
     "_RequiredKmsGrantConfigurationTypeDef",
     {
         "operations": Sequence[KmsGrantOperationType],
         "granteePrincipal": str,
         "issuingAccount": str,
     },
@@ -1211,14 +1383,23 @@
     {
         "policyGenerations": List[PolicyGenerationTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkOriginConfigurationOutputTypeDef = TypedDict(
+    "NetworkOriginConfigurationOutputTypeDef",
+    {
+        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "internetConfiguration": Dict[str, Any],
+    },
+    total=False,
+)
+
 NetworkOriginConfigurationTypeDef = TypedDict(
     "NetworkOriginConfigurationTypeDef",
     {
         "vpcConfiguration": VpcConfigurationTypeDef,
         "internetConfiguration": Mapping[str, Any],
     },
     total=False,
@@ -1239,23 +1420,41 @@
     "SpanTypeDef",
     {
         "start": PositionTypeDef,
         "end": PositionTypeDef,
     },
 )
 
+RdsDbClusterSnapshotConfigurationOutputTypeDef = TypedDict(
+    "RdsDbClusterSnapshotConfigurationOutputTypeDef",
+    {
+        "attributes": Dict[str, RdsDbClusterSnapshotAttributeValueOutputTypeDef],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 RdsDbClusterSnapshotConfigurationTypeDef = TypedDict(
     "RdsDbClusterSnapshotConfigurationTypeDef",
     {
         "attributes": Mapping[str, RdsDbClusterSnapshotAttributeValueTypeDef],
         "kmsKeyId": str,
     },
     total=False,
 )
 
+RdsDbSnapshotConfigurationOutputTypeDef = TypedDict(
+    "RdsDbSnapshotConfigurationOutputTypeDef",
+    {
+        "attributes": Dict[str, RdsDbSnapshotAttributeValueOutputTypeDef],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 RdsDbSnapshotConfigurationTypeDef = TypedDict(
     "RdsDbSnapshotConfigurationTypeDef",
     {
         "attributes": Mapping[str, RdsDbSnapshotAttributeValueTypeDef],
         "kmsKeyId": str,
     },
     total=False,
@@ -1300,36 +1499,14 @@
     {
         "archiveRules": List[ArchiveRuleSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnalyzerRequestRequestTypeDef",
-    {
-        "analyzerName": str,
-        "type": TypeType,
-    },
-)
-_OptionalCreateAnalyzerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnalyzerRequestRequestTypeDef",
-    {
-        "archiveRules": Sequence[InlineArchiveRuleTypeDef],
-        "tags": Mapping[str, str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateAnalyzerRequestRequestTypeDef(
-    _RequiredCreateAnalyzerRequestRequestTypeDef, _OptionalCreateAnalyzerRequestRequestTypeDef
-):
-    pass
-
 _RequiredStartPolicyGenerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartPolicyGenerationRequestRequestTypeDef",
     {
         "policyGenerationDetails": PolicyGenerationDetailsTypeDef,
     },
 )
 _OptionalStartPolicyGenerationRequestRequestTypeDef = TypedDict(
@@ -1363,14 +1540,36 @@
 )
 
 class GeneratedPolicyPropertiesTypeDef(
     _RequiredGeneratedPolicyPropertiesTypeDef, _OptionalGeneratedPolicyPropertiesTypeDef
 ):
     pass
 
+_RequiredCreateAnalyzerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnalyzerRequestRequestTypeDef",
+    {
+        "analyzerName": str,
+        "type": TypeType,
+    },
+)
+_OptionalCreateAnalyzerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnalyzerRequestRequestTypeDef",
+    {
+        "archiveRules": Sequence[InlineArchiveRuleTypeDef],
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateAnalyzerRequestRequestTypeDef(
+    _RequiredCreateAnalyzerRequestRequestTypeDef, _OptionalCreateAnalyzerRequestRequestTypeDef
+):
+    pass
+
 _RequiredAccessPreviewFindingTypeDef = TypedDict(
     "_RequiredAccessPreviewFindingTypeDef",
     {
         "id": str,
         "resourceType": ResourceTypeType,
         "createdAt": datetime,
         "changeType": FindingChangeTypeType,
@@ -1453,23 +1652,42 @@
     },
     total=False,
 )
 
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
+KmsKeyConfigurationOutputTypeDef = TypedDict(
+    "KmsKeyConfigurationOutputTypeDef",
+    {
+        "keyPolicies": Dict[str, str],
+        "grants": List[KmsGrantConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 KmsKeyConfigurationTypeDef = TypedDict(
     "KmsKeyConfigurationTypeDef",
     {
         "keyPolicies": Mapping[str, str],
         "grants": Sequence[KmsGrantConfigurationTypeDef],
     },
     total=False,
 )
 
+S3AccessPointConfigurationOutputTypeDef = TypedDict(
+    "S3AccessPointConfigurationOutputTypeDef",
+    {
+        "accessPointPolicy": str,
+        "publicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "networkOrigin": NetworkOriginConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 S3AccessPointConfigurationTypeDef = TypedDict(
     "S3AccessPointConfigurationTypeDef",
     {
         "accessPointPolicy": str,
         "publicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "networkOrigin": NetworkOriginConfigurationTypeDef,
     },
@@ -1525,14 +1743,25 @@
     "GetFindingResponseTypeDef",
     {
         "finding": FindingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+S3BucketConfigurationOutputTypeDef = TypedDict(
+    "S3BucketConfigurationOutputTypeDef",
+    {
+        "bucketPolicy": str,
+        "bucketAclGrants": List[S3BucketAclGrantConfigurationOutputTypeDef],
+        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "accessPoints": Dict[str, S3AccessPointConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
     {
         "bucketPolicy": str,
         "bucketAclGrants": Sequence[S3BucketAclGrantConfigurationTypeDef],
         "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "accessPoints": Mapping[str, S3AccessPointConfigurationTypeDef],
@@ -1556,14 +1785,32 @@
     {
         "jobDetails": JobDetailsTypeDef,
         "generatedPolicyResult": GeneratedPolicyResultTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationOutputTypeDef = TypedDict(
+    "ConfigurationOutputTypeDef",
+    {
+        "ebsSnapshot": EbsSnapshotConfigurationOutputTypeDef,
+        "ecrRepository": EcrRepositoryConfigurationOutputTypeDef,
+        "iamRole": IamRoleConfigurationOutputTypeDef,
+        "efsFileSystem": EfsFileSystemConfigurationOutputTypeDef,
+        "kmsKey": KmsKeyConfigurationOutputTypeDef,
+        "rdsDbClusterSnapshot": RdsDbClusterSnapshotConfigurationOutputTypeDef,
+        "rdsDbSnapshot": RdsDbSnapshotConfigurationOutputTypeDef,
+        "secretsManagerSecret": SecretsManagerSecretConfigurationOutputTypeDef,
+        "s3Bucket": S3BucketConfigurationOutputTypeDef,
+        "snsTopic": SnsTopicConfigurationOutputTypeDef,
+        "sqsQueue": SqsQueueConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "ebsSnapshot": EbsSnapshotConfigurationTypeDef,
         "ecrRepository": EcrRepositoryConfigurationTypeDef,
         "iamRole": IamRoleConfigurationTypeDef,
         "efsFileSystem": EfsFileSystemConfigurationTypeDef,
@@ -1588,15 +1835,15 @@
 )
 
 _RequiredAccessPreviewTypeDef = TypedDict(
     "_RequiredAccessPreviewTypeDef",
     {
         "id": str,
         "analyzerArn": str,
-        "configurations": Dict[str, ConfigurationTypeDef],
+        "configurations": Dict[str, ConfigurationOutputTypeDef],
         "createdAt": datetime,
         "status": AccessPreviewStatusType,
     },
 )
 _OptionalAccessPreviewTypeDef = TypedDict(
     "_OptionalAccessPreviewTypeDef",
     {
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.0
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-accessanalyzer"></a>
 
 # mypy-boto3-accessanalyzer
 
 [![PyPI - mypy-boto3-accessanalyzer](https://img.shields.io/pypi/v/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-accessanalyzer?color=blue)](https://pypistats.org/packages/mypy-boto3-accessanalyzer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,120 +371,143 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
+    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
-    CriterionTypeDef,
+    CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
+    EbsSnapshotConfigurationOutputTypeDef,
+    EcrRepositoryConfigurationOutputTypeDef,
+    EfsFileSystemConfigurationOutputTypeDef,
+    IamRoleConfigurationOutputTypeDef,
+    SecretsManagerSecretConfigurationOutputTypeDef,
+    SnsTopicConfigurationOutputTypeDef,
+    SqsQueueConfigurationOutputTypeDef,
     EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
     ResponseMetadataTypeDef,
+    CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
     GetAnalyzedResourceRequestRequestTypeDef,
     GetAnalyzerRequestRequestTypeDef,
     GetArchiveRuleRequestRequestTypeDef,
     GetFindingRequestRequestTypeDef,
     GetGeneratedPolicyRequestRequestTypeDef,
     JobErrorTypeDef,
+    KmsGrantConstraintsOutputTypeDef,
     KmsGrantConstraintsTypeDef,
     PaginatorConfigTypeDef,
     ListAccessPreviewsRequestRequestTypeDef,
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
+    RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
+    RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
+    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
+    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
-    CreateArchiveRuleRequestRequestTypeDef,
-    InlineArchiveRuleTypeDef,
-    ListAccessPreviewFindingsRequestRequestTypeDef,
-    UpdateArchiveRuleRequestRequestTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAnalyzedResourceResponseTypeDef,
     ListAnalyzedResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartPolicyGenerationResponseTypeDef,
+    CreateArchiveRuleRequestRequestTypeDef,
+    InlineArchiveRuleTypeDef,
+    ListAccessPreviewFindingsRequestRequestTypeDef,
+    UpdateArchiveRuleRequestRequestTypeDef,
     FindingSourceTypeDef,
     JobDetailsTypeDef,
+    KmsGrantConfigurationOutputTypeDef,
     KmsGrantConfigurationTypeDef,
     ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef,
     ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef,
     ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef,
     ListAnalyzersRequestListAnalyzersPaginateTypeDef,
     ListArchiveRulesRequestListArchiveRulesPaginateTypeDef,
     ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef,
     ValidatePolicyRequestValidatePolicyPaginateTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     ListPolicyGenerationsResponseTypeDef,
+    NetworkOriginConfigurationOutputTypeDef,
     NetworkOriginConfigurationTypeDef,
     PathElementTypeDef,
     SpanTypeDef,
+    RdsDbClusterSnapshotConfigurationOutputTypeDef,
     RdsDbClusterSnapshotConfigurationTypeDef,
+    RdsDbSnapshotConfigurationOutputTypeDef,
     RdsDbSnapshotConfigurationTypeDef,
     ListAccessPreviewsResponseTypeDef,
     GetAnalyzerResponseTypeDef,
     ListAnalyzersResponseTypeDef,
     GetArchiveRuleResponseTypeDef,
     ListArchiveRulesResponseTypeDef,
-    CreateAnalyzerRequestRequestTypeDef,
     StartPolicyGenerationRequestRequestTypeDef,
     GeneratedPolicyPropertiesTypeDef,
+    CreateAnalyzerRequestRequestTypeDef,
     AccessPreviewFindingTypeDef,
     FindingSummaryTypeDef,
     FindingTypeDef,
+    KmsKeyConfigurationOutputTypeDef,
     KmsKeyConfigurationTypeDef,
+    S3AccessPointConfigurationOutputTypeDef,
     S3AccessPointConfigurationTypeDef,
     LocationTypeDef,
     GeneratedPolicyResultTypeDef,
     ListAccessPreviewFindingsResponseTypeDef,
     ListFindingsResponseTypeDef,
     GetFindingResponseTypeDef,
+    S3BucketConfigurationOutputTypeDef,
     S3BucketConfigurationTypeDef,
     ValidatePolicyFindingTypeDef,
     GetGeneratedPolicyResponseTypeDef,
+    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ValidatePolicyResponseTypeDef,
     AccessPreviewTypeDef,
     CreateAccessPreviewRequestRequestTypeDef,
     GetAccessPreviewResponseTypeDef,
 )
```

### Comparing `mypy-boto3-accessanalyzer-1.28.0/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt` & `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.0/setup.py` & `mypy-boto3-accessanalyzer-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-accessanalyzer",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AccessAnalyzer 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

