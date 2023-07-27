# Comparing `tmp/mypy-boto3-s3control-1.28.0.tar.gz` & `tmp/mypy-boto3-s3control-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-s3control-1.28.0.tar", last modified: Thu Jul  6 21:00:30 2023, max compression
+gzip compressed data, was "mypy-boto3-s3control-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
```

## Comparing `mypy-boto3-s3control-1.28.0.tar` & `mypy-boto3-s3control-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.346416 mypy-boto3-s3control-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-07-06 21:00:30.346416 mypy-boto3-s3control-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21197 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.334416 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:54:06.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    70244 2023-07-06 20:54:08.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70167 2023-07-06 20:54:07.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:30.346416 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22690 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 21:00:30.000000 mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:30.346416 mypy-boto3-s3control-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:54:05.000000 mypy-boto3-s3control-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43055 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42983 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-27 11:45:17.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98307 2023-07-27 11:45:19.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98192 2023-07-27 11:45:18.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25817 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 11:49:32.000000 mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.117240 mypy-boto3-s3control-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 11:45:15.000000 mypy-boto3-s3control-1.28.12/setup.py
```

### Comparing `mypy-boto3-s3control-1.28.0/LICENSE` & `mypy-boto3-s3control-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/PKG-INFO` & `mypy-boto3-s3control-1.28.12/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-s3control
-Version: 1.28.0
-Summary: Type annotations for boto3.S3Control 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,231 +364,311 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
+    ActivityMetricsOutputTypeDef,
+    AdvancedCostOptimizationMetricsOutputTypeDef,
+    AdvancedDataProtectionMetricsOutputTypeDef,
+    DetailedStatusCodesMetricsOutputTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
+    DeleteMultiRegionAccessPointInputOutputTypeDef,
+    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
+    AwsLambdaTransformationOutputTypeDef,
     AwsLambdaTransformationTypeDef,
+    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
+    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    CreateAccessPointResultTypeDef,
+    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    CreateJobResultTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
+    RegionOutputTypeDef,
     RegionTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
+    ExcludeOutputTypeDef,
     ExcludeTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
-    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
-    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
+    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
+    MultiRegionAccessPointRouteOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagTypeDef,
+    StorageLensTagOutputTypeDef,
+    IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
+    JobReportOutputTypeDef,
+    JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
+    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
+    JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
+    LambdaInvokeOperationOutputTypeDef,
+    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    PaginatorConfigTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
+    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
+    StorageLensTagTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    ResponseMetadataTypeDef,
+    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
+    S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
+    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
+    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
+    S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
+    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
-    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
-    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    ObjectLambdaContentTransformationOutputTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    CreateAccessPointForObjectLambdaResultTypeDef,
     ObjectLambdaAccessPointTypeDef,
-    CreateAccessPointRequestRequestTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
+    CreateAccessPointForObjectLambdaResultTypeDef,
+    CreateAccessPointResultTypeDef,
+    CreateBucketResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
+    GetAccessPointPolicyResultTypeDef,
+    GetBucketPolicyResultTypeDef,
+    GetBucketResultTypeDef,
+    GetBucketVersioningResultTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
+    UpdateJobPriorityResultTypeDef,
+    UpdateJobStatusResultTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
+    CreateAccessPointRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
+    JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
+    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    S3GrantOutputTypeDef,
     S3GrantTypeDef,
+    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
+    S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
+    StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
+    ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
+    S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
+    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
+    S3AccessControlListOutputTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
     S3CopyObjectOperationTypeDef,
+    S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
+    ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
     LifecycleRuleTypeDef,
+    S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
+    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
+    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
+    S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
+    StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
-    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
+    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
+    JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
+    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
+    S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
+    JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobDescriptorTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.0/README.md` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-s3control
+Version: 1.28.12
+Summary: Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,231 +364,311 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
+    ActivityMetricsOutputTypeDef,
+    AdvancedCostOptimizationMetricsOutputTypeDef,
+    AdvancedDataProtectionMetricsOutputTypeDef,
+    DetailedStatusCodesMetricsOutputTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
+    DeleteMultiRegionAccessPointInputOutputTypeDef,
+    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
+    AwsLambdaTransformationOutputTypeDef,
     AwsLambdaTransformationTypeDef,
+    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
+    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    CreateAccessPointResultTypeDef,
+    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    CreateJobResultTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
+    RegionOutputTypeDef,
     RegionTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
+    ExcludeOutputTypeDef,
     ExcludeTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
-    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
-    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
+    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
+    MultiRegionAccessPointRouteOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagTypeDef,
+    StorageLensTagOutputTypeDef,
+    IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
+    JobReportOutputTypeDef,
+    JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
+    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
+    JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
+    LambdaInvokeOperationOutputTypeDef,
+    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    PaginatorConfigTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
+    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
+    StorageLensTagTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    ResponseMetadataTypeDef,
+    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
+    S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
+    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
+    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
+    S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
+    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
-    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
-    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    ObjectLambdaContentTransformationOutputTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    CreateAccessPointForObjectLambdaResultTypeDef,
     ObjectLambdaAccessPointTypeDef,
-    CreateAccessPointRequestRequestTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
+    CreateAccessPointForObjectLambdaResultTypeDef,
+    CreateAccessPointResultTypeDef,
+    CreateBucketResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
+    GetAccessPointPolicyResultTypeDef,
+    GetBucketPolicyResultTypeDef,
+    GetBucketResultTypeDef,
+    GetBucketVersioningResultTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
+    UpdateJobPriorityResultTypeDef,
+    UpdateJobStatusResultTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
+    CreateAccessPointRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
+    JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
+    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    S3GrantOutputTypeDef,
     S3GrantTypeDef,
+    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
+    S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
+    StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
+    ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
+    S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
+    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
+    S3AccessControlListOutputTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
     S3CopyObjectOperationTypeDef,
+    S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
+    ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
     LifecycleRuleTypeDef,
+    S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
+    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
+    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
+    S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
+    StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
-    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
+    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
+    JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
+    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
+    S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
+    JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobDescriptorTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__init__.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__init__.pyi` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/__main__.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.S3Control 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.S3Control 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control\nOther"
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

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/client.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/client.pyi` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/literals.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,15 @@
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
@@ -399,26 +400,28 @@
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

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/literals.pyi` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -311,14 +311,15 @@
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
@@ -397,26 +398,28 @@
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

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/paginator.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListAccessPointsForObjectLambdaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPointsForObjectLambdaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
         """
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/paginator.pyi` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListAccessPointsForObjectLambdaPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
     """
 
     def paginate(
-        self, *, AccountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAccessPointsForObjectLambdaResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/paginators/#listaccesspointsforobjectlambdapaginator)
         """
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/type_defs.py` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3control service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
+    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -65,251 +65,378 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
+    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
-    "VpcConfigurationTypeDef",
+    "VpcConfigurationOutputTypeDef",
+    "ActivityMetricsOutputTypeDef",
+    "AdvancedCostOptimizationMetricsOutputTypeDef",
+    "AdvancedDataProtectionMetricsOutputTypeDef",
+    "DetailedStatusCodesMetricsOutputTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
-    "DeleteMultiRegionAccessPointInputTypeDef",
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
+    "DeleteMultiRegionAccessPointInputOutputTypeDef",
+    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
+    "AwsLambdaTransformationOutputTypeDef",
     "AwsLambdaTransformationTypeDef",
+    "CloudWatchMetricsOutputTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
+    "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
-    "CreateAccessPointResultTypeDef",
+    "VpcConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketResultTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
-    "CreateJobResultTypeDef",
+    "PublicAccessBlockConfigurationOutputTypeDef",
+    "RegionOutputTypeDef",
     "RegionTypeDef",
-    "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
+    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteMultiRegionAccessPointResultTypeDef",
+    "DeleteMultiRegionAccessPointInputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
+    "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
+    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
+    "SSEKMSEncryptionOutputTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
-    "GetAccessPointPolicyResultTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "GetBucketPolicyResultTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
-    "GetBucketResultTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
+    "S3TagOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
-    "GetBucketVersioningResultTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "MultiRegionAccessPointRouteTypeDef",
+    "MultiRegionAccessPointRouteOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "StorageLensTagTypeDef",
+    "StorageLensTagOutputTypeDef",
+    "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
+    "JobReportOutputTypeDef",
+    "JobManifestGeneratorFilterOutputTypeDef",
     "JobManifestGeneratorFilterTypeDef",
+    "JobManifestLocationOutputTypeDef",
     "JobManifestLocationTypeDef",
+    "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
+    "LambdaInvokeOperationOutputTypeDef",
+    "S3InitiateRestoreObjectOperationOutputTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
+    "NoncurrentVersionExpirationOutputTypeDef",
+    "NoncurrentVersionTransitionOutputTypeDef",
+    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
-    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
+    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
-    "PaginatorConfigTypeDef",
+    "MultiRegionAccessPointRouteTypeDef",
+    "SelectionCriteriaOutputTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
+    "StorageLensTagTypeDef",
+    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3ObjectOwnerOutputTypeDef",
     "S3ObjectOwnerTypeDef",
+    "S3ObjectMetadataOutputTypeDef",
     "S3ObjectMetadataTypeDef",
+    "S3GranteeOutputTypeDef",
     "S3GranteeTypeDef",
+    "S3ObjectLockLegalHoldOutputTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
+    "S3RetentionOutputTypeDef",
     "S3RetentionTypeDef",
+    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
+    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
+    "StorageLensAwsOrgOutputTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
-    "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
-    "UpdateJobStatusResultTypeDef",
     "AccessPointTypeDef",
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    "ObjectLambdaContentTransformationOutputTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
-    "CreateAccessPointForObjectLambdaResultTypeDef",
     "ObjectLambdaAccessPointTypeDef",
-    "CreateAccessPointRequestRequestTypeDef",
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    "GetAccessPointResultTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
+    "CreateAccessPointForObjectLambdaResultTypeDef",
+    "CreateAccessPointResultTypeDef",
+    "CreateBucketResultTypeDef",
+    "CreateJobResultTypeDef",
+    "CreateMultiRegionAccessPointResultTypeDef",
+    "DeleteMultiRegionAccessPointResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    "GetAccessPointPolicyResultTypeDef",
+    "GetBucketPolicyResultTypeDef",
+    "GetBucketResultTypeDef",
+    "GetBucketVersioningResultTypeDef",
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    "UpdateJobPriorityResultTypeDef",
+    "UpdateJobStatusResultTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
+    "CreateAccessPointRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
-    "GetBucketTaggingResultTypeDef",
-    "GetJobTaggingResultTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    "GetAccessPointResultTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
+    "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
+    "GetBucketTaggingResultTypeDef",
+    "GetJobTaggingResultTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    "S3SetObjectTaggingOperationOutputTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
+    "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
+    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
+    "MetricsOutputTypeDef",
+    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+    "PrefixLevelStorageMetricsOutputTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    "S3GrantOutputTypeDef",
     "S3GrantTypeDef",
+    "S3SetObjectLegalHoldOperationOutputTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
+    "S3SetObjectRetentionOperationOutputTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
+    "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
+    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
+    "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
+    "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "JobListDescriptorTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
+    "PrefixLevelOutputTypeDef",
     "PrefixLevelTypeDef",
+    "S3AccessControlListOutputTypeDef",
+    "S3CopyObjectOperationOutputTypeDef",
     "S3AccessControlListTypeDef",
     "S3CopyObjectOperationTypeDef",
+    "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
+    "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
     "LifecycleRuleTypeDef",
+    "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "ListJobsResultTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
+    "BucketLevelOutputTypeDef",
     "BucketLevelTypeDef",
+    "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
+    "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
-    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
-    "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
+    "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
+    "AccountLevelOutputTypeDef",
     "AccountLevelTypeDef",
+    "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
+    "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobDescriptorTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
+    "AbortIncompleteMultipartUploadOutputTypeDef",
+    {
+        "DaysAfterInitiation": int,
+    },
+    total=False,
+)
+
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
+AccessControlTranslationOutputTypeDef = TypedDict(
+    "AccessControlTranslationOutputTypeDef",
+    {
+        "Owner": Literal["Destination"],
+    },
+)
+
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
-VpcConfigurationTypeDef = TypedDict(
-    "VpcConfigurationTypeDef",
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
     {
         "VpcId": str,
     },
 )
 
+ActivityMetricsOutputTypeDef = TypedDict(
+    "ActivityMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+AdvancedCostOptimizationMetricsOutputTypeDef = TypedDict(
+    "AdvancedCostOptimizationMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+AdvancedDataProtectionMetricsOutputTypeDef = TypedDict(
+    "AdvancedDataProtectionMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+DetailedStatusCodesMetricsOutputTypeDef = TypedDict(
+    "DetailedStatusCodesMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
 ActivityMetricsTypeDef = TypedDict(
     "ActivityMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
@@ -345,29 +472,50 @@
         "Message": str,
         "Resource": str,
         "RequestId": str,
     },
     total=False,
 )
 
-DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputTypeDef",
+DeleteMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputOutputTypeDef",
     {
         "Name": str,
     },
 )
 
-PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
+PutMultiRegionAccessPointPolicyInputOutputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
     {
         "Name": str,
         "Policy": str,
     },
 )
 
+_RequiredAwsLambdaTransformationOutputTypeDef = TypedDict(
+    "_RequiredAwsLambdaTransformationOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+)
+_OptionalAwsLambdaTransformationOutputTypeDef = TypedDict(
+    "_OptionalAwsLambdaTransformationOutputTypeDef",
+    {
+        "FunctionPayload": str,
+    },
+    total=False,
+)
+
+
+class AwsLambdaTransformationOutputTypeDef(
+    _RequiredAwsLambdaTransformationOutputTypeDef, _OptionalAwsLambdaTransformationOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsLambdaTransformationTypeDef = TypedDict(
     "_RequiredAwsLambdaTransformationTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalAwsLambdaTransformationTypeDef = TypedDict(
@@ -381,14 +529,21 @@
 
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
 
+CloudWatchMetricsOutputTypeDef = TypedDict(
+    "CloudWatchMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+)
+
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -397,51 +552,51 @@
     {
         "Value": str,
         "Status": ObjectLambdaAccessPointAliasStatusType,
     },
     total=False,
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
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-CreateAccessPointResultTypeDef = TypedDict(
-    "CreateAccessPointResultTypeDef",
+VpcConfigurationTypeDef = TypedDict(
+    "VpcConfigurationTypeDef",
     {
-        "AccessPointArn": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcId": str,
     },
 )
 
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketResultTypeDef = TypedDict(
-    "CreateBucketResultTypeDef",
-    {
-        "Location": str,
-        "BucketArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobReportTypeDef = TypedDict(
     "_RequiredJobReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalJobReportTypeDef = TypedDict(
@@ -464,22 +619,44 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
+PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationOutputTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BlockPublicAcls": bool,
+        "IgnorePublicAcls": bool,
+        "BlockPublicPolicy": bool,
+        "RestrictPublicBuckets": bool,
     },
+    total=False,
 )
 
+_RequiredRegionOutputTypeDef = TypedDict(
+    "_RequiredRegionOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalRegionOutputTypeDef = TypedDict(
+    "_OptionalRegionOutputTypeDef",
+    {
+        "BucketAccountId": str,
+    },
+    total=False,
+)
+
+
+class RegionOutputTypeDef(_RequiredRegionOutputTypeDef, _OptionalRegionOutputTypeDef):
+    pass
+
+
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -491,22 +668,14 @@
 )
 
 
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
 
-CreateMultiRegionAccessPointResultTypeDef = TypedDict(
-    "CreateMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -579,26 +748,32 @@
     "DeleteJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
 
+DeleteMarkerReplicationOutputTypeDef = TypedDict(
+    "DeleteMarkerReplicationOutputTypeDef",
+    {
+        "Status": DeleteMarkerReplicationStatusType,
+    },
+)
+
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
-DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointResultTypeDef",
+DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputTypeDef",
     {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -633,53 +808,77 @@
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     {
         "AccountId": str,
         "RequestTokenARN": str,
     },
 )
 
-EncryptionConfigurationTypeDef = TypedDict(
-    "EncryptionConfigurationTypeDef",
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EncryptionConfigurationTypeDef = TypedDict(
+    "EncryptionConfigurationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicaKmsKeyID": str,
     },
+    total=False,
 )
 
 EstablishedMultiRegionAccessPointPolicyTypeDef = TypedDict(
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-ExcludeTypeDef = TypedDict(
-    "ExcludeTypeDef",
+ExcludeOutputTypeDef = TypedDict(
+    "ExcludeOutputTypeDef",
     {
         "Buckets": List[str],
         "Regions": List[str],
     },
     total=False,
 )
 
+ExcludeTypeDef = TypedDict(
+    "ExcludeTypeDef",
+    {
+        "Buckets": Sequence[str],
+        "Regions": Sequence[str],
+    },
+    total=False,
+)
+
+ExistingObjectReplicationOutputTypeDef = TypedDict(
+    "ExistingObjectReplicationOutputTypeDef",
+    {
+        "Status": ExistingObjectReplicationStatusType,
+    },
+)
+
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
+SSEKMSEncryptionOutputTypeDef = TypedDict(
+    "SSEKMSEncryptionOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSEncryptionTypeDef = TypedDict(
     "SSEKMSEncryptionTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -703,38 +902,22 @@
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
-GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAccessPointPolicyRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
-GetAccessPointPolicyResultTypeDef = TypedDict(
-    "GetAccessPointPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -775,22 +958,14 @@
     "GetBucketPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketPolicyResultTypeDef = TypedDict(
-    "GetBucketPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketReplicationRequestRequestTypeDef = TypedDict(
     "GetBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -799,49 +974,38 @@
     "GetBucketRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketResultTypeDef = TypedDict(
-    "GetBucketResultTypeDef",
+GetBucketTaggingRequestRequestTypeDef = TypedDict(
+    "GetBucketTaggingRequestRequestTypeDef",
     {
+        "AccountId": str,
         "Bucket": str,
-        "PublicAccessBlockEnabled": bool,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketTaggingRequestRequestTypeDef = TypedDict(
-    "GetBucketTaggingRequestRequestTypeDef",
+S3TagOutputTypeDef = TypedDict(
+    "S3TagOutputTypeDef",
     {
-        "AccountId": str,
-        "Bucket": str,
+        "Key": str,
+        "Value": str,
     },
 )
 
 GetBucketVersioningRequestRequestTypeDef = TypedDict(
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketVersioningResultTypeDef = TypedDict(
-    "GetBucketVersioningResultTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobTaggingRequestRequestTypeDef = TypedDict(
     "GetJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
@@ -874,32 +1038,33 @@
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
         "Mrap": str,
     },
 )
 
-_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteTypeDef",
+_RequiredMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteOutputTypeDef",
     {
         "TrafficDialPercentage": int,
     },
 )
-_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteTypeDef",
+_OptionalMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteOutputTypeDef",
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
 
-class MultiRegionAccessPointRouteTypeDef(
-    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
+class MultiRegionAccessPointRouteOutputTypeDef(
+    _RequiredMultiRegionAccessPointRouteOutputTypeDef,
+    _OptionalMultiRegionAccessPointRouteOutputTypeDef,
 ):
     pass
 
 
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
@@ -919,51 +1084,115 @@
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
         "AccountId": str,
     },
 )
 
-StorageLensTagTypeDef = TypedDict(
-    "StorageLensTagTypeDef",
+StorageLensTagOutputTypeDef = TypedDict(
+    "StorageLensTagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-IncludeTypeDef = TypedDict(
-    "IncludeTypeDef",
+IncludeOutputTypeDef = TypedDict(
+    "IncludeOutputTypeDef",
     {
         "Buckets": List[str],
         "Regions": List[str],
     },
     total=False,
 )
 
+IncludeTypeDef = TypedDict(
+    "IncludeTypeDef",
+    {
+        "Buckets": Sequence[str],
+        "Regions": Sequence[str],
+    },
+    total=False,
+)
+
 JobFailureTypeDef = TypedDict(
     "JobFailureTypeDef",
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredJobReportOutputTypeDef = TypedDict(
+    "_RequiredJobReportOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalJobReportOutputTypeDef = TypedDict(
+    "_OptionalJobReportOutputTypeDef",
+    {
+        "Bucket": str,
+        "Format": Literal["Report_CSV_20180820"],
+        "Prefix": str,
+        "ReportScope": JobReportScopeType,
+    },
+    total=False,
+)
+
+
+class JobReportOutputTypeDef(_RequiredJobReportOutputTypeDef, _OptionalJobReportOutputTypeDef):
+    pass
+
+
+JobManifestGeneratorFilterOutputTypeDef = TypedDict(
+    "JobManifestGeneratorFilterOutputTypeDef",
+    {
+        "EligibleForReplication": bool,
+        "CreatedAfter": datetime,
+        "CreatedBefore": datetime,
+        "ObjectReplicationStatuses": List[ReplicationStatusType],
+    },
+    total=False,
+)
+
 JobManifestGeneratorFilterTypeDef = TypedDict(
     "JobManifestGeneratorFilterTypeDef",
     {
         "EligibleForReplication": bool,
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
+_RequiredJobManifestLocationOutputTypeDef = TypedDict(
+    "_RequiredJobManifestLocationOutputTypeDef",
+    {
+        "ObjectArn": str,
+        "ETag": str,
+    },
+)
+_OptionalJobManifestLocationOutputTypeDef = TypedDict(
+    "_OptionalJobManifestLocationOutputTypeDef",
+    {
+        "ObjectVersionId": str,
+    },
+    total=False,
+)
+
+
+class JobManifestLocationOutputTypeDef(
+    _RequiredJobManifestLocationOutputTypeDef, _OptionalJobManifestLocationOutputTypeDef
+):
+    pass
+
+
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -978,14 +1207,35 @@
 
 class JobManifestLocationTypeDef(
     _RequiredJobManifestLocationTypeDef, _OptionalJobManifestLocationTypeDef
 ):
     pass
 
 
+_RequiredJobManifestSpecOutputTypeDef = TypedDict(
+    "_RequiredJobManifestSpecOutputTypeDef",
+    {
+        "Format": JobManifestFormatType,
+    },
+)
+_OptionalJobManifestSpecOutputTypeDef = TypedDict(
+    "_OptionalJobManifestSpecOutputTypeDef",
+    {
+        "Fields": List[JobManifestFieldNameType],
+    },
+    total=False,
+)
+
+
+class JobManifestSpecOutputTypeDef(
+    _RequiredJobManifestSpecOutputTypeDef, _OptionalJobManifestSpecOutputTypeDef
+):
+    pass
+
+
 _RequiredJobManifestSpecTypeDef = TypedDict(
     "_RequiredJobManifestSpecTypeDef",
     {
         "Format": JobManifestFormatType,
     },
 )
 _OptionalJobManifestSpecTypeDef = TypedDict(
@@ -997,14 +1247,31 @@
 )
 
 
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
 
+LambdaInvokeOperationOutputTypeDef = TypedDict(
+    "LambdaInvokeOperationOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+    total=False,
+)
+
+S3InitiateRestoreObjectOperationOutputTypeDef = TypedDict(
+    "S3InitiateRestoreObjectOperationOutputTypeDef",
+    {
+        "ExpirationInDays": int,
+        "GlacierJobTier": S3GlacierJobTierType,
+    },
+    total=False,
+)
+
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1022,73 +1289,99 @@
     "JobTimersTypeDef",
     {
         "ElapsedTimeInActiveSeconds": int,
     },
     total=False,
 )
 
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+    total=False,
+)
+
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
-NoncurrentVersionExpirationTypeDef = TypedDict(
-    "NoncurrentVersionExpirationTypeDef",
+NoncurrentVersionExpirationOutputTypeDef = TypedDict(
+    "NoncurrentVersionExpirationOutputTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
 )
 
-NoncurrentVersionTransitionTypeDef = TypedDict(
-    "NoncurrentVersionTransitionTypeDef",
+NoncurrentVersionTransitionOutputTypeDef = TypedDict(
+    "NoncurrentVersionTransitionOutputTypeDef",
     {
         "NoncurrentDays": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-TransitionTypeDef = TypedDict(
-    "TransitionTypeDef",
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
     {
         "Date": datetime,
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+NoncurrentVersionExpirationTypeDef = TypedDict(
+    "NoncurrentVersionExpirationTypeDef",
     {
-        "AccountId": str,
+        "NoncurrentDays": int,
+        "NewerNoncurrentVersions": int,
     },
+    total=False,
 )
-_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+
+NoncurrentVersionTransitionTypeDef = TypedDict(
+    "NoncurrentVersionTransitionTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "NoncurrentDays": int,
+        "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
+TransitionTypeDef = TypedDict(
+    "TransitionTypeDef",
+    {
+        "Date": Union[datetime, str],
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
 
-class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
-    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-):
-    pass
-
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
 
 _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
@@ -1266,14 +1559,22 @@
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
 
+ReplicationTimeValueOutputTypeDef = TypedDict(
+    "ReplicationTimeValueOutputTypeDef",
+    {
+        "Minutes": int,
+    },
+    total=False,
+)
+
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1301,20 +1602,42 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TrafficDialPercentage": int,
+    },
+)
+_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteTypeDef",
+    {
+        "Bucket": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+
+class MultiRegionAccessPointRouteTypeDef(
+    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
+):
+    pass
+
+
+SelectionCriteriaOutputTypeDef = TypedDict(
+    "SelectionCriteriaOutputTypeDef",
+    {
+        "Delimiter": str,
+        "MaxDepth": int,
+        "MinStorageBytesPercentage": float,
     },
     total=False,
 )
 
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
@@ -1371,49 +1694,80 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
-PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
+PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "Policy": str,
+    },
+)
+
+StorageLensTagTypeDef = TypedDict(
+    "StorageLensTagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+ReplicaModificationsOutputTypeDef = TypedDict(
+    "ReplicaModificationsOutputTypeDef",
+    {
+        "Status": ReplicaModificationsStatusType,
     },
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3ObjectOwnerOutputTypeDef = TypedDict(
+    "S3ObjectOwnerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ID": str,
+        "DisplayName": str,
     },
+    total=False,
 )
 
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+S3ObjectMetadataOutputTypeDef = TypedDict(
+    "S3ObjectMetadataOutputTypeDef",
+    {
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "UserMetadata": Dict[str, str],
+        "ContentLength": int,
+        "ContentMD5": str,
+        "ContentType": str,
+        "HttpExpiresDate": datetime,
+        "RequesterCharged": bool,
+        "SSEAlgorithm": S3SSEAlgorithmType,
+    },
+    total=False,
+)
+
 S3ObjectMetadataTypeDef = TypedDict(
     "S3ObjectMetadataTypeDef",
     {
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
         "ContentLanguage": str,
@@ -1424,54 +1778,101 @@
         "HttpExpiresDate": Union[datetime, str],
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
+S3GranteeOutputTypeDef = TypedDict(
+    "S3GranteeOutputTypeDef",
+    {
+        "TypeIdentifier": S3GranteeTypeIdentifierType,
+        "Identifier": str,
+        "DisplayName": str,
+    },
+    total=False,
+)
+
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+S3ObjectLockLegalHoldOutputTypeDef = TypedDict(
+    "S3ObjectLockLegalHoldOutputTypeDef",
+    {
+        "Status": S3ObjectLockLegalHoldStatusType,
+    },
+)
+
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
+S3RetentionOutputTypeDef = TypedDict(
+    "S3RetentionOutputTypeDef",
+    {
+        "RetainUntilDate": datetime,
+        "Mode": S3ObjectLockRetentionModeType,
+    },
+    total=False,
+)
+
 S3RetentionTypeDef = TypedDict(
     "S3RetentionTypeDef",
     {
         "RetainUntilDate": Union[datetime, str],
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
+SSEKMSOutputTypeDef = TypedDict(
+    "SSEKMSOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
+SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
+    "SseKmsEncryptedObjectsOutputTypeDef",
+    {
+        "Status": SseKmsEncryptedObjectsStatusType,
+    },
+)
+
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
+StorageLensAwsOrgOutputTypeDef = TypedDict(
+    "StorageLensAwsOrgOutputTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
 StorageLensAwsOrgTypeDef = TypedDict(
     "StorageLensAwsOrgTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -1480,23 +1881,14 @@
     {
         "AccountId": str,
         "JobId": str,
         "Priority": int,
     },
 )
 
-UpdateJobPriorityResultTypeDef = TypedDict(
-    "UpdateJobPriorityResultTypeDef",
-    {
-        "JobId": str,
-        "Priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateJobStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobStatusRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
         "RequestedJobStatus": RequestedJobStatusType,
     },
@@ -1512,83 +1904,54 @@
 
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
 
-UpdateJobStatusResultTypeDef = TypedDict(
-    "UpdateJobStatusResultTypeDef",
-    {
-        "JobId": str,
-        "Status": JobStatusType,
-        "StatusUpdateReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
 )
 _OptionalAccessPointTypeDef = TypedDict(
     "_OptionalAccessPointTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
 
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
 
-DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+ObjectLambdaContentTransformationOutputTypeDef = TypedDict(
+    "ObjectLambdaContentTransformationOutputTypeDef",
     {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": DeleteMultiRegionAccessPointInputTypeDef,
-    },
-)
-
-PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
+        "AwsLambda": AwsLambdaTransformationOutputTypeDef,
     },
+    total=False,
 )
 
 ObjectLambdaContentTransformationTypeDef = TypedDict(
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
-CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredObjectLambdaAccessPointTypeDef = TypedDict(
     "_RequiredObjectLambdaAccessPointTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalObjectLambdaAccessPointTypeDef = TypedDict(
@@ -1603,83 +1966,175 @@
 
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
 
-_RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessPointRequestRequestTypeDef",
+CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaResultTypeDef",
     {
-        "AccountId": str,
-        "Name": str,
-        "Bucket": str,
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateAccessPointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessPointRequestRequestTypeDef",
+
+CreateAccessPointResultTypeDef = TypedDict(
+    "CreateAccessPointResultTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "BucketAccountId": str,
+        "AccessPointArn": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+CreateBucketResultTypeDef = TypedDict(
+    "CreateBucketResultTypeDef",
+    {
+        "Location": str,
+        "BucketArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class CreateAccessPointRequestRequestTypeDef(
-    _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
-):
-    pass
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+CreateMultiRegionAccessPointResultTypeDef = TypedDict(
+    "CreateMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointForObjectLambdaResultTypeDef",
+DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointResultTypeDef",
     {
-        "Name": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "CreationDate": datetime,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestTokenARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccessPointResultTypeDef = TypedDict(
-    "GetAccessPointResultTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointPolicyResultTypeDef = TypedDict(
+    "GetAccessPointPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyResultTypeDef = TypedDict(
+    "GetBucketPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketResultTypeDef = TypedDict(
+    "GetBucketResultTypeDef",
     {
-        "Name": str,
         "Bucket": str,
-        "NetworkOrigin": NetworkOriginType,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlockEnabled": bool,
         "CreationDate": datetime,
-        "Alias": str,
-        "AccessPointArn": str,
-        "Endpoints": Dict[str, str],
-        "BucketAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
+GetBucketVersioningResultTypeDef = TypedDict(
+    "GetBucketVersioningResultTypeDef",
     {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobPriorityResultTypeDef = TypedDict(
+    "UpdateJobPriorityResultTypeDef",
+    {
+        "JobId": str,
+        "Priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobStatusResultTypeDef = TypedDict(
+    "UpdateJobStatusResultTypeDef",
+    {
+        "JobId": str,
+        "Status": JobStatusType,
+        "StatusUpdateReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "PutPublicAccessBlockRequestRequestTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "AccountId": str,
     },
 )
 
+_RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessPointRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "Name": str,
+        "Bucket": str,
+    },
+)
+_OptionalCreateAccessPointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessPointRequestRequestTypeDef",
+    {
+        "VpcConfiguration": VpcConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "BucketAccountId": str,
+    },
+    total=False,
+)
+
+
+class CreateAccessPointRequestRequestTypeDef(
+    _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestRequestTypeDef = TypedDict(
@@ -1701,35 +2156,19 @@
 
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
 
-GetBucketTaggingResultTypeDef = TypedDict(
-    "GetBucketTaggingResultTypeDef",
-    {
-        "TagSet": List[S3TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetJobTaggingResultTypeDef = TypedDict(
-    "GetJobTaggingResultTypeDef",
-    {
-        "Tags": List[S3TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[S3TagTypeDef],
+        "Tags": Sequence[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 PutJobTaggingRequestRequestTypeDef = TypedDict(
@@ -1741,15 +2180,15 @@
     },
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[S3TagTypeDef],
+        "Tags": Sequence[S3TagTypeDef],
     },
     total=False,
 )
 
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
@@ -1761,14 +2200,73 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
+GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    {
+        "Name": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointResultTypeDef = TypedDict(
+    "GetAccessPointResultTypeDef",
+    {
+        "Name": str,
+        "Bucket": str,
+        "NetworkOrigin": NetworkOriginType,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "CreationDate": datetime,
+        "Alias": str,
+        "AccessPointArn": str,
+        "Endpoints": Dict[str, str],
+        "BucketAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
+    {
+        "Name": str,
+        "Regions": List[RegionOutputTypeDef],
+    },
+)
+_OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
+    {
+        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateMultiRegionAccessPointInputOutputTypeDef(
+    _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
+    _OptionalCreateMultiRegionAccessPointInputOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateMultiRegionAccessPointInputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
         "Regions": Sequence[RegionTypeDef],
     },
 )
@@ -1784,91 +2282,143 @@
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
 
+DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": DeleteMultiRegionAccessPointInputTypeDef,
+    },
+)
+
+GeneratedManifestEncryptionOutputTypeDef = TypedDict(
+    "GeneratedManifestEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSEncryptionTypeDef,
     },
     total=False,
 )
 
 GetAccessPointPolicyStatusForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMultiRegionAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
-    "GetMultiRegionAccessPointRoutesResultTypeDef",
+GetBucketTaggingResultTypeDef = TypedDict(
+    "GetBucketTaggingResultTypeDef",
     {
-        "Mrap": str,
-        "Routes": List[MultiRegionAccessPointRouteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagSet": List[S3TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+GetJobTaggingResultTypeDef = TypedDict(
+    "GetJobTaggingResultTypeDef",
     {
-        "AccountId": str,
-        "Mrap": str,
-        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
+        "Tags": List[S3TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
-    "GetStorageLensConfigurationTaggingResultTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
-        "Tags": List[StorageLensTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[S3TagOutputTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
     },
+    total=False,
 )
 
-PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
     {
-        "ConfigId": str,
-        "AccountId": str,
-        "Tags": Sequence[StorageLensTagTypeDef],
+        "Prefix": str,
+        "Tags": List[S3TagOutputTypeDef],
+    },
+    total=False,
+)
+
+S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
+    "S3SetObjectTaggingOperationOutputTypeDef",
+    {
+        "TagSet": List[S3TagOutputTypeDef],
+    },
+    total=False,
+)
+
+GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
+    "GetMultiRegionAccessPointRoutesResultTypeDef",
+    {
+        "Mrap": str,
+        "Routes": List[MultiRegionAccessPointRouteOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
+    "GetStorageLensConfigurationTaggingResultTypeDef",
+    {
+        "Tags": List[StorageLensTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
-        "Location": JobManifestLocationTypeDef,
+        "Location": JobManifestLocationOutputTypeDef,
     },
     total=False,
 )
 
+JobManifestOutputTypeDef = TypedDict(
+    "JobManifestOutputTypeDef",
+    {
+        "Spec": JobManifestSpecOutputTypeDef,
+        "Location": JobManifestLocationOutputTypeDef,
+    },
+)
+
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
         "Location": JobManifestLocationTypeDef,
     },
 )
@@ -1880,29 +2430,78 @@
         "NumberOfTasksSucceeded": int,
         "NumberOfTasksFailed": int,
         "Timers": JobTimersTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
+    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+):
+    pass
+
+
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStorageLensConfigurationsResultTypeDef = TypedDict(
     "ListStorageLensConfigurationsResultTypeDef",
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMetricsOutputTypeDef = TypedDict(
+    "_RequiredMetricsOutputTypeDef",
+    {
+        "Status": MetricsStatusType,
+    },
+)
+_OptionalMetricsOutputTypeDef = TypedDict(
+    "_OptionalMetricsOutputTypeDef",
+    {
+        "EventThreshold": ReplicationTimeValueOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MetricsOutputTypeDef(_RequiredMetricsOutputTypeDef, _OptionalMetricsOutputTypeDef):
+    pass
+
+
+ReplicationTimeOutputTypeDef = TypedDict(
+    "ReplicationTimeOutputTypeDef",
+    {
+        "Status": ReplicationTimeStatusType,
+        "Time": ReplicationTimeValueOutputTypeDef,
     },
 )
 
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
@@ -1948,21 +2547,39 @@
 
 MultiRegionAccessPointReportTypeDef = TypedDict(
     "MultiRegionAccessPointReportTypeDef",
     {
         "Name": str,
         "Alias": str,
         "CreatedAt": datetime,
-        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
         "Status": MultiRegionAccessPointStatusType,
         "Regions": List[RegionReportTypeDef],
     },
     total=False,
 )
 
+SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "Mrap": str,
+        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
+    },
+)
+
+PrefixLevelStorageMetricsOutputTypeDef = TypedDict(
+    "PrefixLevelStorageMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+        "SelectionCriteria": SelectionCriteriaOutputTypeDef,
+    },
+    total=False,
+)
+
 PrefixLevelStorageMetricsTypeDef = TypedDict(
     "PrefixLevelStorageMetricsTypeDef",
     {
         "IsEnabled": bool,
         "SelectionCriteria": SelectionCriteriaTypeDef,
     },
     total=False,
@@ -1988,30 +2605,86 @@
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
 
+PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
+    },
+)
+
+PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    {
+        "ConfigId": str,
+        "AccountId": str,
+        "Tags": Sequence[StorageLensTagTypeDef],
+    },
+)
+
+S3GrantOutputTypeDef = TypedDict(
+    "S3GrantOutputTypeDef",
+    {
+        "Grantee": S3GranteeOutputTypeDef,
+        "Permission": S3PermissionType,
+    },
+    total=False,
+)
+
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
 )
 
+S3SetObjectLegalHoldOperationOutputTypeDef = TypedDict(
+    "S3SetObjectLegalHoldOperationOutputTypeDef",
+    {
+        "LegalHold": S3ObjectLockLegalHoldOutputTypeDef,
+    },
+)
+
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
+_RequiredS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
+    "_RequiredS3SetObjectRetentionOperationOutputTypeDef",
+    {
+        "Retention": S3RetentionOutputTypeDef,
+    },
+)
+_OptionalS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
+    "_OptionalS3SetObjectRetentionOperationOutputTypeDef",
+    {
+        "BypassGovernanceRetention": bool,
+    },
+    total=False,
+)
+
+
+class S3SetObjectRetentionOperationOutputTypeDef(
+    _RequiredS3SetObjectRetentionOperationOutputTypeDef,
+    _OptionalS3SetObjectRetentionOperationOutputTypeDef,
+):
+    pass
+
+
 _RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_RequiredS3SetObjectRetentionOperationTypeDef",
     {
         "Retention": S3RetentionTypeDef,
     },
 )
 _OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
@@ -2025,38 +2698,64 @@
 
 class S3SetObjectRetentionOperationTypeDef(
     _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
 ):
     pass
 
 
+StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
+    "StorageLensDataExportEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSOutputTypeDef,
+    },
+    total=False,
+)
+
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
-        "SSES3": Dict[str, Any],
+        "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
+SourceSelectionCriteriaOutputTypeDef = TypedDict(
+    "SourceSelectionCriteriaOutputTypeDef",
+    {
+        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
+        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
 )
 
 ListAccessPointsResultTypeDef = TypedDict(
     "ListAccessPointsResultTypeDef",
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
+    "ObjectLambdaTransformationConfigurationOutputTypeDef",
+    {
+        "Actions": List[ObjectLambdaTransformationConfigurationActionType],
+        "ContentTransformation": ObjectLambdaContentTransformationOutputTypeDef,
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2065,15 +2764,15 @@
 )
 
 ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
     "ListAccessPointsForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
@@ -2103,30 +2802,54 @@
         "Tagging": TaggingTypeDef,
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
-        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputTypeDef,
-        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
-        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
+        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
+        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputOutputTypeDef,
+        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputOutputTypeDef,
     },
     total=False,
 )
 
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
 )
 
+_RequiredS3ManifestOutputLocationOutputTypeDef = TypedDict(
+    "_RequiredS3ManifestOutputLocationOutputTypeDef",
+    {
+        "Bucket": str,
+        "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
+    },
+)
+_OptionalS3ManifestOutputLocationOutputTypeDef = TypedDict(
+    "_OptionalS3ManifestOutputLocationOutputTypeDef",
+    {
+        "ExpectedManifestBucketOwner": str,
+        "ManifestPrefix": str,
+        "ManifestEncryption": GeneratedManifestEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3ManifestOutputLocationOutputTypeDef(
+    _RequiredS3ManifestOutputLocationOutputTypeDef, _OptionalS3ManifestOutputLocationOutputTypeDef
+):
+    pass
+
+
 _RequiredS3ManifestOutputLocationTypeDef = TypedDict(
     "_RequiredS3ManifestOutputLocationTypeDef",
     {
         "Bucket": str,
         "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
     },
 )
@@ -2143,14 +2866,36 @@
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
 
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagOutputTypeDef,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagOutputTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
+    },
+    total=False,
+)
+
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2158,14 +2903,40 @@
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "ProgressSummary": JobProgressSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredDestinationOutputTypeDef = TypedDict(
+    "_RequiredDestinationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalDestinationOutputTypeDef = TypedDict(
+    "_OptionalDestinationOutputTypeDef",
+    {
+        "Account": str,
+        "ReplicationTime": ReplicationTimeOutputTypeDef,
+        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "Metrics": MetricsOutputTypeDef,
+        "StorageClass": ReplicationStorageClassType,
+    },
+    total=False,
+)
+
+
+class DestinationOutputTypeDef(
+    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
+):
+    pass
+
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -2186,15 +2957,15 @@
     pass
 
 
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AsyncResponseDetailsTypeDef = TypedDict(
     "AsyncResponseDetailsTypeDef",
     {
         "MultiRegionAccessPointDetails": MultiRegionAccessPointsAsyncResponseTypeDef,
@@ -2203,34 +2974,87 @@
     total=False,
 )
 
 GetMultiRegionAccessPointResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointResultTypeDef",
     {
         "AccessPoint": MultiRegionAccessPointReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiRegionAccessPointsResultTypeDef = TypedDict(
     "ListMultiRegionAccessPointsResultTypeDef",
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PrefixLevelOutputTypeDef = TypedDict(
+    "PrefixLevelOutputTypeDef",
+    {
+        "StorageMetrics": PrefixLevelStorageMetricsOutputTypeDef,
     },
 )
 
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
+_RequiredS3AccessControlListOutputTypeDef = TypedDict(
+    "_RequiredS3AccessControlListOutputTypeDef",
+    {
+        "Owner": S3ObjectOwnerOutputTypeDef,
+    },
+)
+_OptionalS3AccessControlListOutputTypeDef = TypedDict(
+    "_OptionalS3AccessControlListOutputTypeDef",
+    {
+        "Grants": List[S3GrantOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class S3AccessControlListOutputTypeDef(
+    _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
+):
+    pass
+
+
+S3CopyObjectOperationOutputTypeDef = TypedDict(
+    "S3CopyObjectOperationOutputTypeDef",
+    {
+        "TargetResource": str,
+        "CannedAccessControlList": S3CannedAccessControlListType,
+        "AccessControlGrants": List[S3GrantOutputTypeDef],
+        "MetadataDirective": S3MetadataDirectiveType,
+        "ModifiedSinceConstraint": datetime,
+        "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
+        "NewObjectTagging": List[S3TagOutputTypeDef],
+        "RedirectLocation": str,
+        "RequesterPays": bool,
+        "StorageClass": S3StorageClassType,
+        "UnModifiedSinceConstraint": datetime,
+        "SSEAwsKmsKeyId": str,
+        "TargetKeyPrefix": str,
+        "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
+        "ObjectLockMode": S3ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "BucketKeyEnabled": bool,
+        "ChecksumAlgorithm": S3ChecksumAlgorithmType,
+    },
+    total=False,
+)
+
 _RequiredS3AccessControlListTypeDef = TypedDict(
     "_RequiredS3AccessControlListTypeDef",
     {
         "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListTypeDef = TypedDict(
@@ -2269,14 +3093,39 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
+_RequiredS3BucketDestinationOutputTypeDef = TypedDict(
+    "_RequiredS3BucketDestinationOutputTypeDef",
+    {
+        "Format": FormatType,
+        "OutputSchemaVersion": Literal["V_1"],
+        "AccountId": str,
+        "Arn": str,
+    },
+)
+_OptionalS3BucketDestinationOutputTypeDef = TypedDict(
+    "_OptionalS3BucketDestinationOutputTypeDef",
+    {
+        "Prefix": str,
+        "Encryption": StorageLensDataExportEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3BucketDestinationOutputTypeDef(
+    _RequiredS3BucketDestinationOutputTypeDef, _OptionalS3BucketDestinationOutputTypeDef
+):
+    pass
+
+
 _RequiredS3BucketDestinationTypeDef = TypedDict(
     "_RequiredS3BucketDestinationTypeDef",
     {
         "Format": FormatType,
         "OutputSchemaVersion": Literal["V_1"],
         "AccountId": str,
         "Arn": str,
@@ -2294,14 +3143,37 @@
 
 class S3BucketDestinationTypeDef(
     _RequiredS3BucketDestinationTypeDef, _OptionalS3BucketDestinationTypeDef
 ):
     pass
 
 
+_RequiredObjectLambdaConfigurationOutputTypeDef = TypedDict(
+    "_RequiredObjectLambdaConfigurationOutputTypeDef",
+    {
+        "SupportingAccessPoint": str,
+        "TransformationConfigurations": List[ObjectLambdaTransformationConfigurationOutputTypeDef],
+    },
+)
+_OptionalObjectLambdaConfigurationOutputTypeDef = TypedDict(
+    "_OptionalObjectLambdaConfigurationOutputTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "AllowedFeatures": List[ObjectLambdaAllowedFeatureType],
+    },
+    total=False,
+)
+
+
+class ObjectLambdaConfigurationOutputTypeDef(
+    _RequiredObjectLambdaConfigurationOutputTypeDef, _OptionalObjectLambdaConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredObjectLambdaConfigurationTypeDef = TypedDict(
     "_RequiredObjectLambdaConfigurationTypeDef",
     {
         "SupportingAccessPoint": str,
         "TransformationConfigurations": Sequence[ObjectLambdaTransformationConfigurationTypeDef],
     },
 )
@@ -2329,27 +3201,51 @@
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Transitions": List[TransitionTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Transitions": Sequence[TransitionTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
 
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
 
+_RequiredS3JobManifestGeneratorOutputTypeDef = TypedDict(
+    "_RequiredS3JobManifestGeneratorOutputTypeDef",
+    {
+        "SourceBucket": str,
+        "EnableManifestOutput": bool,
+    },
+)
+_OptionalS3JobManifestGeneratorOutputTypeDef = TypedDict(
+    "_OptionalS3JobManifestGeneratorOutputTypeDef",
+    {
+        "ExpectedBucketOwner": str,
+        "ManifestOutputLocation": S3ManifestOutputLocationOutputTypeDef,
+        "Filter": JobManifestGeneratorFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class S3JobManifestGeneratorOutputTypeDef(
+    _RequiredS3JobManifestGeneratorOutputTypeDef, _OptionalS3JobManifestGeneratorOutputTypeDef
+):
+    pass
+
+
 _RequiredS3JobManifestGeneratorTypeDef = TypedDict(
     "_RequiredS3JobManifestGeneratorTypeDef",
     {
         "SourceBucket": str,
         "EnableManifestOutput": bool,
     },
 )
@@ -2366,23 +3262,79 @@
 
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
 
+_RequiredLifecycleRuleOutputTypeDef = TypedDict(
+    "_RequiredLifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleOutputTypeDef = TypedDict(
+    "_OptionalLifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class LifecycleRuleOutputTypeDef(
+    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+):
+    pass
+
+
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "Status": ReplicationRuleStatusType,
+        "Destination": DestinationOutputTypeDef,
+        "Bucket": str,
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "ID": str,
+        "Priority": int,
+        "Prefix": str,
+        "Filter": ReplicationRuleFilterOutputTypeDef,
+        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
     },
+    total=False,
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
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
         "Bucket": str,
     },
@@ -2415,110 +3367,180 @@
         "RequestParameters": AsyncRequestParametersTypeDef,
         "RequestStatus": str,
         "ResponseDetails": AsyncResponseDetailsTypeDef,
     },
     total=False,
 )
 
+BucketLevelOutputTypeDef = TypedDict(
+    "BucketLevelOutputTypeDef",
+    {
+        "ActivityMetrics": ActivityMetricsOutputTypeDef,
+        "PrefixLevel": PrefixLevelOutputTypeDef,
+        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
+        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
+        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
 BucketLevelTypeDef = TypedDict(
     "BucketLevelTypeDef",
     {
         "ActivityMetrics": ActivityMetricsTypeDef,
         "PrefixLevel": PrefixLevelTypeDef,
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
+S3AccessControlPolicyOutputTypeDef = TypedDict(
+    "S3AccessControlPolicyOutputTypeDef",
+    {
+        "AccessControlList": S3AccessControlListOutputTypeDef,
+        "CannedAccessControlList": S3CannedAccessControlListType,
+    },
+    total=False,
+)
+
 S3AccessControlPolicyTypeDef = TypedDict(
     "S3AccessControlPolicyTypeDef",
     {
         "AccessControlList": S3AccessControlListTypeDef,
         "CannedAccessControlList": S3CannedAccessControlListType,
     },
     total=False,
 )
 
+StorageLensDataExportOutputTypeDef = TypedDict(
+    "StorageLensDataExportOutputTypeDef",
+    {
+        "S3BucketDestination": S3BucketDestinationOutputTypeDef,
+        "CloudWatchMetrics": CloudWatchMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationTypeDef,
         "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
-CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
+GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     {
-        "AccountId": str,
-        "Name": str,
-        "Configuration": ObjectLambdaConfigurationTypeDef,
+        "Configuration": ObjectLambdaConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     {
+        "AccountId": str,
+        "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
-GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationResultTypeDef",
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
     {
-        "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": Sequence[LifecycleRuleTypeDef],
     },
+    total=False,
 )
 
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
+JobManifestGeneratorOutputTypeDef = TypedDict(
+    "JobManifestGeneratorOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleTypeDef],
+        "S3JobManifestGenerator": S3JobManifestGeneratorOutputTypeDef,
     },
     total=False,
 )
 
 JobManifestGeneratorTypeDef = TypedDict(
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
+GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    {
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredAccountLevelOutputTypeDef = TypedDict(
+    "_RequiredAccountLevelOutputTypeDef",
+    {
+        "BucketLevel": BucketLevelOutputTypeDef,
+    },
+)
+_OptionalAccountLevelOutputTypeDef = TypedDict(
+    "_OptionalAccountLevelOutputTypeDef",
+    {
+        "ActivityMetrics": ActivityMetricsOutputTypeDef,
+        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
+        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
+        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AccountLevelOutputTypeDef(
+    _RequiredAccountLevelOutputTypeDef, _OptionalAccountLevelOutputTypeDef
+):
+    pass
+
+
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
     },
 )
 _OptionalAccountLevelTypeDef = TypedDict(
@@ -2533,14 +3555,22 @@
 )
 
 
 class AccountLevelTypeDef(_RequiredAccountLevelTypeDef, _OptionalAccountLevelTypeDef):
     pass
 
 
+S3SetObjectAclOperationOutputTypeDef = TypedDict(
+    "S3SetObjectAclOperationOutputTypeDef",
+    {
+        "AccessControlPolicy": S3AccessControlPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SetObjectAclOperationTypeDef = TypedDict(
     "S3SetObjectAclOperationTypeDef",
     {
         "AccessControlPolicy": S3AccessControlPolicyTypeDef,
     },
     total=False,
 )
@@ -2567,28 +3597,55 @@
 ):
     pass
 
 
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+_RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStorageLensConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "AccountLevel": AccountLevelOutputTypeDef,
+        "IsEnabled": bool,
+    },
+)
+_OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStorageLensConfigurationOutputTypeDef",
+    {
+        "Include": IncludeOutputTypeDef,
+        "Exclude": ExcludeOutputTypeDef,
+        "DataExport": StorageLensDataExportOutputTypeDef,
+        "AwsOrg": StorageLensAwsOrgOutputTypeDef,
+        "StorageLensArn": str,
+    },
+    total=False,
+)
+
+
+class StorageLensConfigurationOutputTypeDef(
+    _RequiredStorageLensConfigurationOutputTypeDef, _OptionalStorageLensConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredStorageLensConfigurationTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -2608,14 +3665,30 @@
 
 class StorageLensConfigurationTypeDef(
     _RequiredStorageLensConfigurationTypeDef, _OptionalStorageLensConfigurationTypeDef
 ):
     pass
 
 
+JobOperationOutputTypeDef = TypedDict(
+    "JobOperationOutputTypeDef",
+    {
+        "LambdaInvoke": LambdaInvokeOperationOutputTypeDef,
+        "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
+        "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
+        "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
+        "S3DeleteObjectTagging": Dict[str, Any],
+        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationOutputTypeDef,
+        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationOutputTypeDef,
+        "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
+        "S3ReplicateObject": Dict[str, Any],
+    },
+    total=False,
+)
+
 JobOperationTypeDef = TypedDict(
     "JobOperationTypeDef",
     {
         "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationTypeDef,
         "S3PutObjectTagging": S3SetObjectTaggingOperationTypeDef,
@@ -2627,16 +3700,16 @@
     },
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
-        "StorageLensConfiguration": StorageLensConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StorageLensConfiguration": StorageLensConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -2656,14 +3729,40 @@
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+JobDescriptorTypeDef = TypedDict(
+    "JobDescriptorTypeDef",
+    {
+        "JobId": str,
+        "ConfirmationRequired": bool,
+        "Description": str,
+        "JobArn": str,
+        "Status": JobStatusType,
+        "Manifest": JobManifestOutputTypeDef,
+        "Operation": JobOperationOutputTypeDef,
+        "Priority": int,
+        "ProgressSummary": JobProgressSummaryTypeDef,
+        "StatusUpdateReason": str,
+        "FailureReasons": List[JobFailureTypeDef],
+        "Report": JobReportOutputTypeDef,
+        "CreationTime": datetime,
+        "TerminationDate": datetime,
+        "RoleArn": str,
+        "SuspendedDate": datetime,
+        "SuspendedCause": str,
+        "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
+        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "AccountId": str,
         "Operation": JobOperationTypeDef,
         "Report": JobReportTypeDef,
         "ClientRequestToken": str,
@@ -2686,40 +3785,14 @@
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
-JobDescriptorTypeDef = TypedDict(
-    "JobDescriptorTypeDef",
-    {
-        "JobId": str,
-        "ConfirmationRequired": bool,
-        "Description": str,
-        "JobArn": str,
-        "Status": JobStatusType,
-        "Manifest": JobManifestTypeDef,
-        "Operation": JobOperationTypeDef,
-        "Priority": int,
-        "ProgressSummary": JobProgressSummaryTypeDef,
-        "StatusUpdateReason": str,
-        "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportTypeDef,
-        "CreationTime": datetime,
-        "TerminationDate": datetime,
-        "RoleArn": str,
-        "SuspendedDate": datetime,
-        "SuspendedCause": str,
-        "ManifestGenerator": JobManifestGeneratorTypeDef,
-        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
-    },
-    total=False,
-)
-
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control/type_defs.pyi` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for s3control service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadTypeDef
+    from mypy_boto3_s3control.type_defs import AbortIncompleteMultipartUploadOutputTypeDef
 
-    data: AbortIncompleteMultipartUploadTypeDef = {...}
+    data: AbortIncompleteMultipartUploadOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,251 +64,378 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbortIncompleteMultipartUploadOutputTypeDef",
     "AbortIncompleteMultipartUploadTypeDef",
+    "AccessControlTranslationOutputTypeDef",
     "AccessControlTranslationTypeDef",
-    "VpcConfigurationTypeDef",
+    "VpcConfigurationOutputTypeDef",
+    "ActivityMetricsOutputTypeDef",
+    "AdvancedCostOptimizationMetricsOutputTypeDef",
+    "AdvancedDataProtectionMetricsOutputTypeDef",
+    "DetailedStatusCodesMetricsOutputTypeDef",
     "ActivityMetricsTypeDef",
     "AdvancedCostOptimizationMetricsTypeDef",
     "AdvancedDataProtectionMetricsTypeDef",
     "DetailedStatusCodesMetricsTypeDef",
     "AsyncErrorDetailsTypeDef",
-    "DeleteMultiRegionAccessPointInputTypeDef",
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
+    "DeleteMultiRegionAccessPointInputOutputTypeDef",
+    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
+    "AwsLambdaTransformationOutputTypeDef",
     "AwsLambdaTransformationTypeDef",
+    "CloudWatchMetricsOutputTypeDef",
     "CloudWatchMetricsTypeDef",
     "ObjectLambdaAccessPointAliasTypeDef",
+    "ResponseMetadataTypeDef",
     "PublicAccessBlockConfigurationTypeDef",
-    "CreateAccessPointResultTypeDef",
+    "VpcConfigurationTypeDef",
     "CreateBucketConfigurationTypeDef",
-    "CreateBucketResultTypeDef",
     "JobReportTypeDef",
     "S3TagTypeDef",
-    "CreateJobResultTypeDef",
+    "PublicAccessBlockConfigurationOutputTypeDef",
+    "RegionOutputTypeDef",
     "RegionTypeDef",
-    "CreateMultiRegionAccessPointResultTypeDef",
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "DeleteAccessPointPolicyRequestRequestTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteBucketLifecycleConfigurationRequestRequestTypeDef",
     "DeleteBucketPolicyRequestRequestTypeDef",
     "DeleteBucketReplicationRequestRequestTypeDef",
     "DeleteBucketRequestRequestTypeDef",
     "DeleteBucketTaggingRequestRequestTypeDef",
     "DeleteJobTaggingRequestRequestTypeDef",
+    "DeleteMarkerReplicationOutputTypeDef",
     "DeleteMarkerReplicationTypeDef",
-    "DeleteMultiRegionAccessPointResultTypeDef",
+    "DeleteMultiRegionAccessPointInputTypeDef",
     "DeletePublicAccessBlockRequestRequestTypeDef",
     "DeleteStorageLensConfigurationRequestRequestTypeDef",
     "DeleteStorageLensConfigurationTaggingRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
+    "ExcludeOutputTypeDef",
     "ExcludeTypeDef",
+    "ExistingObjectReplicationOutputTypeDef",
     "ExistingObjectReplicationTypeDef",
+    "SSEKMSEncryptionOutputTypeDef",
     "SSEKMSEncryptionTypeDef",
     "GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyRequestRequestTypeDef",
-    "GetAccessPointPolicyResultTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     "PolicyStatusTypeDef",
     "GetAccessPointPolicyStatusRequestRequestTypeDef",
     "GetAccessPointRequestRequestTypeDef",
     "GetBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketPolicyRequestRequestTypeDef",
-    "GetBucketPolicyResultTypeDef",
     "GetBucketReplicationRequestRequestTypeDef",
     "GetBucketRequestRequestTypeDef",
-    "GetBucketResultTypeDef",
     "GetBucketTaggingRequestRequestTypeDef",
+    "S3TagOutputTypeDef",
     "GetBucketVersioningRequestRequestTypeDef",
-    "GetBucketVersioningResultTypeDef",
     "GetJobTaggingRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyRequestRequestTypeDef",
     "GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef",
     "GetMultiRegionAccessPointRequestRequestTypeDef",
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
-    "MultiRegionAccessPointRouteTypeDef",
+    "MultiRegionAccessPointRouteOutputTypeDef",
     "GetPublicAccessBlockRequestRequestTypeDef",
     "GetStorageLensConfigurationRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
-    "StorageLensTagTypeDef",
+    "StorageLensTagOutputTypeDef",
+    "IncludeOutputTypeDef",
     "IncludeTypeDef",
     "JobFailureTypeDef",
+    "JobReportOutputTypeDef",
+    "JobManifestGeneratorFilterOutputTypeDef",
     "JobManifestGeneratorFilterTypeDef",
+    "JobManifestLocationOutputTypeDef",
     "JobManifestLocationTypeDef",
+    "JobManifestSpecOutputTypeDef",
     "JobManifestSpecTypeDef",
+    "LambdaInvokeOperationOutputTypeDef",
+    "S3InitiateRestoreObjectOperationOutputTypeDef",
     "LambdaInvokeOperationTypeDef",
     "S3InitiateRestoreObjectOperationTypeDef",
     "JobTimersTypeDef",
+    "LifecycleExpirationOutputTypeDef",
     "LifecycleExpirationTypeDef",
+    "NoncurrentVersionExpirationOutputTypeDef",
+    "NoncurrentVersionTransitionOutputTypeDef",
+    "TransitionOutputTypeDef",
     "NoncurrentVersionExpirationTypeDef",
     "NoncurrentVersionTransitionTypeDef",
     "TransitionTypeDef",
-    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessPointsForObjectLambdaRequestRequestTypeDef",
     "ListAccessPointsRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListMultiRegionAccessPointsRequestRequestTypeDef",
     "ListRegionalBucketsRequestRequestTypeDef",
     "RegionalBucketTypeDef",
     "ListStorageLensConfigurationEntryTypeDef",
     "ListStorageLensConfigurationsRequestRequestTypeDef",
+    "ReplicationTimeValueOutputTypeDef",
     "ReplicationTimeValueTypeDef",
     "ProposedMultiRegionAccessPointPolicyTypeDef",
     "MultiRegionAccessPointRegionalResponseTypeDef",
     "RegionReportTypeDef",
-    "PaginatorConfigTypeDef",
+    "MultiRegionAccessPointRouteTypeDef",
+    "SelectionCriteriaOutputTypeDef",
     "SelectionCriteriaTypeDef",
     "PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointPolicyRequestRequestTypeDef",
     "PutBucketPolicyRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
+    "StorageLensTagTypeDef",
+    "ReplicaModificationsOutputTypeDef",
     "ReplicaModificationsTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3ObjectOwnerOutputTypeDef",
     "S3ObjectOwnerTypeDef",
+    "S3ObjectMetadataOutputTypeDef",
     "S3ObjectMetadataTypeDef",
+    "S3GranteeOutputTypeDef",
     "S3GranteeTypeDef",
+    "S3ObjectLockLegalHoldOutputTypeDef",
     "S3ObjectLockLegalHoldTypeDef",
+    "S3RetentionOutputTypeDef",
     "S3RetentionTypeDef",
+    "SSEKMSOutputTypeDef",
     "SSEKMSTypeDef",
+    "SseKmsEncryptedObjectsOutputTypeDef",
     "SseKmsEncryptedObjectsTypeDef",
+    "StorageLensAwsOrgOutputTypeDef",
     "StorageLensAwsOrgTypeDef",
     "UpdateJobPriorityRequestRequestTypeDef",
-    "UpdateJobPriorityResultTypeDef",
     "UpdateJobStatusRequestRequestTypeDef",
-    "UpdateJobStatusResultTypeDef",
     "AccessPointTypeDef",
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    "ObjectLambdaContentTransformationOutputTypeDef",
     "ObjectLambdaContentTransformationTypeDef",
-    "CreateAccessPointForObjectLambdaResultTypeDef",
     "ObjectLambdaAccessPointTypeDef",
-    "CreateAccessPointRequestRequestTypeDef",
-    "GetAccessPointForObjectLambdaResultTypeDef",
-    "GetAccessPointResultTypeDef",
-    "GetPublicAccessBlockOutputTypeDef",
+    "CreateAccessPointForObjectLambdaResultTypeDef",
+    "CreateAccessPointResultTypeDef",
+    "CreateBucketResultTypeDef",
+    "CreateJobResultTypeDef",
+    "CreateMultiRegionAccessPointResultTypeDef",
+    "DeleteMultiRegionAccessPointResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    "GetAccessPointPolicyResultTypeDef",
+    "GetBucketPolicyResultTypeDef",
+    "GetBucketResultTypeDef",
+    "GetBucketVersioningResultTypeDef",
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    "UpdateJobPriorityResultTypeDef",
+    "UpdateJobStatusResultTypeDef",
     "PutPublicAccessBlockRequestRequestTypeDef",
+    "CreateAccessPointRequestRequestTypeDef",
     "CreateBucketRequestRequestTypeDef",
-    "GetBucketTaggingResultTypeDef",
-    "GetJobTaggingResultTypeDef",
     "LifecycleRuleAndOperatorTypeDef",
     "PutJobTaggingRequestRequestTypeDef",
     "ReplicationRuleAndOperatorTypeDef",
     "S3SetObjectTaggingOperationTypeDef",
     "TaggingTypeDef",
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    "GetAccessPointResultTypeDef",
+    "GetPublicAccessBlockOutputTypeDef",
+    "CreateMultiRegionAccessPointInputOutputTypeDef",
     "CreateMultiRegionAccessPointInputTypeDef",
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    "GeneratedManifestEncryptionOutputTypeDef",
     "GeneratedManifestEncryptionTypeDef",
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     "GetAccessPointPolicyStatusResultTypeDef",
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
+    "GetBucketTaggingResultTypeDef",
+    "GetJobTaggingResultTypeDef",
+    "LifecycleRuleAndOperatorOutputTypeDef",
+    "ReplicationRuleAndOperatorOutputTypeDef",
+    "S3SetObjectTaggingOperationOutputTypeDef",
     "GetMultiRegionAccessPointRoutesResultTypeDef",
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
     "GetStorageLensConfigurationTaggingResultTypeDef",
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
     "S3GeneratedManifestDescriptorTypeDef",
+    "JobManifestOutputTypeDef",
     "JobManifestTypeDef",
     "JobProgressSummaryTypeDef",
+    "ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
     "ListRegionalBucketsResultTypeDef",
     "ListStorageLensConfigurationsResultTypeDef",
+    "MetricsOutputTypeDef",
+    "ReplicationTimeOutputTypeDef",
     "MetricsTypeDef",
     "ReplicationTimeTypeDef",
     "MultiRegionAccessPointPolicyDocumentTypeDef",
     "MultiRegionAccessPointsAsyncResponseTypeDef",
     "MultiRegionAccessPointReportTypeDef",
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+    "PrefixLevelStorageMetricsOutputTypeDef",
     "PrefixLevelStorageMetricsTypeDef",
     "PutBucketVersioningRequestRequestTypeDef",
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    "S3GrantOutputTypeDef",
     "S3GrantTypeDef",
+    "S3SetObjectLegalHoldOperationOutputTypeDef",
     "S3SetObjectLegalHoldOperationTypeDef",
+    "S3SetObjectRetentionOperationOutputTypeDef",
     "S3SetObjectRetentionOperationTypeDef",
+    "StorageLensDataExportEncryptionOutputTypeDef",
     "StorageLensDataExportEncryptionTypeDef",
+    "SourceSelectionCriteriaOutputTypeDef",
     "SourceSelectionCriteriaTypeDef",
     "ListAccessPointsResultTypeDef",
+    "ObjectLambdaTransformationConfigurationOutputTypeDef",
     "ObjectLambdaTransformationConfigurationTypeDef",
     "ListAccessPointsForObjectLambdaResultTypeDef",
     "LifecycleRuleFilterTypeDef",
     "ReplicationRuleFilterTypeDef",
     "PutBucketTaggingRequestRequestTypeDef",
     "AsyncRequestParametersTypeDef",
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
+    "S3ManifestOutputLocationOutputTypeDef",
     "S3ManifestOutputLocationTypeDef",
+    "LifecycleRuleFilterOutputTypeDef",
+    "ReplicationRuleFilterOutputTypeDef",
     "JobListDescriptorTypeDef",
+    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     "AsyncResponseDetailsTypeDef",
     "GetMultiRegionAccessPointResultTypeDef",
     "ListMultiRegionAccessPointsResultTypeDef",
+    "PrefixLevelOutputTypeDef",
     "PrefixLevelTypeDef",
+    "S3AccessControlListOutputTypeDef",
+    "S3CopyObjectOperationOutputTypeDef",
     "S3AccessControlListTypeDef",
     "S3CopyObjectOperationTypeDef",
+    "S3BucketDestinationOutputTypeDef",
     "S3BucketDestinationTypeDef",
+    "ObjectLambdaConfigurationOutputTypeDef",
     "ObjectLambdaConfigurationTypeDef",
     "LifecycleRuleTypeDef",
+    "S3JobManifestGeneratorOutputTypeDef",
     "S3JobManifestGeneratorTypeDef",
+    "LifecycleRuleOutputTypeDef",
     "ListJobsResultTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "AsyncOperationTypeDef",
+    "BucketLevelOutputTypeDef",
     "BucketLevelTypeDef",
+    "S3AccessControlPolicyOutputTypeDef",
     "S3AccessControlPolicyTypeDef",
+    "StorageLensDataExportOutputTypeDef",
     "StorageLensDataExportTypeDef",
-    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
-    "GetBucketLifecycleConfigurationResultTypeDef",
     "LifecycleConfigurationTypeDef",
+    "JobManifestGeneratorOutputTypeDef",
     "JobManifestGeneratorTypeDef",
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
+    "AccountLevelOutputTypeDef",
     "AccountLevelTypeDef",
+    "S3SetObjectAclOperationOutputTypeDef",
     "S3SetObjectAclOperationTypeDef",
     "PutBucketLifecycleConfigurationRequestRequestTypeDef",
     "GetBucketReplicationResultTypeDef",
     "PutBucketReplicationRequestRequestTypeDef",
+    "StorageLensConfigurationOutputTypeDef",
     "StorageLensConfigurationTypeDef",
+    "JobOperationOutputTypeDef",
     "JobOperationTypeDef",
     "GetStorageLensConfigurationResultTypeDef",
     "PutStorageLensConfigurationRequestRequestTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobDescriptorTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "DescribeJobResultTypeDef",
 )
 
+AbortIncompleteMultipartUploadOutputTypeDef = TypedDict(
+    "AbortIncompleteMultipartUploadOutputTypeDef",
+    {
+        "DaysAfterInitiation": int,
+    },
+    total=False,
+)
+
 AbortIncompleteMultipartUploadTypeDef = TypedDict(
     "AbortIncompleteMultipartUploadTypeDef",
     {
         "DaysAfterInitiation": int,
     },
     total=False,
 )
 
+AccessControlTranslationOutputTypeDef = TypedDict(
+    "AccessControlTranslationOutputTypeDef",
+    {
+        "Owner": Literal["Destination"],
+    },
+)
+
 AccessControlTranslationTypeDef = TypedDict(
     "AccessControlTranslationTypeDef",
     {
         "Owner": Literal["Destination"],
     },
 )
 
-VpcConfigurationTypeDef = TypedDict(
-    "VpcConfigurationTypeDef",
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
     {
         "VpcId": str,
     },
 )
 
+ActivityMetricsOutputTypeDef = TypedDict(
+    "ActivityMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+AdvancedCostOptimizationMetricsOutputTypeDef = TypedDict(
+    "AdvancedCostOptimizationMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+AdvancedDataProtectionMetricsOutputTypeDef = TypedDict(
+    "AdvancedDataProtectionMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
+DetailedStatusCodesMetricsOutputTypeDef = TypedDict(
+    "DetailedStatusCodesMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+    total=False,
+)
+
 ActivityMetricsTypeDef = TypedDict(
     "ActivityMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
     total=False,
 )
@@ -344,29 +471,48 @@
         "Message": str,
         "Resource": str,
         "RequestId": str,
     },
     total=False,
 )
 
-DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointInputTypeDef",
+DeleteMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputOutputTypeDef",
     {
         "Name": str,
     },
 )
 
-PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyInputTypeDef",
+PutMultiRegionAccessPointPolicyInputOutputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputOutputTypeDef",
     {
         "Name": str,
         "Policy": str,
     },
 )
 
+_RequiredAwsLambdaTransformationOutputTypeDef = TypedDict(
+    "_RequiredAwsLambdaTransformationOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+)
+_OptionalAwsLambdaTransformationOutputTypeDef = TypedDict(
+    "_OptionalAwsLambdaTransformationOutputTypeDef",
+    {
+        "FunctionPayload": str,
+    },
+    total=False,
+)
+
+class AwsLambdaTransformationOutputTypeDef(
+    _RequiredAwsLambdaTransformationOutputTypeDef, _OptionalAwsLambdaTransformationOutputTypeDef
+):
+    pass
+
 _RequiredAwsLambdaTransformationTypeDef = TypedDict(
     "_RequiredAwsLambdaTransformationTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalAwsLambdaTransformationTypeDef = TypedDict(
@@ -378,14 +524,21 @@
 )
 
 class AwsLambdaTransformationTypeDef(
     _RequiredAwsLambdaTransformationTypeDef, _OptionalAwsLambdaTransformationTypeDef
 ):
     pass
 
+CloudWatchMetricsOutputTypeDef = TypedDict(
+    "CloudWatchMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+    },
+)
+
 CloudWatchMetricsTypeDef = TypedDict(
     "CloudWatchMetricsTypeDef",
     {
         "IsEnabled": bool,
     },
 )
 
@@ -394,51 +547,51 @@
     {
         "Value": str,
         "Status": ObjectLambdaAccessPointAliasStatusType,
     },
     total=False,
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
 PublicAccessBlockConfigurationTypeDef = TypedDict(
     "PublicAccessBlockConfigurationTypeDef",
     {
         "BlockPublicAcls": bool,
         "IgnorePublicAcls": bool,
         "BlockPublicPolicy": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-CreateAccessPointResultTypeDef = TypedDict(
-    "CreateAccessPointResultTypeDef",
+VpcConfigurationTypeDef = TypedDict(
+    "VpcConfigurationTypeDef",
     {
-        "AccessPointArn": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VpcId": str,
     },
 )
 
 CreateBucketConfigurationTypeDef = TypedDict(
     "CreateBucketConfigurationTypeDef",
     {
         "LocationConstraint": BucketLocationConstraintType,
     },
     total=False,
 )
 
-CreateBucketResultTypeDef = TypedDict(
-    "CreateBucketResultTypeDef",
-    {
-        "Location": str,
-        "BucketArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobReportTypeDef = TypedDict(
     "_RequiredJobReportTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalJobReportTypeDef = TypedDict(
@@ -459,22 +612,42 @@
     "S3TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateJobResultTypeDef = TypedDict(
-    "CreateJobResultTypeDef",
+PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
+    "PublicAccessBlockConfigurationOutputTypeDef",
     {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BlockPublicAcls": bool,
+        "IgnorePublicAcls": bool,
+        "BlockPublicPolicy": bool,
+        "RestrictPublicBuckets": bool,
+    },
+    total=False,
+)
+
+_RequiredRegionOutputTypeDef = TypedDict(
+    "_RequiredRegionOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalRegionOutputTypeDef = TypedDict(
+    "_OptionalRegionOutputTypeDef",
+    {
+        "BucketAccountId": str,
     },
+    total=False,
 )
 
+class RegionOutputTypeDef(_RequiredRegionOutputTypeDef, _OptionalRegionOutputTypeDef):
+    pass
+
 _RequiredRegionTypeDef = TypedDict(
     "_RequiredRegionTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalRegionTypeDef = TypedDict(
@@ -484,22 +657,14 @@
     },
     total=False,
 )
 
 class RegionTypeDef(_RequiredRegionTypeDef, _OptionalRegionTypeDef):
     pass
 
-CreateMultiRegionAccessPointResultTypeDef = TypedDict(
-    "CreateMultiRegionAccessPointResultTypeDef",
-    {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
     "DeleteAccessPointForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -572,26 +737,32 @@
     "DeleteJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
 
+DeleteMarkerReplicationOutputTypeDef = TypedDict(
+    "DeleteMarkerReplicationOutputTypeDef",
+    {
+        "Status": DeleteMarkerReplicationStatusType,
+    },
+)
+
 DeleteMarkerReplicationTypeDef = TypedDict(
     "DeleteMarkerReplicationTypeDef",
     {
         "Status": DeleteMarkerReplicationStatusType,
     },
 )
 
-DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointResultTypeDef",
+DeleteMultiRegionAccessPointInputTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointInputTypeDef",
     {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
     },
 )
 
 DeletePublicAccessBlockRequestRequestTypeDef = TypedDict(
     "DeletePublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -626,53 +797,77 @@
     "DescribeMultiRegionAccessPointOperationRequestRequestTypeDef",
     {
         "AccountId": str,
         "RequestTokenARN": str,
     },
 )
 
-EncryptionConfigurationTypeDef = TypedDict(
-    "EncryptionConfigurationTypeDef",
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
     {
         "ReplicaKmsKeyID": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EncryptionConfigurationTypeDef = TypedDict(
+    "EncryptionConfigurationTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicaKmsKeyID": str,
     },
+    total=False,
 )
 
 EstablishedMultiRegionAccessPointPolicyTypeDef = TypedDict(
     "EstablishedMultiRegionAccessPointPolicyTypeDef",
     {
         "Policy": str,
     },
     total=False,
 )
 
-ExcludeTypeDef = TypedDict(
-    "ExcludeTypeDef",
+ExcludeOutputTypeDef = TypedDict(
+    "ExcludeOutputTypeDef",
     {
         "Buckets": List[str],
         "Regions": List[str],
     },
     total=False,
 )
 
+ExcludeTypeDef = TypedDict(
+    "ExcludeTypeDef",
+    {
+        "Buckets": Sequence[str],
+        "Regions": Sequence[str],
+    },
+    total=False,
+)
+
+ExistingObjectReplicationOutputTypeDef = TypedDict(
+    "ExistingObjectReplicationOutputTypeDef",
+    {
+        "Status": ExistingObjectReplicationStatusType,
+    },
+)
+
 ExistingObjectReplicationTypeDef = TypedDict(
     "ExistingObjectReplicationTypeDef",
     {
         "Status": ExistingObjectReplicationStatusType,
     },
 )
 
+SSEKMSEncryptionOutputTypeDef = TypedDict(
+    "SSEKMSEncryptionOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSEncryptionTypeDef = TypedDict(
     "SSEKMSEncryptionTypeDef",
     {
         "KeyId": str,
     },
 )
 
@@ -696,38 +891,22 @@
     "GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
-GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAccessPointPolicyRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
 
-GetAccessPointPolicyResultTypeDef = TypedDict(
-    "GetAccessPointPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
     },
 )
@@ -768,22 +947,14 @@
     "GetBucketPolicyRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketPolicyResultTypeDef = TypedDict(
-    "GetBucketPolicyResultTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketReplicationRequestRequestTypeDef = TypedDict(
     "GetBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
@@ -792,49 +963,38 @@
     "GetBucketRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketResultTypeDef = TypedDict(
-    "GetBucketResultTypeDef",
+GetBucketTaggingRequestRequestTypeDef = TypedDict(
+    "GetBucketTaggingRequestRequestTypeDef",
     {
+        "AccountId": str,
         "Bucket": str,
-        "PublicAccessBlockEnabled": bool,
-        "CreationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetBucketTaggingRequestRequestTypeDef = TypedDict(
-    "GetBucketTaggingRequestRequestTypeDef",
+S3TagOutputTypeDef = TypedDict(
+    "S3TagOutputTypeDef",
     {
-        "AccountId": str,
-        "Bucket": str,
+        "Key": str,
+        "Value": str,
     },
 )
 
 GetBucketVersioningRequestRequestTypeDef = TypedDict(
     "GetBucketVersioningRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
     },
 )
 
-GetBucketVersioningResultTypeDef = TypedDict(
-    "GetBucketVersioningResultTypeDef",
-    {
-        "Status": BucketVersioningStatusType,
-        "MFADelete": MFADeleteStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobTaggingRequestRequestTypeDef = TypedDict(
     "GetJobTaggingRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
     },
 )
@@ -867,31 +1027,32 @@
     "GetMultiRegionAccessPointRoutesRequestRequestTypeDef",
     {
         "AccountId": str,
         "Mrap": str,
     },
 )
 
-_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_RequiredMultiRegionAccessPointRouteTypeDef",
+_RequiredMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteOutputTypeDef",
     {
         "TrafficDialPercentage": int,
     },
 )
-_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
-    "_OptionalMultiRegionAccessPointRouteTypeDef",
+_OptionalMultiRegionAccessPointRouteOutputTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteOutputTypeDef",
     {
         "Bucket": str,
         "Region": str,
     },
     total=False,
 )
 
-class MultiRegionAccessPointRouteTypeDef(
-    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
+class MultiRegionAccessPointRouteOutputTypeDef(
+    _RequiredMultiRegionAccessPointRouteOutputTypeDef,
+    _OptionalMultiRegionAccessPointRouteOutputTypeDef,
 ):
     pass
 
 GetPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "GetPublicAccessBlockRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -910,51 +1071,111 @@
     "GetStorageLensConfigurationTaggingRequestRequestTypeDef",
     {
         "ConfigId": str,
         "AccountId": str,
     },
 )
 
-StorageLensTagTypeDef = TypedDict(
-    "StorageLensTagTypeDef",
+StorageLensTagOutputTypeDef = TypedDict(
+    "StorageLensTagOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-IncludeTypeDef = TypedDict(
-    "IncludeTypeDef",
+IncludeOutputTypeDef = TypedDict(
+    "IncludeOutputTypeDef",
     {
         "Buckets": List[str],
         "Regions": List[str],
     },
     total=False,
 )
 
+IncludeTypeDef = TypedDict(
+    "IncludeTypeDef",
+    {
+        "Buckets": Sequence[str],
+        "Regions": Sequence[str],
+    },
+    total=False,
+)
+
 JobFailureTypeDef = TypedDict(
     "JobFailureTypeDef",
     {
         "FailureCode": str,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredJobReportOutputTypeDef = TypedDict(
+    "_RequiredJobReportOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalJobReportOutputTypeDef = TypedDict(
+    "_OptionalJobReportOutputTypeDef",
+    {
+        "Bucket": str,
+        "Format": Literal["Report_CSV_20180820"],
+        "Prefix": str,
+        "ReportScope": JobReportScopeType,
+    },
+    total=False,
+)
+
+class JobReportOutputTypeDef(_RequiredJobReportOutputTypeDef, _OptionalJobReportOutputTypeDef):
+    pass
+
+JobManifestGeneratorFilterOutputTypeDef = TypedDict(
+    "JobManifestGeneratorFilterOutputTypeDef",
+    {
+        "EligibleForReplication": bool,
+        "CreatedAfter": datetime,
+        "CreatedBefore": datetime,
+        "ObjectReplicationStatuses": List[ReplicationStatusType],
+    },
+    total=False,
+)
+
 JobManifestGeneratorFilterTypeDef = TypedDict(
     "JobManifestGeneratorFilterTypeDef",
     {
         "EligibleForReplication": bool,
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ObjectReplicationStatuses": Sequence[ReplicationStatusType],
     },
     total=False,
 )
 
+_RequiredJobManifestLocationOutputTypeDef = TypedDict(
+    "_RequiredJobManifestLocationOutputTypeDef",
+    {
+        "ObjectArn": str,
+        "ETag": str,
+    },
+)
+_OptionalJobManifestLocationOutputTypeDef = TypedDict(
+    "_OptionalJobManifestLocationOutputTypeDef",
+    {
+        "ObjectVersionId": str,
+    },
+    total=False,
+)
+
+class JobManifestLocationOutputTypeDef(
+    _RequiredJobManifestLocationOutputTypeDef, _OptionalJobManifestLocationOutputTypeDef
+):
+    pass
+
 _RequiredJobManifestLocationTypeDef = TypedDict(
     "_RequiredJobManifestLocationTypeDef",
     {
         "ObjectArn": str,
         "ETag": str,
     },
 )
@@ -967,14 +1188,33 @@
 )
 
 class JobManifestLocationTypeDef(
     _RequiredJobManifestLocationTypeDef, _OptionalJobManifestLocationTypeDef
 ):
     pass
 
+_RequiredJobManifestSpecOutputTypeDef = TypedDict(
+    "_RequiredJobManifestSpecOutputTypeDef",
+    {
+        "Format": JobManifestFormatType,
+    },
+)
+_OptionalJobManifestSpecOutputTypeDef = TypedDict(
+    "_OptionalJobManifestSpecOutputTypeDef",
+    {
+        "Fields": List[JobManifestFieldNameType],
+    },
+    total=False,
+)
+
+class JobManifestSpecOutputTypeDef(
+    _RequiredJobManifestSpecOutputTypeDef, _OptionalJobManifestSpecOutputTypeDef
+):
+    pass
+
 _RequiredJobManifestSpecTypeDef = TypedDict(
     "_RequiredJobManifestSpecTypeDef",
     {
         "Format": JobManifestFormatType,
     },
 )
 _OptionalJobManifestSpecTypeDef = TypedDict(
@@ -984,14 +1224,31 @@
     },
     total=False,
 )
 
 class JobManifestSpecTypeDef(_RequiredJobManifestSpecTypeDef, _OptionalJobManifestSpecTypeDef):
     pass
 
+LambdaInvokeOperationOutputTypeDef = TypedDict(
+    "LambdaInvokeOperationOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+    total=False,
+)
+
+S3InitiateRestoreObjectOperationOutputTypeDef = TypedDict(
+    "S3InitiateRestoreObjectOperationOutputTypeDef",
+    {
+        "ExpirationInDays": int,
+        "GlacierJobTier": S3GlacierJobTierType,
+    },
+    total=False,
+)
+
 LambdaInvokeOperationTypeDef = TypedDict(
     "LambdaInvokeOperationTypeDef",
     {
         "FunctionArn": str,
     },
     total=False,
 )
@@ -1009,24 +1266,62 @@
     "JobTimersTypeDef",
     {
         "ElapsedTimeInActiveSeconds": int,
     },
     total=False,
 )
 
+LifecycleExpirationOutputTypeDef = TypedDict(
+    "LifecycleExpirationOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "ExpiredObjectDeleteMarker": bool,
+    },
+    total=False,
+)
+
 LifecycleExpirationTypeDef = TypedDict(
     "LifecycleExpirationTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "ExpiredObjectDeleteMarker": bool,
     },
     total=False,
 )
 
+NoncurrentVersionExpirationOutputTypeDef = TypedDict(
+    "NoncurrentVersionExpirationOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "NewerNoncurrentVersions": int,
+    },
+    total=False,
+)
+
+NoncurrentVersionTransitionOutputTypeDef = TypedDict(
+    "NoncurrentVersionTransitionOutputTypeDef",
+    {
+        "NoncurrentDays": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
+TransitionOutputTypeDef = TypedDict(
+    "TransitionOutputTypeDef",
+    {
+        "Date": datetime,
+        "Days": int,
+        "StorageClass": TransitionStorageClassType,
+    },
+    total=False,
+)
+
 NoncurrentVersionExpirationTypeDef = TypedDict(
     "NoncurrentVersionExpirationTypeDef",
     {
         "NoncurrentDays": int,
         "NewerNoncurrentVersions": int,
     },
     total=False,
@@ -1040,41 +1335,31 @@
     },
     total=False,
 )
 
 TransitionTypeDef = TypedDict(
     "TransitionTypeDef",
     {
-        "Date": datetime,
+        "Date": Union[datetime, str],
         "Days": int,
         "StorageClass": TransitionStorageClassType,
     },
     total=False,
 )
 
-_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
-    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
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
 
-class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
-    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessPointsForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListAccessPointsForObjectLambdaRequestRequestTypeDef = TypedDict(
@@ -1235,14 +1520,22 @@
 
 class ListStorageLensConfigurationsRequestRequestTypeDef(
     _RequiredListStorageLensConfigurationsRequestRequestTypeDef,
     _OptionalListStorageLensConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+ReplicationTimeValueOutputTypeDef = TypedDict(
+    "ReplicationTimeValueOutputTypeDef",
+    {
+        "Minutes": int,
+    },
+    total=False,
+)
+
 ReplicationTimeValueTypeDef = TypedDict(
     "ReplicationTimeValueTypeDef",
     {
         "Minutes": int,
     },
     total=False,
 )
@@ -1270,20 +1563,40 @@
         "Bucket": str,
         "Region": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_RequiredMultiRegionAccessPointRouteTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "TrafficDialPercentage": int,
+    },
+)
+_OptionalMultiRegionAccessPointRouteTypeDef = TypedDict(
+    "_OptionalMultiRegionAccessPointRouteTypeDef",
+    {
+        "Bucket": str,
+        "Region": str,
+    },
+    total=False,
+)
+
+class MultiRegionAccessPointRouteTypeDef(
+    _RequiredMultiRegionAccessPointRouteTypeDef, _OptionalMultiRegionAccessPointRouteTypeDef
+):
+    pass
+
+SelectionCriteriaOutputTypeDef = TypedDict(
+    "SelectionCriteriaOutputTypeDef",
+    {
+        "Delimiter": str,
+        "MaxDepth": int,
+        "MinStorageBytesPercentage": float,
     },
     total=False,
 )
 
 SelectionCriteriaTypeDef = TypedDict(
     "SelectionCriteriaTypeDef",
     {
@@ -1338,49 +1651,80 @@
     {
         "MFADelete": MFADeleteType,
         "Status": BucketVersioningStatusType,
     },
     total=False,
 )
 
-PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyResultTypeDef",
+PutMultiRegionAccessPointPolicyInputTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyInputTypeDef",
     {
-        "RequestTokenARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Name": str,
+        "Policy": str,
+    },
+)
+
+StorageLensTagTypeDef = TypedDict(
+    "StorageLensTagTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+ReplicaModificationsOutputTypeDef = TypedDict(
+    "ReplicaModificationsOutputTypeDef",
+    {
+        "Status": ReplicaModificationsStatusType,
     },
 )
 
 ReplicaModificationsTypeDef = TypedDict(
     "ReplicaModificationsTypeDef",
     {
         "Status": ReplicaModificationsStatusType,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3ObjectOwnerOutputTypeDef = TypedDict(
+    "S3ObjectOwnerOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ID": str,
+        "DisplayName": str,
     },
+    total=False,
 )
 
 S3ObjectOwnerTypeDef = TypedDict(
     "S3ObjectOwnerTypeDef",
     {
         "ID": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+S3ObjectMetadataOutputTypeDef = TypedDict(
+    "S3ObjectMetadataOutputTypeDef",
+    {
+        "CacheControl": str,
+        "ContentDisposition": str,
+        "ContentEncoding": str,
+        "ContentLanguage": str,
+        "UserMetadata": Dict[str, str],
+        "ContentLength": int,
+        "ContentMD5": str,
+        "ContentType": str,
+        "HttpExpiresDate": datetime,
+        "RequesterCharged": bool,
+        "SSEAlgorithm": S3SSEAlgorithmType,
+    },
+    total=False,
+)
+
 S3ObjectMetadataTypeDef = TypedDict(
     "S3ObjectMetadataTypeDef",
     {
         "CacheControl": str,
         "ContentDisposition": str,
         "ContentEncoding": str,
         "ContentLanguage": str,
@@ -1391,54 +1735,101 @@
         "HttpExpiresDate": Union[datetime, str],
         "RequesterCharged": bool,
         "SSEAlgorithm": S3SSEAlgorithmType,
     },
     total=False,
 )
 
+S3GranteeOutputTypeDef = TypedDict(
+    "S3GranteeOutputTypeDef",
+    {
+        "TypeIdentifier": S3GranteeTypeIdentifierType,
+        "Identifier": str,
+        "DisplayName": str,
+    },
+    total=False,
+)
+
 S3GranteeTypeDef = TypedDict(
     "S3GranteeTypeDef",
     {
         "TypeIdentifier": S3GranteeTypeIdentifierType,
         "Identifier": str,
         "DisplayName": str,
     },
     total=False,
 )
 
+S3ObjectLockLegalHoldOutputTypeDef = TypedDict(
+    "S3ObjectLockLegalHoldOutputTypeDef",
+    {
+        "Status": S3ObjectLockLegalHoldStatusType,
+    },
+)
+
 S3ObjectLockLegalHoldTypeDef = TypedDict(
     "S3ObjectLockLegalHoldTypeDef",
     {
         "Status": S3ObjectLockLegalHoldStatusType,
     },
 )
 
+S3RetentionOutputTypeDef = TypedDict(
+    "S3RetentionOutputTypeDef",
+    {
+        "RetainUntilDate": datetime,
+        "Mode": S3ObjectLockRetentionModeType,
+    },
+    total=False,
+)
+
 S3RetentionTypeDef = TypedDict(
     "S3RetentionTypeDef",
     {
         "RetainUntilDate": Union[datetime, str],
         "Mode": S3ObjectLockRetentionModeType,
     },
     total=False,
 )
 
+SSEKMSOutputTypeDef = TypedDict(
+    "SSEKMSOutputTypeDef",
+    {
+        "KeyId": str,
+    },
+)
+
 SSEKMSTypeDef = TypedDict(
     "SSEKMSTypeDef",
     {
         "KeyId": str,
     },
 )
 
+SseKmsEncryptedObjectsOutputTypeDef = TypedDict(
+    "SseKmsEncryptedObjectsOutputTypeDef",
+    {
+        "Status": SseKmsEncryptedObjectsStatusType,
+    },
+)
+
 SseKmsEncryptedObjectsTypeDef = TypedDict(
     "SseKmsEncryptedObjectsTypeDef",
     {
         "Status": SseKmsEncryptedObjectsStatusType,
     },
 )
 
+StorageLensAwsOrgOutputTypeDef = TypedDict(
+    "StorageLensAwsOrgOutputTypeDef",
+    {
+        "Arn": str,
+    },
+)
+
 StorageLensAwsOrgTypeDef = TypedDict(
     "StorageLensAwsOrgTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -1447,23 +1838,14 @@
     {
         "AccountId": str,
         "JobId": str,
         "Priority": int,
     },
 )
 
-UpdateJobPriorityResultTypeDef = TypedDict(
-    "UpdateJobPriorityResultTypeDef",
-    {
-        "JobId": str,
-        "Priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateJobStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobStatusRequestRequestTypeDef",
     {
         "AccountId": str,
         "JobId": str,
         "RequestedJobStatus": RequestedJobStatusType,
     },
@@ -1477,81 +1859,52 @@
 )
 
 class UpdateJobStatusRequestRequestTypeDef(
     _RequiredUpdateJobStatusRequestRequestTypeDef, _OptionalUpdateJobStatusRequestRequestTypeDef
 ):
     pass
 
-UpdateJobStatusResultTypeDef = TypedDict(
-    "UpdateJobStatusResultTypeDef",
-    {
-        "JobId": str,
-        "Status": JobStatusType,
-        "StatusUpdateReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAccessPointTypeDef = TypedDict(
     "_RequiredAccessPointTypeDef",
     {
         "Name": str,
         "NetworkOrigin": NetworkOriginType,
         "Bucket": str,
     },
 )
 _OptionalAccessPointTypeDef = TypedDict(
     "_OptionalAccessPointTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationTypeDef,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
         "AccessPointArn": str,
         "Alias": str,
         "BucketAccountId": str,
     },
     total=False,
 )
 
 class AccessPointTypeDef(_RequiredAccessPointTypeDef, _OptionalAccessPointTypeDef):
     pass
 
-DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
-    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": DeleteMultiRegionAccessPointInputTypeDef,
-    },
-)
-
-PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
-    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+ObjectLambdaContentTransformationOutputTypeDef = TypedDict(
+    "ObjectLambdaContentTransformationOutputTypeDef",
     {
-        "AccountId": str,
-        "ClientToken": str,
-        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
+        "AwsLambda": AwsLambdaTransformationOutputTypeDef,
     },
+    total=False,
 )
 
 ObjectLambdaContentTransformationTypeDef = TypedDict(
     "ObjectLambdaContentTransformationTypeDef",
     {
         "AwsLambda": AwsLambdaTransformationTypeDef,
     },
     total=False,
 )
 
-CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaResultTypeDef",
-    {
-        "ObjectLambdaAccessPointArn": str,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredObjectLambdaAccessPointTypeDef = TypedDict(
     "_RequiredObjectLambdaAccessPointTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalObjectLambdaAccessPointTypeDef = TypedDict(
@@ -1564,81 +1917,173 @@
 )
 
 class ObjectLambdaAccessPointTypeDef(
     _RequiredObjectLambdaAccessPointTypeDef, _OptionalObjectLambdaAccessPointTypeDef
 ):
     pass
 
-_RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAccessPointRequestRequestTypeDef",
+CreateAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaResultTypeDef",
     {
-        "AccountId": str,
-        "Name": str,
-        "Bucket": str,
+        "ObjectLambdaAccessPointArn": str,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateAccessPointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAccessPointRequestRequestTypeDef",
+
+CreateAccessPointResultTypeDef = TypedDict(
+    "CreateAccessPointResultTypeDef",
     {
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "BucketAccountId": str,
+        "AccessPointArn": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateAccessPointRequestRequestTypeDef(
-    _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
-):
-    pass
+CreateBucketResultTypeDef = TypedDict(
+    "CreateBucketResultTypeDef",
+    {
+        "Location": str,
+        "BucketArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointForObjectLambdaResultTypeDef",
+CreateJobResultTypeDef = TypedDict(
+    "CreateJobResultTypeDef",
     {
-        "Name": str,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "CreationDate": datetime,
-        "Alias": ObjectLambdaAccessPointAliasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccessPointResultTypeDef = TypedDict(
-    "GetAccessPointResultTypeDef",
+CreateMultiRegionAccessPointResultTypeDef = TypedDict(
+    "CreateMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMultiRegionAccessPointResultTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointResultTypeDef",
+    {
+        "RequestTokenARN": str,
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
+GetAccessPointPolicyForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointPolicyForObjectLambdaResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointPolicyResultTypeDef = TypedDict(
+    "GetAccessPointPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketPolicyResultTypeDef = TypedDict(
+    "GetBucketPolicyResultTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBucketResultTypeDef = TypedDict(
+    "GetBucketResultTypeDef",
     {
-        "Name": str,
         "Bucket": str,
-        "NetworkOrigin": NetworkOriginType,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlockEnabled": bool,
         "CreationDate": datetime,
-        "Alias": str,
-        "AccessPointArn": str,
-        "Endpoints": Dict[str, str],
-        "BucketAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetPublicAccessBlockOutputTypeDef = TypedDict(
-    "GetPublicAccessBlockOutputTypeDef",
+GetBucketVersioningResultTypeDef = TypedDict(
+    "GetBucketVersioningResultTypeDef",
     {
-        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Status": BucketVersioningStatusType,
+        "MFADelete": MFADeleteStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyResultTypeDef",
+    {
+        "RequestTokenARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobPriorityResultTypeDef = TypedDict(
+    "UpdateJobPriorityResultTypeDef",
+    {
+        "JobId": str,
+        "Priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobStatusResultTypeDef = TypedDict(
+    "UpdateJobStatusResultTypeDef",
+    {
+        "JobId": str,
+        "Status": JobStatusType,
+        "StatusUpdateReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPublicAccessBlockRequestRequestTypeDef = TypedDict(
     "PutPublicAccessBlockRequestRequestTypeDef",
     {
         "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
         "AccountId": str,
     },
 )
 
+_RequiredCreateAccessPointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAccessPointRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "Name": str,
+        "Bucket": str,
+    },
+)
+_OptionalCreateAccessPointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAccessPointRequestRequestTypeDef",
+    {
+        "VpcConfiguration": VpcConfigurationTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationTypeDef,
+        "BucketAccountId": str,
+    },
+    total=False,
+)
+
+class CreateAccessPointRequestRequestTypeDef(
+    _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalCreateBucketRequestRequestTypeDef = TypedDict(
@@ -1658,35 +2103,19 @@
 )
 
 class CreateBucketRequestRequestTypeDef(
     _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
 ):
     pass
 
-GetBucketTaggingResultTypeDef = TypedDict(
-    "GetBucketTaggingResultTypeDef",
-    {
-        "TagSet": List[S3TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetJobTaggingResultTypeDef = TypedDict(
-    "GetJobTaggingResultTypeDef",
-    {
-        "Tags": List[S3TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleRuleAndOperatorTypeDef = TypedDict(
     "LifecycleRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[S3TagTypeDef],
+        "Tags": Sequence[S3TagTypeDef],
         "ObjectSizeGreaterThan": int,
         "ObjectSizeLessThan": int,
     },
     total=False,
 )
 
 PutJobTaggingRequestRequestTypeDef = TypedDict(
@@ -1698,15 +2127,15 @@
     },
 )
 
 ReplicationRuleAndOperatorTypeDef = TypedDict(
     "ReplicationRuleAndOperatorTypeDef",
     {
         "Prefix": str,
-        "Tags": List[S3TagTypeDef],
+        "Tags": Sequence[S3TagTypeDef],
     },
     total=False,
 )
 
 S3SetObjectTaggingOperationTypeDef = TypedDict(
     "S3SetObjectTaggingOperationTypeDef",
     {
@@ -1718,14 +2147,71 @@
 TaggingTypeDef = TypedDict(
     "TaggingTypeDef",
     {
         "TagSet": Sequence[S3TagTypeDef],
     },
 )
 
+GetAccessPointForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointForObjectLambdaResultTypeDef",
+    {
+        "Name": str,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "CreationDate": datetime,
+        "Alias": ObjectLambdaAccessPointAliasTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccessPointResultTypeDef = TypedDict(
+    "GetAccessPointResultTypeDef",
+    {
+        "Name": str,
+        "Bucket": str,
+        "NetworkOrigin": NetworkOriginType,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "CreationDate": datetime,
+        "Alias": str,
+        "AccessPointArn": str,
+        "Endpoints": Dict[str, str],
+        "BucketAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPublicAccessBlockOutputTypeDef = TypedDict(
+    "GetPublicAccessBlockOutputTypeDef",
+    {
+        "PublicAccessBlockConfiguration": PublicAccessBlockConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "_RequiredCreateMultiRegionAccessPointInputOutputTypeDef",
+    {
+        "Name": str,
+        "Regions": List[RegionOutputTypeDef],
+    },
+)
+_OptionalCreateMultiRegionAccessPointInputOutputTypeDef = TypedDict(
+    "_OptionalCreateMultiRegionAccessPointInputOutputTypeDef",
+    {
+        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class CreateMultiRegionAccessPointInputOutputTypeDef(
+    _RequiredCreateMultiRegionAccessPointInputOutputTypeDef,
+    _OptionalCreateMultiRegionAccessPointInputOutputTypeDef,
+):
+    pass
+
 _RequiredCreateMultiRegionAccessPointInputTypeDef = TypedDict(
     "_RequiredCreateMultiRegionAccessPointInputTypeDef",
     {
         "Name": str,
         "Regions": Sequence[RegionTypeDef],
     },
 )
@@ -1739,91 +2225,143 @@
 
 class CreateMultiRegionAccessPointInputTypeDef(
     _RequiredCreateMultiRegionAccessPointInputTypeDef,
     _OptionalCreateMultiRegionAccessPointInputTypeDef,
 ):
     pass
 
+DeleteMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
+    "DeleteMultiRegionAccessPointRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": DeleteMultiRegionAccessPointInputTypeDef,
+    },
+)
+
+GeneratedManifestEncryptionOutputTypeDef = TypedDict(
+    "GeneratedManifestEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
 GeneratedManifestEncryptionTypeDef = TypedDict(
     "GeneratedManifestEncryptionTypeDef",
     {
         "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSEncryptionTypeDef,
     },
     total=False,
 )
 
 GetAccessPointPolicyStatusForObjectLambdaResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusForObjectLambdaResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetAccessPointPolicyStatusResultTypeDef",
     {
         "PolicyStatus": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMultiRegionAccessPointPolicyStatusResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyStatusResultTypeDef",
     {
         "Established": PolicyStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
-    "GetMultiRegionAccessPointRoutesResultTypeDef",
+GetBucketTaggingResultTypeDef = TypedDict(
+    "GetBucketTaggingResultTypeDef",
     {
-        "Mrap": str,
-        "Routes": List[MultiRegionAccessPointRouteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagSet": List[S3TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
-    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+GetJobTaggingResultTypeDef = TypedDict(
+    "GetJobTaggingResultTypeDef",
     {
-        "AccountId": str,
-        "Mrap": str,
-        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
+        "Tags": List[S3TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
-    "GetStorageLensConfigurationTaggingResultTypeDef",
+LifecycleRuleAndOperatorOutputTypeDef = TypedDict(
+    "LifecycleRuleAndOperatorOutputTypeDef",
     {
-        "Tags": List[StorageLensTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Prefix": str,
+        "Tags": List[S3TagOutputTypeDef],
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
     },
+    total=False,
 )
 
-PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
-    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+ReplicationRuleAndOperatorOutputTypeDef = TypedDict(
+    "ReplicationRuleAndOperatorOutputTypeDef",
     {
-        "ConfigId": str,
-        "AccountId": str,
-        "Tags": Sequence[StorageLensTagTypeDef],
+        "Prefix": str,
+        "Tags": List[S3TagOutputTypeDef],
+    },
+    total=False,
+)
+
+S3SetObjectTaggingOperationOutputTypeDef = TypedDict(
+    "S3SetObjectTaggingOperationOutputTypeDef",
+    {
+        "TagSet": List[S3TagOutputTypeDef],
+    },
+    total=False,
+)
+
+GetMultiRegionAccessPointRoutesResultTypeDef = TypedDict(
+    "GetMultiRegionAccessPointRoutesResultTypeDef",
+    {
+        "Mrap": str,
+        "Routes": List[MultiRegionAccessPointRouteOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStorageLensConfigurationTaggingResultTypeDef = TypedDict(
+    "GetStorageLensConfigurationTaggingResultTypeDef",
+    {
+        "Tags": List[StorageLensTagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3GeneratedManifestDescriptorTypeDef = TypedDict(
     "S3GeneratedManifestDescriptorTypeDef",
     {
         "Format": Literal["S3InventoryReport_CSV_20211130"],
-        "Location": JobManifestLocationTypeDef,
+        "Location": JobManifestLocationOutputTypeDef,
     },
     total=False,
 )
 
+JobManifestOutputTypeDef = TypedDict(
+    "JobManifestOutputTypeDef",
+    {
+        "Spec": JobManifestSpecOutputTypeDef,
+        "Location": JobManifestLocationOutputTypeDef,
+    },
+)
+
 JobManifestTypeDef = TypedDict(
     "JobManifestTypeDef",
     {
         "Spec": JobManifestSpecTypeDef,
         "Location": JobManifestLocationTypeDef,
     },
 )
@@ -1835,29 +2373,74 @@
         "NumberOfTasksSucceeded": int,
         "NumberOfTasksFailed": int,
         "Timers": JobTimersTypeDef,
     },
     total=False,
 )
 
+_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef = TypedDict(
+    "_OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef(
+    _RequiredListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    _OptionalListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+):
+    pass
+
 ListRegionalBucketsResultTypeDef = TypedDict(
     "ListRegionalBucketsResultTypeDef",
     {
         "RegionalBucketList": List[RegionalBucketTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStorageLensConfigurationsResultTypeDef = TypedDict(
     "ListStorageLensConfigurationsResultTypeDef",
     {
         "NextToken": str,
         "StorageLensConfigurationList": List[ListStorageLensConfigurationEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMetricsOutputTypeDef = TypedDict(
+    "_RequiredMetricsOutputTypeDef",
+    {
+        "Status": MetricsStatusType,
+    },
+)
+_OptionalMetricsOutputTypeDef = TypedDict(
+    "_OptionalMetricsOutputTypeDef",
+    {
+        "EventThreshold": ReplicationTimeValueOutputTypeDef,
+    },
+    total=False,
+)
+
+class MetricsOutputTypeDef(_RequiredMetricsOutputTypeDef, _OptionalMetricsOutputTypeDef):
+    pass
+
+ReplicationTimeOutputTypeDef = TypedDict(
+    "ReplicationTimeOutputTypeDef",
+    {
+        "Status": ReplicationTimeStatusType,
+        "Time": ReplicationTimeValueOutputTypeDef,
     },
 )
 
 _RequiredMetricsTypeDef = TypedDict(
     "_RequiredMetricsTypeDef",
     {
         "Status": MetricsStatusType,
@@ -1901,21 +2484,39 @@
 
 MultiRegionAccessPointReportTypeDef = TypedDict(
     "MultiRegionAccessPointReportTypeDef",
     {
         "Name": str,
         "Alias": str,
         "CreatedAt": datetime,
-        "PublicAccessBlock": PublicAccessBlockConfigurationTypeDef,
+        "PublicAccessBlock": PublicAccessBlockConfigurationOutputTypeDef,
         "Status": MultiRegionAccessPointStatusType,
         "Regions": List[RegionReportTypeDef],
     },
     total=False,
 )
 
+SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef = TypedDict(
+    "SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "Mrap": str,
+        "RouteUpdates": Sequence[MultiRegionAccessPointRouteTypeDef],
+    },
+)
+
+PrefixLevelStorageMetricsOutputTypeDef = TypedDict(
+    "PrefixLevelStorageMetricsOutputTypeDef",
+    {
+        "IsEnabled": bool,
+        "SelectionCriteria": SelectionCriteriaOutputTypeDef,
+    },
+    total=False,
+)
+
 PrefixLevelStorageMetricsTypeDef = TypedDict(
     "PrefixLevelStorageMetricsTypeDef",
     {
         "IsEnabled": bool,
         "SelectionCriteria": SelectionCriteriaTypeDef,
     },
     total=False,
@@ -1939,30 +2540,84 @@
 
 class PutBucketVersioningRequestRequestTypeDef(
     _RequiredPutBucketVersioningRequestRequestTypeDef,
     _OptionalPutBucketVersioningRequestRequestTypeDef,
 ):
     pass
 
+PutMultiRegionAccessPointPolicyRequestRequestTypeDef = TypedDict(
+    "PutMultiRegionAccessPointPolicyRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "ClientToken": str,
+        "Details": PutMultiRegionAccessPointPolicyInputTypeDef,
+    },
+)
+
+PutStorageLensConfigurationTaggingRequestRequestTypeDef = TypedDict(
+    "PutStorageLensConfigurationTaggingRequestRequestTypeDef",
+    {
+        "ConfigId": str,
+        "AccountId": str,
+        "Tags": Sequence[StorageLensTagTypeDef],
+    },
+)
+
+S3GrantOutputTypeDef = TypedDict(
+    "S3GrantOutputTypeDef",
+    {
+        "Grantee": S3GranteeOutputTypeDef,
+        "Permission": S3PermissionType,
+    },
+    total=False,
+)
+
 S3GrantTypeDef = TypedDict(
     "S3GrantTypeDef",
     {
         "Grantee": S3GranteeTypeDef,
         "Permission": S3PermissionType,
     },
     total=False,
 )
 
+S3SetObjectLegalHoldOperationOutputTypeDef = TypedDict(
+    "S3SetObjectLegalHoldOperationOutputTypeDef",
+    {
+        "LegalHold": S3ObjectLockLegalHoldOutputTypeDef,
+    },
+)
+
 S3SetObjectLegalHoldOperationTypeDef = TypedDict(
     "S3SetObjectLegalHoldOperationTypeDef",
     {
         "LegalHold": S3ObjectLockLegalHoldTypeDef,
     },
 )
 
+_RequiredS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
+    "_RequiredS3SetObjectRetentionOperationOutputTypeDef",
+    {
+        "Retention": S3RetentionOutputTypeDef,
+    },
+)
+_OptionalS3SetObjectRetentionOperationOutputTypeDef = TypedDict(
+    "_OptionalS3SetObjectRetentionOperationOutputTypeDef",
+    {
+        "BypassGovernanceRetention": bool,
+    },
+    total=False,
+)
+
+class S3SetObjectRetentionOperationOutputTypeDef(
+    _RequiredS3SetObjectRetentionOperationOutputTypeDef,
+    _OptionalS3SetObjectRetentionOperationOutputTypeDef,
+):
+    pass
+
 _RequiredS3SetObjectRetentionOperationTypeDef = TypedDict(
     "_RequiredS3SetObjectRetentionOperationTypeDef",
     {
         "Retention": S3RetentionTypeDef,
     },
 )
 _OptionalS3SetObjectRetentionOperationTypeDef = TypedDict(
@@ -1974,38 +2629,64 @@
 )
 
 class S3SetObjectRetentionOperationTypeDef(
     _RequiredS3SetObjectRetentionOperationTypeDef, _OptionalS3SetObjectRetentionOperationTypeDef
 ):
     pass
 
+StorageLensDataExportEncryptionOutputTypeDef = TypedDict(
+    "StorageLensDataExportEncryptionOutputTypeDef",
+    {
+        "SSES3": Dict[str, Any],
+        "SSEKMS": SSEKMSOutputTypeDef,
+    },
+    total=False,
+)
+
 StorageLensDataExportEncryptionTypeDef = TypedDict(
     "StorageLensDataExportEncryptionTypeDef",
     {
-        "SSES3": Dict[str, Any],
+        "SSES3": Mapping[str, Any],
         "SSEKMS": SSEKMSTypeDef,
     },
     total=False,
 )
 
+SourceSelectionCriteriaOutputTypeDef = TypedDict(
+    "SourceSelectionCriteriaOutputTypeDef",
+    {
+        "SseKmsEncryptedObjects": SseKmsEncryptedObjectsOutputTypeDef,
+        "ReplicaModifications": ReplicaModificationsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceSelectionCriteriaTypeDef = TypedDict(
     "SourceSelectionCriteriaTypeDef",
     {
         "SseKmsEncryptedObjects": SseKmsEncryptedObjectsTypeDef,
         "ReplicaModifications": ReplicaModificationsTypeDef,
     },
     total=False,
 )
 
 ListAccessPointsResultTypeDef = TypedDict(
     "ListAccessPointsResultTypeDef",
     {
         "AccessPointList": List[AccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ObjectLambdaTransformationConfigurationOutputTypeDef = TypedDict(
+    "ObjectLambdaTransformationConfigurationOutputTypeDef",
+    {
+        "Actions": List[ObjectLambdaTransformationConfigurationActionType],
+        "ContentTransformation": ObjectLambdaContentTransformationOutputTypeDef,
     },
 )
 
 ObjectLambdaTransformationConfigurationTypeDef = TypedDict(
     "ObjectLambdaTransformationConfigurationTypeDef",
     {
         "Actions": Sequence[ObjectLambdaTransformationConfigurationActionType],
@@ -2014,15 +2695,15 @@
 )
 
 ListAccessPointsForObjectLambdaResultTypeDef = TypedDict(
     "ListAccessPointsForObjectLambdaResultTypeDef",
     {
         "ObjectLambdaAccessPointList": List[ObjectLambdaAccessPointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LifecycleRuleFilterTypeDef = TypedDict(
     "LifecycleRuleFilterTypeDef",
     {
         "Prefix": str,
@@ -2052,30 +2733,52 @@
         "Tagging": TaggingTypeDef,
     },
 )
 
 AsyncRequestParametersTypeDef = TypedDict(
     "AsyncRequestParametersTypeDef",
     {
-        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputTypeDef,
-        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputTypeDef,
-        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputTypeDef,
+        "CreateMultiRegionAccessPointRequest": CreateMultiRegionAccessPointInputOutputTypeDef,
+        "DeleteMultiRegionAccessPointRequest": DeleteMultiRegionAccessPointInputOutputTypeDef,
+        "PutMultiRegionAccessPointPolicyRequest": PutMultiRegionAccessPointPolicyInputOutputTypeDef,
     },
     total=False,
 )
 
 CreateMultiRegionAccessPointRequestRequestTypeDef = TypedDict(
     "CreateMultiRegionAccessPointRequestRequestTypeDef",
     {
         "AccountId": str,
         "ClientToken": str,
         "Details": CreateMultiRegionAccessPointInputTypeDef,
     },
 )
 
+_RequiredS3ManifestOutputLocationOutputTypeDef = TypedDict(
+    "_RequiredS3ManifestOutputLocationOutputTypeDef",
+    {
+        "Bucket": str,
+        "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
+    },
+)
+_OptionalS3ManifestOutputLocationOutputTypeDef = TypedDict(
+    "_OptionalS3ManifestOutputLocationOutputTypeDef",
+    {
+        "ExpectedManifestBucketOwner": str,
+        "ManifestPrefix": str,
+        "ManifestEncryption": GeneratedManifestEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3ManifestOutputLocationOutputTypeDef(
+    _RequiredS3ManifestOutputLocationOutputTypeDef, _OptionalS3ManifestOutputLocationOutputTypeDef
+):
+    pass
+
 _RequiredS3ManifestOutputLocationTypeDef = TypedDict(
     "_RequiredS3ManifestOutputLocationTypeDef",
     {
         "Bucket": str,
         "ManifestFormat": Literal["S3InventoryReport_CSV_20211130"],
     },
 )
@@ -2090,14 +2793,36 @@
 )
 
 class S3ManifestOutputLocationTypeDef(
     _RequiredS3ManifestOutputLocationTypeDef, _OptionalS3ManifestOutputLocationTypeDef
 ):
     pass
 
+LifecycleRuleFilterOutputTypeDef = TypedDict(
+    "LifecycleRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagOutputTypeDef,
+        "And": LifecycleRuleAndOperatorOutputTypeDef,
+        "ObjectSizeGreaterThan": int,
+        "ObjectSizeLessThan": int,
+    },
+    total=False,
+)
+
+ReplicationRuleFilterOutputTypeDef = TypedDict(
+    "ReplicationRuleFilterOutputTypeDef",
+    {
+        "Prefix": str,
+        "Tag": S3TagOutputTypeDef,
+        "And": ReplicationRuleAndOperatorOutputTypeDef,
+    },
+    total=False,
+)
+
 JobListDescriptorTypeDef = TypedDict(
     "JobListDescriptorTypeDef",
     {
         "JobId": str,
         "Description": str,
         "Operation": OperationNameType,
         "Priority": int,
@@ -2105,14 +2830,38 @@
         "CreationTime": datetime,
         "TerminationDate": datetime,
         "ProgressSummary": JobProgressSummaryTypeDef,
     },
     total=False,
 )
 
+_RequiredDestinationOutputTypeDef = TypedDict(
+    "_RequiredDestinationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalDestinationOutputTypeDef = TypedDict(
+    "_OptionalDestinationOutputTypeDef",
+    {
+        "Account": str,
+        "ReplicationTime": ReplicationTimeOutputTypeDef,
+        "AccessControlTranslation": AccessControlTranslationOutputTypeDef,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "Metrics": MetricsOutputTypeDef,
+        "StorageClass": ReplicationStorageClassType,
+    },
+    total=False,
+)
+
+class DestinationOutputTypeDef(
+    _RequiredDestinationOutputTypeDef, _OptionalDestinationOutputTypeDef
+):
+    pass
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalDestinationTypeDef = TypedDict(
@@ -2131,15 +2880,15 @@
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 GetMultiRegionAccessPointPolicyResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointPolicyResultTypeDef",
     {
         "Policy": MultiRegionAccessPointPolicyDocumentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AsyncResponseDetailsTypeDef = TypedDict(
     "AsyncResponseDetailsTypeDef",
     {
         "MultiRegionAccessPointDetails": MultiRegionAccessPointsAsyncResponseTypeDef,
@@ -2148,34 +2897,85 @@
     total=False,
 )
 
 GetMultiRegionAccessPointResultTypeDef = TypedDict(
     "GetMultiRegionAccessPointResultTypeDef",
     {
         "AccessPoint": MultiRegionAccessPointReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMultiRegionAccessPointsResultTypeDef = TypedDict(
     "ListMultiRegionAccessPointsResultTypeDef",
     {
         "AccessPoints": List[MultiRegionAccessPointReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PrefixLevelOutputTypeDef = TypedDict(
+    "PrefixLevelOutputTypeDef",
+    {
+        "StorageMetrics": PrefixLevelStorageMetricsOutputTypeDef,
     },
 )
 
 PrefixLevelTypeDef = TypedDict(
     "PrefixLevelTypeDef",
     {
         "StorageMetrics": PrefixLevelStorageMetricsTypeDef,
     },
 )
 
+_RequiredS3AccessControlListOutputTypeDef = TypedDict(
+    "_RequiredS3AccessControlListOutputTypeDef",
+    {
+        "Owner": S3ObjectOwnerOutputTypeDef,
+    },
+)
+_OptionalS3AccessControlListOutputTypeDef = TypedDict(
+    "_OptionalS3AccessControlListOutputTypeDef",
+    {
+        "Grants": List[S3GrantOutputTypeDef],
+    },
+    total=False,
+)
+
+class S3AccessControlListOutputTypeDef(
+    _RequiredS3AccessControlListOutputTypeDef, _OptionalS3AccessControlListOutputTypeDef
+):
+    pass
+
+S3CopyObjectOperationOutputTypeDef = TypedDict(
+    "S3CopyObjectOperationOutputTypeDef",
+    {
+        "TargetResource": str,
+        "CannedAccessControlList": S3CannedAccessControlListType,
+        "AccessControlGrants": List[S3GrantOutputTypeDef],
+        "MetadataDirective": S3MetadataDirectiveType,
+        "ModifiedSinceConstraint": datetime,
+        "NewObjectMetadata": S3ObjectMetadataOutputTypeDef,
+        "NewObjectTagging": List[S3TagOutputTypeDef],
+        "RedirectLocation": str,
+        "RequesterPays": bool,
+        "StorageClass": S3StorageClassType,
+        "UnModifiedSinceConstraint": datetime,
+        "SSEAwsKmsKeyId": str,
+        "TargetKeyPrefix": str,
+        "ObjectLockLegalHoldStatus": S3ObjectLockLegalHoldStatusType,
+        "ObjectLockMode": S3ObjectLockModeType,
+        "ObjectLockRetainUntilDate": datetime,
+        "BucketKeyEnabled": bool,
+        "ChecksumAlgorithm": S3ChecksumAlgorithmType,
+    },
+    total=False,
+)
+
 _RequiredS3AccessControlListTypeDef = TypedDict(
     "_RequiredS3AccessControlListTypeDef",
     {
         "Owner": S3ObjectOwnerTypeDef,
     },
 )
 _OptionalS3AccessControlListTypeDef = TypedDict(
@@ -2212,14 +3012,37 @@
         "ObjectLockRetainUntilDate": Union[datetime, str],
         "BucketKeyEnabled": bool,
         "ChecksumAlgorithm": S3ChecksumAlgorithmType,
     },
     total=False,
 )
 
+_RequiredS3BucketDestinationOutputTypeDef = TypedDict(
+    "_RequiredS3BucketDestinationOutputTypeDef",
+    {
+        "Format": FormatType,
+        "OutputSchemaVersion": Literal["V_1"],
+        "AccountId": str,
+        "Arn": str,
+    },
+)
+_OptionalS3BucketDestinationOutputTypeDef = TypedDict(
+    "_OptionalS3BucketDestinationOutputTypeDef",
+    {
+        "Prefix": str,
+        "Encryption": StorageLensDataExportEncryptionOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3BucketDestinationOutputTypeDef(
+    _RequiredS3BucketDestinationOutputTypeDef, _OptionalS3BucketDestinationOutputTypeDef
+):
+    pass
+
 _RequiredS3BucketDestinationTypeDef = TypedDict(
     "_RequiredS3BucketDestinationTypeDef",
     {
         "Format": FormatType,
         "OutputSchemaVersion": Literal["V_1"],
         "AccountId": str,
         "Arn": str,
@@ -2235,14 +3058,35 @@
 )
 
 class S3BucketDestinationTypeDef(
     _RequiredS3BucketDestinationTypeDef, _OptionalS3BucketDestinationTypeDef
 ):
     pass
 
+_RequiredObjectLambdaConfigurationOutputTypeDef = TypedDict(
+    "_RequiredObjectLambdaConfigurationOutputTypeDef",
+    {
+        "SupportingAccessPoint": str,
+        "TransformationConfigurations": List[ObjectLambdaTransformationConfigurationOutputTypeDef],
+    },
+)
+_OptionalObjectLambdaConfigurationOutputTypeDef = TypedDict(
+    "_OptionalObjectLambdaConfigurationOutputTypeDef",
+    {
+        "CloudWatchMetricsEnabled": bool,
+        "AllowedFeatures": List[ObjectLambdaAllowedFeatureType],
+    },
+    total=False,
+)
+
+class ObjectLambdaConfigurationOutputTypeDef(
+    _RequiredObjectLambdaConfigurationOutputTypeDef, _OptionalObjectLambdaConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredObjectLambdaConfigurationTypeDef = TypedDict(
     "_RequiredObjectLambdaConfigurationTypeDef",
     {
         "SupportingAccessPoint": str,
         "TransformationConfigurations": Sequence[ObjectLambdaTransformationConfigurationTypeDef],
     },
 )
@@ -2268,25 +3112,47 @@
 )
 _OptionalLifecycleRuleTypeDef = TypedDict(
     "_OptionalLifecycleRuleTypeDef",
     {
         "Expiration": LifecycleExpirationTypeDef,
         "ID": str,
         "Filter": LifecycleRuleFilterTypeDef,
-        "Transitions": List[TransitionTypeDef],
-        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionTypeDef],
+        "Transitions": Sequence[TransitionTypeDef],
+        "NoncurrentVersionTransitions": Sequence[NoncurrentVersionTransitionTypeDef],
         "NoncurrentVersionExpiration": NoncurrentVersionExpirationTypeDef,
         "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadTypeDef,
     },
     total=False,
 )
 
 class LifecycleRuleTypeDef(_RequiredLifecycleRuleTypeDef, _OptionalLifecycleRuleTypeDef):
     pass
 
+_RequiredS3JobManifestGeneratorOutputTypeDef = TypedDict(
+    "_RequiredS3JobManifestGeneratorOutputTypeDef",
+    {
+        "SourceBucket": str,
+        "EnableManifestOutput": bool,
+    },
+)
+_OptionalS3JobManifestGeneratorOutputTypeDef = TypedDict(
+    "_OptionalS3JobManifestGeneratorOutputTypeDef",
+    {
+        "ExpectedBucketOwner": str,
+        "ManifestOutputLocation": S3ManifestOutputLocationOutputTypeDef,
+        "Filter": JobManifestGeneratorFilterOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3JobManifestGeneratorOutputTypeDef(
+    _RequiredS3JobManifestGeneratorOutputTypeDef, _OptionalS3JobManifestGeneratorOutputTypeDef
+):
+    pass
+
 _RequiredS3JobManifestGeneratorTypeDef = TypedDict(
     "_RequiredS3JobManifestGeneratorTypeDef",
     {
         "SourceBucket": str,
         "EnableManifestOutput": bool,
     },
 )
@@ -2301,23 +3167,75 @@
 )
 
 class S3JobManifestGeneratorTypeDef(
     _RequiredS3JobManifestGeneratorTypeDef, _OptionalS3JobManifestGeneratorTypeDef
 ):
     pass
 
+_RequiredLifecycleRuleOutputTypeDef = TypedDict(
+    "_RequiredLifecycleRuleOutputTypeDef",
+    {
+        "Status": ExpirationStatusType,
+    },
+)
+_OptionalLifecycleRuleOutputTypeDef = TypedDict(
+    "_OptionalLifecycleRuleOutputTypeDef",
+    {
+        "Expiration": LifecycleExpirationOutputTypeDef,
+        "ID": str,
+        "Filter": LifecycleRuleFilterOutputTypeDef,
+        "Transitions": List[TransitionOutputTypeDef],
+        "NoncurrentVersionTransitions": List[NoncurrentVersionTransitionOutputTypeDef],
+        "NoncurrentVersionExpiration": NoncurrentVersionExpirationOutputTypeDef,
+        "AbortIncompleteMultipartUpload": AbortIncompleteMultipartUploadOutputTypeDef,
+    },
+    total=False,
+)
+
+class LifecycleRuleOutputTypeDef(
+    _RequiredLifecycleRuleOutputTypeDef, _OptionalLifecycleRuleOutputTypeDef
+):
+    pass
+
 ListJobsResultTypeDef = TypedDict(
     "ListJobsResultTypeDef",
     {
         "NextToken": str,
         "Jobs": List[JobListDescriptorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "Status": ReplicationRuleStatusType,
+        "Destination": DestinationOutputTypeDef,
+        "Bucket": str,
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "ID": str,
+        "Priority": int,
+        "Prefix": str,
+        "Filter": ReplicationRuleFilterOutputTypeDef,
+        "SourceSelectionCriteria": SourceSelectionCriteriaOutputTypeDef,
+        "ExistingObjectReplication": ExistingObjectReplicationOutputTypeDef,
+        "DeleteMarkerReplication": DeleteMarkerReplicationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ReplicationRuleOutputTypeDef(
+    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+):
+    pass
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
         "Status": ReplicationRuleStatusType,
         "Destination": DestinationTypeDef,
         "Bucket": str,
     },
@@ -2348,109 +3266,177 @@
         "RequestParameters": AsyncRequestParametersTypeDef,
         "RequestStatus": str,
         "ResponseDetails": AsyncResponseDetailsTypeDef,
     },
     total=False,
 )
 
+BucketLevelOutputTypeDef = TypedDict(
+    "BucketLevelOutputTypeDef",
+    {
+        "ActivityMetrics": ActivityMetricsOutputTypeDef,
+        "PrefixLevel": PrefixLevelOutputTypeDef,
+        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
+        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
+        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
 BucketLevelTypeDef = TypedDict(
     "BucketLevelTypeDef",
     {
         "ActivityMetrics": ActivityMetricsTypeDef,
         "PrefixLevel": PrefixLevelTypeDef,
         "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsTypeDef,
         "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsTypeDef,
         "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsTypeDef,
     },
     total=False,
 )
 
+S3AccessControlPolicyOutputTypeDef = TypedDict(
+    "S3AccessControlPolicyOutputTypeDef",
+    {
+        "AccessControlList": S3AccessControlListOutputTypeDef,
+        "CannedAccessControlList": S3CannedAccessControlListType,
+    },
+    total=False,
+)
+
 S3AccessControlPolicyTypeDef = TypedDict(
     "S3AccessControlPolicyTypeDef",
     {
         "AccessControlList": S3AccessControlListTypeDef,
         "CannedAccessControlList": S3CannedAccessControlListType,
     },
     total=False,
 )
 
+StorageLensDataExportOutputTypeDef = TypedDict(
+    "StorageLensDataExportOutputTypeDef",
+    {
+        "S3BucketDestination": S3BucketDestinationOutputTypeDef,
+        "CloudWatchMetrics": CloudWatchMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
 StorageLensDataExportTypeDef = TypedDict(
     "StorageLensDataExportTypeDef",
     {
         "S3BucketDestination": S3BucketDestinationTypeDef,
         "CloudWatchMetrics": CloudWatchMetricsTypeDef,
     },
     total=False,
 )
 
-CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
-    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
+GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
+    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
     {
-        "AccountId": str,
-        "Name": str,
-        "Configuration": ObjectLambdaConfigurationTypeDef,
+        "Configuration": ObjectLambdaConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccessPointConfigurationForObjectLambdaResultTypeDef = TypedDict(
-    "GetAccessPointConfigurationForObjectLambdaResultTypeDef",
+CreateAccessPointForObjectLambdaRequestRequestTypeDef = TypedDict(
+    "CreateAccessPointForObjectLambdaRequestRequestTypeDef",
     {
+        "AccountId": str,
+        "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef = TypedDict(
     "PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef",
     {
         "AccountId": str,
         "Name": str,
         "Configuration": ObjectLambdaConfigurationTypeDef,
     },
 )
 
-GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
-    "GetBucketLifecycleConfigurationResultTypeDef",
+LifecycleConfigurationTypeDef = TypedDict(
+    "LifecycleConfigurationTypeDef",
     {
-        "Rules": List[LifecycleRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": Sequence[LifecycleRuleTypeDef],
     },
+    total=False,
 )
 
-LifecycleConfigurationTypeDef = TypedDict(
-    "LifecycleConfigurationTypeDef",
+JobManifestGeneratorOutputTypeDef = TypedDict(
+    "JobManifestGeneratorOutputTypeDef",
     {
-        "Rules": Sequence[LifecycleRuleTypeDef],
+        "S3JobManifestGenerator": S3JobManifestGeneratorOutputTypeDef,
     },
     total=False,
 )
 
 JobManifestGeneratorTypeDef = TypedDict(
     "JobManifestGeneratorTypeDef",
     {
         "S3JobManifestGenerator": S3JobManifestGeneratorTypeDef,
     },
     total=False,
 )
 
+GetBucketLifecycleConfigurationResultTypeDef = TypedDict(
+    "GetBucketLifecycleConfigurationResultTypeDef",
+    {
+        "Rules": List[LifecycleRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "Role": str,
+        "Rules": List[ReplicationRuleOutputTypeDef],
+    },
+)
+
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
         "Role": str,
-        "Rules": List[ReplicationRuleTypeDef],
+        "Rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 DescribeMultiRegionAccessPointOperationResultTypeDef = TypedDict(
     "DescribeMultiRegionAccessPointOperationResultTypeDef",
     {
         "AsyncOperation": AsyncOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredAccountLevelOutputTypeDef = TypedDict(
+    "_RequiredAccountLevelOutputTypeDef",
+    {
+        "BucketLevel": BucketLevelOutputTypeDef,
     },
 )
+_OptionalAccountLevelOutputTypeDef = TypedDict(
+    "_OptionalAccountLevelOutputTypeDef",
+    {
+        "ActivityMetrics": ActivityMetricsOutputTypeDef,
+        "AdvancedCostOptimizationMetrics": AdvancedCostOptimizationMetricsOutputTypeDef,
+        "AdvancedDataProtectionMetrics": AdvancedDataProtectionMetricsOutputTypeDef,
+        "DetailedStatusCodesMetrics": DetailedStatusCodesMetricsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AccountLevelOutputTypeDef(
+    _RequiredAccountLevelOutputTypeDef, _OptionalAccountLevelOutputTypeDef
+):
+    pass
 
 _RequiredAccountLevelTypeDef = TypedDict(
     "_RequiredAccountLevelTypeDef",
     {
         "BucketLevel": BucketLevelTypeDef,
     },
 )
@@ -2464,14 +3450,22 @@
     },
     total=False,
 )
 
 class AccountLevelTypeDef(_RequiredAccountLevelTypeDef, _OptionalAccountLevelTypeDef):
     pass
 
+S3SetObjectAclOperationOutputTypeDef = TypedDict(
+    "S3SetObjectAclOperationOutputTypeDef",
+    {
+        "AccessControlPolicy": S3AccessControlPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SetObjectAclOperationTypeDef = TypedDict(
     "S3SetObjectAclOperationTypeDef",
     {
         "AccessControlPolicy": S3AccessControlPolicyTypeDef,
     },
     total=False,
 )
@@ -2496,28 +3490,53 @@
     _OptionalPutBucketLifecycleConfigurationRequestRequestTypeDef,
 ):
     pass
 
 GetBucketReplicationResultTypeDef = TypedDict(
     "GetBucketReplicationResultTypeDef",
     {
-        "ReplicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReplicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBucketReplicationRequestRequestTypeDef = TypedDict(
     "PutBucketReplicationRequestRequestTypeDef",
     {
         "AccountId": str,
         "Bucket": str,
         "ReplicationConfiguration": ReplicationConfigurationTypeDef,
     },
 )
 
+_RequiredStorageLensConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStorageLensConfigurationOutputTypeDef",
+    {
+        "Id": str,
+        "AccountLevel": AccountLevelOutputTypeDef,
+        "IsEnabled": bool,
+    },
+)
+_OptionalStorageLensConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStorageLensConfigurationOutputTypeDef",
+    {
+        "Include": IncludeOutputTypeDef,
+        "Exclude": ExcludeOutputTypeDef,
+        "DataExport": StorageLensDataExportOutputTypeDef,
+        "AwsOrg": StorageLensAwsOrgOutputTypeDef,
+        "StorageLensArn": str,
+    },
+    total=False,
+)
+
+class StorageLensConfigurationOutputTypeDef(
+    _RequiredStorageLensConfigurationOutputTypeDef, _OptionalStorageLensConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredStorageLensConfigurationTypeDef = TypedDict(
     "_RequiredStorageLensConfigurationTypeDef",
     {
         "Id": str,
         "AccountLevel": AccountLevelTypeDef,
         "IsEnabled": bool,
     },
@@ -2535,14 +3554,30 @@
 )
 
 class StorageLensConfigurationTypeDef(
     _RequiredStorageLensConfigurationTypeDef, _OptionalStorageLensConfigurationTypeDef
 ):
     pass
 
+JobOperationOutputTypeDef = TypedDict(
+    "JobOperationOutputTypeDef",
+    {
+        "LambdaInvoke": LambdaInvokeOperationOutputTypeDef,
+        "S3PutObjectCopy": S3CopyObjectOperationOutputTypeDef,
+        "S3PutObjectAcl": S3SetObjectAclOperationOutputTypeDef,
+        "S3PutObjectTagging": S3SetObjectTaggingOperationOutputTypeDef,
+        "S3DeleteObjectTagging": Dict[str, Any],
+        "S3InitiateRestoreObject": S3InitiateRestoreObjectOperationOutputTypeDef,
+        "S3PutObjectLegalHold": S3SetObjectLegalHoldOperationOutputTypeDef,
+        "S3PutObjectRetention": S3SetObjectRetentionOperationOutputTypeDef,
+        "S3ReplicateObject": Dict[str, Any],
+    },
+    total=False,
+)
+
 JobOperationTypeDef = TypedDict(
     "JobOperationTypeDef",
     {
         "LambdaInvoke": LambdaInvokeOperationTypeDef,
         "S3PutObjectCopy": S3CopyObjectOperationTypeDef,
         "S3PutObjectAcl": S3SetObjectAclOperationTypeDef,
         "S3PutObjectTagging": S3SetObjectTaggingOperationTypeDef,
@@ -2554,16 +3589,16 @@
     },
     total=False,
 )
 
 GetStorageLensConfigurationResultTypeDef = TypedDict(
     "GetStorageLensConfigurationResultTypeDef",
     {
-        "StorageLensConfiguration": StorageLensConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StorageLensConfiguration": StorageLensConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutStorageLensConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutStorageLensConfigurationRequestRequestTypeDef",
     {
         "ConfigId": str,
@@ -2581,14 +3616,40 @@
 
 class PutStorageLensConfigurationRequestRequestTypeDef(
     _RequiredPutStorageLensConfigurationRequestRequestTypeDef,
     _OptionalPutStorageLensConfigurationRequestRequestTypeDef,
 ):
     pass
 
+JobDescriptorTypeDef = TypedDict(
+    "JobDescriptorTypeDef",
+    {
+        "JobId": str,
+        "ConfirmationRequired": bool,
+        "Description": str,
+        "JobArn": str,
+        "Status": JobStatusType,
+        "Manifest": JobManifestOutputTypeDef,
+        "Operation": JobOperationOutputTypeDef,
+        "Priority": int,
+        "ProgressSummary": JobProgressSummaryTypeDef,
+        "StatusUpdateReason": str,
+        "FailureReasons": List[JobFailureTypeDef],
+        "Report": JobReportOutputTypeDef,
+        "CreationTime": datetime,
+        "TerminationDate": datetime,
+        "RoleArn": str,
+        "SuspendedDate": datetime,
+        "SuspendedCause": str,
+        "ManifestGenerator": JobManifestGeneratorOutputTypeDef,
+        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "AccountId": str,
         "Operation": JobOperationTypeDef,
         "Report": JobReportTypeDef,
         "ClientRequestToken": str,
@@ -2609,40 +3670,14 @@
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-JobDescriptorTypeDef = TypedDict(
-    "JobDescriptorTypeDef",
-    {
-        "JobId": str,
-        "ConfirmationRequired": bool,
-        "Description": str,
-        "JobArn": str,
-        "Status": JobStatusType,
-        "Manifest": JobManifestTypeDef,
-        "Operation": JobOperationTypeDef,
-        "Priority": int,
-        "ProgressSummary": JobProgressSummaryTypeDef,
-        "StatusUpdateReason": str,
-        "FailureReasons": List[JobFailureTypeDef],
-        "Report": JobReportTypeDef,
-        "CreationTime": datetime,
-        "TerminationDate": datetime,
-        "RoleArn": str,
-        "SuspendedDate": datetime,
-        "SuspendedCause": str,
-        "ManifestGenerator": JobManifestGeneratorTypeDef,
-        "GeneratedManifestDescriptor": S3GeneratedManifestDescriptorTypeDef,
-    },
-    total=False,
-)
-
 DescribeJobResultTypeDef = TypedDict(
     "DescribeJobResultTypeDef",
     {
         "Job": JobDescriptorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/PKG-INFO` & `mypy-boto3-s3control-1.28.12/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-s3control
-Version: 1.28.0
-Summary: Type annotations for boto3.S3Control 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 s3control type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-s3control"></a>
 
 # mypy-boto3-s3control
 
 [![PyPI - mypy-boto3-s3control](https://img.shields.io/pypi/v/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-s3control.svg?color=blue)](https://pypi.org/project/mypy-boto3-s3control)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-s3control?color=blue)](https://pypistats.org/packages/mypy-boto3-s3control)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-s3control)](https://pepy.tech/project/mypy-boto3-s3control)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.S3Control 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
+[boto3.S3Control 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
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
 [mypy-boto3-s3control docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_s3control/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,231 +332,311 @@
 ### Typed dictionaries
 
 `mypy_boto3_s3control.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_s3control.type_defs import (
+    AbortIncompleteMultipartUploadOutputTypeDef,
     AbortIncompleteMultipartUploadTypeDef,
+    AccessControlTranslationOutputTypeDef,
     AccessControlTranslationTypeDef,
-    VpcConfigurationTypeDef,
+    VpcConfigurationOutputTypeDef,
+    ActivityMetricsOutputTypeDef,
+    AdvancedCostOptimizationMetricsOutputTypeDef,
+    AdvancedDataProtectionMetricsOutputTypeDef,
+    DetailedStatusCodesMetricsOutputTypeDef,
     ActivityMetricsTypeDef,
     AdvancedCostOptimizationMetricsTypeDef,
     AdvancedDataProtectionMetricsTypeDef,
     DetailedStatusCodesMetricsTypeDef,
     AsyncErrorDetailsTypeDef,
-    DeleteMultiRegionAccessPointInputTypeDef,
-    PutMultiRegionAccessPointPolicyInputTypeDef,
+    DeleteMultiRegionAccessPointInputOutputTypeDef,
+    PutMultiRegionAccessPointPolicyInputOutputTypeDef,
+    AwsLambdaTransformationOutputTypeDef,
     AwsLambdaTransformationTypeDef,
+    CloudWatchMetricsOutputTypeDef,
     CloudWatchMetricsTypeDef,
     ObjectLambdaAccessPointAliasTypeDef,
+    ResponseMetadataTypeDef,
     PublicAccessBlockConfigurationTypeDef,
-    CreateAccessPointResultTypeDef,
+    VpcConfigurationTypeDef,
     CreateBucketConfigurationTypeDef,
-    CreateBucketResultTypeDef,
     JobReportTypeDef,
     S3TagTypeDef,
-    CreateJobResultTypeDef,
+    PublicAccessBlockConfigurationOutputTypeDef,
+    RegionOutputTypeDef,
     RegionTypeDef,
-    CreateMultiRegionAccessPointResultTypeDef,
     DeleteAccessPointForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     DeleteAccessPointPolicyRequestRequestTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteBucketLifecycleConfigurationRequestRequestTypeDef,
     DeleteBucketPolicyRequestRequestTypeDef,
     DeleteBucketReplicationRequestRequestTypeDef,
     DeleteBucketRequestRequestTypeDef,
     DeleteBucketTaggingRequestRequestTypeDef,
     DeleteJobTaggingRequestRequestTypeDef,
+    DeleteMarkerReplicationOutputTypeDef,
     DeleteMarkerReplicationTypeDef,
-    DeleteMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointInputTypeDef,
     DeletePublicAccessBlockRequestRequestTypeDef,
     DeleteStorageLensConfigurationRequestRequestTypeDef,
     DeleteStorageLensConfigurationTaggingRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeMultiRegionAccessPointOperationRequestRequestTypeDef,
+    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EstablishedMultiRegionAccessPointPolicyTypeDef,
+    ExcludeOutputTypeDef,
     ExcludeTypeDef,
+    ExistingObjectReplicationOutputTypeDef,
     ExistingObjectReplicationTypeDef,
+    SSEKMSEncryptionOutputTypeDef,
     SSEKMSEncryptionTypeDef,
     GetAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
     GetAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
-    GetAccessPointPolicyForObjectLambdaResultTypeDef,
     GetAccessPointPolicyRequestRequestTypeDef,
-    GetAccessPointPolicyResultTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaRequestRequestTypeDef,
     PolicyStatusTypeDef,
     GetAccessPointPolicyStatusRequestRequestTypeDef,
     GetAccessPointRequestRequestTypeDef,
     GetBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketPolicyRequestRequestTypeDef,
-    GetBucketPolicyResultTypeDef,
     GetBucketReplicationRequestRequestTypeDef,
     GetBucketRequestRequestTypeDef,
-    GetBucketResultTypeDef,
     GetBucketTaggingRequestRequestTypeDef,
+    S3TagOutputTypeDef,
     GetBucketVersioningRequestRequestTypeDef,
-    GetBucketVersioningResultTypeDef,
     GetJobTaggingRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyRequestRequestTypeDef,
     GetMultiRegionAccessPointPolicyStatusRequestRequestTypeDef,
     GetMultiRegionAccessPointRequestRequestTypeDef,
     GetMultiRegionAccessPointRoutesRequestRequestTypeDef,
-    MultiRegionAccessPointRouteTypeDef,
+    MultiRegionAccessPointRouteOutputTypeDef,
     GetPublicAccessBlockRequestRequestTypeDef,
     GetStorageLensConfigurationRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingRequestRequestTypeDef,
-    StorageLensTagTypeDef,
+    StorageLensTagOutputTypeDef,
+    IncludeOutputTypeDef,
     IncludeTypeDef,
     JobFailureTypeDef,
+    JobReportOutputTypeDef,
+    JobManifestGeneratorFilterOutputTypeDef,
     JobManifestGeneratorFilterTypeDef,
+    JobManifestLocationOutputTypeDef,
     JobManifestLocationTypeDef,
+    JobManifestSpecOutputTypeDef,
     JobManifestSpecTypeDef,
+    LambdaInvokeOperationOutputTypeDef,
+    S3InitiateRestoreObjectOperationOutputTypeDef,
     LambdaInvokeOperationTypeDef,
     S3InitiateRestoreObjectOperationTypeDef,
     JobTimersTypeDef,
+    LifecycleExpirationOutputTypeDef,
     LifecycleExpirationTypeDef,
+    NoncurrentVersionExpirationOutputTypeDef,
+    NoncurrentVersionTransitionOutputTypeDef,
+    TransitionOutputTypeDef,
     NoncurrentVersionExpirationTypeDef,
     NoncurrentVersionTransitionTypeDef,
     TransitionTypeDef,
-    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessPointsForObjectLambdaRequestRequestTypeDef,
     ListAccessPointsRequestRequestTypeDef,
     ListJobsRequestRequestTypeDef,
     ListMultiRegionAccessPointsRequestRequestTypeDef,
     ListRegionalBucketsRequestRequestTypeDef,
     RegionalBucketTypeDef,
     ListStorageLensConfigurationEntryTypeDef,
     ListStorageLensConfigurationsRequestRequestTypeDef,
+    ReplicationTimeValueOutputTypeDef,
     ReplicationTimeValueTypeDef,
     ProposedMultiRegionAccessPointPolicyTypeDef,
     MultiRegionAccessPointRegionalResponseTypeDef,
     RegionReportTypeDef,
-    PaginatorConfigTypeDef,
+    MultiRegionAccessPointRouteTypeDef,
+    SelectionCriteriaOutputTypeDef,
     SelectionCriteriaTypeDef,
     PutAccessPointPolicyForObjectLambdaRequestRequestTypeDef,
     PutAccessPointPolicyRequestRequestTypeDef,
     PutBucketPolicyRequestRequestTypeDef,
     VersioningConfigurationTypeDef,
-    PutMultiRegionAccessPointPolicyResultTypeDef,
+    PutMultiRegionAccessPointPolicyInputTypeDef,
+    StorageLensTagTypeDef,
+    ReplicaModificationsOutputTypeDef,
     ReplicaModificationsTypeDef,
-    ResponseMetadataTypeDef,
+    S3ObjectOwnerOutputTypeDef,
     S3ObjectOwnerTypeDef,
+    S3ObjectMetadataOutputTypeDef,
     S3ObjectMetadataTypeDef,
+    S3GranteeOutputTypeDef,
     S3GranteeTypeDef,
+    S3ObjectLockLegalHoldOutputTypeDef,
     S3ObjectLockLegalHoldTypeDef,
+    S3RetentionOutputTypeDef,
     S3RetentionTypeDef,
+    SSEKMSOutputTypeDef,
     SSEKMSTypeDef,
+    SseKmsEncryptedObjectsOutputTypeDef,
     SseKmsEncryptedObjectsTypeDef,
+    StorageLensAwsOrgOutputTypeDef,
     StorageLensAwsOrgTypeDef,
     UpdateJobPriorityRequestRequestTypeDef,
-    UpdateJobPriorityResultTypeDef,
     UpdateJobStatusRequestRequestTypeDef,
-    UpdateJobStatusResultTypeDef,
     AccessPointTypeDef,
-    DeleteMultiRegionAccessPointRequestRequestTypeDef,
-    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    ObjectLambdaContentTransformationOutputTypeDef,
     ObjectLambdaContentTransformationTypeDef,
-    CreateAccessPointForObjectLambdaResultTypeDef,
     ObjectLambdaAccessPointTypeDef,
-    CreateAccessPointRequestRequestTypeDef,
-    GetAccessPointForObjectLambdaResultTypeDef,
-    GetAccessPointResultTypeDef,
-    GetPublicAccessBlockOutputTypeDef,
+    CreateAccessPointForObjectLambdaResultTypeDef,
+    CreateAccessPointResultTypeDef,
+    CreateBucketResultTypeDef,
+    CreateJobResultTypeDef,
+    CreateMultiRegionAccessPointResultTypeDef,
+    DeleteMultiRegionAccessPointResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccessPointPolicyForObjectLambdaResultTypeDef,
+    GetAccessPointPolicyResultTypeDef,
+    GetBucketPolicyResultTypeDef,
+    GetBucketResultTypeDef,
+    GetBucketVersioningResultTypeDef,
+    PutMultiRegionAccessPointPolicyResultTypeDef,
+    UpdateJobPriorityResultTypeDef,
+    UpdateJobStatusResultTypeDef,
     PutPublicAccessBlockRequestRequestTypeDef,
+    CreateAccessPointRequestRequestTypeDef,
     CreateBucketRequestRequestTypeDef,
-    GetBucketTaggingResultTypeDef,
-    GetJobTaggingResultTypeDef,
     LifecycleRuleAndOperatorTypeDef,
     PutJobTaggingRequestRequestTypeDef,
     ReplicationRuleAndOperatorTypeDef,
     S3SetObjectTaggingOperationTypeDef,
     TaggingTypeDef,
+    GetAccessPointForObjectLambdaResultTypeDef,
+    GetAccessPointResultTypeDef,
+    GetPublicAccessBlockOutputTypeDef,
+    CreateMultiRegionAccessPointInputOutputTypeDef,
     CreateMultiRegionAccessPointInputTypeDef,
+    DeleteMultiRegionAccessPointRequestRequestTypeDef,
+    GeneratedManifestEncryptionOutputTypeDef,
     GeneratedManifestEncryptionTypeDef,
     GetAccessPointPolicyStatusForObjectLambdaResultTypeDef,
     GetAccessPointPolicyStatusResultTypeDef,
     GetMultiRegionAccessPointPolicyStatusResultTypeDef,
+    GetBucketTaggingResultTypeDef,
+    GetJobTaggingResultTypeDef,
+    LifecycleRuleAndOperatorOutputTypeDef,
+    ReplicationRuleAndOperatorOutputTypeDef,
+    S3SetObjectTaggingOperationOutputTypeDef,
     GetMultiRegionAccessPointRoutesResultTypeDef,
-    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
     GetStorageLensConfigurationTaggingResultTypeDef,
-    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
     S3GeneratedManifestDescriptorTypeDef,
+    JobManifestOutputTypeDef,
     JobManifestTypeDef,
     JobProgressSummaryTypeDef,
+    ListAccessPointsForObjectLambdaRequestListAccessPointsForObjectLambdaPaginateTypeDef,
     ListRegionalBucketsResultTypeDef,
     ListStorageLensConfigurationsResultTypeDef,
+    MetricsOutputTypeDef,
+    ReplicationTimeOutputTypeDef,
     MetricsTypeDef,
     ReplicationTimeTypeDef,
     MultiRegionAccessPointPolicyDocumentTypeDef,
     MultiRegionAccessPointsAsyncResponseTypeDef,
     MultiRegionAccessPointReportTypeDef,
+    SubmitMultiRegionAccessPointRoutesRequestRequestTypeDef,
+    PrefixLevelStorageMetricsOutputTypeDef,
     PrefixLevelStorageMetricsTypeDef,
     PutBucketVersioningRequestRequestTypeDef,
+    PutMultiRegionAccessPointPolicyRequestRequestTypeDef,
+    PutStorageLensConfigurationTaggingRequestRequestTypeDef,
+    S3GrantOutputTypeDef,
     S3GrantTypeDef,
+    S3SetObjectLegalHoldOperationOutputTypeDef,
     S3SetObjectLegalHoldOperationTypeDef,
+    S3SetObjectRetentionOperationOutputTypeDef,
     S3SetObjectRetentionOperationTypeDef,
+    StorageLensDataExportEncryptionOutputTypeDef,
     StorageLensDataExportEncryptionTypeDef,
+    SourceSelectionCriteriaOutputTypeDef,
     SourceSelectionCriteriaTypeDef,
     ListAccessPointsResultTypeDef,
+    ObjectLambdaTransformationConfigurationOutputTypeDef,
     ObjectLambdaTransformationConfigurationTypeDef,
     ListAccessPointsForObjectLambdaResultTypeDef,
     LifecycleRuleFilterTypeDef,
     ReplicationRuleFilterTypeDef,
     PutBucketTaggingRequestRequestTypeDef,
     AsyncRequestParametersTypeDef,
     CreateMultiRegionAccessPointRequestRequestTypeDef,
+    S3ManifestOutputLocationOutputTypeDef,
     S3ManifestOutputLocationTypeDef,
+    LifecycleRuleFilterOutputTypeDef,
+    ReplicationRuleFilterOutputTypeDef,
     JobListDescriptorTypeDef,
+    DestinationOutputTypeDef,
     DestinationTypeDef,
     GetMultiRegionAccessPointPolicyResultTypeDef,
     AsyncResponseDetailsTypeDef,
     GetMultiRegionAccessPointResultTypeDef,
     ListMultiRegionAccessPointsResultTypeDef,
+    PrefixLevelOutputTypeDef,
     PrefixLevelTypeDef,
+    S3AccessControlListOutputTypeDef,
+    S3CopyObjectOperationOutputTypeDef,
     S3AccessControlListTypeDef,
     S3CopyObjectOperationTypeDef,
+    S3BucketDestinationOutputTypeDef,
     S3BucketDestinationTypeDef,
+    ObjectLambdaConfigurationOutputTypeDef,
     ObjectLambdaConfigurationTypeDef,
     LifecycleRuleTypeDef,
+    S3JobManifestGeneratorOutputTypeDef,
     S3JobManifestGeneratorTypeDef,
+    LifecycleRuleOutputTypeDef,
     ListJobsResultTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     AsyncOperationTypeDef,
+    BucketLevelOutputTypeDef,
     BucketLevelTypeDef,
+    S3AccessControlPolicyOutputTypeDef,
     S3AccessControlPolicyTypeDef,
+    StorageLensDataExportOutputTypeDef,
     StorageLensDataExportTypeDef,
-    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     GetAccessPointConfigurationForObjectLambdaResultTypeDef,
+    CreateAccessPointForObjectLambdaRequestRequestTypeDef,
     PutAccessPointConfigurationForObjectLambdaRequestRequestTypeDef,
-    GetBucketLifecycleConfigurationResultTypeDef,
     LifecycleConfigurationTypeDef,
+    JobManifestGeneratorOutputTypeDef,
     JobManifestGeneratorTypeDef,
+    GetBucketLifecycleConfigurationResultTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     DescribeMultiRegionAccessPointOperationResultTypeDef,
+    AccountLevelOutputTypeDef,
     AccountLevelTypeDef,
+    S3SetObjectAclOperationOutputTypeDef,
     S3SetObjectAclOperationTypeDef,
     PutBucketLifecycleConfigurationRequestRequestTypeDef,
     GetBucketReplicationResultTypeDef,
     PutBucketReplicationRequestRequestTypeDef,
+    StorageLensConfigurationOutputTypeDef,
     StorageLensConfigurationTypeDef,
+    JobOperationOutputTypeDef,
     JobOperationTypeDef,
     GetStorageLensConfigurationResultTypeDef,
     PutStorageLensConfigurationRequestRequestTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobDescriptorTypeDef,
+    CreateJobRequestRequestTypeDef,
     DescribeJobResultTypeDef,
 )
 
 
-def get_structure() -> AbortIncompleteMultipartUploadTypeDef:
+def get_structure() -> AbortIncompleteMultipartUploadOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-s3control-1.28.0/mypy_boto3_s3control.egg-info/SOURCES.txt` & `mypy-boto3-s3control-1.28.12/mypy_boto3_s3control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-s3control-1.28.0/setup.py` & `mypy-boto3-s3control-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-s3control",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_s3control"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.S3Control 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.S3Control 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

