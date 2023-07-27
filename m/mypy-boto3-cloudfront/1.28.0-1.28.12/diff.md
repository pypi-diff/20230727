# Comparing `tmp/mypy-boto3-cloudfront-1.28.0.tar.gz` & `tmp/mypy-boto3-cloudfront-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudfront-1.28.0.tar", last modified: Thu Jul  6 20:59:09 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudfront-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
```

## Comparing `mypy-boto3-cloudfront-1.28.0.tar` & `mypy-boto3-cloudfront-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.270243 mypy-boto3-cloudfront-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-07-06 20:59:09.270243 mypy-boto3-cloudfront-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    29195 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.266243 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79436 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79316 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   138513 2023-07-06 20:35:22.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   138250 2023-07-06 20:35:20.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-06 20:35:17.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:09.270243 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30692 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:09.000000 mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:09.270243 mypy-boto3-cloudfront-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:16.000000 mypy-boto3-cloudfront-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    34787 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33288 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79436 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79316 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   186569 2023-07-27 05:18:42.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186182 2023-07-27 05:18:40.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-27 05:18:38.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34787 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.076562 mypy-boto3-cloudfront-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:37.000000 mypy-boto3-cloudfront-1.28.12/setup.py
```

### Comparing `mypy-boto3-cloudfront-1.28.0/LICENSE` & `mypy-boto3-cloudfront-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/PKG-INFO` & `mypy-boto3-cloudfront-1.28.12/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudfront
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudFront 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,36 +407,51 @@
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
+    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
+    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
+    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
+    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
+    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
+    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -446,23 +461,31 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
+    LoggingConfigOutputTypeDef,
+    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
     EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
+    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
+    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -473,30 +496,35 @@
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
+    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
+    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
+    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
@@ -517,224 +545,295 @@
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
     ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
+    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
+    OriginShieldOutputTypeDef,
+    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
     PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
+    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
+    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
+    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
+    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
+    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
+    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
+    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
+    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
+    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     ResponseMetadataTypeDef,
+    S3OriginOutputTypeDef,
     S3OriginTypeDef,
+    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
+    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
+    EndPointOutputTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    MonitoringSubscriptionOutputTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
+    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
+    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
+    CreateRealtimeLogConfigRequestRequestTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -745,34 +844,34 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
 def get_structure() -> AliasICPRecordalTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudfront-1.28.0/README.md` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-cloudfront
+Version: 1.28.12
+Summary: Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,36 +407,51 @@
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
+    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
+    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
+    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
+    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
+    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
+    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -414,23 +461,31 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
+    LoggingConfigOutputTypeDef,
+    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
     EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
+    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
+    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -441,30 +496,35 @@
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
+    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
+    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
+    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
@@ -485,224 +545,295 @@
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
     ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
+    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
+    OriginShieldOutputTypeDef,
+    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
     PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
+    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
+    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
+    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
+    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
+    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
+    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
+    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
+    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
+    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     ResponseMetadataTypeDef,
+    S3OriginOutputTypeDef,
     S3OriginTypeDef,
+    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
+    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
+    EndPointOutputTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    MonitoringSubscriptionOutputTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
+    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
+    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
+    CreateRealtimeLogConfigRequestRequestTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -713,34 +844,34 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
 def get_structure() -> AliasICPRecordalTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__init__.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__init__.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/__main__.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFront 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CloudFront 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront\nOther"
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

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/client.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/client.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/literals.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,14 +241,15 @@
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
@@ -327,26 +328,28 @@
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

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/literals.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -239,14 +239,15 @@
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
@@ -325,26 +326,28 @@
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

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/paginator.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/paginator.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/type_defs.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -58,36 +58,51 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AliasICPRecordalTypeDef",
+    "AliasesOutputTypeDef",
     "AliasesTypeDef",
+    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "TrustedKeyGroupsOutputTypeDef",
+    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
+    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
+    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
+    "ContentTypeProfileOutputTypeDef",
     "ContentTypeProfileTypeDef",
+    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
+    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
+    "SessionStickinessConfigOutputTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
+    "CustomErrorResponseOutputTypeDef",
     "CustomErrorResponseTypeDef",
+    "OriginCustomHeaderOutputTypeDef",
     "OriginCustomHeaderTypeDef",
+    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -97,23 +112,31 @@
     "DeleteOriginAccessControlRequestRequestTypeDef",
     "DeleteOriginRequestPolicyRequestRequestTypeDef",
     "DeletePublicKeyRequestRequestTypeDef",
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
+    "LoggingConfigOutputTypeDef",
+    "ViewerCertificateOutputTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
+    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
+    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
+    "FunctionAssociationOutputTypeDef",
     "FunctionAssociationTypeDef",
+    "FunctionConfigOutputTypeDef",
     "FunctionMetadataTypeDef",
+    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -124,30 +147,35 @@
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
+    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
+    "OriginAccessControlConfigOutputTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
+    "PublicKeyConfigOutputTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
+    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
+    "LambdaFunctionAssociationOutputTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
@@ -168,224 +196,295 @@
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
+    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
+    "OriginGroupMemberOutputTypeDef",
     "OriginGroupMemberTypeDef",
+    "OriginShieldOutputTypeDef",
+    "S3OriginConfigOutputTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
+    "QueryArgProfileOutputTypeDef",
     "QueryArgProfileTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
+    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
+    "ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
+    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
+    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
+    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
+    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
+    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
+    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
+    "ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    "ResponseHeadersPolicyXSSProtectionOutputTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "ResponseMetadataTypeDef",
+    "S3OriginOutputTypeDef",
     "S3OriginTypeDef",
+    "StreamingLoggingConfigOutputTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "CachePolicyCookiesConfigOutputTypeDef",
+    "CookiePreferenceOutputTypeDef",
+    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
+    "CachePolicyHeadersConfigOutputTypeDef",
+    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
+    "CachePolicyQueryStringsConfigOutputTypeDef",
+    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
-    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
+    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
+    "ContinuousDeploymentSingleWeightConfigOutputTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
-    "GetOriginAccessControlConfigResultTypeDef",
-    "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
-    "GetPublicKeyConfigResultTypeDef",
-    "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
+    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
+    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
+    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
+    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
+    "EndPointOutputTypeDef",
     "EndPointTypeDef",
+    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
+    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
+    "GetOriginAccessControlConfigResultTypeDef",
+    "OriginAccessControlTypeDef",
+    "GetPublicKeyConfigResultTypeDef",
+    "PublicKeyTypeDef",
+    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
+    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
+    "MonitoringSubscriptionOutputTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
+    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
+    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
+    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
+    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
+    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
+    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
+    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
+    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "TagsOutputTypeDef",
     "TagsTypeDef",
+    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
+    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
+    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
+    "TrafficConfigOutputTypeDef",
     "TrafficConfigTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "CreateOriginAccessControlResultTypeDef",
-    "GetOriginAccessControlResultTypeDef",
-    "UpdateOriginAccessControlResultTypeDef",
-    "CreatePublicKeyResultTypeDef",
-    "GetPublicKeyResultTypeDef",
-    "UpdatePublicKeyResultTypeDef",
+    "OriginOutputTypeDef",
     "OriginTypeDef",
+    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateInvalidationRequestRequestTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
+    "CreateOriginAccessControlResultTypeDef",
+    "GetOriginAccessControlResultTypeDef",
+    "UpdateOriginAccessControlResultTypeDef",
+    "CreatePublicKeyResultTypeDef",
+    "GetPublicKeyResultTypeDef",
+    "UpdatePublicKeyResultTypeDef",
     "InvalidationTypeDef",
+    "CreateInvalidationRequestRequestTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "ListOriginAccessControlsResultTypeDef",
+    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
+    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
+    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "CreateStreamingDistributionRequestRequestTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
+    "CreateStreamingDistributionRequestRequestTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigTypeDef",
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
+    "CachePolicyConfigTypeDef",
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
+    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "KeyGroupListTypeDef",
+    "OriginsOutputTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
+    "FieldLevelEncryptionProfileConfigTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
+    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
+    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
+    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
-    "ListKeyGroupsResultTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
+    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionListTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigTypeDef",
+    "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
+    "DistributionConfigTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -396,93 +495,164 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigWithTagsTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
-    "UpdateDistributionRequestRequestTypeDef",
     "DistributionListTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigWithTagsTypeDef",
+    "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
+_RequiredAliasesOutputTypeDef = TypedDict(
+    "_RequiredAliasesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalAliasesOutputTypeDef = TypedDict(
+    "_OptionalAliasesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
+    pass
+
+
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
 
+CachedMethodsOutputTypeDef = TypedDict(
+    "CachedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_RequiredTrustedKeyGroupsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_OptionalTrustedKeyGroupsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class TrustedKeyGroupsOutputTypeDef(
+    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
+):
+    pass
+
+
+_RequiredTrustedSignersOutputTypeDef = TypedDict(
+    "_RequiredTrustedSignersOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedSignersOutputTypeDef = TypedDict(
+    "_OptionalTrustedSignersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class TrustedSignersOutputTypeDef(
+    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
+):
+    pass
+
+
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
@@ -494,62 +664,123 @@
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
 
+_RequiredCookieNamesOutputTypeDef = TypedDict(
+    "_RequiredCookieNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCookieNamesOutputTypeDef = TypedDict(
+    "_OptionalCookieNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class CookieNamesOutputTypeDef(
+    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
+):
+    pass
+
+
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
 
+_RequiredHeadersOutputTypeDef = TypedDict(
+    "_RequiredHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalHeadersOutputTypeDef = TypedDict(
+    "_OptionalHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
+    pass
+
+
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
 
+_RequiredQueryStringNamesOutputTypeDef = TypedDict(
+    "_RequiredQueryStringNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringNamesOutputTypeDef = TypedDict(
+    "_OptionalQueryStringNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class QueryStringNamesOutputTypeDef(
+    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringNamesTypeDef = TypedDict(
@@ -561,14 +792,22 @@
 )
 
 
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
 
+CloudFrontOriginAccessIdentityConfigOutputTypeDef = TypedDict(
+    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "Comment": str,
+    },
+)
+
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -588,14 +827,36 @@
         "Alias": str,
         "DistributionId": str,
         "AccountId": str,
     },
     total=False,
 )
 
+_RequiredContentTypeProfileOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileOutputTypeDef",
+    {
+        "Format": Literal["URLEncoded"],
+        "ContentType": str,
+    },
+)
+_OptionalContentTypeProfileOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileOutputTypeDef",
+    {
+        "ProfileId": str,
+    },
+    total=False,
+)
+
+
+class ContentTypeProfileOutputTypeDef(
+    _RequiredContentTypeProfileOutputTypeDef, _OptionalContentTypeProfileOutputTypeDef
+):
+    pass
+
+
 _RequiredContentTypeProfileTypeDef = TypedDict(
     "_RequiredContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
     },
 )
@@ -610,14 +871,36 @@
 
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
 
+_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class StagingDistributionDnsNamesOutputTypeDef(
+    _RequiredStagingDistributionDnsNamesOutputTypeDef,
+    _OptionalStagingDistributionDnsNamesOutputTypeDef,
+):
+    pass
+
+
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalStagingDistributionDnsNamesTypeDef = TypedDict(
@@ -631,22 +914,38 @@
 
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
 
+ContinuousDeploymentSingleHeaderConfigOutputTypeDef = TypedDict(
+    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
+    {
+        "Header": str,
+        "Value": str,
+    },
+)
+
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
 
+SessionStickinessConfigOutputTypeDef = TypedDict(
+    "SessionStickinessConfigOutputTypeDef",
+    {
+        "IdleTTL": int,
+        "MaximumTTL": int,
+    },
+)
+
 SessionStickinessConfigTypeDef = TypedDict(
     "SessionStickinessConfigTypeDef",
     {
         "IdleTTL": int,
         "MaximumTTL": int,
     },
 )
@@ -743,14 +1042,37 @@
 )
 
 
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
 
+_RequiredCustomErrorResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponseOutputTypeDef",
+    {
+        "ErrorCode": int,
+    },
+)
+_OptionalCustomErrorResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponseOutputTypeDef",
+    {
+        "ResponsePagePath": str,
+        "ResponseCode": str,
+        "ErrorCachingMinTTL": int,
+    },
+    total=False,
+)
+
+
+class CustomErrorResponseOutputTypeDef(
+    _RequiredCustomErrorResponseOutputTypeDef, _OptionalCustomErrorResponseOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -766,27 +1088,43 @@
 
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
 
+OriginCustomHeaderOutputTypeDef = TypedDict(
+    "OriginCustomHeaderOutputTypeDef",
+    {
+        "HeaderName": str,
+        "HeaderValue": str,
+    },
+)
+
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+OriginSslProtocolsOutputTypeDef = TypedDict(
+    "OriginSslProtocolsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[SslProtocolType],
+    },
+)
+
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": List[SslProtocolType],
+        "Items": Sequence[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -1088,14 +1426,38 @@
 
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "IncludeCookies": bool,
+        "Bucket": str,
+        "Prefix": str,
+    },
+)
+
+ViewerCertificateOutputTypeDef = TypedDict(
+    "ViewerCertificateOutputTypeDef",
+    {
+        "CloudFrontDefaultCertificate": bool,
+        "IAMCertificateId": str,
+        "ACMCertificateArn": str,
+        "SSLSupportMethod": SSLSupportMethodType,
+        "MinimumProtocolVersion": MinimumProtocolVersionType,
+        "Certificate": str,
+        "CertificateSource": CertificateSourceType,
+    },
+    total=False,
+)
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1144,14 +1506,35 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFieldPatternsOutputTypeDef = TypedDict(
+    "_RequiredFieldPatternsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFieldPatternsOutputTypeDef = TypedDict(
+    "_OptionalFieldPatternsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class FieldPatternsOutputTypeDef(
+    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
+):
+    pass
+
+
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsTypeDef = TypedDict(
@@ -1163,51 +1546,96 @@
 )
 
 
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
 
+KinesisStreamConfigOutputTypeDef = TypedDict(
+    "KinesisStreamConfigOutputTypeDef",
+    {
+        "RoleARN": str,
+        "StreamARN": str,
+    },
+)
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
+_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_RequiredQueryStringCacheKeysOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_OptionalQueryStringCacheKeysOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class QueryStringCacheKeysOutputTypeDef(
+    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
 
+FunctionAssociationOutputTypeDef = TypedDict(
+    "FunctionAssociationOutputTypeDef",
+    {
+        "FunctionARN": str,
+        "EventType": EventTypeType,
+    },
+)
+
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
 
+FunctionConfigOutputTypeDef = TypedDict(
+    "FunctionConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "Runtime": Literal["cloudfront-js-1.0"],
+    },
+)
+
 _RequiredFunctionMetadataTypeDef = TypedDict(
     "_RequiredFunctionMetadataTypeDef",
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
     },
 )
@@ -1221,25 +1649,47 @@
 )
 
 
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
 
+_RequiredGeoRestrictionOutputTypeDef = TypedDict(
+    "_RequiredGeoRestrictionOutputTypeDef",
+    {
+        "RestrictionType": GeoRestrictionTypeType,
+        "Quantity": int,
+    },
+)
+_OptionalGeoRestrictionOutputTypeDef = TypedDict(
+    "_OptionalGeoRestrictionOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class GeoRestrictionOutputTypeDef(
+    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
+):
+    pass
+
+
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
@@ -1380,14 +1830,36 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredKeyGroupConfigOutputTypeDef",
+    {
+        "Name": str,
+        "Items": List[str],
+    },
+)
+_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalKeyGroupConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class KeyGroupConfigOutputTypeDef(
+    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
+):
+    pass
+
+
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1401,14 +1873,38 @@
 GetOriginAccessControlConfigRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredOriginAccessControlConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginAccessControlConfigOutputTypeDef",
+    {
+        "Name": str,
+        "SigningProtocol": Literal["sigv4"],
+        "SigningBehavior": OriginAccessControlSigningBehaviorsType,
+        "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
+    },
+)
+_OptionalOriginAccessControlConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginAccessControlConfigOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class OriginAccessControlConfigOutputTypeDef(
+    _RequiredOriginAccessControlConfigOutputTypeDef, _OptionalOriginAccessControlConfigOutputTypeDef
+):
+    pass
+
+
 GetOriginAccessControlRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1429,14 +1925,37 @@
 GetPublicKeyConfigRequestRequestTypeDef = TypedDict(
     "GetPublicKeyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPublicKeyConfigOutputTypeDef = TypedDict(
+    "_RequiredPublicKeyConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "Name": str,
+        "EncodedKey": str,
+    },
+)
+_OptionalPublicKeyConfigOutputTypeDef = TypedDict(
+    "_OptionalPublicKeyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class PublicKeyConfigOutputTypeDef(
+    _RequiredPublicKeyConfigOutputTypeDef, _OptionalPublicKeyConfigOutputTypeDef
+):
+    pass
+
+
 GetPublicKeyRequestRequestTypeDef = TypedDict(
     "GetPublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1473,14 +1992,33 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPathsOutputTypeDef = TypedDict(
+    "_RequiredPathsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalPathsOutputTypeDef = TypedDict(
+    "_OptionalPathsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
+    pass
+
+
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
@@ -1520,14 +2058,36 @@
 )
 
 
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
 
+_RequiredLambdaFunctionAssociationOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationOutputTypeDef",
+    {
+        "LambdaFunctionARN": str,
+        "EventType": EventTypeType,
+    },
+)
+_OptionalLambdaFunctionAssociationOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationOutputTypeDef",
+    {
+        "IncludeBody": bool,
+    },
+    total=False,
+)
+
+
+class LambdaFunctionAssociationOutputTypeDef(
+    _RequiredLambdaFunctionAssociationOutputTypeDef, _OptionalLambdaFunctionAssociationOutputTypeDef
+):
+    pass
+
+
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1897,14 +2457,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+RealtimeMetricsSubscriptionConfigOutputTypeDef = TypedDict(
+    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
+    {
+        "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
+    },
+)
+
 RealtimeMetricsSubscriptionConfigTypeDef = TypedDict(
     "RealtimeMetricsSubscriptionConfigTypeDef",
     {
         "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
     },
 )
 
@@ -1916,29 +2483,72 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
+StatusCodesOutputTypeDef = TypedDict(
+    "StatusCodesOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[int],
+    },
+)
+
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": List[int],
+        "Items": Sequence[int],
+    },
+)
+
+OriginGroupMemberOutputTypeDef = TypedDict(
+    "OriginGroupMemberOutputTypeDef",
+    {
+        "OriginId": str,
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
 )
 
+_RequiredOriginShieldOutputTypeDef = TypedDict(
+    "_RequiredOriginShieldOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalOriginShieldOutputTypeDef = TypedDict(
+    "_OptionalOriginShieldOutputTypeDef",
+    {
+        "OriginShieldRegion": str,
+    },
+    total=False,
+)
+
+
+class OriginShieldOutputTypeDef(
+    _RequiredOriginShieldOutputTypeDef, _OptionalOriginShieldOutputTypeDef
+):
+    pass
+
+
+S3OriginConfigOutputTypeDef = TypedDict(
+    "S3OriginConfigOutputTypeDef",
+    {
+        "OriginAccessIdentity": str,
+    },
+)
+
 _RequiredOriginShieldTypeDef = TypedDict(
     "_RequiredOriginShieldTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOriginShieldTypeDef = TypedDict(
@@ -1997,46 +2607,100 @@
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
 
+QueryArgProfileOutputTypeDef = TypedDict(
+    "QueryArgProfileOutputTypeDef",
+    {
+        "QueryArg": str,
+        "ProfileId": str,
+    },
+)
+
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
+    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
@@ -2051,14 +2715,36 @@
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
 
+_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
+    {
+        "SamplingRate": float,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
@@ -2073,61 +2759,156 @@
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
 
+ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
+    {
+        "Override": bool,
+        "ContentSecurityPolicy": str,
+    },
+)
+
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
 
+ResponseHeadersPolicyContentTypeOptionsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
+    {
+        "Override": bool,
+    },
+)
+
 ResponseHeadersPolicyContentTypeOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     {
         "Override": bool,
     },
 )
 
+ResponseHeadersPolicyCustomHeaderOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
+    {
+        "Header": str,
+        "Value": str,
+        "Override": bool,
+    },
+)
+
 ResponseHeadersPolicyCustomHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     {
         "Header": str,
         "Value": str,
         "Override": bool,
     },
 )
 
+ResponseHeadersPolicyFrameOptionsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
+    {
+        "Override": bool,
+        "FrameOption": FrameOptionsListType,
+    },
+)
+
 ResponseHeadersPolicyFrameOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     {
         "Override": bool,
         "FrameOption": FrameOptionsListType,
     },
 )
 
+ResponseHeadersPolicyReferrerPolicyOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
+    {
+        "Override": bool,
+        "ReferrerPolicy": ReferrerPolicyListType,
+    },
+)
+
 ResponseHeadersPolicyReferrerPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     {
         "Override": bool,
         "ReferrerPolicy": ReferrerPolicyListType,
     },
 )
 
+ResponseHeadersPolicyRemoveHeaderOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
+    {
+        "Header": str,
+    },
+)
+
 ResponseHeadersPolicyRemoveHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     {
         "Header": str,
     },
 )
 
+_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    {
+        "Override": bool,
+        "AccessControlMaxAgeSec": int,
+    },
+)
+_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    {
+        "IncludeSubdomains": bool,
+        "Preload": bool,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef(
+    _RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    _OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+):
+    pass
+
+
+_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef",
+    {
+        "Override": bool,
+        "Protection": bool,
+    },
+)
+_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef",
+    {
+        "ModeBlock": bool,
+        "ReportUri": str,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyXSSProtectionOutputTypeDef(
+    _RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef,
+    _OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef",
     {
         "Override": bool,
         "AccessControlMaxAgeSec": int,
     },
 )
@@ -2179,22 +2960,39 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3OriginOutputTypeDef = TypedDict(
+    "S3OriginOutputTypeDef",
+    {
+        "DomainName": str,
+        "OriginAccessIdentity": str,
+    },
+)
+
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
 
+StreamingLoggingConfigOutputTypeDef = TypedDict(
+    "StreamingLoggingConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Bucket": str,
+        "Prefix": str,
+    },
+)
+
 StreamingLoggingConfigTypeDef = TypedDict(
     "StreamingLoggingConfigTypeDef",
     {
         "Enabled": bool,
         "Bucket": str,
         "Prefix": str,
     },
@@ -2204,14 +3002,33 @@
     "TagKeysTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -2269,19 +3086,41 @@
 class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
     _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
     _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredAllowedMethodsOutputTypeDef = TypedDict(
+    "_RequiredAllowedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+_OptionalAllowedMethodsOutputTypeDef = TypedDict(
+    "_OptionalAllowedMethodsOutputTypeDef",
+    {
+        "CachedMethods": CachedMethodsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AllowedMethodsOutputTypeDef(
+    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
+):
+    pass
+
+
 _RequiredAllowedMethodsTypeDef = TypedDict(
     "_RequiredAllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 _OptionalAllowedMethodsTypeDef = TypedDict(
     "_OptionalAllowedMethodsTypeDef",
     {
         "CachedMethods": CachedMethodsTypeDef,
     },
@@ -2289,14 +3128,78 @@
 )
 
 
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
 
+_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": CachePolicyCookieBehaviorType,
+    },
+)
+_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyCookiesConfigOutputTypeDef(
+    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredCookiePreferenceOutputTypeDef = TypedDict(
+    "_RequiredCookiePreferenceOutputTypeDef",
+    {
+        "Forward": ItemSelectionType,
+    },
+)
+_OptionalCookiePreferenceOutputTypeDef = TypedDict(
+    "_OptionalCookiePreferenceOutputTypeDef",
+    {
+        "WhitelistedNames": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CookiePreferenceOutputTypeDef(
+    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
+):
+    pass
+
+
+_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyCookiesConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigTypeDef = TypedDict(
@@ -2351,14 +3254,57 @@
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
 
+_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": CachePolicyHeaderBehaviorType,
+    },
+)
+_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyHeadersConfigOutputTypeDef(
+    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyHeadersConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
 _OptionalCachePolicyHeadersConfigTypeDef = TypedDict(
@@ -2394,14 +3340,58 @@
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
 
+_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
+    },
+)
+_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyQueryStringsConfigOutputTypeDef(
+    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
+    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+
+_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
 _OptionalCachePolicyQueryStringsConfigTypeDef = TypedDict(
@@ -2447,39 +3437,39 @@
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
 _OptionalCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
 
-CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
-    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
+    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
@@ -2535,14 +3525,35 @@
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
+_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfilesOutputTypeDef",
+    {
+        "Items": List[ContentTypeProfileOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ContentTypeProfilesOutputTypeDef(
+    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
+):
+    pass
+
+
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
@@ -2556,14 +3567,36 @@
 
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
 
+_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef",
+    {
+        "Weight": float,
+    },
+)
+_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef",
+    {
+        "SessionStickinessConfig": SessionStickinessConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ContinuousDeploymentSingleWeightConfigOutputTypeDef(
+    _RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef,
+    _OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
@@ -2604,32 +3637,14 @@
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-    },
-)
-
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -2651,44 +3666,14 @@
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
-GetOriginAccessControlConfigResultTypeDef = TypedDict(
-    "GetOriginAccessControlConfigResultTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredOriginAccessControlTypeDef = TypedDict(
-    "_RequiredOriginAccessControlTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalOriginAccessControlTypeDef = TypedDict(
-    "_OptionalOriginAccessControlTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class OriginAccessControlTypeDef(
-    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
-):
-    pass
-
-
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -2711,32 +3696,14 @@
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
-GetPublicKeyConfigResultTypeDef = TypedDict(
-    "GetPublicKeyConfigResultTypeDef",
-    {
-        "PublicKeyConfig": PublicKeyConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublicKeyTypeDef = TypedDict(
-    "PublicKeyTypeDef",
-    {
-        "Id": str,
-        "CreatedTime": datetime,
-        "PublicKeyConfig": PublicKeyConfigTypeDef,
-    },
-)
-
 _RequiredUpdatePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
     },
 )
@@ -2751,54 +3718,121 @@
 
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponsesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponsesOutputTypeDef",
+    {
+        "Items": List[CustomErrorResponseOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomErrorResponsesOutputTypeDef(
+    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": List[CustomErrorResponseTypeDef],
+        "Items": Sequence[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
 
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
 
+_RequiredCustomHeadersOutputTypeDef = TypedDict(
+    "_RequiredCustomHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomHeadersOutputTypeDef = TypedDict(
+    "_OptionalCustomHeadersOutputTypeDef",
+    {
+        "Items": List[OriginCustomHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CustomHeadersOutputTypeDef(
+    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": List[OriginCustomHeaderTypeDef],
+        "Items": Sequence[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
 
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
 
+_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
+    "_RequiredCustomOriginConfigOutputTypeDef",
+    {
+        "HTTPPort": int,
+        "HTTPSPort": int,
+        "OriginProtocolPolicy": OriginProtocolPolicyType,
+    },
+)
+_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
+    "_OptionalCustomOriginConfigOutputTypeDef",
+    {
+        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
+        "OriginReadTimeout": int,
+        "OriginKeepaliveTimeout": int,
+    },
+    total=False,
+)
+
+
+class CustomOriginConfigOutputTypeDef(
+    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
     },
@@ -2848,23 +3882,51 @@
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionEntityOutputTypeDef = TypedDict(
+    "EncryptionEntityOutputTypeDef",
+    {
+        "PublicKeyId": str,
+        "ProviderId": str,
+        "FieldPatterns": FieldPatternsOutputTypeDef,
+    },
+)
+
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
 )
 
+_RequiredEndPointOutputTypeDef = TypedDict(
+    "_RequiredEndPointOutputTypeDef",
+    {
+        "StreamType": str,
+    },
+)
+_OptionalEndPointOutputTypeDef = TypedDict(
+    "_OptionalEndPointOutputTypeDef",
+    {
+        "KinesisStreamConfig": KinesisStreamConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EndPointOutputTypeDef(_RequiredEndPointOutputTypeDef, _OptionalEndPointOutputTypeDef):
+    pass
+
+
 _RequiredEndPointTypeDef = TypedDict(
     "_RequiredEndPointTypeDef",
     {
         "StreamType": str,
     },
 )
 _OptionalEndPointTypeDef = TypedDict(
@@ -2876,24 +3938,45 @@
 )
 
 
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
 
+_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[FunctionAssociationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class FunctionAssociationsOutputTypeDef(
+    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
+):
+    pass
+
+
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": List[FunctionAssociationTypeDef],
+        "Items": Sequence[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
 
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
@@ -2901,15 +3984,15 @@
     pass
 
 
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigTypeDef,
+        "FunctionConfig": FunctionConfigOutputTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
 )
 _OptionalFunctionSummaryTypeDef = TypedDict(
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
@@ -2918,14 +4001,21 @@
 )
 
 
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
 
+RestrictionsOutputTypeDef = TypedDict(
+    "RestrictionsOutputTypeDef",
+    {
+        "GeoRestriction": GeoRestrictionOutputTypeDef,
+    },
+)
+
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
 
@@ -2992,14 +4082,88 @@
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
 
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+    },
+)
+
+GetOriginAccessControlConfigResultTypeDef = TypedDict(
+    "GetOriginAccessControlConfigResultTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredOriginAccessControlTypeDef = TypedDict(
+    "_RequiredOriginAccessControlTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalOriginAccessControlTypeDef = TypedDict(
+    "_OptionalOriginAccessControlTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class OriginAccessControlTypeDef(
+    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
+):
+    pass
+
+
+GetPublicKeyConfigResultTypeDef = TypedDict(
+    "GetPublicKeyConfigResultTypeDef",
+    {
+        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PublicKeyTypeDef = TypedDict(
+    "PublicKeyTypeDef",
+    {
+        "Id": str,
+        "CreatedTime": datetime,
+        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
+    },
+)
+
+InvalidationBatchOutputTypeDef = TypedDict(
+    "InvalidationBatchOutputTypeDef",
+    {
+        "Paths": PathsOutputTypeDef,
+        "CallerReference": str,
+    },
+)
+
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -3041,35 +4205,65 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
+_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[LambdaFunctionAssociationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class LambdaFunctionAssociationsOutputTypeDef(
+    _RequiredLambdaFunctionAssociationsOutputTypeDef,
+    _OptionalLambdaFunctionAssociationsOutputTypeDef,
+):
+    pass
+
+
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationTypeDef],
+        "Items": Sequence[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
 
+MonitoringSubscriptionOutputTypeDef = TypedDict(
+    "MonitoringSubscriptionOutputTypeDef",
+    {
+        "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
 )
@@ -3095,26 +4289,41 @@
 
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
 
+OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
+    "OriginGroupFailoverCriteriaOutputTypeDef",
+    {
+        "StatusCodes": StatusCodesOutputTypeDef,
+    },
+)
+
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
+OriginGroupMembersOutputTypeDef = TypedDict(
+    "OriginGroupMembersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[OriginGroupMemberOutputTypeDef],
+    },
+)
+
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
+        "Items": Sequence[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -3131,14 +4340,35 @@
 )
 
 
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
 
+_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfilesOutputTypeDef",
+    {
+        "Items": List[QueryArgProfileOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class QueryArgProfilesOutputTypeDef(
+    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesTypeDef = TypedDict(
@@ -3150,14 +4380,41 @@
 )
 
 
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
 
+_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
+        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
+        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
+        "AccessControlAllowCredentials": bool,
+        "OriginOverride": bool,
+    },
+)
+_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+        "AccessControlMaxAgeSec": int,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyCorsConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
@@ -3176,14 +4433,36 @@
 
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
 
+_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyCustomHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
@@ -3198,14 +4477,36 @@
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
 
+_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyRemoveHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
@@ -3220,14 +4521,27 @@
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
 
+ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
+    {
+        "XSSProtection": ResponseHeadersPolicyXSSProtectionOutputTypeDef,
+        "FrameOptions": ResponseHeadersPolicyFrameOptionsOutputTypeDef,
+        "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
+        "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
+        "ContentTypeOptions": ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
+        "StrictTransportSecurity": ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -3241,23 +4555,51 @@
     "StreamingDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesTypeDef,
-        "TrustedSigners": TrustedSignersTypeDef,
+        "S3Origin": S3OriginOutputTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
+_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredStreamingDistributionConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "S3Origin": S3OriginOutputTypeDef,
+        "Comment": str,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalStreamingDistributionConfigOutputTypeDef",
+    {
+        "Aliases": AliasesOutputTypeDef,
+        "Logging": StreamingLoggingConfigOutputTypeDef,
+        "PriceClass": PriceClassType,
+    },
+    total=False,
+)
+
+
+class StreamingDistributionConfigOutputTypeDef(
+    _RequiredStreamingDistributionConfigOutputTypeDef,
+    _OptionalStreamingDistributionConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -3285,22 +4627,53 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
+TagsOutputTypeDef = TypedDict(
+    "TagsOutputTypeDef",
+    {
+        "Items": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredForwardedValuesOutputTypeDef = TypedDict(
+    "_RequiredForwardedValuesOutputTypeDef",
+    {
+        "QueryString": bool,
+        "Cookies": CookiePreferenceOutputTypeDef,
+    },
+)
+_OptionalForwardedValuesOutputTypeDef = TypedDict(
+    "_OptionalForwardedValuesOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ForwardedValuesOutputTypeDef(
+    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
+):
+    pass
+
+
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -3314,14 +4687,63 @@
 )
 
 
 class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
 
+_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingGzip": bool,
+        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingBrotli": bool,
+    },
+    total=False,
+)
+
+
+class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
+    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+):
+    pass
+
+
+_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class OriginRequestPolicyConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -3407,14 +4829,35 @@
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenContentTypeIsUnknown": bool,
+    },
+)
+_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileConfigOutputTypeDef",
+    {
+        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ContentTypeProfileConfigOutputTypeDef(
+    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredContentTypeProfileConfigTypeDef = TypedDict(
     "_RequiredContentTypeProfileConfigTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
 _OptionalContentTypeProfileConfigTypeDef = TypedDict(
@@ -3428,124 +4871,82 @@
 
 class ContentTypeProfileConfigTypeDef(
     _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
 ):
     pass
 
 
-_RequiredTrafficConfigTypeDef = TypedDict(
-    "_RequiredTrafficConfigTypeDef",
+_RequiredTrafficConfigOutputTypeDef = TypedDict(
+    "_RequiredTrafficConfigOutputTypeDef",
     {
         "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-_OptionalTrafficConfigTypeDef = TypedDict(
-    "_OptionalTrafficConfigTypeDef",
+_OptionalTrafficConfigOutputTypeDef = TypedDict(
+    "_OptionalTrafficConfigOutputTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigOutputTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     },
     total=False,
 )
 
 
-class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
+class TrafficConfigOutputTypeDef(
+    _RequiredTrafficConfigOutputTypeDef, _OptionalTrafficConfigOutputTypeDef
+):
     pass
 
 
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
+_RequiredTrafficConfigTypeDef = TypedDict(
+    "_RequiredTrafficConfigTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
+_OptionalTrafficConfigTypeDef = TypedDict(
+    "_OptionalTrafficConfigTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
+    total=False,
 )
 
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-    },
-)
 
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
+    pass
 
-CreateOriginAccessControlResultTypeDef = TypedDict(
-    "CreateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-GetOriginAccessControlResultTypeDef = TypedDict(
-    "GetOriginAccessControlResultTypeDef",
+_RequiredOriginOutputTypeDef = TypedDict(
+    "_RequiredOriginOutputTypeDef",
     {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "DomainName": str,
     },
 )
-
-UpdateOriginAccessControlResultTypeDef = TypedDict(
-    "UpdateOriginAccessControlResultTypeDef",
+_OptionalOriginOutputTypeDef = TypedDict(
+    "_OptionalOriginOutputTypeDef",
     {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OriginPath": str,
+        "CustomHeaders": CustomHeadersOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigOutputTypeDef,
+        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
+        "ConnectionAttempts": int,
+        "ConnectionTimeout": int,
+        "OriginShield": OriginShieldOutputTypeDef,
+        "OriginAccessControlId": str,
     },
+    total=False,
 )
 
-CreatePublicKeyResultTypeDef = TypedDict(
-    "CreatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-GetPublicKeyResultTypeDef = TypedDict(
-    "GetPublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
+    pass
 
-UpdatePublicKeyResultTypeDef = TypedDict(
-    "UpdatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
@@ -3566,14 +4967,35 @@
 )
 
 
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
 
+_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_RequiredEncryptionEntitiesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_OptionalEncryptionEntitiesOutputTypeDef",
+    {
+        "Items": List[EncryptionEntityOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class EncryptionEntitiesOutputTypeDef(
+    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
+):
+    pass
+
+
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalEncryptionEntitiesTypeDef = TypedDict(
@@ -3587,32 +5009,32 @@
 
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
 
-CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
+RealtimeLogConfigTypeDef = TypedDict(
+    "RealtimeLogConfigTypeDef",
     {
-        "EndPoints": Sequence[EndPointTypeDef],
-        "Fields": Sequence[str],
+        "ARN": str,
         "Name": str,
         "SamplingRate": int,
+        "EndPoints": List[EndPointOutputTypeDef],
+        "Fields": List[str],
     },
 )
 
-RealtimeLogConfigTypeDef = TypedDict(
-    "RealtimeLogConfigTypeDef",
+CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
-        "ARN": str,
+        "EndPoints": Sequence[EndPointTypeDef],
+        "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
-        "EndPoints": List[EndPointTypeDef],
-        "Fields": List[str],
     },
 )
 
 UpdateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
@@ -3689,28 +5111,119 @@
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
     {
-        "DistributionId": str,
-        "InvalidationBatch": InvalidationBatchTypeDef,
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateOriginAccessControlResultTypeDef = TypedDict(
+    "CreateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOriginAccessControlResultTypeDef = TypedDict(
+    "GetOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateOriginAccessControlResultTypeDef = TypedDict(
+    "UpdateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePublicKeyResultTypeDef = TypedDict(
+    "CreatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPublicKeyResultTypeDef = TypedDict(
+    "GetPublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdatePublicKeyResultTypeDef = TypedDict(
+    "UpdatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
+        "InvalidationBatch": InvalidationBatchOutputTypeDef,
+    },
+)
+
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
+    {
+        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
@@ -3759,46 +5272,55 @@
 
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
 
-CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
-    {
-        "DistributionId": str,
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-    },
-)
-
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
+    {
+        "DistributionId": str,
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+    },
+)
+
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OriginGroupOutputTypeDef = TypedDict(
+    "OriginGroupOutputTypeDef",
+    {
+        "Id": str,
+        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
+        "Members": OriginGroupMembersOutputTypeDef,
+    },
+)
+
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -3808,14 +5330,35 @@
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenQueryArgProfileIsUnknown": bool,
+    },
+)
+_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfileConfigOutputTypeDef",
+    {
+        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryArgProfileConfigOutputTypeDef(
+    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
 _OptionalQueryArgProfileConfigTypeDef = TypedDict(
@@ -3829,14 +5372,41 @@
 
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
 
+_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ResponseHeadersPolicyConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalResponseHeadersPolicyConfigTypeDef = TypedDict(
@@ -3880,27 +5450,27 @@
 
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
 
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3922,15 +5492,15 @@
 ):
     pass
 
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsTypeDef,
+        "Tags": TagsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
@@ -3943,14 +5513,89 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorOutputTypeDef",
+    {
+        "PathPattern": str,
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+
+class CacheBehaviorOutputTypeDef(
+    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
+):
+    pass
+
+
+_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+
+class DefaultCacheBehaviorOutputTypeDef(
+    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
+):
+    pass
+
+
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -4016,60 +5661,87 @@
 
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
 
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
+_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigOutputTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
+_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+        "ParametersInCacheKeyAndForwardedToOrigin": (
+            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+        ),
     },
     total=False,
 )
 
 
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+class CachePolicyConfigOutputTypeDef(
+    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
 ):
     pass
 
 
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
-    },
-)
-
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+    },
+)
+
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
+    {
+        "Name": str,
+        "MinTTL": int,
+    },
+)
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
+    {
+        "Comment": str,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+    },
+    total=False,
+)
+
+
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+):
+    pass
+
+
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
@@ -4089,14 +5761,37 @@
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "TrafficConfig": TrafficConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ContinuousDeploymentPolicyConfigOutputTypeDef(
+    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
+    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
+):
+    pass
+
+
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
 )
@@ -4112,74 +5807,61 @@
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
 
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
+OriginsOutputTypeDef = TypedDict(
+    "OriginsOutputTypeDef",
     {
-        "MaxItems": int,
         "Quantity": int,
+        "Items": List[OriginOutputTypeDef],
     },
 )
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
-
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginTypeDef],
+        "Items": Sequence[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
 
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+class FieldLevelEncryptionProfileConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
 ):
     pass
 
 
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
@@ -4190,14 +5872,38 @@
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
 
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Name": str,
+        "CallerReference": str,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
+    },
+)
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+):
+    pass
+
+
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4254,14 +5960,35 @@
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
+    {
+        "MaxItems": int,
+        "Quantity": int,
+    },
+)
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
+
+
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -4279,15 +6006,15 @@
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
@@ -4297,52 +6024,74 @@
 
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
 
+_RequiredOriginGroupsOutputTypeDef = TypedDict(
+    "_RequiredOriginGroupsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalOriginGroupsOutputTypeDef = TypedDict(
+    "_OptionalOriginGroupsOutputTypeDef",
+    {
+        "Items": List[OriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class OriginGroupsOutputTypeDef(
+    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
+):
+    pass
+
+
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": List[OriginGroupTypeDef],
+        "Items": Sequence[OriginGroupTypeDef],
     },
     total=False,
 )
 
 
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
 
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
+_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
 
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+class FieldLevelEncryptionConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
 ):
     pass
 
 
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
@@ -4350,48 +6099,71 @@
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
 
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
 
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "CallerReference": str,
     },
 )
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
+    {
+        "Comment": str,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+):
+    pass
+
 
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+    },
+)
+
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
@@ -4426,80 +6198,72 @@
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[CacheBehaviorOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CacheBehaviorsOutputTypeDef(
+    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
+):
+    pass
+
+
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": List[CacheBehaviorTypeDef],
+        "Items": Sequence[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
 
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
 
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
-
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4528,39 +6292,68 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ContinuousDeploymentPolicyTypeDef = TypedDict(
-    "ContinuousDeploymentPolicyTypeDef",
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
     {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "Id": str,
-        "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
 
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
+
+ContinuousDeploymentPolicyTypeDef = TypedDict(
+    "ContinuousDeploymentPolicyTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    {
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+    },
+)
+
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4576,101 +6369,101 @@
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
-    {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-    },
-)
-
 FieldLevelEncryptionProfileTypeDef = TypedDict(
     "FieldLevelEncryptionProfileTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
     },
 )
 
 GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
     },
     total=False,
 )
 
 
-class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
 ):
     pass
 
 
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+
+_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    {
+        "IfMatch": str,
     },
     total=False,
 )
 
 
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
 
 ListRealtimeLogConfigsResultTypeDef = TypedDict(
     "ListRealtimeLogConfigsResultTypeDef",
     {
         "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
+    {
+        "KeyGroupList": KeyGroupListTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4701,81 +6494,81 @@
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
-
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
     },
     total=False,
 )
 
 
-class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
 ):
     pass
 
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
+
+_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "IfMatch": str,
     },
     total=False,
 )
 
 
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
@@ -4808,92 +6601,130 @@
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
+_RequiredDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
+_OptionalDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalDistributionConfigOutputTypeDef",
     {
-        "Aliases": AliasesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
-        "Logging": LoggingConfigTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Logging": LoggingConfigOutputTypeDef,
         "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
 
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+class DistributionConfigOutputTypeDef(
+    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
 ):
     pass
 
 
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesTypeDef,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
 
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
 
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
+    {
+        "CallerReference": str,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Comment": str,
+        "Enabled": bool,
+    },
+)
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
+    {
+        "Aliases": AliasesTypeDef,
+        "DefaultRootObject": str,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Logging": LoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+        "ViewerCertificate": ViewerCertificateTypeDef,
+        "Restrictions": RestrictionsTypeDef,
+        "WebACLId": str,
+        "HttpVersion": HttpVersionType,
+        "IsIPV6Enabled": bool,
+        "ContinuousDeploymentPolicyId": str,
+        "Staging": bool,
+    },
+    total=False,
+)
+
+
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+):
+    pass
+
+
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
 )
@@ -5075,39 +6906,24 @@
 
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
 
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
@@ -5120,63 +6936,78 @@
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionRequestRequestTypeDef",
+_RequiredDistributionListTypeDef = TypedDict(
+    "_RequiredDistributionListTypeDef",
     {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
+        "Marker": str,
+        "MaxItems": int,
+        "IsTruncated": bool,
+        "Quantity": int,
     },
 )
-_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionRequestRequestTypeDef",
+_OptionalDistributionListTypeDef = TypedDict(
+    "_OptionalDistributionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[DistributionSummaryTypeDef],
     },
     total=False,
 )
 
 
-class UpdateDistributionRequestRequestTypeDef(
-    _RequiredUpdateDistributionRequestRequestTypeDef,
-    _OptionalUpdateDistributionRequestRequestTypeDef,
-):
+class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
     pass
 
 
-_RequiredDistributionListTypeDef = TypedDict(
-    "_RequiredDistributionListTypeDef",
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
     {
-        "Marker": str,
-        "MaxItems": int,
-        "IsTruncated": bool,
-        "Quantity": int,
+        "DistributionConfig": DistributionConfigTypeDef,
     },
 )
-_OptionalDistributionListTypeDef = TypedDict(
-    "_OptionalDistributionListTypeDef",
+
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[DistributionSummaryTypeDef],
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
+
+_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionRequestRequestTypeDef",
+    {
+        "IfMatch": str,
     },
     total=False,
 )
 
 
-class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
+class UpdateDistributionRequestRequestTypeDef(
+    _RequiredUpdateDistributionRequestRequestTypeDef,
+    _OptionalUpdateDistributionRequestRequestTypeDef,
+):
     pass
 
 
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
@@ -5232,21 +7063,14 @@
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
-
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -5320,14 +7144,21 @@
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
+
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/type_defs.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -57,36 +57,51 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AliasICPRecordalTypeDef",
+    "AliasesOutputTypeDef",
     "AliasesTypeDef",
+    "CachedMethodsOutputTypeDef",
     "CachedMethodsTypeDef",
     "AssociateAliasRequestRequestTypeDef",
+    "TrustedKeyGroupsOutputTypeDef",
+    "TrustedSignersOutputTypeDef",
     "TrustedKeyGroupsTypeDef",
     "TrustedSignersTypeDef",
+    "CookieNamesOutputTypeDef",
     "CookieNamesTypeDef",
+    "HeadersOutputTypeDef",
     "HeadersTypeDef",
+    "QueryStringNamesOutputTypeDef",
     "QueryStringNamesTypeDef",
+    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     "CloudFrontOriginAccessIdentitySummaryTypeDef",
     "ConflictingAliasTypeDef",
+    "ContentTypeProfileOutputTypeDef",
     "ContentTypeProfileTypeDef",
+    "StagingDistributionDnsNamesOutputTypeDef",
     "StagingDistributionDnsNamesTypeDef",
+    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
+    "SessionStickinessConfigOutputTypeDef",
     "SessionStickinessConfigTypeDef",
     "CopyDistributionRequestRequestTypeDef",
     "FunctionConfigTypeDef",
     "KeyGroupConfigTypeDef",
     "OriginAccessControlConfigTypeDef",
     "PublicKeyConfigTypeDef",
+    "CustomErrorResponseOutputTypeDef",
     "CustomErrorResponseTypeDef",
+    "OriginCustomHeaderOutputTypeDef",
     "OriginCustomHeaderTypeDef",
+    "OriginSslProtocolsOutputTypeDef",
     "OriginSslProtocolsTypeDef",
     "DeleteCachePolicyRequestRequestTypeDef",
     "DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "DeleteContinuousDeploymentPolicyRequestRequestTypeDef",
     "DeleteDistributionRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionConfigRequestRequestTypeDef",
     "DeleteFieldLevelEncryptionProfileRequestRequestTypeDef",
@@ -96,23 +111,31 @@
     "DeleteOriginAccessControlRequestRequestTypeDef",
     "DeleteOriginRequestPolicyRequestRequestTypeDef",
     "DeletePublicKeyRequestRequestTypeDef",
     "DeleteRealtimeLogConfigRequestRequestTypeDef",
     "DeleteResponseHeadersPolicyRequestRequestTypeDef",
     "DeleteStreamingDistributionRequestRequestTypeDef",
     "DescribeFunctionRequestRequestTypeDef",
+    "LoggingConfigOutputTypeDef",
+    "ViewerCertificateOutputTypeDef",
     "LoggingConfigTypeDef",
     "ViewerCertificateTypeDef",
     "DistributionIdListTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "FieldPatternsOutputTypeDef",
     "FieldPatternsTypeDef",
+    "KinesisStreamConfigOutputTypeDef",
     "KinesisStreamConfigTypeDef",
+    "QueryStringCacheKeysOutputTypeDef",
     "QueryStringCacheKeysTypeDef",
+    "FunctionAssociationOutputTypeDef",
     "FunctionAssociationTypeDef",
+    "FunctionConfigOutputTypeDef",
     "FunctionMetadataTypeDef",
+    "GeoRestrictionOutputTypeDef",
     "GeoRestrictionTypeDef",
     "GetCachePolicyConfigRequestRequestTypeDef",
     "GetCachePolicyRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyRequestRequestTypeDef",
@@ -123,30 +146,35 @@
     "GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef",
     "GetFieldLevelEncryptionProfileRequestRequestTypeDef",
     "GetFieldLevelEncryptionRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionResultTypeDef",
     "GetInvalidationRequestRequestTypeDef",
     "GetKeyGroupConfigRequestRequestTypeDef",
+    "KeyGroupConfigOutputTypeDef",
     "GetKeyGroupRequestRequestTypeDef",
     "GetMonitoringSubscriptionRequestRequestTypeDef",
     "GetOriginAccessControlConfigRequestRequestTypeDef",
+    "OriginAccessControlConfigOutputTypeDef",
     "GetOriginAccessControlRequestRequestTypeDef",
     "GetOriginRequestPolicyConfigRequestRequestTypeDef",
     "GetOriginRequestPolicyRequestRequestTypeDef",
     "GetPublicKeyConfigRequestRequestTypeDef",
+    "PublicKeyConfigOutputTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
     "GetRealtimeLogConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyConfigRequestRequestTypeDef",
     "GetResponseHeadersPolicyRequestRequestTypeDef",
     "GetStreamingDistributionConfigRequestRequestTypeDef",
     "GetStreamingDistributionRequestRequestTypeDef",
+    "PathsOutputTypeDef",
     "PathsTypeDef",
     "InvalidationSummaryTypeDef",
     "KeyPairIdsTypeDef",
+    "LambdaFunctionAssociationOutputTypeDef",
     "LambdaFunctionAssociationTypeDef",
     "ListCachePoliciesRequestRequestTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef",
     "ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef",
     "ListConflictingAliasesRequestRequestTypeDef",
     "ListContinuousDeploymentPoliciesRequestRequestTypeDef",
     "ListDistributionsByCachePolicyIdRequestRequestTypeDef",
@@ -167,224 +195,295 @@
     "ListOriginRequestPoliciesRequestRequestTypeDef",
     "ListPublicKeysRequestRequestTypeDef",
     "ListRealtimeLogConfigsRequestRequestTypeDef",
     "ListResponseHeadersPoliciesRequestRequestTypeDef",
     "ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef",
     "ListStreamingDistributionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
     "RealtimeMetricsSubscriptionConfigTypeDef",
     "OriginAccessControlSummaryTypeDef",
+    "StatusCodesOutputTypeDef",
     "StatusCodesTypeDef",
+    "OriginGroupMemberOutputTypeDef",
     "OriginGroupMemberTypeDef",
+    "OriginShieldOutputTypeDef",
+    "S3OriginConfigOutputTypeDef",
     "OriginShieldTypeDef",
     "S3OriginConfigTypeDef",
     "PaginatorConfigTypeDef",
     "PublicKeySummaryTypeDef",
     "PublishFunctionRequestRequestTypeDef",
+    "QueryArgProfileOutputTypeDef",
     "QueryArgProfileTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
+    "ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
     "ResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
+    "ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
+    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
+    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
+    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
     "ResponseHeadersPolicyCustomHeaderTypeDef",
+    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
     "ResponseHeadersPolicyFrameOptionsTypeDef",
+    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
+    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
+    "ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    "ResponseHeadersPolicyXSSProtectionOutputTypeDef",
     "ResponseHeadersPolicyStrictTransportSecurityTypeDef",
     "ResponseHeadersPolicyXSSProtectionTypeDef",
     "ResponseMetadataTypeDef",
+    "S3OriginOutputTypeDef",
     "S3OriginTypeDef",
+    "StreamingLoggingConfigOutputTypeDef",
     "StreamingLoggingConfigTypeDef",
     "TagKeysTypeDef",
+    "TagOutputTypeDef",
     "TagTypeDef",
     "TestFunctionRequestRequestTypeDef",
     "UpdateDistributionWithStagingConfigRequestRequestTypeDef",
+    "AllowedMethodsOutputTypeDef",
     "AllowedMethodsTypeDef",
+    "CachePolicyCookiesConfigOutputTypeDef",
+    "CookiePreferenceOutputTypeDef",
+    "OriginRequestPolicyCookiesConfigOutputTypeDef",
     "CachePolicyCookiesConfigTypeDef",
     "CookiePreferenceTypeDef",
     "OriginRequestPolicyCookiesConfigTypeDef",
+    "CachePolicyHeadersConfigOutputTypeDef",
+    "OriginRequestPolicyHeadersConfigOutputTypeDef",
     "CachePolicyHeadersConfigTypeDef",
     "OriginRequestPolicyHeadersConfigTypeDef",
+    "CachePolicyQueryStringsConfigOutputTypeDef",
+    "OriginRequestPolicyQueryStringsConfigOutputTypeDef",
     "CachePolicyQueryStringsConfigTypeDef",
     "OriginRequestPolicyQueryStringsConfigTypeDef",
     "CloudFrontOriginAccessIdentityTypeDef",
-    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     "CloudFrontOriginAccessIdentityListTypeDef",
     "ConflictingAliasesListTypeDef",
+    "ContentTypeProfilesOutputTypeDef",
     "ContentTypeProfilesTypeDef",
+    "ContinuousDeploymentSingleWeightConfigOutputTypeDef",
     "ContinuousDeploymentSingleWeightConfigTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionRequestRequestTypeDef",
     "CreateKeyGroupRequestRequestTypeDef",
-    "GetKeyGroupConfigResultTypeDef",
-    "KeyGroupTypeDef",
     "UpdateKeyGroupRequestRequestTypeDef",
     "CreateOriginAccessControlRequestRequestTypeDef",
-    "GetOriginAccessControlConfigResultTypeDef",
-    "OriginAccessControlTypeDef",
     "UpdateOriginAccessControlRequestRequestTypeDef",
     "CreatePublicKeyRequestRequestTypeDef",
-    "GetPublicKeyConfigResultTypeDef",
-    "PublicKeyTypeDef",
     "UpdatePublicKeyRequestRequestTypeDef",
+    "CustomErrorResponsesOutputTypeDef",
     "CustomErrorResponsesTypeDef",
+    "CustomHeadersOutputTypeDef",
     "CustomHeadersTypeDef",
+    "CustomOriginConfigOutputTypeDef",
     "CustomOriginConfigTypeDef",
     "ListDistributionsByCachePolicyIdResultTypeDef",
     "ListDistributionsByKeyGroupResultTypeDef",
     "ListDistributionsByOriginRequestPolicyIdResultTypeDef",
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
+    "EncryptionEntityOutputTypeDef",
     "EncryptionEntityTypeDef",
+    "EndPointOutputTypeDef",
     "EndPointTypeDef",
+    "FunctionAssociationsOutputTypeDef",
     "FunctionAssociationsTypeDef",
     "FunctionSummaryTypeDef",
+    "RestrictionsOutputTypeDef",
     "RestrictionsTypeDef",
     "GetDistributionRequestDistributionDeployedWaitTypeDef",
     "GetInvalidationRequestInvalidationCompletedWaitTypeDef",
     "GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef",
+    "GetKeyGroupConfigResultTypeDef",
+    "KeyGroupTypeDef",
+    "GetOriginAccessControlConfigResultTypeDef",
+    "OriginAccessControlTypeDef",
+    "GetPublicKeyConfigResultTypeDef",
+    "PublicKeyTypeDef",
+    "InvalidationBatchOutputTypeDef",
     "InvalidationBatchTypeDef",
     "InvalidationListTypeDef",
     "KGKeyPairIdsTypeDef",
     "SignerTypeDef",
+    "LambdaFunctionAssociationsOutputTypeDef",
     "LambdaFunctionAssociationsTypeDef",
+    "MonitoringSubscriptionOutputTypeDef",
     "MonitoringSubscriptionTypeDef",
     "OriginAccessControlListTypeDef",
+    "OriginGroupFailoverCriteriaOutputTypeDef",
     "OriginGroupFailoverCriteriaTypeDef",
+    "OriginGroupMembersOutputTypeDef",
     "OriginGroupMembersTypeDef",
     "PublicKeyListTypeDef",
+    "QueryArgProfilesOutputTypeDef",
     "QueryArgProfilesTypeDef",
+    "ResponseHeadersPolicyCorsConfigOutputTypeDef",
     "ResponseHeadersPolicyCorsConfigTypeDef",
+    "ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyCustomHeadersConfigTypeDef",
+    "ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicyRemoveHeadersConfigTypeDef",
+    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     "StreamingDistributionSummaryTypeDef",
+    "StreamingDistributionConfigOutputTypeDef",
     "StreamingDistributionConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "TagsOutputTypeDef",
     "TagsTypeDef",
+    "ForwardedValuesOutputTypeDef",
     "ForwardedValuesTypeDef",
+    "ParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    "OriginRequestPolicyConfigOutputTypeDef",
     "ParametersInCacheKeyAndForwardedToOriginTypeDef",
     "OriginRequestPolicyConfigTypeDef",
     "CreateCloudFrontOriginAccessIdentityResultTypeDef",
     "GetCloudFrontOriginAccessIdentityResultTypeDef",
     "UpdateCloudFrontOriginAccessIdentityResultTypeDef",
     "ListCloudFrontOriginAccessIdentitiesResultTypeDef",
     "ListConflictingAliasesResultTypeDef",
+    "ContentTypeProfileConfigOutputTypeDef",
     "ContentTypeProfileConfigTypeDef",
+    "TrafficConfigOutputTypeDef",
     "TrafficConfigTypeDef",
-    "CreateKeyGroupResultTypeDef",
-    "GetKeyGroupResultTypeDef",
-    "KeyGroupSummaryTypeDef",
-    "UpdateKeyGroupResultTypeDef",
-    "CreateOriginAccessControlResultTypeDef",
-    "GetOriginAccessControlResultTypeDef",
-    "UpdateOriginAccessControlResultTypeDef",
-    "CreatePublicKeyResultTypeDef",
-    "GetPublicKeyResultTypeDef",
-    "UpdatePublicKeyResultTypeDef",
+    "OriginOutputTypeDef",
     "OriginTypeDef",
+    "EncryptionEntitiesOutputTypeDef",
     "EncryptionEntitiesTypeDef",
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
     "RealtimeLogConfigTypeDef",
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     "CreateFunctionResultTypeDef",
     "DescribeFunctionResultTypeDef",
     "FunctionListTypeDef",
     "PublishFunctionResultTypeDef",
     "TestResultTypeDef",
     "UpdateFunctionResultTypeDef",
-    "CreateInvalidationRequestRequestTypeDef",
+    "CreateKeyGroupResultTypeDef",
+    "GetKeyGroupResultTypeDef",
+    "KeyGroupSummaryTypeDef",
+    "UpdateKeyGroupResultTypeDef",
+    "CreateOriginAccessControlResultTypeDef",
+    "GetOriginAccessControlResultTypeDef",
+    "UpdateOriginAccessControlResultTypeDef",
+    "CreatePublicKeyResultTypeDef",
+    "GetPublicKeyResultTypeDef",
+    "UpdatePublicKeyResultTypeDef",
     "InvalidationTypeDef",
+    "CreateInvalidationRequestRequestTypeDef",
     "ListInvalidationsResultTypeDef",
     "ActiveTrustedKeyGroupsTypeDef",
     "ActiveTrustedSignersTypeDef",
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "CreateMonitoringSubscriptionResultTypeDef",
     "GetMonitoringSubscriptionResultTypeDef",
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
     "ListOriginAccessControlsResultTypeDef",
+    "OriginGroupOutputTypeDef",
     "OriginGroupTypeDef",
     "ListPublicKeysResultTypeDef",
+    "QueryArgProfileConfigOutputTypeDef",
     "QueryArgProfileConfigTypeDef",
+    "ResponseHeadersPolicyConfigOutputTypeDef",
     "ResponseHeadersPolicyConfigTypeDef",
     "StreamingDistributionListTypeDef",
-    "CreateStreamingDistributionRequestRequestTypeDef",
     "GetStreamingDistributionConfigResultTypeDef",
+    "CreateStreamingDistributionRequestRequestTypeDef",
     "UpdateStreamingDistributionRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "StreamingDistributionConfigWithTagsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CacheBehaviorOutputTypeDef",
+    "DefaultCacheBehaviorOutputTypeDef",
     "CacheBehaviorTypeDef",
     "DefaultCacheBehaviorTypeDef",
-    "CachePolicyConfigTypeDef",
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    "CachePolicyConfigOutputTypeDef",
     "GetOriginRequestPolicyConfigResultTypeDef",
     "OriginRequestPolicyTypeDef",
+    "CachePolicyConfigTypeDef",
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
     "UpdateOriginRequestPolicyRequestRequestTypeDef",
+    "ContinuousDeploymentPolicyConfigOutputTypeDef",
     "ContinuousDeploymentPolicyConfigTypeDef",
-    "KeyGroupListTypeDef",
+    "OriginsOutputTypeDef",
     "OriginsTypeDef",
-    "FieldLevelEncryptionProfileConfigTypeDef",
+    "FieldLevelEncryptionProfileConfigOutputTypeDef",
     "FieldLevelEncryptionProfileSummaryTypeDef",
+    "FieldLevelEncryptionProfileConfigTypeDef",
     "CreateRealtimeLogConfigResultTypeDef",
     "GetRealtimeLogConfigResultTypeDef",
     "RealtimeLogConfigsTypeDef",
     "UpdateRealtimeLogConfigResultTypeDef",
     "ListFunctionsResultTypeDef",
     "TestFunctionResultTypeDef",
+    "KeyGroupListTypeDef",
     "CreateInvalidationResultTypeDef",
     "GetInvalidationResultTypeDef",
     "StreamingDistributionTypeDef",
+    "OriginGroupsOutputTypeDef",
     "OriginGroupsTypeDef",
-    "FieldLevelEncryptionConfigTypeDef",
+    "FieldLevelEncryptionConfigOutputTypeDef",
     "FieldLevelEncryptionSummaryTypeDef",
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    "FieldLevelEncryptionConfigTypeDef",
     "GetResponseHeadersPolicyConfigResultTypeDef",
     "ResponseHeadersPolicyTypeDef",
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
     "UpdateResponseHeadersPolicyRequestRequestTypeDef",
     "ListStreamingDistributionsResultTypeDef",
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
+    "CacheBehaviorsOutputTypeDef",
     "CacheBehaviorsTypeDef",
     "CachePolicyTypeDef",
-    "CreateCachePolicyRequestRequestTypeDef",
     "GetCachePolicyConfigResultTypeDef",
-    "UpdateCachePolicyRequestRequestTypeDef",
     "CreateOriginRequestPolicyResultTypeDef",
     "GetOriginRequestPolicyResultTypeDef",
     "OriginRequestPolicySummaryTypeDef",
     "UpdateOriginRequestPolicyResultTypeDef",
+    "CreateCachePolicyRequestRequestTypeDef",
+    "UpdateCachePolicyRequestRequestTypeDef",
     "ContinuousDeploymentPolicyTypeDef",
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
     "UpdateContinuousDeploymentPolicyRequestRequestTypeDef",
-    "ListKeyGroupsResultTypeDef",
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileTypeDef",
     "GetFieldLevelEncryptionProfileConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "FieldLevelEncryptionProfileListTypeDef",
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+    "UpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     "ListRealtimeLogConfigsResultTypeDef",
+    "ListKeyGroupsResultTypeDef",
     "CreateStreamingDistributionResultTypeDef",
     "CreateStreamingDistributionWithTagsResultTypeDef",
     "GetStreamingDistributionResultTypeDef",
     "UpdateStreamingDistributionResultTypeDef",
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionTypeDef",
     "GetFieldLevelEncryptionConfigResultTypeDef",
-    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "FieldLevelEncryptionListTypeDef",
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    "UpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     "CreateResponseHeadersPolicyResultTypeDef",
     "GetResponseHeadersPolicyResultTypeDef",
     "ResponseHeadersPolicySummaryTypeDef",
     "UpdateResponseHeadersPolicyResultTypeDef",
-    "DistributionConfigTypeDef",
+    "DistributionConfigOutputTypeDef",
     "DistributionSummaryTypeDef",
+    "DistributionConfigTypeDef",
     "CachePolicySummaryTypeDef",
     "CreateCachePolicyResultTypeDef",
     "GetCachePolicyResultTypeDef",
     "UpdateCachePolicyResultTypeDef",
     "OriginRequestPolicyListTypeDef",
     "ContinuousDeploymentPolicySummaryTypeDef",
     "CreateContinuousDeploymentPolicyResultTypeDef",
@@ -395,91 +494,156 @@
     "UpdateFieldLevelEncryptionProfileResultTypeDef",
     "ListFieldLevelEncryptionProfilesResultTypeDef",
     "CreateFieldLevelEncryptionConfigResultTypeDef",
     "GetFieldLevelEncryptionResultTypeDef",
     "UpdateFieldLevelEncryptionConfigResultTypeDef",
     "ListFieldLevelEncryptionConfigsResultTypeDef",
     "ResponseHeadersPolicyListTypeDef",
-    "CreateDistributionRequestRequestTypeDef",
-    "DistributionConfigWithTagsTypeDef",
     "DistributionTypeDef",
     "GetDistributionConfigResultTypeDef",
-    "UpdateDistributionRequestRequestTypeDef",
     "DistributionListTypeDef",
+    "CreateDistributionRequestRequestTypeDef",
+    "DistributionConfigWithTagsTypeDef",
+    "UpdateDistributionRequestRequestTypeDef",
     "CachePolicyListTypeDef",
     "ListOriginRequestPoliciesResultTypeDef",
     "ContinuousDeploymentPolicyListTypeDef",
     "ListResponseHeadersPoliciesResultTypeDef",
-    "CreateDistributionWithTagsRequestRequestTypeDef",
     "CopyDistributionResultTypeDef",
     "CreateDistributionResultTypeDef",
     "CreateDistributionWithTagsResultTypeDef",
     "GetDistributionResultTypeDef",
     "UpdateDistributionResultTypeDef",
     "UpdateDistributionWithStagingConfigResultTypeDef",
     "ListDistributionsByRealtimeLogConfigResultTypeDef",
     "ListDistributionsByWebACLIdResultTypeDef",
     "ListDistributionsResultTypeDef",
+    "CreateDistributionWithTagsRequestRequestTypeDef",
     "ListCachePoliciesResultTypeDef",
     "ListContinuousDeploymentPoliciesResultTypeDef",
 )
 
 AliasICPRecordalTypeDef = TypedDict(
     "AliasICPRecordalTypeDef",
     {
         "CNAME": str,
         "ICPRecordalStatus": ICPRecordalStatusType,
     },
     total=False,
 )
 
+_RequiredAliasesOutputTypeDef = TypedDict(
+    "_RequiredAliasesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalAliasesOutputTypeDef = TypedDict(
+    "_OptionalAliasesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class AliasesOutputTypeDef(_RequiredAliasesOutputTypeDef, _OptionalAliasesOutputTypeDef):
+    pass
+
 _RequiredAliasesTypeDef = TypedDict(
     "_RequiredAliasesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalAliasesTypeDef = TypedDict(
     "_OptionalAliasesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class AliasesTypeDef(_RequiredAliasesTypeDef, _OptionalAliasesTypeDef):
     pass
 
+CachedMethodsOutputTypeDef = TypedDict(
+    "CachedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+
 CachedMethodsTypeDef = TypedDict(
     "CachedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 
 AssociateAliasRequestRequestTypeDef = TypedDict(
     "AssociateAliasRequestRequestTypeDef",
     {
         "TargetDistributionId": str,
         "Alias": str,
     },
 )
 
+_RequiredTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_RequiredTrustedKeyGroupsOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedKeyGroupsOutputTypeDef = TypedDict(
+    "_OptionalTrustedKeyGroupsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class TrustedKeyGroupsOutputTypeDef(
+    _RequiredTrustedKeyGroupsOutputTypeDef, _OptionalTrustedKeyGroupsOutputTypeDef
+):
+    pass
+
+_RequiredTrustedSignersOutputTypeDef = TypedDict(
+    "_RequiredTrustedSignersOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Quantity": int,
+    },
+)
+_OptionalTrustedSignersOutputTypeDef = TypedDict(
+    "_OptionalTrustedSignersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class TrustedSignersOutputTypeDef(
+    _RequiredTrustedSignersOutputTypeDef, _OptionalTrustedSignersOutputTypeDef
+):
+    pass
+
 _RequiredTrustedKeyGroupsTypeDef = TypedDict(
     "_RequiredTrustedKeyGroupsTypeDef",
     {
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedKeyGroupsTypeDef = TypedDict(
     "_OptionalTrustedKeyGroupsTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class TrustedKeyGroupsTypeDef(_RequiredTrustedKeyGroupsTypeDef, _OptionalTrustedKeyGroupsTypeDef):
     pass
 
@@ -489,56 +653,111 @@
         "Enabled": bool,
         "Quantity": int,
     },
 )
 _OptionalTrustedSignersTypeDef = TypedDict(
     "_OptionalTrustedSignersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class TrustedSignersTypeDef(_RequiredTrustedSignersTypeDef, _OptionalTrustedSignersTypeDef):
     pass
 
+_RequiredCookieNamesOutputTypeDef = TypedDict(
+    "_RequiredCookieNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCookieNamesOutputTypeDef = TypedDict(
+    "_OptionalCookieNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class CookieNamesOutputTypeDef(
+    _RequiredCookieNamesOutputTypeDef, _OptionalCookieNamesOutputTypeDef
+):
+    pass
+
 _RequiredCookieNamesTypeDef = TypedDict(
     "_RequiredCookieNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCookieNamesTypeDef = TypedDict(
     "_OptionalCookieNamesTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class CookieNamesTypeDef(_RequiredCookieNamesTypeDef, _OptionalCookieNamesTypeDef):
     pass
 
+_RequiredHeadersOutputTypeDef = TypedDict(
+    "_RequiredHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalHeadersOutputTypeDef = TypedDict(
+    "_OptionalHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class HeadersOutputTypeDef(_RequiredHeadersOutputTypeDef, _OptionalHeadersOutputTypeDef):
+    pass
+
 _RequiredHeadersTypeDef = TypedDict(
     "_RequiredHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalHeadersTypeDef = TypedDict(
     "_OptionalHeadersTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class HeadersTypeDef(_RequiredHeadersTypeDef, _OptionalHeadersTypeDef):
     pass
 
+_RequiredQueryStringNamesOutputTypeDef = TypedDict(
+    "_RequiredQueryStringNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringNamesOutputTypeDef = TypedDict(
+    "_OptionalQueryStringNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class QueryStringNamesOutputTypeDef(
+    _RequiredQueryStringNamesOutputTypeDef, _OptionalQueryStringNamesOutputTypeDef
+):
+    pass
+
 _RequiredQueryStringNamesTypeDef = TypedDict(
     "_RequiredQueryStringNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringNamesTypeDef = TypedDict(
@@ -548,14 +767,22 @@
     },
     total=False,
 )
 
 class QueryStringNamesTypeDef(_RequiredQueryStringNamesTypeDef, _OptionalQueryStringNamesTypeDef):
     pass
 
+CloudFrontOriginAccessIdentityConfigOutputTypeDef = TypedDict(
+    "CloudFrontOriginAccessIdentityConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "Comment": str,
+    },
+)
+
 CloudFrontOriginAccessIdentityConfigTypeDef = TypedDict(
     "CloudFrontOriginAccessIdentityConfigTypeDef",
     {
         "CallerReference": str,
         "Comment": str,
     },
 )
@@ -575,14 +802,34 @@
         "Alias": str,
         "DistributionId": str,
         "AccountId": str,
     },
     total=False,
 )
 
+_RequiredContentTypeProfileOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileOutputTypeDef",
+    {
+        "Format": Literal["URLEncoded"],
+        "ContentType": str,
+    },
+)
+_OptionalContentTypeProfileOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileOutputTypeDef",
+    {
+        "ProfileId": str,
+    },
+    total=False,
+)
+
+class ContentTypeProfileOutputTypeDef(
+    _RequiredContentTypeProfileOutputTypeDef, _OptionalContentTypeProfileOutputTypeDef
+):
+    pass
+
 _RequiredContentTypeProfileTypeDef = TypedDict(
     "_RequiredContentTypeProfileTypeDef",
     {
         "Format": Literal["URLEncoded"],
         "ContentType": str,
     },
 )
@@ -595,14 +842,34 @@
 )
 
 class ContentTypeProfileTypeDef(
     _RequiredContentTypeProfileTypeDef, _OptionalContentTypeProfileTypeDef
 ):
     pass
 
+_RequiredStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_RequiredStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalStagingDistributionDnsNamesOutputTypeDef = TypedDict(
+    "_OptionalStagingDistributionDnsNamesOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class StagingDistributionDnsNamesOutputTypeDef(
+    _RequiredStagingDistributionDnsNamesOutputTypeDef,
+    _OptionalStagingDistributionDnsNamesOutputTypeDef,
+):
+    pass
+
 _RequiredStagingDistributionDnsNamesTypeDef = TypedDict(
     "_RequiredStagingDistributionDnsNamesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalStagingDistributionDnsNamesTypeDef = TypedDict(
@@ -614,22 +881,38 @@
 )
 
 class StagingDistributionDnsNamesTypeDef(
     _RequiredStagingDistributionDnsNamesTypeDef, _OptionalStagingDistributionDnsNamesTypeDef
 ):
     pass
 
+ContinuousDeploymentSingleHeaderConfigOutputTypeDef = TypedDict(
+    "ContinuousDeploymentSingleHeaderConfigOutputTypeDef",
+    {
+        "Header": str,
+        "Value": str,
+    },
+)
+
 ContinuousDeploymentSingleHeaderConfigTypeDef = TypedDict(
     "ContinuousDeploymentSingleHeaderConfigTypeDef",
     {
         "Header": str,
         "Value": str,
     },
 )
 
+SessionStickinessConfigOutputTypeDef = TypedDict(
+    "SessionStickinessConfigOutputTypeDef",
+    {
+        "IdleTTL": int,
+        "MaximumTTL": int,
+    },
+)
+
 SessionStickinessConfigTypeDef = TypedDict(
     "SessionStickinessConfigTypeDef",
     {
         "IdleTTL": int,
         "MaximumTTL": int,
     },
 )
@@ -718,14 +1001,35 @@
     },
     total=False,
 )
 
 class PublicKeyConfigTypeDef(_RequiredPublicKeyConfigTypeDef, _OptionalPublicKeyConfigTypeDef):
     pass
 
+_RequiredCustomErrorResponseOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponseOutputTypeDef",
+    {
+        "ErrorCode": int,
+    },
+)
+_OptionalCustomErrorResponseOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponseOutputTypeDef",
+    {
+        "ResponsePagePath": str,
+        "ResponseCode": str,
+        "ErrorCachingMinTTL": int,
+    },
+    total=False,
+)
+
+class CustomErrorResponseOutputTypeDef(
+    _RequiredCustomErrorResponseOutputTypeDef, _OptionalCustomErrorResponseOutputTypeDef
+):
+    pass
+
 _RequiredCustomErrorResponseTypeDef = TypedDict(
     "_RequiredCustomErrorResponseTypeDef",
     {
         "ErrorCode": int,
     },
 )
 _OptionalCustomErrorResponseTypeDef = TypedDict(
@@ -739,27 +1043,43 @@
 )
 
 class CustomErrorResponseTypeDef(
     _RequiredCustomErrorResponseTypeDef, _OptionalCustomErrorResponseTypeDef
 ):
     pass
 
+OriginCustomHeaderOutputTypeDef = TypedDict(
+    "OriginCustomHeaderOutputTypeDef",
+    {
+        "HeaderName": str,
+        "HeaderValue": str,
+    },
+)
+
 OriginCustomHeaderTypeDef = TypedDict(
     "OriginCustomHeaderTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
 
+OriginSslProtocolsOutputTypeDef = TypedDict(
+    "OriginSslProtocolsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[SslProtocolType],
+    },
+)
+
 OriginSslProtocolsTypeDef = TypedDict(
     "OriginSslProtocolsTypeDef",
     {
         "Quantity": int,
-        "Items": List[SslProtocolType],
+        "Items": Sequence[SslProtocolType],
     },
 )
 
 _RequiredDeleteCachePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCachePolicyRequestRequestTypeDef",
     {
         "Id": str,
@@ -1035,14 +1355,38 @@
 )
 
 class DescribeFunctionRequestRequestTypeDef(
     _RequiredDescribeFunctionRequestRequestTypeDef, _OptionalDescribeFunctionRequestRequestTypeDef
 ):
     pass
 
+LoggingConfigOutputTypeDef = TypedDict(
+    "LoggingConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "IncludeCookies": bool,
+        "Bucket": str,
+        "Prefix": str,
+    },
+)
+
+ViewerCertificateOutputTypeDef = TypedDict(
+    "ViewerCertificateOutputTypeDef",
+    {
+        "CloudFrontDefaultCertificate": bool,
+        "IAMCertificateId": str,
+        "ACMCertificateArn": str,
+        "SSLSupportMethod": SSLSupportMethodType,
+        "MinimumProtocolVersion": MinimumProtocolVersionType,
+        "Certificate": str,
+        "CertificateSource": CertificateSourceType,
+    },
+    total=False,
+)
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "Enabled": bool,
         "IncludeCookies": bool,
         "Bucket": str,
         "Prefix": str,
@@ -1089,14 +1433,33 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredFieldPatternsOutputTypeDef = TypedDict(
+    "_RequiredFieldPatternsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFieldPatternsOutputTypeDef = TypedDict(
+    "_OptionalFieldPatternsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class FieldPatternsOutputTypeDef(
+    _RequiredFieldPatternsOutputTypeDef, _OptionalFieldPatternsOutputTypeDef
+):
+    pass
+
 _RequiredFieldPatternsTypeDef = TypedDict(
     "_RequiredFieldPatternsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFieldPatternsTypeDef = TypedDict(
@@ -1106,49 +1469,92 @@
     },
     total=False,
 )
 
 class FieldPatternsTypeDef(_RequiredFieldPatternsTypeDef, _OptionalFieldPatternsTypeDef):
     pass
 
+KinesisStreamConfigOutputTypeDef = TypedDict(
+    "KinesisStreamConfigOutputTypeDef",
+    {
+        "RoleARN": str,
+        "StreamARN": str,
+    },
+)
+
 KinesisStreamConfigTypeDef = TypedDict(
     "KinesisStreamConfigTypeDef",
     {
         "RoleARN": str,
         "StreamARN": str,
     },
 )
 
+_RequiredQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_RequiredQueryStringCacheKeysOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryStringCacheKeysOutputTypeDef = TypedDict(
+    "_OptionalQueryStringCacheKeysOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class QueryStringCacheKeysOutputTypeDef(
+    _RequiredQueryStringCacheKeysOutputTypeDef, _OptionalQueryStringCacheKeysOutputTypeDef
+):
+    pass
+
 _RequiredQueryStringCacheKeysTypeDef = TypedDict(
     "_RequiredQueryStringCacheKeysTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryStringCacheKeysTypeDef = TypedDict(
     "_OptionalQueryStringCacheKeysTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class QueryStringCacheKeysTypeDef(
     _RequiredQueryStringCacheKeysTypeDef, _OptionalQueryStringCacheKeysTypeDef
 ):
     pass
 
+FunctionAssociationOutputTypeDef = TypedDict(
+    "FunctionAssociationOutputTypeDef",
+    {
+        "FunctionARN": str,
+        "EventType": EventTypeType,
+    },
+)
+
 FunctionAssociationTypeDef = TypedDict(
     "FunctionAssociationTypeDef",
     {
         "FunctionARN": str,
         "EventType": EventTypeType,
     },
 )
 
+FunctionConfigOutputTypeDef = TypedDict(
+    "FunctionConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "Runtime": Literal["cloudfront-js-1.0"],
+    },
+)
+
 _RequiredFunctionMetadataTypeDef = TypedDict(
     "_RequiredFunctionMetadataTypeDef",
     {
         "FunctionARN": str,
         "LastModifiedTime": datetime,
     },
 )
@@ -1160,25 +1566,45 @@
     },
     total=False,
 )
 
 class FunctionMetadataTypeDef(_RequiredFunctionMetadataTypeDef, _OptionalFunctionMetadataTypeDef):
     pass
 
+_RequiredGeoRestrictionOutputTypeDef = TypedDict(
+    "_RequiredGeoRestrictionOutputTypeDef",
+    {
+        "RestrictionType": GeoRestrictionTypeType,
+        "Quantity": int,
+    },
+)
+_OptionalGeoRestrictionOutputTypeDef = TypedDict(
+    "_OptionalGeoRestrictionOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class GeoRestrictionOutputTypeDef(
+    _RequiredGeoRestrictionOutputTypeDef, _OptionalGeoRestrictionOutputTypeDef
+):
+    pass
+
 _RequiredGeoRestrictionTypeDef = TypedDict(
     "_RequiredGeoRestrictionTypeDef",
     {
         "RestrictionType": GeoRestrictionTypeType,
         "Quantity": int,
     },
 )
 _OptionalGeoRestrictionTypeDef = TypedDict(
     "_OptionalGeoRestrictionTypeDef",
     {
-        "Items": List[str],
+        "Items": Sequence[str],
     },
     total=False,
 )
 
 class GeoRestrictionTypeDef(_RequiredGeoRestrictionTypeDef, _OptionalGeoRestrictionTypeDef):
     pass
 
@@ -1315,14 +1741,34 @@
 GetKeyGroupConfigRequestRequestTypeDef = TypedDict(
     "GetKeyGroupConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredKeyGroupConfigOutputTypeDef = TypedDict(
+    "_RequiredKeyGroupConfigOutputTypeDef",
+    {
+        "Name": str,
+        "Items": List[str],
+    },
+)
+_OptionalKeyGroupConfigOutputTypeDef = TypedDict(
+    "_OptionalKeyGroupConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class KeyGroupConfigOutputTypeDef(
+    _RequiredKeyGroupConfigOutputTypeDef, _OptionalKeyGroupConfigOutputTypeDef
+):
+    pass
+
 GetKeyGroupRequestRequestTypeDef = TypedDict(
     "GetKeyGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1336,14 +1782,36 @@
 GetOriginAccessControlConfigRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredOriginAccessControlConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginAccessControlConfigOutputTypeDef",
+    {
+        "Name": str,
+        "SigningProtocol": Literal["sigv4"],
+        "SigningBehavior": OriginAccessControlSigningBehaviorsType,
+        "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
+    },
+)
+_OptionalOriginAccessControlConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginAccessControlConfigOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class OriginAccessControlConfigOutputTypeDef(
+    _RequiredOriginAccessControlConfigOutputTypeDef, _OptionalOriginAccessControlConfigOutputTypeDef
+):
+    pass
+
 GetOriginAccessControlRequestRequestTypeDef = TypedDict(
     "GetOriginAccessControlRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1364,14 +1832,35 @@
 GetPublicKeyConfigRequestRequestTypeDef = TypedDict(
     "GetPublicKeyConfigRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPublicKeyConfigOutputTypeDef = TypedDict(
+    "_RequiredPublicKeyConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "Name": str,
+        "EncodedKey": str,
+    },
+)
+_OptionalPublicKeyConfigOutputTypeDef = TypedDict(
+    "_OptionalPublicKeyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class PublicKeyConfigOutputTypeDef(
+    _RequiredPublicKeyConfigOutputTypeDef, _OptionalPublicKeyConfigOutputTypeDef
+):
+    pass
+
 GetPublicKeyRequestRequestTypeDef = TypedDict(
     "GetPublicKeyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1408,14 +1897,31 @@
 GetStreamingDistributionRequestRequestTypeDef = TypedDict(
     "GetStreamingDistributionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+_RequiredPathsOutputTypeDef = TypedDict(
+    "_RequiredPathsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalPathsOutputTypeDef = TypedDict(
+    "_OptionalPathsOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class PathsOutputTypeDef(_RequiredPathsOutputTypeDef, _OptionalPathsOutputTypeDef):
+    pass
+
 _RequiredPathsTypeDef = TypedDict(
     "_RequiredPathsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalPathsTypeDef = TypedDict(
@@ -1451,14 +1957,34 @@
     },
     total=False,
 )
 
 class KeyPairIdsTypeDef(_RequiredKeyPairIdsTypeDef, _OptionalKeyPairIdsTypeDef):
     pass
 
+_RequiredLambdaFunctionAssociationOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationOutputTypeDef",
+    {
+        "LambdaFunctionARN": str,
+        "EventType": EventTypeType,
+    },
+)
+_OptionalLambdaFunctionAssociationOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationOutputTypeDef",
+    {
+        "IncludeBody": bool,
+    },
+    total=False,
+)
+
+class LambdaFunctionAssociationOutputTypeDef(
+    _RequiredLambdaFunctionAssociationOutputTypeDef, _OptionalLambdaFunctionAssociationOutputTypeDef
+):
+    pass
+
 _RequiredLambdaFunctionAssociationTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationTypeDef",
     {
         "LambdaFunctionARN": str,
         "EventType": EventTypeType,
     },
 )
@@ -1810,14 +2336,21 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
+RealtimeMetricsSubscriptionConfigOutputTypeDef = TypedDict(
+    "RealtimeMetricsSubscriptionConfigOutputTypeDef",
+    {
+        "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
+    },
+)
+
 RealtimeMetricsSubscriptionConfigTypeDef = TypedDict(
     "RealtimeMetricsSubscriptionConfigTypeDef",
     {
         "RealtimeMetricsSubscriptionStatus": RealtimeMetricsSubscriptionStatusType,
     },
 )
 
@@ -1829,29 +2362,70 @@
         "Name": str,
         "SigningProtocol": Literal["sigv4"],
         "SigningBehavior": OriginAccessControlSigningBehaviorsType,
         "OriginAccessControlOriginType": OriginAccessControlOriginTypesType,
     },
 )
 
+StatusCodesOutputTypeDef = TypedDict(
+    "StatusCodesOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[int],
+    },
+)
+
 StatusCodesTypeDef = TypedDict(
     "StatusCodesTypeDef",
     {
         "Quantity": int,
-        "Items": List[int],
+        "Items": Sequence[int],
+    },
+)
+
+OriginGroupMemberOutputTypeDef = TypedDict(
+    "OriginGroupMemberOutputTypeDef",
+    {
+        "OriginId": str,
     },
 )
 
 OriginGroupMemberTypeDef = TypedDict(
     "OriginGroupMemberTypeDef",
     {
         "OriginId": str,
     },
 )
 
+_RequiredOriginShieldOutputTypeDef = TypedDict(
+    "_RequiredOriginShieldOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalOriginShieldOutputTypeDef = TypedDict(
+    "_OptionalOriginShieldOutputTypeDef",
+    {
+        "OriginShieldRegion": str,
+    },
+    total=False,
+)
+
+class OriginShieldOutputTypeDef(
+    _RequiredOriginShieldOutputTypeDef, _OptionalOriginShieldOutputTypeDef
+):
+    pass
+
+S3OriginConfigOutputTypeDef = TypedDict(
+    "S3OriginConfigOutputTypeDef",
+    {
+        "OriginAccessIdentity": str,
+    },
+)
+
 _RequiredOriginShieldTypeDef = TypedDict(
     "_RequiredOriginShieldTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalOriginShieldTypeDef = TypedDict(
@@ -1906,46 +2480,98 @@
     "PublishFunctionRequestRequestTypeDef",
     {
         "Name": str,
         "IfMatch": str,
     },
 )
 
+QueryArgProfileOutputTypeDef = TypedDict(
+    "QueryArgProfileOutputTypeDef",
+    {
+        "QueryArg": str,
+        "ProfileId": str,
+    },
+)
+
 QueryArgProfileTypeDef = TypedDict(
     "QueryArgProfileTypeDef",
     {
         "QueryArg": str,
         "ProfileId": str,
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowHeadersTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowHeadersTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowMethodsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowMethodsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[ResponseHeadersPolicyAccessControlAllowMethodsValuesType],
     },
 )
 
+ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[str],
+    },
+)
+
 ResponseHeadersPolicyAccessControlAllowOriginsTypeDef = TypedDict(
     "ResponseHeadersPolicyAccessControlAllowOriginsTypeDef",
     {
         "Quantity": int,
         "Items": Sequence[str],
     },
 )
 
+_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef",
+    {
+        "Items": List[str],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef(
+    _RequiredResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+    _OptionalResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef = TypedDict(
@@ -1958,14 +2584,34 @@
 
 class ResponseHeadersPolicyAccessControlExposeHeadersTypeDef(
     _RequiredResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
     _OptionalResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
 ):
     pass
 
+_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+    },
+)
+_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef",
+    {
+        "SamplingRate": float,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef = TypedDict(
@@ -1978,61 +2624,152 @@
 
 class ResponseHeadersPolicyServerTimingHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
 ):
     pass
 
+ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef",
+    {
+        "Override": bool,
+        "ContentSecurityPolicy": str,
+    },
+)
+
 ResponseHeadersPolicyContentSecurityPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyContentSecurityPolicyTypeDef",
     {
         "Override": bool,
         "ContentSecurityPolicy": str,
     },
 )
 
+ResponseHeadersPolicyContentTypeOptionsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyContentTypeOptionsOutputTypeDef",
+    {
+        "Override": bool,
+    },
+)
+
 ResponseHeadersPolicyContentTypeOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyContentTypeOptionsTypeDef",
     {
         "Override": bool,
     },
 )
 
+ResponseHeadersPolicyCustomHeaderOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyCustomHeaderOutputTypeDef",
+    {
+        "Header": str,
+        "Value": str,
+        "Override": bool,
+    },
+)
+
 ResponseHeadersPolicyCustomHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyCustomHeaderTypeDef",
     {
         "Header": str,
         "Value": str,
         "Override": bool,
     },
 )
 
+ResponseHeadersPolicyFrameOptionsOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyFrameOptionsOutputTypeDef",
+    {
+        "Override": bool,
+        "FrameOption": FrameOptionsListType,
+    },
+)
+
 ResponseHeadersPolicyFrameOptionsTypeDef = TypedDict(
     "ResponseHeadersPolicyFrameOptionsTypeDef",
     {
         "Override": bool,
         "FrameOption": FrameOptionsListType,
     },
 )
 
+ResponseHeadersPolicyReferrerPolicyOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyReferrerPolicyOutputTypeDef",
+    {
+        "Override": bool,
+        "ReferrerPolicy": ReferrerPolicyListType,
+    },
+)
+
 ResponseHeadersPolicyReferrerPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyReferrerPolicyTypeDef",
     {
         "Override": bool,
         "ReferrerPolicy": ReferrerPolicyListType,
     },
 )
 
+ResponseHeadersPolicyRemoveHeaderOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicyRemoveHeaderOutputTypeDef",
+    {
+        "Header": str,
+    },
+)
+
 ResponseHeadersPolicyRemoveHeaderTypeDef = TypedDict(
     "ResponseHeadersPolicyRemoveHeaderTypeDef",
     {
         "Header": str,
     },
 )
 
+_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    {
+        "Override": bool,
+        "AccessControlMaxAgeSec": int,
+    },
+)
+_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef",
+    {
+        "IncludeSubdomains": bool,
+        "Preload": bool,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef(
+    _RequiredResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    _OptionalResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+):
+    pass
+
+_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef",
+    {
+        "Override": bool,
+        "Protection": bool,
+    },
+)
+_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef",
+    {
+        "ModeBlock": bool,
+        "ReportUri": str,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyXSSProtectionOutputTypeDef(
+    _RequiredResponseHeadersPolicyXSSProtectionOutputTypeDef,
+    _OptionalResponseHeadersPolicyXSSProtectionOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyStrictTransportSecurityTypeDef",
     {
         "Override": bool,
         "AccessControlMaxAgeSec": int,
     },
 )
@@ -2080,22 +2817,39 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+S3OriginOutputTypeDef = TypedDict(
+    "S3OriginOutputTypeDef",
+    {
+        "DomainName": str,
+        "OriginAccessIdentity": str,
+    },
+)
+
 S3OriginTypeDef = TypedDict(
     "S3OriginTypeDef",
     {
         "DomainName": str,
         "OriginAccessIdentity": str,
     },
 )
 
+StreamingLoggingConfigOutputTypeDef = TypedDict(
+    "StreamingLoggingConfigOutputTypeDef",
+    {
+        "Enabled": bool,
+        "Bucket": str,
+        "Prefix": str,
+    },
+)
+
 StreamingLoggingConfigTypeDef = TypedDict(
     "StreamingLoggingConfigTypeDef",
     {
         "Enabled": bool,
         "Bucket": str,
         "Prefix": str,
     },
@@ -2105,14 +2859,31 @@
     "TagKeysTypeDef",
     {
         "Items": Sequence[str],
     },
     total=False,
 )
 
+_RequiredTagOutputTypeDef = TypedDict(
+    "_RequiredTagOutputTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalTagOutputTypeDef = TypedDict(
+    "_OptionalTagOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
+    pass
+
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -2164,32 +2935,110 @@
 
 class UpdateDistributionWithStagingConfigRequestRequestTypeDef(
     _RequiredUpdateDistributionWithStagingConfigRequestRequestTypeDef,
     _OptionalUpdateDistributionWithStagingConfigRequestRequestTypeDef,
 ):
     pass
 
+_RequiredAllowedMethodsOutputTypeDef = TypedDict(
+    "_RequiredAllowedMethodsOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[MethodType],
+    },
+)
+_OptionalAllowedMethodsOutputTypeDef = TypedDict(
+    "_OptionalAllowedMethodsOutputTypeDef",
+    {
+        "CachedMethods": CachedMethodsOutputTypeDef,
+    },
+    total=False,
+)
+
+class AllowedMethodsOutputTypeDef(
+    _RequiredAllowedMethodsOutputTypeDef, _OptionalAllowedMethodsOutputTypeDef
+):
+    pass
+
 _RequiredAllowedMethodsTypeDef = TypedDict(
     "_RequiredAllowedMethodsTypeDef",
     {
         "Quantity": int,
-        "Items": List[MethodType],
+        "Items": Sequence[MethodType],
     },
 )
 _OptionalAllowedMethodsTypeDef = TypedDict(
     "_OptionalAllowedMethodsTypeDef",
     {
         "CachedMethods": CachedMethodsTypeDef,
     },
     total=False,
 )
 
 class AllowedMethodsTypeDef(_RequiredAllowedMethodsTypeDef, _OptionalAllowedMethodsTypeDef):
     pass
 
+_RequiredCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": CachePolicyCookieBehaviorType,
+    },
+)
+_OptionalCachePolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyCookiesConfigOutputTypeDef(
+    _RequiredCachePolicyCookiesConfigOutputTypeDef, _OptionalCachePolicyCookiesConfigOutputTypeDef
+):
+    pass
+
+_RequiredCookiePreferenceOutputTypeDef = TypedDict(
+    "_RequiredCookiePreferenceOutputTypeDef",
+    {
+        "Forward": ItemSelectionType,
+    },
+)
+_OptionalCookiePreferenceOutputTypeDef = TypedDict(
+    "_OptionalCookiePreferenceOutputTypeDef",
+    {
+        "WhitelistedNames": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class CookiePreferenceOutputTypeDef(
+    _RequiredCookiePreferenceOutputTypeDef, _OptionalCookiePreferenceOutputTypeDef
+):
+    pass
+
+_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "CookieBehavior": OriginRequestPolicyCookieBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyCookiesConfigOutputTypeDef",
+    {
+        "Cookies": CookieNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyCookiesConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyCookiesConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyCookiesConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCachePolicyCookiesConfigTypeDef = TypedDict(
     "_RequiredCachePolicyCookiesConfigTypeDef",
     {
         "CookieBehavior": CachePolicyCookieBehaviorType,
     },
 )
 _OptionalCachePolicyCookiesConfigTypeDef = TypedDict(
@@ -2238,14 +3087,53 @@
 
 class OriginRequestPolicyCookiesConfigTypeDef(
     _RequiredOriginRequestPolicyCookiesConfigTypeDef,
     _OptionalOriginRequestPolicyCookiesConfigTypeDef,
 ):
     pass
 
+_RequiredCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": CachePolicyHeaderBehaviorType,
+    },
+)
+_OptionalCachePolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyHeadersConfigOutputTypeDef(
+    _RequiredCachePolicyHeadersConfigOutputTypeDef, _OptionalCachePolicyHeadersConfigOutputTypeDef
+):
+    pass
+
+_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "HeaderBehavior": OriginRequestPolicyHeaderBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyHeadersConfigOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyHeadersConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyHeadersConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyHeadersConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCachePolicyHeadersConfigTypeDef = TypedDict(
     "_RequiredCachePolicyHeadersConfigTypeDef",
     {
         "HeaderBehavior": CachePolicyHeaderBehaviorType,
     },
 )
 _OptionalCachePolicyHeadersConfigTypeDef = TypedDict(
@@ -2277,14 +3165,54 @@
 
 class OriginRequestPolicyHeadersConfigTypeDef(
     _RequiredOriginRequestPolicyHeadersConfigTypeDef,
     _OptionalOriginRequestPolicyHeadersConfigTypeDef,
 ):
     pass
 
+_RequiredCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
+    },
+)
+_OptionalCachePolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyQueryStringsConfigOutputTypeDef(
+    _RequiredCachePolicyQueryStringsConfigOutputTypeDef,
+    _OptionalCachePolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
+_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStringBehavior": OriginRequestPolicyQueryStringBehaviorType,
+    },
+)
+_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef",
+    {
+        "QueryStrings": QueryStringNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyQueryStringsConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    _OptionalOriginRequestPolicyQueryStringsConfigOutputTypeDef,
+):
+    pass
+
 _RequiredCachePolicyQueryStringsConfigTypeDef = TypedDict(
     "_RequiredCachePolicyQueryStringsConfigTypeDef",
     {
         "QueryStringBehavior": CachePolicyQueryStringBehaviorType,
     },
 )
 _OptionalCachePolicyQueryStringsConfigTypeDef = TypedDict(
@@ -2326,37 +3254,37 @@
         "Id": str,
         "S3CanonicalUserId": str,
     },
 )
 _OptionalCloudFrontOriginAccessIdentityTypeDef = TypedDict(
     "_OptionalCloudFrontOriginAccessIdentityTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     },
     total=False,
 )
 
 class CloudFrontOriginAccessIdentityTypeDef(
     _RequiredCloudFrontOriginAccessIdentityTypeDef, _OptionalCloudFrontOriginAccessIdentityTypeDef
 ):
     pass
 
-CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
-    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
+GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
+    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
     {
-        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
+        "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetCloudFrontOriginAccessIdentityConfigResultTypeDef = TypedDict(
-    "GetCloudFrontOriginAccessIdentityConfigResultTypeDef",
+CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
+    "CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef",
     {
         "CloudFrontOriginAccessIdentityConfig": CloudFrontOriginAccessIdentityConfigTypeDef,
@@ -2408,14 +3336,33 @@
         "MaxItems": int,
         "Quantity": int,
         "Items": List[ConflictingAliasTypeDef],
     },
     total=False,
 )
 
+_RequiredContentTypeProfilesOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalContentTypeProfilesOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfilesOutputTypeDef",
+    {
+        "Items": List[ContentTypeProfileOutputTypeDef],
+    },
+    total=False,
+)
+
+class ContentTypeProfilesOutputTypeDef(
+    _RequiredContentTypeProfilesOutputTypeDef, _OptionalContentTypeProfilesOutputTypeDef
+):
+    pass
+
 _RequiredContentTypeProfilesTypeDef = TypedDict(
     "_RequiredContentTypeProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalContentTypeProfilesTypeDef = TypedDict(
@@ -2427,14 +3374,34 @@
 )
 
 class ContentTypeProfilesTypeDef(
     _RequiredContentTypeProfilesTypeDef, _OptionalContentTypeProfilesTypeDef
 ):
     pass
 
+_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef",
+    {
+        "Weight": float,
+    },
+)
+_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef",
+    {
+        "SessionStickinessConfig": SessionStickinessConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class ContinuousDeploymentSingleWeightConfigOutputTypeDef(
+    _RequiredContinuousDeploymentSingleWeightConfigOutputTypeDef,
+    _OptionalContinuousDeploymentSingleWeightConfigOutputTypeDef,
+):
+    pass
+
 _RequiredContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentSingleWeightConfigTypeDef",
     {
         "Weight": float,
     },
 )
 _OptionalContinuousDeploymentSingleWeightConfigTypeDef = TypedDict(
@@ -2473,32 +3440,14 @@
 CreateKeyGroupRequestRequestTypeDef = TypedDict(
     "CreateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
     },
 )
 
-GetKeyGroupConfigResultTypeDef = TypedDict(
-    "GetKeyGroupConfigResultTypeDef",
-    {
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-KeyGroupTypeDef = TypedDict(
-    "KeyGroupTypeDef",
-    {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "KeyGroupConfig": KeyGroupConfigTypeDef,
-    },
-)
-
 _RequiredUpdateKeyGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKeyGroupRequestRequestTypeDef",
     {
         "KeyGroupConfig": KeyGroupConfigTypeDef,
         "Id": str,
     },
 )
@@ -2518,42 +3467,14 @@
 CreateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "CreateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
     },
 )
 
-GetOriginAccessControlConfigResultTypeDef = TypedDict(
-    "GetOriginAccessControlConfigResultTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredOriginAccessControlTypeDef = TypedDict(
-    "_RequiredOriginAccessControlTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalOriginAccessControlTypeDef = TypedDict(
-    "_OptionalOriginAccessControlTypeDef",
-    {
-        "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
-    },
-    total=False,
-)
-
-class OriginAccessControlTypeDef(
-    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
-):
-    pass
-
 _RequiredUpdateOriginAccessControlRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginAccessControlRequestRequestTypeDef",
     {
         "OriginAccessControlConfig": OriginAccessControlConfigTypeDef,
         "Id": str,
     },
 )
@@ -2574,32 +3495,14 @@
 CreatePublicKeyRequestRequestTypeDef = TypedDict(
     "CreatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
     },
 )
 
-GetPublicKeyConfigResultTypeDef = TypedDict(
-    "GetPublicKeyConfigResultTypeDef",
-    {
-        "PublicKeyConfig": PublicKeyConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PublicKeyTypeDef = TypedDict(
-    "PublicKeyTypeDef",
-    {
-        "Id": str,
-        "CreatedTime": datetime,
-        "PublicKeyConfig": PublicKeyConfigTypeDef,
-    },
-)
-
 _RequiredUpdatePublicKeyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublicKeyRequestRequestTypeDef",
     {
         "PublicKeyConfig": PublicKeyConfigTypeDef,
         "Id": str,
     },
 )
@@ -2612,50 +3515,111 @@
 )
 
 class UpdatePublicKeyRequestRequestTypeDef(
     _RequiredUpdatePublicKeyRequestRequestTypeDef, _OptionalUpdatePublicKeyRequestRequestTypeDef
 ):
     pass
 
+_RequiredCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_RequiredCustomErrorResponsesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomErrorResponsesOutputTypeDef = TypedDict(
+    "_OptionalCustomErrorResponsesOutputTypeDef",
+    {
+        "Items": List[CustomErrorResponseOutputTypeDef],
+    },
+    total=False,
+)
+
+class CustomErrorResponsesOutputTypeDef(
+    _RequiredCustomErrorResponsesOutputTypeDef, _OptionalCustomErrorResponsesOutputTypeDef
+):
+    pass
+
 _RequiredCustomErrorResponsesTypeDef = TypedDict(
     "_RequiredCustomErrorResponsesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomErrorResponsesTypeDef = TypedDict(
     "_OptionalCustomErrorResponsesTypeDef",
     {
-        "Items": List[CustomErrorResponseTypeDef],
+        "Items": Sequence[CustomErrorResponseTypeDef],
     },
     total=False,
 )
 
 class CustomErrorResponsesTypeDef(
     _RequiredCustomErrorResponsesTypeDef, _OptionalCustomErrorResponsesTypeDef
 ):
     pass
 
+_RequiredCustomHeadersOutputTypeDef = TypedDict(
+    "_RequiredCustomHeadersOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCustomHeadersOutputTypeDef = TypedDict(
+    "_OptionalCustomHeadersOutputTypeDef",
+    {
+        "Items": List[OriginCustomHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+class CustomHeadersOutputTypeDef(
+    _RequiredCustomHeadersOutputTypeDef, _OptionalCustomHeadersOutputTypeDef
+):
+    pass
+
 _RequiredCustomHeadersTypeDef = TypedDict(
     "_RequiredCustomHeadersTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCustomHeadersTypeDef = TypedDict(
     "_OptionalCustomHeadersTypeDef",
     {
-        "Items": List[OriginCustomHeaderTypeDef],
+        "Items": Sequence[OriginCustomHeaderTypeDef],
     },
     total=False,
 )
 
 class CustomHeadersTypeDef(_RequiredCustomHeadersTypeDef, _OptionalCustomHeadersTypeDef):
     pass
 
+_RequiredCustomOriginConfigOutputTypeDef = TypedDict(
+    "_RequiredCustomOriginConfigOutputTypeDef",
+    {
+        "HTTPPort": int,
+        "HTTPSPort": int,
+        "OriginProtocolPolicy": OriginProtocolPolicyType,
+    },
+)
+_OptionalCustomOriginConfigOutputTypeDef = TypedDict(
+    "_OptionalCustomOriginConfigOutputTypeDef",
+    {
+        "OriginSslProtocols": OriginSslProtocolsOutputTypeDef,
+        "OriginReadTimeout": int,
+        "OriginKeepaliveTimeout": int,
+    },
+    total=False,
+)
+
+class CustomOriginConfigOutputTypeDef(
+    _RequiredCustomOriginConfigOutputTypeDef, _OptionalCustomOriginConfigOutputTypeDef
+):
+    pass
+
 _RequiredCustomOriginConfigTypeDef = TypedDict(
     "_RequiredCustomOriginConfigTypeDef",
     {
         "HTTPPort": int,
         "HTTPSPort": int,
         "OriginProtocolPolicy": OriginProtocolPolicyType,
     },
@@ -2703,23 +3667,49 @@
     "ListDistributionsByResponseHeadersPolicyIdResultTypeDef",
     {
         "DistributionIdList": DistributionIdListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EncryptionEntityOutputTypeDef = TypedDict(
+    "EncryptionEntityOutputTypeDef",
+    {
+        "PublicKeyId": str,
+        "ProviderId": str,
+        "FieldPatterns": FieldPatternsOutputTypeDef,
+    },
+)
+
 EncryptionEntityTypeDef = TypedDict(
     "EncryptionEntityTypeDef",
     {
         "PublicKeyId": str,
         "ProviderId": str,
         "FieldPatterns": FieldPatternsTypeDef,
     },
 )
 
+_RequiredEndPointOutputTypeDef = TypedDict(
+    "_RequiredEndPointOutputTypeDef",
+    {
+        "StreamType": str,
+    },
+)
+_OptionalEndPointOutputTypeDef = TypedDict(
+    "_OptionalEndPointOutputTypeDef",
+    {
+        "KinesisStreamConfig": KinesisStreamConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class EndPointOutputTypeDef(_RequiredEndPointOutputTypeDef, _OptionalEndPointOutputTypeDef):
+    pass
+
 _RequiredEndPointTypeDef = TypedDict(
     "_RequiredEndPointTypeDef",
     {
         "StreamType": str,
     },
 )
 _OptionalEndPointTypeDef = TypedDict(
@@ -2729,52 +3719,78 @@
     },
     total=False,
 )
 
 class EndPointTypeDef(_RequiredEndPointTypeDef, _OptionalEndPointTypeDef):
     pass
 
+_RequiredFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[FunctionAssociationOutputTypeDef],
+    },
+    total=False,
+)
+
+class FunctionAssociationsOutputTypeDef(
+    _RequiredFunctionAssociationsOutputTypeDef, _OptionalFunctionAssociationsOutputTypeDef
+):
+    pass
+
 _RequiredFunctionAssociationsTypeDef = TypedDict(
     "_RequiredFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalFunctionAssociationsTypeDef = TypedDict(
     "_OptionalFunctionAssociationsTypeDef",
     {
-        "Items": List[FunctionAssociationTypeDef],
+        "Items": Sequence[FunctionAssociationTypeDef],
     },
     total=False,
 )
 
 class FunctionAssociationsTypeDef(
     _RequiredFunctionAssociationsTypeDef, _OptionalFunctionAssociationsTypeDef
 ):
     pass
 
 _RequiredFunctionSummaryTypeDef = TypedDict(
     "_RequiredFunctionSummaryTypeDef",
     {
         "Name": str,
-        "FunctionConfig": FunctionConfigTypeDef,
+        "FunctionConfig": FunctionConfigOutputTypeDef,
         "FunctionMetadata": FunctionMetadataTypeDef,
     },
 )
 _OptionalFunctionSummaryTypeDef = TypedDict(
     "_OptionalFunctionSummaryTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
 class FunctionSummaryTypeDef(_RequiredFunctionSummaryTypeDef, _OptionalFunctionSummaryTypeDef):
     pass
 
+RestrictionsOutputTypeDef = TypedDict(
+    "RestrictionsOutputTypeDef",
+    {
+        "GeoRestriction": GeoRestrictionOutputTypeDef,
+    },
+)
+
 RestrictionsTypeDef = TypedDict(
     "RestrictionsTypeDef",
     {
         "GeoRestriction": GeoRestrictionTypeDef,
     },
 )
 
@@ -2835,14 +3851,86 @@
 
 class GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef(
     _RequiredGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
     _OptionalGetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
 ):
     pass
 
+GetKeyGroupConfigResultTypeDef = TypedDict(
+    "GetKeyGroupConfigResultTypeDef",
+    {
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+KeyGroupTypeDef = TypedDict(
+    "KeyGroupTypeDef",
+    {
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "KeyGroupConfig": KeyGroupConfigOutputTypeDef,
+    },
+)
+
+GetOriginAccessControlConfigResultTypeDef = TypedDict(
+    "GetOriginAccessControlConfigResultTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredOriginAccessControlTypeDef = TypedDict(
+    "_RequiredOriginAccessControlTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalOriginAccessControlTypeDef = TypedDict(
+    "_OptionalOriginAccessControlTypeDef",
+    {
+        "OriginAccessControlConfig": OriginAccessControlConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class OriginAccessControlTypeDef(
+    _RequiredOriginAccessControlTypeDef, _OptionalOriginAccessControlTypeDef
+):
+    pass
+
+GetPublicKeyConfigResultTypeDef = TypedDict(
+    "GetPublicKeyConfigResultTypeDef",
+    {
+        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PublicKeyTypeDef = TypedDict(
+    "PublicKeyTypeDef",
+    {
+        "Id": str,
+        "CreatedTime": datetime,
+        "PublicKeyConfig": PublicKeyConfigOutputTypeDef,
+    },
+)
+
+InvalidationBatchOutputTypeDef = TypedDict(
+    "InvalidationBatchOutputTypeDef",
+    {
+        "Paths": PathsOutputTypeDef,
+        "CallerReference": str,
+    },
+)
+
 InvalidationBatchTypeDef = TypedDict(
     "InvalidationBatchTypeDef",
     {
         "Paths": PathsTypeDef,
         "CallerReference": str,
     },
 )
@@ -2882,33 +3970,61 @@
     {
         "AwsAccountNumber": str,
         "KeyPairIds": KeyPairIdsTypeDef,
     },
     total=False,
 )
 
+_RequiredLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_RequiredLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalLambdaFunctionAssociationsOutputTypeDef = TypedDict(
+    "_OptionalLambdaFunctionAssociationsOutputTypeDef",
+    {
+        "Items": List[LambdaFunctionAssociationOutputTypeDef],
+    },
+    total=False,
+)
+
+class LambdaFunctionAssociationsOutputTypeDef(
+    _RequiredLambdaFunctionAssociationsOutputTypeDef,
+    _OptionalLambdaFunctionAssociationsOutputTypeDef,
+):
+    pass
+
 _RequiredLambdaFunctionAssociationsTypeDef = TypedDict(
     "_RequiredLambdaFunctionAssociationsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalLambdaFunctionAssociationsTypeDef = TypedDict(
     "_OptionalLambdaFunctionAssociationsTypeDef",
     {
-        "Items": List[LambdaFunctionAssociationTypeDef],
+        "Items": Sequence[LambdaFunctionAssociationTypeDef],
     },
     total=False,
 )
 
 class LambdaFunctionAssociationsTypeDef(
     _RequiredLambdaFunctionAssociationsTypeDef, _OptionalLambdaFunctionAssociationsTypeDef
 ):
     pass
 
+MonitoringSubscriptionOutputTypeDef = TypedDict(
+    "MonitoringSubscriptionOutputTypeDef",
+    {
+        "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 MonitoringSubscriptionTypeDef = TypedDict(
     "MonitoringSubscriptionTypeDef",
     {
         "RealtimeMetricsSubscriptionConfig": RealtimeMetricsSubscriptionConfigTypeDef,
     },
     total=False,
 )
@@ -2932,26 +4048,41 @@
 )
 
 class OriginAccessControlListTypeDef(
     _RequiredOriginAccessControlListTypeDef, _OptionalOriginAccessControlListTypeDef
 ):
     pass
 
+OriginGroupFailoverCriteriaOutputTypeDef = TypedDict(
+    "OriginGroupFailoverCriteriaOutputTypeDef",
+    {
+        "StatusCodes": StatusCodesOutputTypeDef,
+    },
+)
+
 OriginGroupFailoverCriteriaTypeDef = TypedDict(
     "OriginGroupFailoverCriteriaTypeDef",
     {
         "StatusCodes": StatusCodesTypeDef,
     },
 )
 
+OriginGroupMembersOutputTypeDef = TypedDict(
+    "OriginGroupMembersOutputTypeDef",
+    {
+        "Quantity": int,
+        "Items": List[OriginGroupMemberOutputTypeDef],
+    },
+)
+
 OriginGroupMembersTypeDef = TypedDict(
     "OriginGroupMembersTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginGroupMemberTypeDef],
+        "Items": Sequence[OriginGroupMemberTypeDef],
     },
 )
 
 _RequiredPublicKeyListTypeDef = TypedDict(
     "_RequiredPublicKeyListTypeDef",
     {
         "MaxItems": int,
@@ -2966,14 +4097,33 @@
     },
     total=False,
 )
 
 class PublicKeyListTypeDef(_RequiredPublicKeyListTypeDef, _OptionalPublicKeyListTypeDef):
     pass
 
+_RequiredQueryArgProfilesOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfilesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalQueryArgProfilesOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfilesOutputTypeDef",
+    {
+        "Items": List[QueryArgProfileOutputTypeDef],
+    },
+    total=False,
+)
+
+class QueryArgProfilesOutputTypeDef(
+    _RequiredQueryArgProfilesOutputTypeDef, _OptionalQueryArgProfilesOutputTypeDef
+):
+    pass
+
 _RequiredQueryArgProfilesTypeDef = TypedDict(
     "_RequiredQueryArgProfilesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalQueryArgProfilesTypeDef = TypedDict(
@@ -2983,14 +4133,39 @@
     },
     total=False,
 )
 
 class QueryArgProfilesTypeDef(_RequiredQueryArgProfilesTypeDef, _OptionalQueryArgProfilesTypeDef):
     pass
 
+_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
+        "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
+        "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
+        "AccessControlAllowCredentials": bool,
+        "OriginOverride": bool,
+    },
+)
+_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCorsConfigOutputTypeDef",
+    {
+        "AccessControlExposeHeaders": ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
+        "AccessControlMaxAgeSec": int,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyCorsConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCorsConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCorsConfigOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyCorsConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCorsConfigTypeDef",
     {
         "AccessControlAllowOrigins": ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
         "AccessControlAllowHeaders": ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
         "AccessControlAllowMethods": ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
         "AccessControlAllowCredentials": bool,
@@ -3007,14 +4182,34 @@
 )
 
 class ResponseHeadersPolicyCorsConfigTypeDef(
     _RequiredResponseHeadersPolicyCorsConfigTypeDef, _OptionalResponseHeadersPolicyCorsConfigTypeDef
 ):
     pass
 
+_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyCustomHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef = TypedDict(
@@ -3027,14 +4222,34 @@
 
 class ResponseHeadersPolicyCustomHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyCustomHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyCustomHeadersConfigTypeDef,
 ):
     pass
 
+_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef",
+    {
+        "Items": List[ResponseHeadersPolicyRemoveHeaderOutputTypeDef],
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef = TypedDict(
@@ -3047,14 +4262,27 @@
 
 class ResponseHeadersPolicyRemoveHeadersConfigTypeDef(
     _RequiredResponseHeadersPolicyRemoveHeadersConfigTypeDef,
     _OptionalResponseHeadersPolicyRemoveHeadersConfigTypeDef,
 ):
     pass
 
+ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef = TypedDict(
+    "ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef",
+    {
+        "XSSProtection": ResponseHeadersPolicyXSSProtectionOutputTypeDef,
+        "FrameOptions": ResponseHeadersPolicyFrameOptionsOutputTypeDef,
+        "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
+        "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
+        "ContentTypeOptions": ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
+        "StrictTransportSecurity": ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    },
+    total=False,
+)
+
 ResponseHeadersPolicySecurityHeadersConfigTypeDef = TypedDict(
     "ResponseHeadersPolicySecurityHeadersConfigTypeDef",
     {
         "XSSProtection": ResponseHeadersPolicyXSSProtectionTypeDef,
         "FrameOptions": ResponseHeadersPolicyFrameOptionsTypeDef,
         "ReferrerPolicy": ResponseHeadersPolicyReferrerPolicyTypeDef,
         "ContentSecurityPolicy": ResponseHeadersPolicyContentSecurityPolicyTypeDef,
@@ -3068,23 +4296,49 @@
     "StreamingDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "S3Origin": S3OriginTypeDef,
-        "Aliases": AliasesTypeDef,
-        "TrustedSigners": TrustedSignersTypeDef,
+        "S3Origin": S3OriginOutputTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
     },
 )
 
+_RequiredStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredStreamingDistributionConfigOutputTypeDef",
+    {
+        "CallerReference": str,
+        "S3Origin": S3OriginOutputTypeDef,
+        "Comment": str,
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalStreamingDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalStreamingDistributionConfigOutputTypeDef",
+    {
+        "Aliases": AliasesOutputTypeDef,
+        "Logging": StreamingLoggingConfigOutputTypeDef,
+        "PriceClass": PriceClassType,
+    },
+    total=False,
+)
+
+class StreamingDistributionConfigOutputTypeDef(
+    _RequiredStreamingDistributionConfigOutputTypeDef,
+    _OptionalStreamingDistributionConfigOutputTypeDef,
+):
+    pass
+
 _RequiredStreamingDistributionConfigTypeDef = TypedDict(
     "_RequiredStreamingDistributionConfigTypeDef",
     {
         "CallerReference": str,
         "S3Origin": S3OriginTypeDef,
         "Comment": str,
         "TrustedSigners": TrustedSignersTypeDef,
@@ -3110,22 +4364,51 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": TagKeysTypeDef,
     },
 )
 
+TagsOutputTypeDef = TypedDict(
+    "TagsOutputTypeDef",
+    {
+        "Items": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
 TagsTypeDef = TypedDict(
     "TagsTypeDef",
     {
         "Items": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredForwardedValuesOutputTypeDef = TypedDict(
+    "_RequiredForwardedValuesOutputTypeDef",
+    {
+        "QueryString": bool,
+        "Cookies": CookiePreferenceOutputTypeDef,
+    },
+)
+_OptionalForwardedValuesOutputTypeDef = TypedDict(
+    "_OptionalForwardedValuesOutputTypeDef",
+    {
+        "Headers": HeadersOutputTypeDef,
+        "QueryStringCacheKeys": QueryStringCacheKeysOutputTypeDef,
+    },
+    total=False,
+)
+
+class ForwardedValuesOutputTypeDef(
+    _RequiredForwardedValuesOutputTypeDef, _OptionalForwardedValuesOutputTypeDef
+):
+    pass
+
 _RequiredForwardedValuesTypeDef = TypedDict(
     "_RequiredForwardedValuesTypeDef",
     {
         "QueryString": bool,
         "Cookies": CookiePreferenceTypeDef,
     },
 )
@@ -3137,14 +4420,59 @@
     },
     total=False,
 )
 
 class ForwardedValuesTypeDef(_RequiredForwardedValuesTypeDef, _OptionalForwardedValuesTypeDef):
     pass
 
+_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingGzip": bool,
+        "HeadersConfig": CachePolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": CachePolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": CachePolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef = TypedDict(
+    "_OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef",
+    {
+        "EnableAcceptEncodingBrotli": bool,
+    },
+    total=False,
+)
+
+class ParametersInCacheKeyAndForwardedToOriginOutputTypeDef(
+    _RequiredParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    _OptionalParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+):
+    pass
+
+_RequiredOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+        "HeadersConfig": OriginRequestPolicyHeadersConfigOutputTypeDef,
+        "CookiesConfig": OriginRequestPolicyCookiesConfigOutputTypeDef,
+        "QueryStringsConfig": OriginRequestPolicyQueryStringsConfigOutputTypeDef,
+    },
+)
+_OptionalOriginRequestPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalOriginRequestPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class OriginRequestPolicyConfigOutputTypeDef(
+    _RequiredOriginRequestPolicyConfigOutputTypeDef, _OptionalOriginRequestPolicyConfigOutputTypeDef
+):
+    pass
+
 _RequiredParametersInCacheKeyAndForwardedToOriginTypeDef = TypedDict(
     "_RequiredParametersInCacheKeyAndForwardedToOriginTypeDef",
     {
         "EnableAcceptEncodingGzip": bool,
         "HeadersConfig": CachePolicyHeadersConfigTypeDef,
         "CookiesConfig": CachePolicyCookiesConfigTypeDef,
         "QueryStringsConfig": CachePolicyQueryStringsConfigTypeDef,
@@ -3226,141 +4554,114 @@
     "ListConflictingAliasesResultTypeDef",
     {
         "ConflictingAliasesList": ConflictingAliasesListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredContentTypeProfileConfigTypeDef = TypedDict(
-    "_RequiredContentTypeProfileConfigTypeDef",
+_RequiredContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredContentTypeProfileConfigOutputTypeDef",
     {
         "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
-_OptionalContentTypeProfileConfigTypeDef = TypedDict(
-    "_OptionalContentTypeProfileConfigTypeDef",
+_OptionalContentTypeProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalContentTypeProfileConfigOutputTypeDef",
     {
-        "ContentTypeProfiles": ContentTypeProfilesTypeDef,
+        "ContentTypeProfiles": ContentTypeProfilesOutputTypeDef,
     },
     total=False,
 )
 
-class ContentTypeProfileConfigTypeDef(
-    _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
+class ContentTypeProfileConfigOutputTypeDef(
+    _RequiredContentTypeProfileConfigOutputTypeDef, _OptionalContentTypeProfileConfigOutputTypeDef
 ):
     pass
 
-_RequiredTrafficConfigTypeDef = TypedDict(
-    "_RequiredTrafficConfigTypeDef",
+_RequiredContentTypeProfileConfigTypeDef = TypedDict(
+    "_RequiredContentTypeProfileConfigTypeDef",
     {
-        "Type": ContinuousDeploymentPolicyTypeType,
+        "ForwardWhenContentTypeIsUnknown": bool,
     },
 )
-_OptionalTrafficConfigTypeDef = TypedDict(
-    "_OptionalTrafficConfigTypeDef",
+_OptionalContentTypeProfileConfigTypeDef = TypedDict(
+    "_OptionalContentTypeProfileConfigTypeDef",
     {
-        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
-        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
+        "ContentTypeProfiles": ContentTypeProfilesTypeDef,
     },
     total=False,
 )
 
-class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
+class ContentTypeProfileConfigTypeDef(
+    _RequiredContentTypeProfileConfigTypeDef, _OptionalContentTypeProfileConfigTypeDef
+):
     pass
 
-CreateKeyGroupResultTypeDef = TypedDict(
-    "CreateKeyGroupResultTypeDef",
+_RequiredTrafficConfigOutputTypeDef = TypedDict(
+    "_RequiredTrafficConfigOutputTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetKeyGroupResultTypeDef = TypedDict(
-    "GetKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-
-KeyGroupSummaryTypeDef = TypedDict(
-    "KeyGroupSummaryTypeDef",
+_OptionalTrafficConfigOutputTypeDef = TypedDict(
+    "_OptionalTrafficConfigOutputTypeDef",
     {
-        "KeyGroup": KeyGroupTypeDef,
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigOutputTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     },
+    total=False,
 )
 
-UpdateKeyGroupResultTypeDef = TypedDict(
-    "UpdateKeyGroupResultTypeDef",
-    {
-        "KeyGroup": KeyGroupTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class TrafficConfigOutputTypeDef(
+    _RequiredTrafficConfigOutputTypeDef, _OptionalTrafficConfigOutputTypeDef
+):
+    pass
 
-CreateOriginAccessControlResultTypeDef = TypedDict(
-    "CreateOriginAccessControlResultTypeDef",
+_RequiredTrafficConfigTypeDef = TypedDict(
+    "_RequiredTrafficConfigTypeDef",
     {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": ContinuousDeploymentPolicyTypeType,
     },
 )
-
-GetOriginAccessControlResultTypeDef = TypedDict(
-    "GetOriginAccessControlResultTypeDef",
+_OptionalTrafficConfigTypeDef = TypedDict(
+    "_OptionalTrafficConfigTypeDef",
     {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SingleWeightConfig": ContinuousDeploymentSingleWeightConfigTypeDef,
+        "SingleHeaderConfig": ContinuousDeploymentSingleHeaderConfigTypeDef,
     },
+    total=False,
 )
 
-UpdateOriginAccessControlResultTypeDef = TypedDict(
-    "UpdateOriginAccessControlResultTypeDef",
-    {
-        "OriginAccessControl": OriginAccessControlTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class TrafficConfigTypeDef(_RequiredTrafficConfigTypeDef, _OptionalTrafficConfigTypeDef):
+    pass
 
-CreatePublicKeyResultTypeDef = TypedDict(
-    "CreatePublicKeyResultTypeDef",
+_RequiredOriginOutputTypeDef = TypedDict(
+    "_RequiredOriginOutputTypeDef",
     {
-        "PublicKey": PublicKeyTypeDef,
-        "Location": str,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "DomainName": str,
     },
 )
-
-GetPublicKeyResultTypeDef = TypedDict(
-    "GetPublicKeyResultTypeDef",
+_OptionalOriginOutputTypeDef = TypedDict(
+    "_OptionalOriginOutputTypeDef",
     {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OriginPath": str,
+        "CustomHeaders": CustomHeadersOutputTypeDef,
+        "S3OriginConfig": S3OriginConfigOutputTypeDef,
+        "CustomOriginConfig": CustomOriginConfigOutputTypeDef,
+        "ConnectionAttempts": int,
+        "ConnectionTimeout": int,
+        "OriginShield": OriginShieldOutputTypeDef,
+        "OriginAccessControlId": str,
     },
+    total=False,
 )
 
-UpdatePublicKeyResultTypeDef = TypedDict(
-    "UpdatePublicKeyResultTypeDef",
-    {
-        "PublicKey": PublicKeyTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+class OriginOutputTypeDef(_RequiredOriginOutputTypeDef, _OptionalOriginOutputTypeDef):
+    pass
 
 _RequiredOriginTypeDef = TypedDict(
     "_RequiredOriginTypeDef",
     {
         "Id": str,
         "DomainName": str,
     },
@@ -3379,14 +4680,33 @@
     },
     total=False,
 )
 
 class OriginTypeDef(_RequiredOriginTypeDef, _OptionalOriginTypeDef):
     pass
 
+_RequiredEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_RequiredEncryptionEntitiesOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalEncryptionEntitiesOutputTypeDef = TypedDict(
+    "_OptionalEncryptionEntitiesOutputTypeDef",
+    {
+        "Items": List[EncryptionEntityOutputTypeDef],
+    },
+    total=False,
+)
+
+class EncryptionEntitiesOutputTypeDef(
+    _RequiredEncryptionEntitiesOutputTypeDef, _OptionalEncryptionEntitiesOutputTypeDef
+):
+    pass
+
 _RequiredEncryptionEntitiesTypeDef = TypedDict(
     "_RequiredEncryptionEntitiesTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalEncryptionEntitiesTypeDef = TypedDict(
@@ -3398,32 +4718,32 @@
 )
 
 class EncryptionEntitiesTypeDef(
     _RequiredEncryptionEntitiesTypeDef, _OptionalEncryptionEntitiesTypeDef
 ):
     pass
 
-CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
-    "CreateRealtimeLogConfigRequestRequestTypeDef",
+RealtimeLogConfigTypeDef = TypedDict(
+    "RealtimeLogConfigTypeDef",
     {
-        "EndPoints": Sequence[EndPointTypeDef],
-        "Fields": Sequence[str],
+        "ARN": str,
         "Name": str,
         "SamplingRate": int,
+        "EndPoints": List[EndPointOutputTypeDef],
+        "Fields": List[str],
     },
 )
 
-RealtimeLogConfigTypeDef = TypedDict(
-    "RealtimeLogConfigTypeDef",
+CreateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
+    "CreateRealtimeLogConfigRequestRequestTypeDef",
     {
-        "ARN": str,
+        "EndPoints": Sequence[EndPointTypeDef],
+        "Fields": Sequence[str],
         "Name": str,
         "SamplingRate": int,
-        "EndPoints": List[EndPointTypeDef],
-        "Fields": List[str],
     },
 )
 
 UpdateRealtimeLogConfigRequestRequestTypeDef = TypedDict(
     "UpdateRealtimeLogConfigRequestRequestTypeDef",
     {
         "EndPoints": Sequence[EndPointTypeDef],
@@ -3498,28 +4818,119 @@
     {
         "FunctionSummary": FunctionSummaryTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateInvalidationRequestRequestTypeDef = TypedDict(
-    "CreateInvalidationRequestRequestTypeDef",
+CreateKeyGroupResultTypeDef = TypedDict(
+    "CreateKeyGroupResultTypeDef",
     {
-        "DistributionId": str,
-        "InvalidationBatch": InvalidationBatchTypeDef,
+        "KeyGroup": KeyGroupTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetKeyGroupResultTypeDef = TypedDict(
+    "GetKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+KeyGroupSummaryTypeDef = TypedDict(
+    "KeyGroupSummaryTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+    },
+)
+
+UpdateKeyGroupResultTypeDef = TypedDict(
+    "UpdateKeyGroupResultTypeDef",
+    {
+        "KeyGroup": KeyGroupTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateOriginAccessControlResultTypeDef = TypedDict(
+    "CreateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetOriginAccessControlResultTypeDef = TypedDict(
+    "GetOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateOriginAccessControlResultTypeDef = TypedDict(
+    "UpdateOriginAccessControlResultTypeDef",
+    {
+        "OriginAccessControl": OriginAccessControlTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePublicKeyResultTypeDef = TypedDict(
+    "CreatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "Location": str,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPublicKeyResultTypeDef = TypedDict(
+    "GetPublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdatePublicKeyResultTypeDef = TypedDict(
+    "UpdatePublicKeyResultTypeDef",
+    {
+        "PublicKey": PublicKeyTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 InvalidationTypeDef = TypedDict(
     "InvalidationTypeDef",
     {
         "Id": str,
         "Status": str,
         "CreateTime": datetime,
+        "InvalidationBatch": InvalidationBatchOutputTypeDef,
+    },
+)
+
+CreateInvalidationRequestRequestTypeDef = TypedDict(
+    "CreateInvalidationRequestRequestTypeDef",
+    {
+        "DistributionId": str,
         "InvalidationBatch": InvalidationBatchTypeDef,
     },
 )
 
 ListInvalidationsResultTypeDef = TypedDict(
     "ListInvalidationsResultTypeDef",
     {
@@ -3564,46 +4975,55 @@
 )
 
 class ActiveTrustedSignersTypeDef(
     _RequiredActiveTrustedSignersTypeDef, _OptionalActiveTrustedSignersTypeDef
 ):
     pass
 
-CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
-    "CreateMonitoringSubscriptionRequestRequestTypeDef",
-    {
-        "DistributionId": str,
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
-    },
-)
-
 CreateMonitoringSubscriptionResultTypeDef = TypedDict(
     "CreateMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetMonitoringSubscriptionResultTypeDef = TypedDict(
     "GetMonitoringSubscriptionResultTypeDef",
     {
-        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+        "MonitoringSubscription": MonitoringSubscriptionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateMonitoringSubscriptionRequestRequestTypeDef = TypedDict(
+    "CreateMonitoringSubscriptionRequestRequestTypeDef",
+    {
+        "DistributionId": str,
+        "MonitoringSubscription": MonitoringSubscriptionTypeDef,
+    },
+)
+
 ListOriginAccessControlsResultTypeDef = TypedDict(
     "ListOriginAccessControlsResultTypeDef",
     {
         "OriginAccessControlList": OriginAccessControlListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+OriginGroupOutputTypeDef = TypedDict(
+    "OriginGroupOutputTypeDef",
+    {
+        "Id": str,
+        "FailoverCriteria": OriginGroupFailoverCriteriaOutputTypeDef,
+        "Members": OriginGroupMembersOutputTypeDef,
+    },
+)
+
 OriginGroupTypeDef = TypedDict(
     "OriginGroupTypeDef",
     {
         "Id": str,
         "FailoverCriteria": OriginGroupFailoverCriteriaTypeDef,
         "Members": OriginGroupMembersTypeDef,
     },
@@ -3613,14 +5033,33 @@
     "ListPublicKeysResultTypeDef",
     {
         "PublicKeyList": PublicKeyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredQueryArgProfileConfigOutputTypeDef",
+    {
+        "ForwardWhenQueryArgProfileIsUnknown": bool,
+    },
+)
+_OptionalQueryArgProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalQueryArgProfileConfigOutputTypeDef",
+    {
+        "QueryArgProfiles": QueryArgProfilesOutputTypeDef,
+    },
+    total=False,
+)
+
+class QueryArgProfileConfigOutputTypeDef(
+    _RequiredQueryArgProfileConfigOutputTypeDef, _OptionalQueryArgProfileConfigOutputTypeDef
+):
+    pass
+
 _RequiredQueryArgProfileConfigTypeDef = TypedDict(
     "_RequiredQueryArgProfileConfigTypeDef",
     {
         "ForwardWhenQueryArgProfileIsUnknown": bool,
     },
 )
 _OptionalQueryArgProfileConfigTypeDef = TypedDict(
@@ -3632,14 +5071,39 @@
 )
 
 class QueryArgProfileConfigTypeDef(
     _RequiredQueryArgProfileConfigTypeDef, _OptionalQueryArgProfileConfigTypeDef
 ):
     pass
 
+_RequiredResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalResponseHeadersPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalResponseHeadersPolicyConfigOutputTypeDef",
+    {
+        "Comment": str,
+        "CorsConfig": ResponseHeadersPolicyCorsConfigOutputTypeDef,
+        "SecurityHeadersConfig": ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
+        "ServerTimingHeadersConfig": ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
+        "CustomHeadersConfig": ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
+        "RemoveHeadersConfig": ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class ResponseHeadersPolicyConfigOutputTypeDef(
+    _RequiredResponseHeadersPolicyConfigOutputTypeDef,
+    _OptionalResponseHeadersPolicyConfigOutputTypeDef,
+):
+    pass
+
 _RequiredResponseHeadersPolicyConfigTypeDef = TypedDict(
     "_RequiredResponseHeadersPolicyConfigTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalResponseHeadersPolicyConfigTypeDef = TypedDict(
@@ -3679,27 +5143,27 @@
 )
 
 class StreamingDistributionListTypeDef(
     _RequiredStreamingDistributionListTypeDef, _OptionalStreamingDistributionListTypeDef
 ):
     pass
 
-CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
-    "CreateStreamingDistributionRequestRequestTypeDef",
+GetStreamingDistributionConfigResultTypeDef = TypedDict(
+    "GetStreamingDistributionConfigResultTypeDef",
     {
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetStreamingDistributionConfigResultTypeDef = TypedDict(
-    "GetStreamingDistributionConfigResultTypeDef",
+CreateStreamingDistributionRequestRequestTypeDef = TypedDict(
+    "CreateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateStreamingDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingDistributionRequestRequestTypeDef",
     {
         "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
@@ -3719,15 +5183,15 @@
     _OptionalUpdateStreamingDistributionRequestRequestTypeDef,
 ):
     pass
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "Tags": TagsTypeDef,
+        "Tags": TagsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StreamingDistributionConfigWithTagsTypeDef = TypedDict(
     "StreamingDistributionConfigWithTagsTypeDef",
     {
@@ -3740,14 +5204,85 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Resource": str,
         "Tags": TagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorOutputTypeDef",
+    {
+        "PathPattern": str,
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+class CacheBehaviorOutputTypeDef(
+    _RequiredCacheBehaviorOutputTypeDef, _OptionalCacheBehaviorOutputTypeDef
+):
+    pass
+
+_RequiredDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_RequiredDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TargetOriginId": str,
+        "ViewerProtocolPolicy": ViewerProtocolPolicyType,
+    },
+)
+_OptionalDefaultCacheBehaviorOutputTypeDef = TypedDict(
+    "_OptionalDefaultCacheBehaviorOutputTypeDef",
+    {
+        "TrustedSigners": TrustedSignersOutputTypeDef,
+        "TrustedKeyGroups": TrustedKeyGroupsOutputTypeDef,
+        "AllowedMethods": AllowedMethodsOutputTypeDef,
+        "SmoothStreaming": bool,
+        "Compress": bool,
+        "LambdaFunctionAssociations": LambdaFunctionAssociationsOutputTypeDef,
+        "FunctionAssociations": FunctionAssociationsOutputTypeDef,
+        "FieldLevelEncryptionId": str,
+        "RealtimeLogConfigArn": str,
+        "CachePolicyId": str,
+        "OriginRequestPolicyId": str,
+        "ResponseHeadersPolicyId": str,
+        "ForwardedValues": ForwardedValuesOutputTypeDef,
+        "MinTTL": int,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+    },
+    total=False,
+)
+
+class DefaultCacheBehaviorOutputTypeDef(
+    _RequiredDefaultCacheBehaviorOutputTypeDef, _OptionalDefaultCacheBehaviorOutputTypeDef
+):
+    pass
+
 _RequiredCacheBehaviorTypeDef = TypedDict(
     "_RequiredCacheBehaviorTypeDef",
     {
         "PathPattern": str,
         "TargetOriginId": str,
         "ViewerProtocolPolicy": ViewerProtocolPolicyType,
     },
@@ -3809,58 +5344,83 @@
 )
 
 class DefaultCacheBehaviorTypeDef(
     _RequiredDefaultCacheBehaviorTypeDef, _OptionalDefaultCacheBehaviorTypeDef
 ):
     pass
 
-_RequiredCachePolicyConfigTypeDef = TypedDict(
-    "_RequiredCachePolicyConfigTypeDef",
+_RequiredCachePolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigOutputTypeDef",
     {
         "Name": str,
         "MinTTL": int,
     },
 )
-_OptionalCachePolicyConfigTypeDef = TypedDict(
-    "_OptionalCachePolicyConfigTypeDef",
+_OptionalCachePolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigOutputTypeDef",
     {
         "Comment": str,
         "DefaultTTL": int,
         "MaxTTL": int,
-        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+        "ParametersInCacheKeyAndForwardedToOrigin": (
+            ParametersInCacheKeyAndForwardedToOriginOutputTypeDef
+        ),
     },
     total=False,
 )
 
-class CachePolicyConfigTypeDef(
-    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+class CachePolicyConfigOutputTypeDef(
+    _RequiredCachePolicyConfigOutputTypeDef, _OptionalCachePolicyConfigOutputTypeDef
 ):
     pass
 
-CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
-    "CreateOriginRequestPolicyRequestRequestTypeDef",
-    {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
-    },
-)
-
 GetOriginRequestPolicyConfigResultTypeDef = TypedDict(
     "GetOriginRequestPolicyConfigResultTypeDef",
     {
-        "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 OriginRequestPolicyTypeDef = TypedDict(
     "OriginRequestPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "OriginRequestPolicyConfig": OriginRequestPolicyConfigOutputTypeDef,
+    },
+)
+
+_RequiredCachePolicyConfigTypeDef = TypedDict(
+    "_RequiredCachePolicyConfigTypeDef",
+    {
+        "Name": str,
+        "MinTTL": int,
+    },
+)
+_OptionalCachePolicyConfigTypeDef = TypedDict(
+    "_OptionalCachePolicyConfigTypeDef",
+    {
+        "Comment": str,
+        "DefaultTTL": int,
+        "MaxTTL": int,
+        "ParametersInCacheKeyAndForwardedToOrigin": ParametersInCacheKeyAndForwardedToOriginTypeDef,
+    },
+    total=False,
+)
+
+class CachePolicyConfigTypeDef(
+    _RequiredCachePolicyConfigTypeDef, _OptionalCachePolicyConfigTypeDef
+):
+    pass
+
+CreateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
+    "CreateOriginRequestPolicyRequestRequestTypeDef",
+    {
         "OriginRequestPolicyConfig": OriginRequestPolicyConfigTypeDef,
     },
 )
 
 _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOriginRequestPolicyRequestRequestTypeDef",
     {
@@ -3878,14 +5438,35 @@
 
 class UpdateOriginRequestPolicyRequestRequestTypeDef(
     _RequiredUpdateOriginRequestPolicyRequestRequestTypeDef,
     _OptionalUpdateOriginRequestPolicyRequestRequestTypeDef,
 ):
     pass
 
+_RequiredContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_RequiredContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "StagingDistributionDnsNames": StagingDistributionDnsNamesOutputTypeDef,
+        "Enabled": bool,
+    },
+)
+_OptionalContinuousDeploymentPolicyConfigOutputTypeDef = TypedDict(
+    "_OptionalContinuousDeploymentPolicyConfigOutputTypeDef",
+    {
+        "TrafficConfig": TrafficConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class ContinuousDeploymentPolicyConfigOutputTypeDef(
+    _RequiredContinuousDeploymentPolicyConfigOutputTypeDef,
+    _OptionalContinuousDeploymentPolicyConfigOutputTypeDef,
+):
+    pass
+
 _RequiredContinuousDeploymentPolicyConfigTypeDef = TypedDict(
     "_RequiredContinuousDeploymentPolicyConfigTypeDef",
     {
         "StagingDistributionDnsNames": StagingDistributionDnsNamesTypeDef,
         "Enabled": bool,
     },
 )
@@ -3899,70 +5480,59 @@
 
 class ContinuousDeploymentPolicyConfigTypeDef(
     _RequiredContinuousDeploymentPolicyConfigTypeDef,
     _OptionalContinuousDeploymentPolicyConfigTypeDef,
 ):
     pass
 
-_RequiredKeyGroupListTypeDef = TypedDict(
-    "_RequiredKeyGroupListTypeDef",
+OriginsOutputTypeDef = TypedDict(
+    "OriginsOutputTypeDef",
     {
-        "MaxItems": int,
         "Quantity": int,
+        "Items": List[OriginOutputTypeDef],
     },
 )
-_OptionalKeyGroupListTypeDef = TypedDict(
-    "_OptionalKeyGroupListTypeDef",
-    {
-        "NextMarker": str,
-        "Items": List[KeyGroupSummaryTypeDef],
-    },
-    total=False,
-)
-
-class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
-    pass
 
 OriginsTypeDef = TypedDict(
     "OriginsTypeDef",
     {
         "Quantity": int,
-        "Items": List[OriginTypeDef],
+        "Items": Sequence[OriginTypeDef],
     },
 )
 
-_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Name": str,
         "CallerReference": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigOutputTypeDef",
     {
         "Comment": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionProfileConfigTypeDef(
-    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
-    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+class FieldLevelEncryptionProfileConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigOutputTypeDef,
 ):
     pass
 
 _RequiredFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
         "Name": str,
-        "EncryptionEntities": EncryptionEntitiesTypeDef,
+        "EncryptionEntities": EncryptionEntitiesOutputTypeDef,
     },
 )
 _OptionalFieldLevelEncryptionProfileSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionProfileSummaryTypeDef",
     {
         "Comment": str,
     },
@@ -3971,14 +5541,36 @@
 
 class FieldLevelEncryptionProfileSummaryTypeDef(
     _RequiredFieldLevelEncryptionProfileSummaryTypeDef,
     _OptionalFieldLevelEncryptionProfileSummaryTypeDef,
 ):
     pass
 
+_RequiredFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Name": str,
+        "CallerReference": str,
+        "EncryptionEntities": EncryptionEntitiesTypeDef,
+    },
+)
+_OptionalFieldLevelEncryptionProfileConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileConfigTypeDef",
+    {
+        "Comment": str,
+    },
+    total=False,
+)
+
+class FieldLevelEncryptionProfileConfigTypeDef(
+    _RequiredFieldLevelEncryptionProfileConfigTypeDef,
+    _OptionalFieldLevelEncryptionProfileConfigTypeDef,
+):
+    pass
+
 CreateRealtimeLogConfigResultTypeDef = TypedDict(
     "CreateRealtimeLogConfigResultTypeDef",
     {
         "RealtimeLogConfig": RealtimeLogConfigTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -4033,14 +5625,33 @@
     "TestFunctionResultTypeDef",
     {
         "TestResult": TestResultTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredKeyGroupListTypeDef = TypedDict(
+    "_RequiredKeyGroupListTypeDef",
+    {
+        "MaxItems": int,
+        "Quantity": int,
+    },
+)
+_OptionalKeyGroupListTypeDef = TypedDict(
+    "_OptionalKeyGroupListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[KeyGroupSummaryTypeDef],
+    },
+    total=False,
+)
+
+class KeyGroupListTypeDef(_RequiredKeyGroupListTypeDef, _OptionalKeyGroupListTypeDef):
+    pass
+
 CreateInvalidationResultTypeDef = TypedDict(
     "CreateInvalidationResultTypeDef",
     {
         "Location": str,
         "Invalidation": InvalidationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -4058,15 +5669,15 @@
     "_RequiredStreamingDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "DomainName": str,
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
-        "StreamingDistributionConfig": StreamingDistributionConfigTypeDef,
+        "StreamingDistributionConfig": StreamingDistributionConfigOutputTypeDef,
     },
 )
 _OptionalStreamingDistributionTypeDef = TypedDict(
     "_OptionalStreamingDistributionTypeDef",
     {
         "LastModifiedTime": datetime,
     },
@@ -4074,95 +5685,136 @@
 )
 
 class StreamingDistributionTypeDef(
     _RequiredStreamingDistributionTypeDef, _OptionalStreamingDistributionTypeDef
 ):
     pass
 
+_RequiredOriginGroupsOutputTypeDef = TypedDict(
+    "_RequiredOriginGroupsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalOriginGroupsOutputTypeDef = TypedDict(
+    "_OptionalOriginGroupsOutputTypeDef",
+    {
+        "Items": List[OriginGroupOutputTypeDef],
+    },
+    total=False,
+)
+
+class OriginGroupsOutputTypeDef(
+    _RequiredOriginGroupsOutputTypeDef, _OptionalOriginGroupsOutputTypeDef
+):
+    pass
+
 _RequiredOriginGroupsTypeDef = TypedDict(
     "_RequiredOriginGroupsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalOriginGroupsTypeDef = TypedDict(
     "_OptionalOriginGroupsTypeDef",
     {
-        "Items": List[OriginGroupTypeDef],
+        "Items": Sequence[OriginGroupTypeDef],
     },
     total=False,
 )
 
 class OriginGroupsTypeDef(_RequiredOriginGroupsTypeDef, _OptionalOriginGroupsTypeDef):
     pass
 
-_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionConfigTypeDef",
+_RequiredFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigOutputTypeDef",
     {
         "CallerReference": str,
     },
 )
-_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionConfigTypeDef",
+_OptionalFieldLevelEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigOutputTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
-class FieldLevelEncryptionConfigTypeDef(
-    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+class FieldLevelEncryptionConfigOutputTypeDef(
+    _RequiredFieldLevelEncryptionConfigOutputTypeDef,
+    _OptionalFieldLevelEncryptionConfigOutputTypeDef,
 ):
     pass
 
 _RequiredFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_RequiredFieldLevelEncryptionSummaryTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
     },
 )
 _OptionalFieldLevelEncryptionSummaryTypeDef = TypedDict(
     "_OptionalFieldLevelEncryptionSummaryTypeDef",
     {
         "Comment": str,
-        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
-        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
+        "QueryArgProfileConfig": QueryArgProfileConfigOutputTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigOutputTypeDef,
     },
     total=False,
 )
 
 class FieldLevelEncryptionSummaryTypeDef(
     _RequiredFieldLevelEncryptionSummaryTypeDef, _OptionalFieldLevelEncryptionSummaryTypeDef
 ):
     pass
 
-CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
-    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionConfigTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "CallerReference": str,
+    },
+)
+_OptionalFieldLevelEncryptionConfigTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionConfigTypeDef",
+    {
+        "Comment": str,
+        "QueryArgProfileConfig": QueryArgProfileConfigTypeDef,
+        "ContentTypeProfileConfig": ContentTypeProfileConfigTypeDef,
     },
+    total=False,
 )
 
+class FieldLevelEncryptionConfigTypeDef(
+    _RequiredFieldLevelEncryptionConfigTypeDef, _OptionalFieldLevelEncryptionConfigTypeDef
+):
+    pass
+
 GetResponseHeadersPolicyConfigResultTypeDef = TypedDict(
     "GetResponseHeadersPolicyConfigResultTypeDef",
     {
-        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResponseHeadersPolicyTypeDef = TypedDict(
     "ResponseHeadersPolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
+        "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigOutputTypeDef,
+    },
+)
+
+CreateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
+    "CreateResponseHeadersPolicyRequestRequestTypeDef",
+    {
         "ResponseHeadersPolicyConfig": ResponseHeadersPolicyConfigTypeDef,
     },
 )
 
 _RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResponseHeadersPolicyRequestRequestTypeDef",
     {
@@ -4195,76 +5847,68 @@
 CreateStreamingDistributionWithTagsRequestRequestTypeDef = TypedDict(
     "CreateStreamingDistributionWithTagsRequestRequestTypeDef",
     {
         "StreamingDistributionConfigWithTags": StreamingDistributionConfigWithTagsTypeDef,
     },
 )
 
+_RequiredCacheBehaviorsOutputTypeDef = TypedDict(
+    "_RequiredCacheBehaviorsOutputTypeDef",
+    {
+        "Quantity": int,
+    },
+)
+_OptionalCacheBehaviorsOutputTypeDef = TypedDict(
+    "_OptionalCacheBehaviorsOutputTypeDef",
+    {
+        "Items": List[CacheBehaviorOutputTypeDef],
+    },
+    total=False,
+)
+
+class CacheBehaviorsOutputTypeDef(
+    _RequiredCacheBehaviorsOutputTypeDef, _OptionalCacheBehaviorsOutputTypeDef
+):
+    pass
+
 _RequiredCacheBehaviorsTypeDef = TypedDict(
     "_RequiredCacheBehaviorsTypeDef",
     {
         "Quantity": int,
     },
 )
 _OptionalCacheBehaviorsTypeDef = TypedDict(
     "_OptionalCacheBehaviorsTypeDef",
     {
-        "Items": List[CacheBehaviorTypeDef],
+        "Items": Sequence[CacheBehaviorTypeDef],
     },
     total=False,
 )
 
 class CacheBehaviorsTypeDef(_RequiredCacheBehaviorsTypeDef, _OptionalCacheBehaviorsTypeDef):
     pass
 
 CachePolicyTypeDef = TypedDict(
     "CachePolicyTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-    },
-)
-
-CreateCachePolicyRequestRequestTypeDef = TypedDict(
-    "CreateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
     },
 )
 
 GetCachePolicyConfigResultTypeDef = TypedDict(
     "GetCachePolicyConfigResultTypeDef",
     {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
+        "CachePolicyConfig": CachePolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "CachePolicyConfig": CachePolicyConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-class UpdateCachePolicyRequestRequestTypeDef(
-    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
-):
-    pass
-
 CreateOriginRequestPolicyResultTypeDef = TypedDict(
     "CreateOriginRequestPolicyResultTypeDef",
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -4293,39 +5937,66 @@
     {
         "OriginRequestPolicy": OriginRequestPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ContinuousDeploymentPolicyTypeDef = TypedDict(
-    "ContinuousDeploymentPolicyTypeDef",
+CreateCachePolicyRequestRequestTypeDef = TypedDict(
+    "CreateCachePolicyRequestRequestTypeDef",
     {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
+    },
+)
+
+_RequiredUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "CachePolicyConfig": CachePolicyConfigTypeDef,
         "Id": str,
-        "LastModifiedTime": datetime,
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
     },
 )
+_OptionalUpdateCachePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCachePolicyRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
 
-CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
-    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+class UpdateCachePolicyRequestRequestTypeDef(
+    _RequiredUpdateCachePolicyRequestRequestTypeDef, _OptionalUpdateCachePolicyRequestRequestTypeDef
+):
+    pass
+
+ContinuousDeploymentPolicyTypeDef = TypedDict(
+    "ContinuousDeploymentPolicyTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
     },
 )
 
 GetContinuousDeploymentPolicyConfigResultTypeDef = TypedDict(
     "GetContinuousDeploymentPolicyConfigResultTypeDef",
     {
-        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
+    "CreateContinuousDeploymentPolicyRequestRequestTypeDef",
+    {
+        "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
+    },
+)
+
 _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef",
     {
         "ContinuousDeploymentPolicyConfig": ContinuousDeploymentPolicyConfigTypeDef,
         "Id": str,
     },
 )
@@ -4339,44 +6010,57 @@
 
 class UpdateContinuousDeploymentPolicyRequestRequestTypeDef(
     _RequiredUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
     _OptionalUpdateContinuousDeploymentPolicyRequestRequestTypeDef,
 ):
     pass
 
-ListKeyGroupsResultTypeDef = TypedDict(
-    "ListKeyGroupsResultTypeDef",
+FieldLevelEncryptionProfileTypeDef = TypedDict(
+    "FieldLevelEncryptionProfileTypeDef",
     {
-        "KeyGroupList": KeyGroupListTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
+        "LastModifiedTime": datetime,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
     },
 )
 
-CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
+GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
+    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
     {
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigOutputTypeDef,
+        "ETag": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-FieldLevelEncryptionProfileTypeDef = TypedDict(
-    "FieldLevelEncryptionProfileTypeDef",
+_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionProfileListTypeDef",
     {
-        "Id": str,
-        "LastModifiedTime": datetime,
-        "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
+_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+    {
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+    },
+    total=False,
+)
 
-GetFieldLevelEncryptionProfileConfigResultTypeDef = TypedDict(
-    "GetFieldLevelEncryptionProfileConfigResultTypeDef",
+class FieldLevelEncryptionProfileListTypeDef(
+    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
+):
+    pass
+
+CreateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
-        "ETag": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef",
     {
         "FieldLevelEncryptionProfileConfig": FieldLevelEncryptionProfileConfigTypeDef,
@@ -4393,39 +6077,26 @@
 
 class UpdateFieldLevelEncryptionProfileRequestRequestTypeDef(
     _RequiredUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     _OptionalUpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
 ):
     pass
 
-_RequiredFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionProfileListTypeDef",
-    {
-        "MaxItems": int,
-        "Quantity": int,
-    },
-)
-_OptionalFieldLevelEncryptionProfileListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionProfileListTypeDef",
+ListRealtimeLogConfigsResultTypeDef = TypedDict(
+    "ListRealtimeLogConfigsResultTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionProfileSummaryTypeDef],
+        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-class FieldLevelEncryptionProfileListTypeDef(
-    _RequiredFieldLevelEncryptionProfileListTypeDef, _OptionalFieldLevelEncryptionProfileListTypeDef
-):
-    pass
-
-ListRealtimeLogConfigsResultTypeDef = TypedDict(
-    "ListRealtimeLogConfigsResultTypeDef",
+ListKeyGroupsResultTypeDef = TypedDict(
+    "ListKeyGroupsResultTypeDef",
     {
-        "RealtimeLogConfigs": RealtimeLogConfigsTypeDef,
+        "KeyGroupList": KeyGroupListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateStreamingDistributionResultTypeDef = TypedDict(
     "CreateStreamingDistributionResultTypeDef",
     {
@@ -4460,78 +6131,78 @@
     {
         "StreamingDistribution": StreamingDistributionTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
-    {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-    },
-)
-
 FieldLevelEncryptionTypeDef = TypedDict(
     "FieldLevelEncryptionTypeDef",
     {
         "Id": str,
         "LastModifiedTime": datetime,
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
     },
 )
 
 GetFieldLevelEncryptionConfigResultTypeDef = TypedDict(
     "GetFieldLevelEncryptionConfigResultTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
+    "_RequiredFieldLevelEncryptionListTypeDef",
     {
-        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
-        "Id": str,
+        "MaxItems": int,
+        "Quantity": int,
     },
 )
-_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
+    "_OptionalFieldLevelEncryptionListTypeDef",
     {
-        "IfMatch": str,
+        "NextMarker": str,
+        "Items": List[FieldLevelEncryptionSummaryTypeDef],
     },
     total=False,
 )
 
-class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
-    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
-    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+class FieldLevelEncryptionListTypeDef(
+    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
 ):
     pass
 
-_RequiredFieldLevelEncryptionListTypeDef = TypedDict(
-    "_RequiredFieldLevelEncryptionListTypeDef",
+CreateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "CreateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "Quantity": int,
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
     },
 )
-_OptionalFieldLevelEncryptionListTypeDef = TypedDict(
-    "_OptionalFieldLevelEncryptionListTypeDef",
+
+_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
     {
-        "NextMarker": str,
-        "Items": List[FieldLevelEncryptionSummaryTypeDef],
+        "FieldLevelEncryptionConfig": FieldLevelEncryptionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef",
+    {
+        "IfMatch": str,
     },
     total=False,
 )
 
-class FieldLevelEncryptionListTypeDef(
-    _RequiredFieldLevelEncryptionListTypeDef, _OptionalFieldLevelEncryptionListTypeDef
+class UpdateFieldLevelEncryptionConfigRequestRequestTypeDef(
+    _RequiredUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    _OptionalUpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 CreateResponseHeadersPolicyResultTypeDef = TypedDict(
     "CreateResponseHeadersPolicyResultTypeDef",
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
@@ -4563,88 +6234,124 @@
     {
         "ResponseHeadersPolicy": ResponseHeadersPolicyTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDistributionConfigTypeDef = TypedDict(
-    "_RequiredDistributionConfigTypeDef",
+_RequiredDistributionConfigOutputTypeDef = TypedDict(
+    "_RequiredDistributionConfigOutputTypeDef",
     {
         "CallerReference": str,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
         "Comment": str,
         "Enabled": bool,
     },
 )
-_OptionalDistributionConfigTypeDef = TypedDict(
-    "_OptionalDistributionConfigTypeDef",
+_OptionalDistributionConfigOutputTypeDef = TypedDict(
+    "_OptionalDistributionConfigOutputTypeDef",
     {
-        "Aliases": AliasesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
         "DefaultRootObject": str,
-        "OriginGroups": OriginGroupsTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
-        "Logging": LoggingConfigTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
+        "Logging": LoggingConfigOutputTypeDef,
         "PriceClass": PriceClassType,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "ContinuousDeploymentPolicyId": str,
         "Staging": bool,
     },
     total=False,
 )
 
-class DistributionConfigTypeDef(
-    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+class DistributionConfigOutputTypeDef(
+    _RequiredDistributionConfigOutputTypeDef, _OptionalDistributionConfigOutputTypeDef
 ):
     pass
 
 _RequiredDistributionSummaryTypeDef = TypedDict(
     "_RequiredDistributionSummaryTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "DomainName": str,
-        "Aliases": AliasesTypeDef,
-        "Origins": OriginsTypeDef,
-        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
-        "CacheBehaviors": CacheBehaviorsTypeDef,
-        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Aliases": AliasesOutputTypeDef,
+        "Origins": OriginsOutputTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorOutputTypeDef,
+        "CacheBehaviors": CacheBehaviorsOutputTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesOutputTypeDef,
         "Comment": str,
         "PriceClass": PriceClassType,
         "Enabled": bool,
-        "ViewerCertificate": ViewerCertificateTypeDef,
-        "Restrictions": RestrictionsTypeDef,
+        "ViewerCertificate": ViewerCertificateOutputTypeDef,
+        "Restrictions": RestrictionsOutputTypeDef,
         "WebACLId": str,
         "HttpVersion": HttpVersionType,
         "IsIPV6Enabled": bool,
         "Staging": bool,
     },
 )
 _OptionalDistributionSummaryTypeDef = TypedDict(
     "_OptionalDistributionSummaryTypeDef",
     {
-        "OriginGroups": OriginGroupsTypeDef,
+        "OriginGroups": OriginGroupsOutputTypeDef,
         "AliasICPRecordals": List[AliasICPRecordalTypeDef],
     },
     total=False,
 )
 
 class DistributionSummaryTypeDef(
     _RequiredDistributionSummaryTypeDef, _OptionalDistributionSummaryTypeDef
 ):
     pass
 
+_RequiredDistributionConfigTypeDef = TypedDict(
+    "_RequiredDistributionConfigTypeDef",
+    {
+        "CallerReference": str,
+        "Origins": OriginsTypeDef,
+        "DefaultCacheBehavior": DefaultCacheBehaviorTypeDef,
+        "Comment": str,
+        "Enabled": bool,
+    },
+)
+_OptionalDistributionConfigTypeDef = TypedDict(
+    "_OptionalDistributionConfigTypeDef",
+    {
+        "Aliases": AliasesTypeDef,
+        "DefaultRootObject": str,
+        "OriginGroups": OriginGroupsTypeDef,
+        "CacheBehaviors": CacheBehaviorsTypeDef,
+        "CustomErrorResponses": CustomErrorResponsesTypeDef,
+        "Logging": LoggingConfigTypeDef,
+        "PriceClass": PriceClassType,
+        "ViewerCertificate": ViewerCertificateTypeDef,
+        "Restrictions": RestrictionsTypeDef,
+        "WebACLId": str,
+        "HttpVersion": HttpVersionType,
+        "IsIPV6Enabled": bool,
+        "ContinuousDeploymentPolicyId": str,
+        "Staging": bool,
+    },
+    total=False,
+)
+
+class DistributionConfigTypeDef(
+    _RequiredDistributionConfigTypeDef, _OptionalDistributionConfigTypeDef
+):
+    pass
+
 CachePolicySummaryTypeDef = TypedDict(
     "CachePolicySummaryTypeDef",
     {
         "Type": CachePolicyTypeType,
         "CachePolicy": CachePolicyTypeDef,
     },
 )
@@ -4822,39 +6529,24 @@
 )
 
 class ResponseHeadersPolicyListTypeDef(
     _RequiredResponseHeadersPolicyListTypeDef, _OptionalResponseHeadersPolicyListTypeDef
 ):
     pass
 
-CreateDistributionRequestRequestTypeDef = TypedDict(
-    "CreateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-    },
-)
-
-DistributionConfigWithTagsTypeDef = TypedDict(
-    "DistributionConfigWithTagsTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Tags": TagsTypeDef,
-    },
-)
-
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "Id": str,
         "ARN": str,
         "Status": str,
         "LastModifiedTime": datetime,
         "InProgressInvalidationBatches": int,
         "DomainName": str,
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
     "_OptionalDistributionTypeDef",
     {
         "ActiveTrustedSigners": ActiveTrustedSignersTypeDef,
         "ActiveTrustedKeyGroups": ActiveTrustedKeyGroupsTypeDef,
@@ -4865,41 +6557,20 @@
 
 class DistributionTypeDef(_RequiredDistributionTypeDef, _OptionalDistributionTypeDef):
     pass
 
 GetDistributionConfigResultTypeDef = TypedDict(
     "GetDistributionConfigResultTypeDef",
     {
-        "DistributionConfig": DistributionConfigTypeDef,
+        "DistributionConfig": DistributionConfigOutputTypeDef,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionRequestRequestTypeDef",
-    {
-        "DistributionConfig": DistributionConfigTypeDef,
-        "Id": str,
-    },
-)
-_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionRequestRequestTypeDef",
-    {
-        "IfMatch": str,
-    },
-    total=False,
-)
-
-class UpdateDistributionRequestRequestTypeDef(
-    _RequiredUpdateDistributionRequestRequestTypeDef,
-    _OptionalUpdateDistributionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDistributionListTypeDef = TypedDict(
     "_RequiredDistributionListTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
         "IsTruncated": bool,
         "Quantity": int,
@@ -4913,14 +6584,50 @@
     },
     total=False,
 )
 
 class DistributionListTypeDef(_RequiredDistributionListTypeDef, _OptionalDistributionListTypeDef):
     pass
 
+CreateDistributionRequestRequestTypeDef = TypedDict(
+    "CreateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+    },
+)
+
+DistributionConfigWithTagsTypeDef = TypedDict(
+    "DistributionConfigWithTagsTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Tags": TagsTypeDef,
+    },
+)
+
+_RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionRequestRequestTypeDef",
+    {
+        "DistributionConfig": DistributionConfigTypeDef,
+        "Id": str,
+    },
+)
+_OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionRequestRequestTypeDef",
+    {
+        "IfMatch": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionRequestRequestTypeDef(
+    _RequiredUpdateDistributionRequestRequestTypeDef,
+    _OptionalUpdateDistributionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCachePolicyListTypeDef = TypedDict(
     "_RequiredCachePolicyListTypeDef",
     {
         "MaxItems": int,
         "Quantity": int,
     },
 )
@@ -4969,21 +6676,14 @@
     "ListResponseHeadersPoliciesResultTypeDef",
     {
         "ResponseHeadersPolicyList": ResponseHeadersPolicyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
-    "CreateDistributionWithTagsRequestRequestTypeDef",
-    {
-        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
-    },
-)
-
 CopyDistributionResultTypeDef = TypedDict(
     "CopyDistributionResultTypeDef",
     {
         "Distribution": DistributionTypeDef,
         "Location": str,
         "ETag": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -5057,14 +6757,21 @@
     "ListDistributionsResultTypeDef",
     {
         "DistributionList": DistributionListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreateDistributionWithTagsRequestRequestTypeDef = TypedDict(
+    "CreateDistributionWithTagsRequestRequestTypeDef",
+    {
+        "DistributionConfigWithTags": DistributionConfigWithTagsTypeDef,
+    },
+)
+
 ListCachePoliciesResultTypeDef = TypedDict(
     "ListCachePoliciesResultTypeDef",
     {
         "CachePolicyList": CachePolicyListTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/waiter.py` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront/waiter.pyi` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/PKG-INFO` & `mypy-boto3-cloudfront-1.28.12/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-cloudfront
-Version: 1.28.0
-Summary: Type annotations for boto3.CloudFront 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 cloudfront type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-cloudfront"></a>
 
 # mypy-boto3-cloudfront
 
 [![PyPI - mypy-boto3-cloudfront](https://img.shields.io/pypi/v/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudfront.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudfront)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cloudfront?color=blue)](https://pypistats.org/packages/mypy-boto3-cloudfront)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudfront)](https://pepy.tech/project/mypy-boto3-cloudfront)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFront 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
+[boto3.CloudFront 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#CloudFront)
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
 [mypy-boto3-cloudfront docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudfront/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,36 +375,51 @@
 
 `mypy_boto3_cloudfront.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudfront.type_defs import (
     AliasICPRecordalTypeDef,
+    AliasesOutputTypeDef,
     AliasesTypeDef,
+    CachedMethodsOutputTypeDef,
     CachedMethodsTypeDef,
     AssociateAliasRequestRequestTypeDef,
+    TrustedKeyGroupsOutputTypeDef,
+    TrustedSignersOutputTypeDef,
     TrustedKeyGroupsTypeDef,
     TrustedSignersTypeDef,
+    CookieNamesOutputTypeDef,
     CookieNamesTypeDef,
+    HeadersOutputTypeDef,
     HeadersTypeDef,
+    QueryStringNamesOutputTypeDef,
     QueryStringNamesTypeDef,
+    CloudFrontOriginAccessIdentityConfigOutputTypeDef,
     CloudFrontOriginAccessIdentityConfigTypeDef,
     CloudFrontOriginAccessIdentitySummaryTypeDef,
     ConflictingAliasTypeDef,
+    ContentTypeProfileOutputTypeDef,
     ContentTypeProfileTypeDef,
+    StagingDistributionDnsNamesOutputTypeDef,
     StagingDistributionDnsNamesTypeDef,
+    ContinuousDeploymentSingleHeaderConfigOutputTypeDef,
     ContinuousDeploymentSingleHeaderConfigTypeDef,
+    SessionStickinessConfigOutputTypeDef,
     SessionStickinessConfigTypeDef,
     CopyDistributionRequestRequestTypeDef,
     FunctionConfigTypeDef,
     KeyGroupConfigTypeDef,
     OriginAccessControlConfigTypeDef,
     PublicKeyConfigTypeDef,
+    CustomErrorResponseOutputTypeDef,
     CustomErrorResponseTypeDef,
+    OriginCustomHeaderOutputTypeDef,
     OriginCustomHeaderTypeDef,
+    OriginSslProtocolsOutputTypeDef,
     OriginSslProtocolsTypeDef,
     DeleteCachePolicyRequestRequestTypeDef,
     DeleteCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     DeleteContinuousDeploymentPolicyRequestRequestTypeDef,
     DeleteDistributionRequestRequestTypeDef,
     DeleteFieldLevelEncryptionConfigRequestRequestTypeDef,
     DeleteFieldLevelEncryptionProfileRequestRequestTypeDef,
@@ -446,23 +429,31 @@
     DeleteOriginAccessControlRequestRequestTypeDef,
     DeleteOriginRequestPolicyRequestRequestTypeDef,
     DeletePublicKeyRequestRequestTypeDef,
     DeleteRealtimeLogConfigRequestRequestTypeDef,
     DeleteResponseHeadersPolicyRequestRequestTypeDef,
     DeleteStreamingDistributionRequestRequestTypeDef,
     DescribeFunctionRequestRequestTypeDef,
+    LoggingConfigOutputTypeDef,
+    ViewerCertificateOutputTypeDef,
     LoggingConfigTypeDef,
     ViewerCertificateTypeDef,
     DistributionIdListTypeDef,
     EmptyResponseMetadataTypeDef,
+    FieldPatternsOutputTypeDef,
     FieldPatternsTypeDef,
+    KinesisStreamConfigOutputTypeDef,
     KinesisStreamConfigTypeDef,
+    QueryStringCacheKeysOutputTypeDef,
     QueryStringCacheKeysTypeDef,
+    FunctionAssociationOutputTypeDef,
     FunctionAssociationTypeDef,
+    FunctionConfigOutputTypeDef,
     FunctionMetadataTypeDef,
+    GeoRestrictionOutputTypeDef,
     GeoRestrictionTypeDef,
     GetCachePolicyConfigRequestRequestTypeDef,
     GetCachePolicyRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigRequestRequestTypeDef,
     GetContinuousDeploymentPolicyRequestRequestTypeDef,
@@ -473,30 +464,35 @@
     GetFieldLevelEncryptionProfileConfigRequestRequestTypeDef,
     GetFieldLevelEncryptionProfileRequestRequestTypeDef,
     GetFieldLevelEncryptionRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionResultTypeDef,
     GetInvalidationRequestRequestTypeDef,
     GetKeyGroupConfigRequestRequestTypeDef,
+    KeyGroupConfigOutputTypeDef,
     GetKeyGroupRequestRequestTypeDef,
     GetMonitoringSubscriptionRequestRequestTypeDef,
     GetOriginAccessControlConfigRequestRequestTypeDef,
+    OriginAccessControlConfigOutputTypeDef,
     GetOriginAccessControlRequestRequestTypeDef,
     GetOriginRequestPolicyConfigRequestRequestTypeDef,
     GetOriginRequestPolicyRequestRequestTypeDef,
     GetPublicKeyConfigRequestRequestTypeDef,
+    PublicKeyConfigOutputTypeDef,
     GetPublicKeyRequestRequestTypeDef,
     GetRealtimeLogConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyConfigRequestRequestTypeDef,
     GetResponseHeadersPolicyRequestRequestTypeDef,
     GetStreamingDistributionConfigRequestRequestTypeDef,
     GetStreamingDistributionRequestRequestTypeDef,
+    PathsOutputTypeDef,
     PathsTypeDef,
     InvalidationSummaryTypeDef,
     KeyPairIdsTypeDef,
+    LambdaFunctionAssociationOutputTypeDef,
     LambdaFunctionAssociationTypeDef,
     ListCachePoliciesRequestRequestTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestListCloudFrontOriginAccessIdentitiesPaginateTypeDef,
     ListCloudFrontOriginAccessIdentitiesRequestRequestTypeDef,
     ListConflictingAliasesRequestRequestTypeDef,
     ListContinuousDeploymentPoliciesRequestRequestTypeDef,
     ListDistributionsByCachePolicyIdRequestRequestTypeDef,
@@ -517,224 +513,295 @@
     ListOriginRequestPoliciesRequestRequestTypeDef,
     ListPublicKeysRequestRequestTypeDef,
     ListRealtimeLogConfigsRequestRequestTypeDef,
     ListResponseHeadersPoliciesRequestRequestTypeDef,
     ListStreamingDistributionsRequestListStreamingDistributionsPaginateTypeDef,
     ListStreamingDistributionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    RealtimeMetricsSubscriptionConfigOutputTypeDef,
     RealtimeMetricsSubscriptionConfigTypeDef,
     OriginAccessControlSummaryTypeDef,
+    StatusCodesOutputTypeDef,
     StatusCodesTypeDef,
+    OriginGroupMemberOutputTypeDef,
     OriginGroupMemberTypeDef,
+    OriginShieldOutputTypeDef,
+    S3OriginConfigOutputTypeDef,
     OriginShieldTypeDef,
     S3OriginConfigTypeDef,
     PaginatorConfigTypeDef,
     PublicKeySummaryTypeDef,
     PublishFunctionRequestRequestTypeDef,
+    QueryArgProfileOutputTypeDef,
     QueryArgProfileTypeDef,
+    ResponseHeadersPolicyAccessControlAllowHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowHeadersTypeDef,
+    ResponseHeadersPolicyAccessControlAllowMethodsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowMethodsTypeDef,
+    ResponseHeadersPolicyAccessControlAllowOriginsOutputTypeDef,
     ResponseHeadersPolicyAccessControlAllowOriginsTypeDef,
+    ResponseHeadersPolicyAccessControlExposeHeadersOutputTypeDef,
     ResponseHeadersPolicyAccessControlExposeHeadersTypeDef,
+    ResponseHeadersPolicyServerTimingHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyServerTimingHeadersConfigTypeDef,
+    ResponseHeadersPolicyContentSecurityPolicyOutputTypeDef,
     ResponseHeadersPolicyContentSecurityPolicyTypeDef,
+    ResponseHeadersPolicyContentTypeOptionsOutputTypeDef,
     ResponseHeadersPolicyContentTypeOptionsTypeDef,
+    ResponseHeadersPolicyCustomHeaderOutputTypeDef,
     ResponseHeadersPolicyCustomHeaderTypeDef,
+    ResponseHeadersPolicyFrameOptionsOutputTypeDef,
     ResponseHeadersPolicyFrameOptionsTypeDef,
+    ResponseHeadersPolicyReferrerPolicyOutputTypeDef,
     ResponseHeadersPolicyReferrerPolicyTypeDef,
+    ResponseHeadersPolicyRemoveHeaderOutputTypeDef,
     ResponseHeadersPolicyRemoveHeaderTypeDef,
+    ResponseHeadersPolicyStrictTransportSecurityOutputTypeDef,
+    ResponseHeadersPolicyXSSProtectionOutputTypeDef,
     ResponseHeadersPolicyStrictTransportSecurityTypeDef,
     ResponseHeadersPolicyXSSProtectionTypeDef,
     ResponseMetadataTypeDef,
+    S3OriginOutputTypeDef,
     S3OriginTypeDef,
+    StreamingLoggingConfigOutputTypeDef,
     StreamingLoggingConfigTypeDef,
     TagKeysTypeDef,
+    TagOutputTypeDef,
     TagTypeDef,
     TestFunctionRequestRequestTypeDef,
     UpdateDistributionWithStagingConfigRequestRequestTypeDef,
+    AllowedMethodsOutputTypeDef,
     AllowedMethodsTypeDef,
+    CachePolicyCookiesConfigOutputTypeDef,
+    CookiePreferenceOutputTypeDef,
+    OriginRequestPolicyCookiesConfigOutputTypeDef,
     CachePolicyCookiesConfigTypeDef,
     CookiePreferenceTypeDef,
     OriginRequestPolicyCookiesConfigTypeDef,
+    CachePolicyHeadersConfigOutputTypeDef,
+    OriginRequestPolicyHeadersConfigOutputTypeDef,
     CachePolicyHeadersConfigTypeDef,
     OriginRequestPolicyHeadersConfigTypeDef,
+    CachePolicyQueryStringsConfigOutputTypeDef,
+    OriginRequestPolicyQueryStringsConfigOutputTypeDef,
     CachePolicyQueryStringsConfigTypeDef,
     OriginRequestPolicyQueryStringsConfigTypeDef,
     CloudFrontOriginAccessIdentityTypeDef,
-    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     GetCloudFrontOriginAccessIdentityConfigResultTypeDef,
+    CreateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     UpdateCloudFrontOriginAccessIdentityRequestRequestTypeDef,
     CloudFrontOriginAccessIdentityListTypeDef,
     ConflictingAliasesListTypeDef,
+    ContentTypeProfilesOutputTypeDef,
     ContentTypeProfilesTypeDef,
+    ContinuousDeploymentSingleWeightConfigOutputTypeDef,
     ContinuousDeploymentSingleWeightConfigTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionRequestRequestTypeDef,
     CreateKeyGroupRequestRequestTypeDef,
-    GetKeyGroupConfigResultTypeDef,
-    KeyGroupTypeDef,
     UpdateKeyGroupRequestRequestTypeDef,
     CreateOriginAccessControlRequestRequestTypeDef,
-    GetOriginAccessControlConfigResultTypeDef,
-    OriginAccessControlTypeDef,
     UpdateOriginAccessControlRequestRequestTypeDef,
     CreatePublicKeyRequestRequestTypeDef,
-    GetPublicKeyConfigResultTypeDef,
-    PublicKeyTypeDef,
     UpdatePublicKeyRequestRequestTypeDef,
+    CustomErrorResponsesOutputTypeDef,
     CustomErrorResponsesTypeDef,
+    CustomHeadersOutputTypeDef,
     CustomHeadersTypeDef,
+    CustomOriginConfigOutputTypeDef,
     CustomOriginConfigTypeDef,
     ListDistributionsByCachePolicyIdResultTypeDef,
     ListDistributionsByKeyGroupResultTypeDef,
     ListDistributionsByOriginRequestPolicyIdResultTypeDef,
     ListDistributionsByResponseHeadersPolicyIdResultTypeDef,
+    EncryptionEntityOutputTypeDef,
     EncryptionEntityTypeDef,
+    EndPointOutputTypeDef,
     EndPointTypeDef,
+    FunctionAssociationsOutputTypeDef,
     FunctionAssociationsTypeDef,
     FunctionSummaryTypeDef,
+    RestrictionsOutputTypeDef,
     RestrictionsTypeDef,
     GetDistributionRequestDistributionDeployedWaitTypeDef,
     GetInvalidationRequestInvalidationCompletedWaitTypeDef,
     GetStreamingDistributionRequestStreamingDistributionDeployedWaitTypeDef,
+    GetKeyGroupConfigResultTypeDef,
+    KeyGroupTypeDef,
+    GetOriginAccessControlConfigResultTypeDef,
+    OriginAccessControlTypeDef,
+    GetPublicKeyConfigResultTypeDef,
+    PublicKeyTypeDef,
+    InvalidationBatchOutputTypeDef,
     InvalidationBatchTypeDef,
     InvalidationListTypeDef,
     KGKeyPairIdsTypeDef,
     SignerTypeDef,
+    LambdaFunctionAssociationsOutputTypeDef,
     LambdaFunctionAssociationsTypeDef,
+    MonitoringSubscriptionOutputTypeDef,
     MonitoringSubscriptionTypeDef,
     OriginAccessControlListTypeDef,
+    OriginGroupFailoverCriteriaOutputTypeDef,
     OriginGroupFailoverCriteriaTypeDef,
+    OriginGroupMembersOutputTypeDef,
     OriginGroupMembersTypeDef,
     PublicKeyListTypeDef,
+    QueryArgProfilesOutputTypeDef,
     QueryArgProfilesTypeDef,
+    ResponseHeadersPolicyCorsConfigOutputTypeDef,
     ResponseHeadersPolicyCorsConfigTypeDef,
+    ResponseHeadersPolicyCustomHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyCustomHeadersConfigTypeDef,
+    ResponseHeadersPolicyRemoveHeadersConfigOutputTypeDef,
     ResponseHeadersPolicyRemoveHeadersConfigTypeDef,
+    ResponseHeadersPolicySecurityHeadersConfigOutputTypeDef,
     ResponseHeadersPolicySecurityHeadersConfigTypeDef,
     StreamingDistributionSummaryTypeDef,
+    StreamingDistributionConfigOutputTypeDef,
     StreamingDistributionConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
+    TagsOutputTypeDef,
     TagsTypeDef,
+    ForwardedValuesOutputTypeDef,
     ForwardedValuesTypeDef,
+    ParametersInCacheKeyAndForwardedToOriginOutputTypeDef,
+    OriginRequestPolicyConfigOutputTypeDef,
     ParametersInCacheKeyAndForwardedToOriginTypeDef,
     OriginRequestPolicyConfigTypeDef,
     CreateCloudFrontOriginAccessIdentityResultTypeDef,
     GetCloudFrontOriginAccessIdentityResultTypeDef,
     UpdateCloudFrontOriginAccessIdentityResultTypeDef,
     ListCloudFrontOriginAccessIdentitiesResultTypeDef,
     ListConflictingAliasesResultTypeDef,
+    ContentTypeProfileConfigOutputTypeDef,
     ContentTypeProfileConfigTypeDef,
+    TrafficConfigOutputTypeDef,
     TrafficConfigTypeDef,
-    CreateKeyGroupResultTypeDef,
-    GetKeyGroupResultTypeDef,
-    KeyGroupSummaryTypeDef,
-    UpdateKeyGroupResultTypeDef,
-    CreateOriginAccessControlResultTypeDef,
-    GetOriginAccessControlResultTypeDef,
-    UpdateOriginAccessControlResultTypeDef,
-    CreatePublicKeyResultTypeDef,
-    GetPublicKeyResultTypeDef,
-    UpdatePublicKeyResultTypeDef,
+    OriginOutputTypeDef,
     OriginTypeDef,
+    EncryptionEntitiesOutputTypeDef,
     EncryptionEntitiesTypeDef,
-    CreateRealtimeLogConfigRequestRequestTypeDef,
     RealtimeLogConfigTypeDef,
+    CreateRealtimeLogConfigRequestRequestTypeDef,
     UpdateRealtimeLogConfigRequestRequestTypeDef,
     CreateFunctionResultTypeDef,
     DescribeFunctionResultTypeDef,
     FunctionListTypeDef,
     PublishFunctionResultTypeDef,
     TestResultTypeDef,
     UpdateFunctionResultTypeDef,
-    CreateInvalidationRequestRequestTypeDef,
+    CreateKeyGroupResultTypeDef,
+    GetKeyGroupResultTypeDef,
+    KeyGroupSummaryTypeDef,
+    UpdateKeyGroupResultTypeDef,
+    CreateOriginAccessControlResultTypeDef,
+    GetOriginAccessControlResultTypeDef,
+    UpdateOriginAccessControlResultTypeDef,
+    CreatePublicKeyResultTypeDef,
+    GetPublicKeyResultTypeDef,
+    UpdatePublicKeyResultTypeDef,
     InvalidationTypeDef,
+    CreateInvalidationRequestRequestTypeDef,
     ListInvalidationsResultTypeDef,
     ActiveTrustedKeyGroupsTypeDef,
     ActiveTrustedSignersTypeDef,
-    CreateMonitoringSubscriptionRequestRequestTypeDef,
     CreateMonitoringSubscriptionResultTypeDef,
     GetMonitoringSubscriptionResultTypeDef,
+    CreateMonitoringSubscriptionRequestRequestTypeDef,
     ListOriginAccessControlsResultTypeDef,
+    OriginGroupOutputTypeDef,
     OriginGroupTypeDef,
     ListPublicKeysResultTypeDef,
+    QueryArgProfileConfigOutputTypeDef,
     QueryArgProfileConfigTypeDef,
+    ResponseHeadersPolicyConfigOutputTypeDef,
     ResponseHeadersPolicyConfigTypeDef,
     StreamingDistributionListTypeDef,
-    CreateStreamingDistributionRequestRequestTypeDef,
     GetStreamingDistributionConfigResultTypeDef,
+    CreateStreamingDistributionRequestRequestTypeDef,
     UpdateStreamingDistributionRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     StreamingDistributionConfigWithTagsTypeDef,
     TagResourceRequestRequestTypeDef,
+    CacheBehaviorOutputTypeDef,
+    DefaultCacheBehaviorOutputTypeDef,
     CacheBehaviorTypeDef,
     DefaultCacheBehaviorTypeDef,
-    CachePolicyConfigTypeDef,
-    CreateOriginRequestPolicyRequestRequestTypeDef,
+    CachePolicyConfigOutputTypeDef,
     GetOriginRequestPolicyConfigResultTypeDef,
     OriginRequestPolicyTypeDef,
+    CachePolicyConfigTypeDef,
+    CreateOriginRequestPolicyRequestRequestTypeDef,
     UpdateOriginRequestPolicyRequestRequestTypeDef,
+    ContinuousDeploymentPolicyConfigOutputTypeDef,
     ContinuousDeploymentPolicyConfigTypeDef,
-    KeyGroupListTypeDef,
+    OriginsOutputTypeDef,
     OriginsTypeDef,
-    FieldLevelEncryptionProfileConfigTypeDef,
+    FieldLevelEncryptionProfileConfigOutputTypeDef,
     FieldLevelEncryptionProfileSummaryTypeDef,
+    FieldLevelEncryptionProfileConfigTypeDef,
     CreateRealtimeLogConfigResultTypeDef,
     GetRealtimeLogConfigResultTypeDef,
     RealtimeLogConfigsTypeDef,
     UpdateRealtimeLogConfigResultTypeDef,
     ListFunctionsResultTypeDef,
     TestFunctionResultTypeDef,
+    KeyGroupListTypeDef,
     CreateInvalidationResultTypeDef,
     GetInvalidationResultTypeDef,
     StreamingDistributionTypeDef,
+    OriginGroupsOutputTypeDef,
     OriginGroupsTypeDef,
-    FieldLevelEncryptionConfigTypeDef,
+    FieldLevelEncryptionConfigOutputTypeDef,
     FieldLevelEncryptionSummaryTypeDef,
-    CreateResponseHeadersPolicyRequestRequestTypeDef,
+    FieldLevelEncryptionConfigTypeDef,
     GetResponseHeadersPolicyConfigResultTypeDef,
     ResponseHeadersPolicyTypeDef,
+    CreateResponseHeadersPolicyRequestRequestTypeDef,
     UpdateResponseHeadersPolicyRequestRequestTypeDef,
     ListStreamingDistributionsResultTypeDef,
     CreateStreamingDistributionWithTagsRequestRequestTypeDef,
+    CacheBehaviorsOutputTypeDef,
     CacheBehaviorsTypeDef,
     CachePolicyTypeDef,
-    CreateCachePolicyRequestRequestTypeDef,
     GetCachePolicyConfigResultTypeDef,
-    UpdateCachePolicyRequestRequestTypeDef,
     CreateOriginRequestPolicyResultTypeDef,
     GetOriginRequestPolicyResultTypeDef,
     OriginRequestPolicySummaryTypeDef,
     UpdateOriginRequestPolicyResultTypeDef,
+    CreateCachePolicyRequestRequestTypeDef,
+    UpdateCachePolicyRequestRequestTypeDef,
     ContinuousDeploymentPolicyTypeDef,
-    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     GetContinuousDeploymentPolicyConfigResultTypeDef,
+    CreateContinuousDeploymentPolicyRequestRequestTypeDef,
     UpdateContinuousDeploymentPolicyRequestRequestTypeDef,
-    ListKeyGroupsResultTypeDef,
-    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileTypeDef,
     GetFieldLevelEncryptionProfileConfigResultTypeDef,
-    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     FieldLevelEncryptionProfileListTypeDef,
+    CreateFieldLevelEncryptionProfileRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionProfileRequestRequestTypeDef,
     ListRealtimeLogConfigsResultTypeDef,
+    ListKeyGroupsResultTypeDef,
     CreateStreamingDistributionResultTypeDef,
     CreateStreamingDistributionWithTagsResultTypeDef,
     GetStreamingDistributionResultTypeDef,
     UpdateStreamingDistributionResultTypeDef,
-    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionTypeDef,
     GetFieldLevelEncryptionConfigResultTypeDef,
-    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     FieldLevelEncryptionListTypeDef,
+    CreateFieldLevelEncryptionConfigRequestRequestTypeDef,
+    UpdateFieldLevelEncryptionConfigRequestRequestTypeDef,
     CreateResponseHeadersPolicyResultTypeDef,
     GetResponseHeadersPolicyResultTypeDef,
     ResponseHeadersPolicySummaryTypeDef,
     UpdateResponseHeadersPolicyResultTypeDef,
-    DistributionConfigTypeDef,
+    DistributionConfigOutputTypeDef,
     DistributionSummaryTypeDef,
+    DistributionConfigTypeDef,
     CachePolicySummaryTypeDef,
     CreateCachePolicyResultTypeDef,
     GetCachePolicyResultTypeDef,
     UpdateCachePolicyResultTypeDef,
     OriginRequestPolicyListTypeDef,
     ContinuousDeploymentPolicySummaryTypeDef,
     CreateContinuousDeploymentPolicyResultTypeDef,
@@ -745,34 +812,34 @@
     UpdateFieldLevelEncryptionProfileResultTypeDef,
     ListFieldLevelEncryptionProfilesResultTypeDef,
     CreateFieldLevelEncryptionConfigResultTypeDef,
     GetFieldLevelEncryptionResultTypeDef,
     UpdateFieldLevelEncryptionConfigResultTypeDef,
     ListFieldLevelEncryptionConfigsResultTypeDef,
     ResponseHeadersPolicyListTypeDef,
-    CreateDistributionRequestRequestTypeDef,
-    DistributionConfigWithTagsTypeDef,
     DistributionTypeDef,
     GetDistributionConfigResultTypeDef,
-    UpdateDistributionRequestRequestTypeDef,
     DistributionListTypeDef,
+    CreateDistributionRequestRequestTypeDef,
+    DistributionConfigWithTagsTypeDef,
+    UpdateDistributionRequestRequestTypeDef,
     CachePolicyListTypeDef,
     ListOriginRequestPoliciesResultTypeDef,
     ContinuousDeploymentPolicyListTypeDef,
     ListResponseHeadersPoliciesResultTypeDef,
-    CreateDistributionWithTagsRequestRequestTypeDef,
     CopyDistributionResultTypeDef,
     CreateDistributionResultTypeDef,
     CreateDistributionWithTagsResultTypeDef,
     GetDistributionResultTypeDef,
     UpdateDistributionResultTypeDef,
     UpdateDistributionWithStagingConfigResultTypeDef,
     ListDistributionsByRealtimeLogConfigResultTypeDef,
     ListDistributionsByWebACLIdResultTypeDef,
     ListDistributionsResultTypeDef,
+    CreateDistributionWithTagsRequestRequestTypeDef,
     ListCachePoliciesResultTypeDef,
     ListContinuousDeploymentPoliciesResultTypeDef,
 )
 
 
 def get_structure() -> AliasICPRecordalTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudfront-1.28.0/mypy_boto3_cloudfront.egg-info/SOURCES.txt` & `mypy-boto3-cloudfront-1.28.12/mypy_boto3_cloudfront.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudfront-1.28.0/setup.py` & `mypy-boto3-cloudfront-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudfront",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cloudfront"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFront 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CloudFront 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

