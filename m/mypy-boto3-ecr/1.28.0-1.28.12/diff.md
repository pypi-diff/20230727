# Comparing `tmp/mypy-boto3-ecr-1.28.0.tar.gz` & `tmp/mypy-boto3-ecr-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecr-1.28.0.tar", last modified: Thu Jul  6 20:59:29 2023, max compression
+gzip compressed data, was "mypy-boto3-ecr-1.28.12.tar", last modified: Thu Jul 27 05:34:37 2023, max compression
```

## Comparing `mypy-boto3-ecr-1.28.0.tar` & `mypy-boto3-ecr-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.662291 mypy-boto3-ecr-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-07-06 20:59:29.662291 mypy-boto3-ecr-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.662291 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51967 2023-07-06 20:39:51.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51894 2023-07-06 20:39:50.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-06 20:39:47.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:29.662291 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20004 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:29.000000 mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:29.662291 mypy-boto3-ecr-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:39:46.000000 mypy-boto3-ecr-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.788523 mypy-boto3-ecr-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33677 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-27 05:21:29.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54739 2023-07-27 05:21:28.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:37.780523 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20369 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:37.000000 mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:37.788523 mypy-boto3-ecr-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:27.000000 mypy-boto3-ecr-1.28.12/setup.py
```

### Comparing `mypy-boto3-ecr-1.28.0/LICENSE` & `mypy-boto3-ecr-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/PKG-INFO` & `mypy-boto3-ecr-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.0
-Summary: Type annotations for boto3.ECR 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,14 +391,15 @@
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
@@ -419,42 +420,48 @@
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
     DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
     DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
     GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
     PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
+    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
+    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
+    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -465,63 +472,66 @@
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
+    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
-    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
-    RegistryScanningRuleTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    RegistryScanningRuleTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ecr-1.28.0/README.md` & `mypy-boto3-ecr-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,14 +359,15 @@
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
@@ -387,42 +388,48 @@
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
     DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
     DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
     GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
     PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
+    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
+    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
+    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -433,63 +440,66 @@
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
+    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
-    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
-    RegistryScanningRuleTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    RegistryScanningRuleTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__init__.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__init__.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/__main__.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECR 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ECR 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/client.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/client.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/literals.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.py`

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

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/literals.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -208,14 +208,15 @@
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
@@ -294,26 +295,28 @@
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

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/paginator.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/paginator.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/type_defs.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ImageIdentifierTypeDef",
+    "ImageIdentifierOutputTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
     "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
@@ -74,42 +74,48 @@
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
     "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
     "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
     "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
     "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "VulnerablePackageTypeDef",
     "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
     "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
     "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
     "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
+    "ScanningRepositoryFilterOutputTypeDef",
     "ScanningRepositoryFilterTypeDef",
+    "ReplicationDestinationOutputTypeDef",
     "ReplicationDestinationTypeDef",
+    "RepositoryFilterOutputTypeDef",
     "RepositoryFilterTypeDef",
     "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
     "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -120,63 +126,66 @@
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
     "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
+    "StartImageScanRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
-    "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
-    "PutImageScanningConfigurationResponseTypeDef",
-    "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
+    "PutImageScanningConfigurationResponseTypeDef",
+    "RepositoryTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "RegistryScanningRuleTypeDef",
+    "RegistryScanningRuleOutputTypeDef",
     "RepositoryScanningConfigurationTypeDef",
+    "RegistryScanningRuleTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "ScoreDetailsTypeDef",
+    "DescribeImagesResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
-    "ScoreDetailsTypeDef",
-    "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationRequestRequestTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
+    "PutReplicationConfigurationRequestRequestTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -187,19 +196,17 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -232,22 +239,20 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -270,14 +275,23 @@
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+ImageIdentifierOutputTypeDef = TypedDict(
+    "ImageIdentifierOutputTypeDef",
+    {
+        "imageDigest": str,
+        "imageTag": str,
+    },
+    total=False,
+)
+
 BatchGetRepositoryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryNames": Sequence[str],
     },
 )
 
@@ -303,22 +317,20 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
 CompleteLayerUploadResponseTypeDef = TypedDict(
     "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "layerDigest": str,
@@ -337,22 +349,20 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
 CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
     "CreatePullThroughCacheRuleResponseTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
@@ -370,21 +380,19 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
-
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -428,22 +436,20 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteLifecyclePolicyResponseTypeDef = TypedDict(
     "DeleteLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "lastEvaluatedAt": datetime,
@@ -461,22 +467,20 @@
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
 DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
     "DeletePullThroughCacheRuleResponseTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
@@ -503,22 +507,20 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteRepositoryPolicyResponseTypeDef = TypedDict(
     "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -536,21 +538,19 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
@@ -633,14 +633,33 @@
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKey": str,
+    },
+    total=False,
+)
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "registryIds": Sequence[str],
     },
     total=False,
 )
@@ -656,22 +675,20 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
-
 GetDownloadUrlForLayerResponseTypeDef = TypedDict(
     "GetDownloadUrlForLayerResponseTypeDef",
     {
         "downloadUrl": str,
         "layerDigest": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -703,22 +720,20 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "lastEvaluatedAt": datetime,
@@ -745,22 +760,20 @@
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetRepositoryPolicyResponseTypeDef = TypedDict(
     "GetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -773,36 +786,42 @@
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "scanOnPush": bool,
+    },
+    total=False,
+)
+
 _RequiredInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
 InitiateLayerUploadResponseTypeDef = TypedDict(
     "InitiateLayerUploadResponseTypeDef",
     {
         "uploadId": str,
         "partSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -827,14 +846,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 VulnerablePackageTypeDef = TypedDict(
     "VulnerablePackageTypeDef",
     {
         "arch": str,
         "epoch": int,
         "filePath": str,
         "name": str,
@@ -870,21 +898,19 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
-
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -892,22 +918,20 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
-
 PutImageTagMutabilityResponseTypeDef = TypedDict(
     "PutImageTagMutabilityResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -925,22 +949,20 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 PutLifecyclePolicyResponseTypeDef = TypedDict(
     "PutLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -968,30 +990,54 @@
     {
         "url": str,
         "text": str,
     },
     total=False,
 )
 
+ScanningRepositoryFilterOutputTypeDef = TypedDict(
+    "ScanningRepositoryFilterOutputTypeDef",
+    {
+        "filter": str,
+        "filterType": Literal["WILDCARD"],
+    },
+)
+
 ScanningRepositoryFilterTypeDef = TypedDict(
     "ScanningRepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["WILDCARD"],
     },
 )
 
+ReplicationDestinationOutputTypeDef = TypedDict(
+    "ReplicationDestinationOutputTypeDef",
+    {
+        "region": str,
+        "registryId": str,
+    },
+)
+
 ReplicationDestinationTypeDef = TypedDict(
     "ReplicationDestinationTypeDef",
     {
         "region": str,
         "registryId": str,
     },
 )
 
+RepositoryFilterOutputTypeDef = TypedDict(
+    "RepositoryFilterOutputTypeDef",
+    {
+        "filter": str,
+        "filterType": Literal["PREFIX_MATCH"],
+    },
+)
+
 RepositoryFilterTypeDef = TypedDict(
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
 )
@@ -1019,22 +1065,20 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 SetRepositoryPolicyResponseTypeDef = TypedDict(
     "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1052,22 +1096,20 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
-
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "StartLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
@@ -1097,21 +1139,19 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
-
 UploadLayerPartResponseTypeDef = TypedDict(
     "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "lastByteReceived": int,
@@ -1167,21 +1207,19 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1190,21 +1228,19 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1212,22 +1248,20 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1236,22 +1270,20 @@
     {
         "registryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
     _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1261,75 +1293,71 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImageScanRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImageScanRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class StartImageScanRequestRequestTypeDef(
+    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
+):
+    pass
 
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImageScanRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImageScanRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-
-class StartImageScanRequestRequestTypeDef(
-    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
 )
@@ -1337,47 +1365,20 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
-PutImageScanningConfigurationResponseTypeDef = TypedDict(
-    "PutImageScanningConfigurationResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
-    {
-        "repositoryArn": str,
-        "registryId": str,
-        "repositoryName": str,
-        "repositoryUri": str,
-        "createdAt": datetime,
-        "imageTagMutability": ImageTagMutabilityType,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "encryptionConfiguration": EncryptionConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalCreateRepositoryRequestRequestTypeDef = TypedDict(
@@ -1388,29 +1389,19 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1427,15 +1418,15 @@
     total=False,
 )
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
@@ -1451,28 +1442,26 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
-
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
@@ -1487,22 +1476,20 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1513,21 +1500,19 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
-
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1546,22 +1531,20 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1573,22 +1556,20 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1599,22 +1580,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1625,14 +1604,39 @@
         "imageManifestMediaType": str,
         "artifactMediaType": str,
         "lastRecordedPullTime": datetime,
     },
     total=False,
 )
 
+PutImageScanningConfigurationResponseTypeDef = TypedDict(
+    "PutImageScanningConfigurationResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
+    {
+        "repositoryArn": str,
+        "registryId": str,
+        "repositoryName": str,
+        "repositoryUri": str,
+        "createdAt": datetime,
+        "imageTagMutability": ImageTagMutabilityType,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+        "encryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LifecyclePolicyPreviewResultTypeDef = TypedDict(
     "LifecyclePolicyPreviewResultTypeDef",
     {
         "imageTags": List[str],
         "imageDigest": str,
         "imagePushedAt": datetime,
         "action": LifecyclePolicyRuleActionTypeDef,
@@ -1653,22 +1657,20 @@
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1678,20 +1680,26 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
@@ -1710,68 +1718,93 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-RegistryScanningRuleTypeDef = TypedDict(
-    "RegistryScanningRuleTypeDef",
+RegistryScanningRuleOutputTypeDef = TypedDict(
+    "RegistryScanningRuleOutputTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterOutputTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
         "repositoryName": str,
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
-        "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
+        "appliedScanFilters": List[ScanningRepositoryFilterOutputTypeDef],
+    },
+    total=False,
+)
+
+RegistryScanningRuleTypeDef = TypedDict(
+    "RegistryScanningRuleTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
+    },
+)
+
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "destinations": List[ReplicationDestinationOutputTypeDef],
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "repositoryFilters": List[RepositoryFilterOutputTypeDef],
     },
     total=False,
 )
 
+class ReplicationRuleOutputTypeDef(
+    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+):
+    pass
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
-        "destinations": List[ReplicationDestinationTypeDef],
+        "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
-
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
     },
     total=False,
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "failures": List[ImageFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
@@ -1786,14 +1819,31 @@
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ScoreDetailsTypeDef = TypedDict(
+    "ScoreDetailsTypeDef",
+    {
+        "cvss": CvssScoreDetailsTypeDef,
+    },
+    total=False,
+)
+
+DescribeImagesResponseTypeDef = TypedDict(
+    "DescribeImagesResponseTypeDef",
+    {
+        "imageDetails": List[ImageDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1811,76 +1861,66 @@
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ScoreDetailsTypeDef = TypedDict(
-    "ScoreDetailsTypeDef",
-    {
-        "cvss": CvssScoreDetailsTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesResponseTypeDef = TypedDict(
-    "DescribeImagesResponseTypeDef",
-    {
-        "imageDetails": List[ImageDetailTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
-    },
-    total=False,
-)
-
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleTypeDef],
+        "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleTypeDef],
+    },
+    total=False,
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": List[ReplicationRuleTypeDef],
+        "rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1919,31 +1959,31 @@
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
@@ -1956,14 +1996,14 @@
 )
 
 DescribeImageScanFindingsResponseTypeDef = TypedDict(
     "DescribeImageScanFindingsResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/type_defs.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,22 +37,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
     "ImageIdentifierTypeDef",
+    "ImageIdentifierOutputTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
     "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
     "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
@@ -73,42 +75,48 @@
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
     "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
     "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
     "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
     "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
     "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
     "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "VulnerablePackageTypeDef",
     "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
     "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
     "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
     "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
+    "ScanningRepositoryFilterOutputTypeDef",
     "ScanningRepositoryFilterTypeDef",
+    "ReplicationDestinationOutputTypeDef",
     "ReplicationDestinationTypeDef",
+    "RepositoryFilterOutputTypeDef",
     "RepositoryFilterTypeDef",
     "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
     "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
     "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -119,63 +127,66 @@
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
     "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
+    "StartImageScanRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
-    "StartImageScanRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
-    "PutImageScanningConfigurationResponseTypeDef",
-    "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
+    "PutImageScanningConfigurationResponseTypeDef",
+    "RepositoryTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
-    "RegistryScanningRuleTypeDef",
+    "RegistryScanningRuleOutputTypeDef",
     "RepositoryScanningConfigurationTypeDef",
+    "RegistryScanningRuleTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
+    "ScoreDetailsTypeDef",
+    "DescribeImagesResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
-    "ScoreDetailsTypeDef",
-    "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationRequestRequestTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
+    "PutReplicationConfigurationRequestRequestTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -186,17 +197,19 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -229,20 +242,22 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -265,14 +280,23 @@
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
 )
 
+ImageIdentifierOutputTypeDef = TypedDict(
+    "ImageIdentifierOutputTypeDef",
+    {
+        "imageDigest": str,
+        "imageTag": str,
+    },
+    total=False,
+)
+
 BatchGetRepositoryScanningConfigurationRequestRequestTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryNames": Sequence[str],
     },
 )
 
@@ -298,20 +322,22 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
 CompleteLayerUploadResponseTypeDef = TypedDict(
     "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "layerDigest": str,
@@ -330,20 +356,22 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
+
 CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
     "CreatePullThroughCacheRuleResponseTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
@@ -361,19 +389,21 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
+
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -417,20 +447,22 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteLifecyclePolicyResponseTypeDef = TypedDict(
     "DeleteLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "lastEvaluatedAt": datetime,
@@ -448,20 +480,22 @@
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
+
 DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
     "DeletePullThroughCacheRuleResponseTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
@@ -488,20 +522,22 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteRepositoryPolicyResponseTypeDef = TypedDict(
     "DeleteRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -519,19 +555,21 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
@@ -614,14 +652,35 @@
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigurationOutputTypeDef",
+    {
+        "encryptionType": EncryptionTypeType,
+    },
+)
+_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKey": str,
+    },
+    total=False,
+)
+
+
+class EncryptionConfigurationOutputTypeDef(
+    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
+):
+    pass
+
+
 GetAuthorizationTokenRequestRequestTypeDef = TypedDict(
     "GetAuthorizationTokenRequestRequestTypeDef",
     {
         "registryIds": Sequence[str],
     },
     total=False,
 )
@@ -637,20 +696,22 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
+
 GetDownloadUrlForLayerResponseTypeDef = TypedDict(
     "GetDownloadUrlForLayerResponseTypeDef",
     {
         "downloadUrl": str,
         "layerDigest": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -682,20 +743,22 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "lastEvaluatedAt": datetime,
@@ -722,20 +785,22 @@
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetRepositoryPolicyResponseTypeDef = TypedDict(
     "GetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -748,34 +813,44 @@
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "scanOnPush": bool,
+    },
+    total=False,
+)
+
 _RequiredInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredInitiateLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalInitiateLayerUploadRequestRequestTypeDef = TypedDict(
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
+
 InitiateLayerUploadResponseTypeDef = TypedDict(
     "InitiateLayerUploadResponseTypeDef",
     {
         "uploadId": str,
         "partSize": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -800,14 +875,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 VulnerablePackageTypeDef = TypedDict(
     "VulnerablePackageTypeDef",
     {
         "arch": str,
         "epoch": int,
         "filePath": str,
         "name": str,
@@ -843,19 +927,21 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
+
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -863,20 +949,22 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
+
 PutImageTagMutabilityResponseTypeDef = TypedDict(
     "PutImageTagMutabilityResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -894,20 +982,22 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 PutLifecyclePolicyResponseTypeDef = TypedDict(
     "PutLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -935,30 +1025,54 @@
     {
         "url": str,
         "text": str,
     },
     total=False,
 )
 
+ScanningRepositoryFilterOutputTypeDef = TypedDict(
+    "ScanningRepositoryFilterOutputTypeDef",
+    {
+        "filter": str,
+        "filterType": Literal["WILDCARD"],
+    },
+)
+
 ScanningRepositoryFilterTypeDef = TypedDict(
     "ScanningRepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["WILDCARD"],
     },
 )
 
+ReplicationDestinationOutputTypeDef = TypedDict(
+    "ReplicationDestinationOutputTypeDef",
+    {
+        "region": str,
+        "registryId": str,
+    },
+)
+
 ReplicationDestinationTypeDef = TypedDict(
     "ReplicationDestinationTypeDef",
     {
         "region": str,
         "registryId": str,
     },
 )
 
+RepositoryFilterOutputTypeDef = TypedDict(
+    "RepositoryFilterOutputTypeDef",
+    {
+        "filter": str,
+        "filterType": Literal["PREFIX_MATCH"],
+    },
+)
+
 RepositoryFilterTypeDef = TypedDict(
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
 )
@@ -986,20 +1100,22 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 SetRepositoryPolicyResponseTypeDef = TypedDict(
     "SetRepositoryPolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "policyText": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1017,20 +1133,22 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
+
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "StartLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
@@ -1060,19 +1178,21 @@
     "_OptionalUploadLayerPartRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class UploadLayerPartRequestRequestTypeDef(
     _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
 ):
     pass
 
+
 UploadLayerPartResponseTypeDef = TypedDict(
     "UploadLayerPartResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
         "lastByteReceived": int,
@@ -1128,19 +1248,21 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1149,19 +1271,21 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1169,20 +1293,22 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1191,20 +1317,22 @@
     {
         "registryId": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
     _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1214,71 +1342,75 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
+    "_RequiredStartImageScanRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
+    "_OptionalStartImageScanRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class StartImageScanRequestRequestTypeDef(
+    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
+):
+    pass
+
+
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
     total=False,
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageManifest": str,
         "imageManifestMediaType": str,
     },
     total=False,
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredStartImageScanRequestRequestTypeDef = TypedDict(
-    "_RequiredStartImageScanRequestRequestTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalStartImageScanRequestRequestTypeDef = TypedDict(
-    "_OptionalStartImageScanRequestRequestTypeDef",
-    {
-        "registryId": str,
-    },
-    total=False,
-)
-
-class StartImageScanRequestRequestTypeDef(
-    _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
-):
-    pass
-
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
 )
@@ -1286,44 +1418,21 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
-PutImageScanningConfigurationResponseTypeDef = TypedDict(
-    "PutImageScanningConfigurationResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RepositoryTypeDef = TypedDict(
-    "RepositoryTypeDef",
-    {
-        "repositoryArn": str,
-        "registryId": str,
-        "repositoryName": str,
-        "repositoryUri": str,
-        "createdAt": datetime,
-        "imageTagMutability": ImageTagMutabilityType,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "encryptionConfiguration": EncryptionConfigurationTypeDef,
-    },
-    total=False,
-)
 
 _RequiredCreateRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -1335,26 +1444,20 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -1372,15 +1475,15 @@
     total=False,
 )
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
@@ -1396,26 +1499,28 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
+
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
@@ -1430,20 +1535,22 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1454,19 +1561,21 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
+
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1485,20 +1594,22 @@
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1510,20 +1621,22 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1534,20 +1647,22 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1558,14 +1673,39 @@
         "imageManifestMediaType": str,
         "artifactMediaType": str,
         "lastRecordedPullTime": datetime,
     },
     total=False,
 )
 
+PutImageScanningConfigurationResponseTypeDef = TypedDict(
+    "PutImageScanningConfigurationResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RepositoryTypeDef = TypedDict(
+    "RepositoryTypeDef",
+    {
+        "repositoryArn": str,
+        "registryId": str,
+        "repositoryName": str,
+        "repositoryUri": str,
+        "createdAt": datetime,
+        "imageTagMutability": ImageTagMutabilityType,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+        "encryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 LifecyclePolicyPreviewResultTypeDef = TypedDict(
     "LifecyclePolicyPreviewResultTypeDef",
     {
         "imageTags": List[str],
         "imageDigest": str,
         "imagePushedAt": datetime,
         "action": LifecyclePolicyRuleActionTypeDef,
@@ -1586,20 +1726,22 @@
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1609,19 +1751,29 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
         "source": str,
@@ -1639,66 +1791,97 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
-RegistryScanningRuleTypeDef = TypedDict(
-    "RegistryScanningRuleTypeDef",
+RegistryScanningRuleOutputTypeDef = TypedDict(
+    "RegistryScanningRuleOutputTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": List[ScanningRepositoryFilterOutputTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
         "repositoryName": str,
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
-        "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
+        "appliedScanFilters": List[ScanningRepositoryFilterOutputTypeDef],
+    },
+    total=False,
+)
+
+RegistryScanningRuleTypeDef = TypedDict(
+    "RegistryScanningRuleTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
+    },
+)
+
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "destinations": List[ReplicationDestinationOutputTypeDef],
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "repositoryFilters": List[RepositoryFilterOutputTypeDef],
     },
     total=False,
 )
 
+
+class ReplicationRuleOutputTypeDef(
+    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
-        "destinations": List[ReplicationDestinationTypeDef],
+        "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
+
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
     },
     total=False,
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
-        "imageIds": List[ImageIdentifierTypeDef],
+        "imageIds": List[ImageIdentifierOutputTypeDef],
         "failures": List[ImageFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
@@ -1713,14 +1896,31 @@
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ScoreDetailsTypeDef = TypedDict(
+    "ScoreDetailsTypeDef",
+    {
+        "cvss": CvssScoreDetailsTypeDef,
+    },
+    total=False,
+)
+
+DescribeImagesResponseTypeDef = TypedDict(
+    "DescribeImagesResponseTypeDef",
+    {
+        "imageDetails": List[ImageDetailTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1738,76 +1938,66 @@
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ScoreDetailsTypeDef = TypedDict(
-    "ScoreDetailsTypeDef",
-    {
-        "cvss": CvssScoreDetailsTypeDef,
-    },
-    total=False,
-)
-
-DescribeImagesResponseTypeDef = TypedDict(
-    "DescribeImagesResponseTypeDef",
-    {
-        "imageDetails": List[ImageDetailTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
-    },
-    total=False,
-)
-
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleTypeDef],
+        "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleTypeDef],
+    },
+    total=False,
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": List[ReplicationRuleTypeDef],
+        "rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1846,31 +2036,31 @@
     },
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
@@ -1883,14 +2073,14 @@
 )
 
 DescribeImageScanFindingsResponseTypeDef = TypedDict(
     "DescribeImageScanFindingsResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
+        "imageId": ImageIdentifierOutputTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/waiter.py` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr/waiter.pyi` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/PKG-INFO` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ecr
-Version: 1.28.0
-Summary: Type annotations for boto3.ECR 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ecr"></a>
 
 # mypy-boto3-ecr
 
 [![PyPI - mypy-boto3-ecr](https://img.shields.io/pypi/v/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ecr.svg?color=blue)](https://pypi.org/project/mypy-boto3-ecr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ecr?color=blue)](https://pypistats.org/packages/mypy-boto3-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ecr)](https://pepy.tech/project/mypy-boto3-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ECR 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[boto3.ECR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [mypy-boto3-ecr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -391,14 +391,15 @@
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
     ImageIdentifierTypeDef,
+    ImageIdentifierOutputTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
@@ -419,42 +420,48 @@
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
     DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
     DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
     GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
     GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
     GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
     InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     VulnerablePackageTypeDef,
     PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
     PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
+    ScanningRepositoryFilterOutputTypeDef,
     ScanningRepositoryFilterTypeDef,
+    ReplicationDestinationOutputTypeDef,
     ReplicationDestinationTypeDef,
+    RepositoryFilterOutputTypeDef,
     RepositoryFilterTypeDef,
     ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
@@ -465,63 +472,66 @@
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
     DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
+    StartImageScanRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
-    StartImageScanRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
-    PutImageScanningConfigurationResponseTypeDef,
-    RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
+    PutImageScanningConfigurationResponseTypeDef,
+    RepositoryTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
-    RegistryScanningRuleTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    RegistryScanningRuleTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
+    ScoreDetailsTypeDef,
+    DescribeImagesResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
-    ScoreDetailsTypeDef,
-    DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
 def get_structure() -> AttributeTypeDef:
     return {...}
```

### Comparing `mypy-boto3-ecr-1.28.0/mypy_boto3_ecr.egg-info/SOURCES.txt` & `mypy-boto3-ecr-1.28.12/mypy_boto3_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecr-1.28.0/setup.py` & `mypy-boto3-ecr-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecr",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECR 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ECR 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

