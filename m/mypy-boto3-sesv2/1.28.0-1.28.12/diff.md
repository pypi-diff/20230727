# Comparing `tmp/mypy-boto3-sesv2-1.28.0.tar.gz` & `tmp/mypy-boto3-sesv2-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sesv2-1.28.0.tar", last modified: Thu Jul  6 21:00:38 2023, max compression
+gzip compressed data, was "mypy-boto3-sesv2-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-sesv2-1.28.0.tar` & `mypy-boto3-sesv2-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.766433 mypy-boto3-sesv2-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-06 21:00:38.766433 mypy-boto3-sesv2-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19504 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.746433 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-06 20:55:51.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-07-06 20:55:51.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-06 20:55:51.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69232 2023-07-06 20:55:53.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69162 2023-07-06 20:55:52.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.766433 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-06 21:00:38.000000 mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:38.766433 mypy-boto3-sesv2-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-06 20:55:50.000000 mypy-boto3-sesv2-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20451 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56738 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56645 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75683 2023-07-27 11:46:56.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75609 2023-07-27 11:46:55.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21930 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 11:49:38.000000 mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.829293 mypy-boto3-sesv2-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 11:46:54.000000 mypy-boto3-sesv2-1.28.12/setup.py
```

### Comparing `mypy-boto3-sesv2-1.28.0/LICENSE` & `mypy-boto3-sesv2-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.0/PKG-INFO` & `mypy-boto3-sesv2-1.28.12/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sesv2
-Version: 1.28.0
-Summary: Type annotations for boto3.SESV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,99 +333,115 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceTypeDef,
+    TopicPreferenceOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
+    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
+    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
+    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
+    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
+    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
+    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
+    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
+    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -443,99 +459,109 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
-    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
-    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
+    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
+    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
+    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sesv2-1.28.0/README.md` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sesv2
+Version: 1.28.12
+Summary: Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,99 +333,115 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceTypeDef,
+    TopicPreferenceOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
+    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
+    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
+    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
+    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
+    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
+    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
+    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
+    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -411,99 +459,109 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
-    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
-    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
+    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
+    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
+    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/__main__.py` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SESV2 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SESV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2\nOther"
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

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/client.py` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/client.pyi` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/literals.py` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,15 @@
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
@@ -334,26 +335,28 @@
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

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/literals.pyi` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,15 @@
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
@@ -332,26 +333,28 @@
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

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/type_defs.py` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,99 +64,115 @@
 
 
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
+    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
+    "ContactListDestinationOutputTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
-    "TopicPreferenceTypeDef",
+    "TopicPreferenceOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
+    "TopicPreferenceTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
-    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
+    "DashboardAttributesOutputTypeDef",
     "DashboardAttributesTypeDef",
+    "DashboardOptionsOutputTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteContactListRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteCustomVerificationEmailTemplateRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
+    "EmailTemplateContentOutputTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "PinpointDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SendingOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
+    "TopicOutputTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
+    "ImportDataSourceOutputTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
+    "GuardianAttributesOutputTypeDef",
     "GuardianAttributesTypeDef",
+    "GuardianOptionsOutputTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
+    "SuppressionListDestinationOutputTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
@@ -174,99 +190,109 @@
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
-    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "BatchGetMetricDataResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "CreateImportJobResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateContactListRequestRequestTypeDef",
-    "GetContactListResponseTypeDef",
     "UpdateContactListRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetContactListResponseTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
+    "VdmAttributesOutputTypeDef",
     "VdmAttributesTypeDef",
+    "VdmOptionsOutputTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
+    "ImportDestinationOutputTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
-    "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
+    "CreateImportJobRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -319,14 +345,25 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
@@ -386,23 +423,40 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchDimensionConfigurationOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueSource": DimensionValueSourceType,
+        "DefaultDimensionValue": str,
+    },
+)
+
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
 )
 
+ContactListDestinationOutputTypeDef = TypedDict(
+    "ContactListDestinationOutputTypeDef",
+    {
+        "ContactListName": str,
+        "ContactListImportAction": ContactListImportActionType,
+    },
+)
+
 ContactListDestinationTypeDef = TypedDict(
     "ContactListDestinationTypeDef",
     {
         "ContactListName": str,
         "ContactListImportAction": ContactListImportActionType,
     },
 )
@@ -412,16 +466,16 @@
     {
         "ContactListName": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-TopicPreferenceTypeDef = TypedDict(
-    "TopicPreferenceTypeDef",
+TopicPreferenceOutputTypeDef = TypedDict(
+    "TopicPreferenceOutputTypeDef",
     {
         "TopicName": str,
         "SubscriptionStatus": SubscriptionStatusType,
     },
 )
 
 DeliveryOptionsTypeDef = TypedDict(
@@ -490,35 +544,34 @@
 )
 
 
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
 
+TopicPreferenceTypeDef = TypedDict(
+    "TopicPreferenceTypeDef",
+    {
+        "TopicName": str,
+        "SubscriptionStatus": SubscriptionStatusType,
+    },
+)
+
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -562,22 +615,14 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -605,22 +650,38 @@
         "SpamRawCount": int,
         "ProjectedInbox": int,
         "ProjectedSpam": int,
     },
     total=False,
 )
 
+DashboardAttributesOutputTypeDef = TypedDict(
+    "DashboardAttributesOutputTypeDef",
+    {
+        "EngagementMetrics": FeatureStatusType,
+    },
+    total=False,
+)
+
 DashboardAttributesTypeDef = TypedDict(
     "DashboardAttributesTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
 
+DashboardOptionsOutputTypeDef = TypedDict(
+    "DashboardOptionsOutputTypeDef",
+    {
+        "EngagementMetrics": FeatureStatusType,
+    },
+    total=False,
+)
+
 DashboardOptionsTypeDef = TypedDict(
     "DashboardOptionsTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
@@ -736,14 +797,23 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
+DeliveryOptionsOutputTypeDef = TypedDict(
+    "DeliveryOptionsOutputTypeDef",
+    {
+        "TlsPolicy": TlsPolicyType,
+        "SendingPoolName": str,
+    },
+    total=False,
+)
+
 DomainDeliverabilityCampaignTypeDef = TypedDict(
     "DomainDeliverabilityCampaignTypeDef",
     {
         "CampaignId": str,
         "ImageUrl": str,
         "Subject": str,
         "FromAddress": str,
@@ -757,30 +827,49 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
+    {
+        "Global": bool,
+        "TrackedIsps": List[str],
+    },
+    total=False,
+)
+
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": List[str],
+        "TrackedIsps": Sequence[str],
     },
     total=False,
 )
 
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+EmailTemplateContentOutputTypeDef = TypedDict(
+    "EmailTemplateContentOutputTypeDef",
+    {
+        "Subject": str,
+        "Text": str,
+        "Html": str,
+    },
+    total=False,
+)
+
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -805,14 +894,37 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "DeliveryStreamArn": str,
+    },
+)
+
+PinpointDestinationOutputTypeDef = TypedDict(
+    "PinpointDestinationOutputTypeDef",
+    {
+        "ApplicationArn": str,
+    },
+    total=False,
+)
+
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "FailedRecordsS3Url": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -853,21 +965,82 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": datetime,
+    },
+    total=False,
+)
+
+SendingOptionsOutputTypeDef = TypedDict(
+    "SendingOptionsOutputTypeDef",
+    {
+        "SendingEnabled": bool,
+    },
+    total=False,
+)
+
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": List[SuppressionListReasonType],
+    },
+    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+TrackingOptionsOutputTypeDef = TypedDict(
+    "TrackingOptionsOutputTypeDef",
+    {
+        "CustomRedirectDomain": str,
+    },
+)
+
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
+_RequiredTopicOutputTypeDef = TypedDict(
+    "_RequiredTopicOutputTypeDef",
+    {
+        "TopicName": str,
+        "DisplayName": str,
+        "DefaultSubscriptionStatus": SubscriptionStatusType,
+    },
+)
+_OptionalTopicOutputTypeDef = TypedDict(
+    "_OptionalTopicOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+
+class TopicOutputTypeDef(_RequiredTopicOutputTypeDef, _OptionalTopicOutputTypeDef):
+    pass
+
+
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
     },
 )
@@ -875,27 +1048,14 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -954,22 +1114,14 @@
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -992,29 +1144,53 @@
 GetImportJobRequestRequestTypeDef = TypedDict(
     "GetImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+ImportDataSourceOutputTypeDef = TypedDict(
+    "ImportDataSourceOutputTypeDef",
+    {
+        "S3Url": str,
+        "DataFormat": DataFormatType,
+    },
+)
+
 GetSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "GetSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+GuardianAttributesOutputTypeDef = TypedDict(
+    "GuardianAttributesOutputTypeDef",
+    {
+        "OptimizedSharedDelivery": FeatureStatusType,
+    },
+    total=False,
+)
+
 GuardianAttributesTypeDef = TypedDict(
     "GuardianAttributesTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
 
+GuardianOptionsOutputTypeDef = TypedDict(
+    "GuardianOptionsOutputTypeDef",
+    {
+        "OptimizedSharedDelivery": FeatureStatusType,
+    },
+    total=False,
+)
+
 GuardianOptionsTypeDef = TypedDict(
     "GuardianOptionsTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
@@ -1026,14 +1202,21 @@
         "IdentityName": str,
         "SendingEnabled": bool,
         "VerificationStatus": VerificationStatusType,
     },
     total=False,
 )
 
+SuppressionListDestinationOutputTypeDef = TypedDict(
+    "SuppressionListDestinationOutputTypeDef",
+    {
+        "SuppressionListImportAction": SuppressionListImportActionType,
+    },
+)
+
 SuppressionListDestinationTypeDef = TypedDict(
     "SuppressionListDestinationTypeDef",
     {
         "SuppressionListImportAction": SuppressionListImportActionType,
     },
 )
 
@@ -1042,23 +1225,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1087,23 +1261,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1459,23 +1624,14 @@
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
@@ -1529,25 +1685,14 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1563,30 +1708,14 @@
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
 
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1596,22 +1725,14 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1658,23 +1779,112 @@
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1691,15 +1901,22 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1707,93 +1924,45 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
+        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
         "UnsubscribeAll": bool,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
-
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
+        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1809,22 +1978,14 @@
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1848,27 +2009,14 @@
 
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
 
-GetContactListResponseTypeDef = TypedDict(
-    "GetContactListResponseTypeDef",
-    {
-        "ContactListName": str,
-        "Topics": List[TopicTypeDef],
-        "Description": str,
-        "CreatedTimestamp": datetime,
-        "LastUpdatedTimestamp": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalUpdateContactListRequestRequestTypeDef = TypedDict(
@@ -1883,14 +2031,62 @@
 
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
@@ -1936,49 +2132,40 @@
 
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1998,77 +2185,117 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": str,
+        "SubscriptionStartDate": datetime,
+        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
     },
+    total=False,
 )
 
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": datetime,
+        "SubscriptionStartDate": Union[datetime, str],
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateContent": EmailTemplateContentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactListResponseTypeDef = TypedDict(
+    "GetContactListResponseTypeDef",
+    {
+        "ContactListName": str,
+        "Topics": List[TopicOutputTypeDef],
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "LastUpdatedTimestamp": datetime,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
@@ -2082,21 +2309,43 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredVdmAttributesOutputTypeDef = TypedDict(
+    "_RequiredVdmAttributesOutputTypeDef",
+    {
+        "VdmEnabled": FeatureStatusType,
+    },
+)
+_OptionalVdmAttributesOutputTypeDef = TypedDict(
+    "_OptionalVdmAttributesOutputTypeDef",
+    {
+        "DashboardAttributes": DashboardAttributesOutputTypeDef,
+        "GuardianAttributes": GuardianAttributesOutputTypeDef,
     },
+    total=False,
 )
 
+
+class VdmAttributesOutputTypeDef(
+    _RequiredVdmAttributesOutputTypeDef, _OptionalVdmAttributesOutputTypeDef
+):
+    pass
+
+
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
     },
 )
 _OptionalVdmAttributesTypeDef = TypedDict(
@@ -2109,32 +2358,50 @@
 )
 
 
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
 
+VdmOptionsOutputTypeDef = TypedDict(
+    "VdmOptionsOutputTypeDef",
+    {
+        "DashboardOptions": DashboardOptionsOutputTypeDef,
+        "GuardianOptions": GuardianOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
     total=False,
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportDestinationOutputTypeDef = TypedDict(
+    "ImportDestinationOutputTypeDef",
+    {
+        "SuppressionListDestination": SuppressionListDestinationOutputTypeDef,
+        "ContactListDestination": ContactListDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
         "ContactListDestination": ContactListDestinationTypeDef,
     },
     total=False,
@@ -2150,24 +2417,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2202,78 +2469,78 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
+        "PinpointDestination": PinpointDestinationOutputTypeDef,
     },
     total=False,
 )
 
 
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "DashboardEnabled": bool,
@@ -2298,41 +2565,56 @@
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
-        "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VdmAttributes": VdmAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
     },
 )
 
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsOutputTypeDef,
+        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "SendingOptions": SendingOptionsOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "VdmOptions": VdmOptionsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -2353,29 +2635,14 @@
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
-        "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
@@ -2390,51 +2657,51 @@
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
 
-CreateImportJobRequestRequestTypeDef = TypedDict(
-    "CreateImportJobRequestRequestTypeDef",
-    {
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
-    },
-)
-
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
+        "ImportDestination": ImportDestinationOutputTypeDef,
+        "ImportDataSource": ImportDataSourceOutputTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDestination": ImportDestinationOutputTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
     },
     total=False,
 )
 
+CreateImportJobRequestRequestTypeDef = TypedDict(
+    "CreateImportJobRequestRequestTypeDef",
+    {
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
+    },
+)
+
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalListContactsRequestRequestTypeDef = TypedDict(
@@ -2474,28 +2741,36 @@
     pass
 
 
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2506,28 +2781,20 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2/type_defs.pyi` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -63,99 +63,115 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ReviewDetailsTypeDef",
     "BatchGetMetricDataQueryTypeDef",
     "MetricDataErrorTypeDef",
     "MetricDataResultTypeDef",
+    "ResponseMetadataTypeDef",
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
     "TemplateTypeDef",
     "BulkEmailEntryResultTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
+    "ContactListDestinationOutputTypeDef",
     "ContactListDestinationTypeDef",
     "ContactListTypeDef",
-    "TopicPreferenceTypeDef",
+    "TopicPreferenceOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "SuppressionOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
     "TopicTypeDef",
+    "TopicPreferenceTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     "DkimSigningAttributesTypeDef",
     "DkimAttributesTypeDef",
     "EmailTemplateContentTypeDef",
     "ImportDataSourceTypeDef",
-    "CreateImportJobResponseTypeDef",
     "CustomVerificationEmailTemplateMetadataTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
+    "DashboardAttributesOutputTypeDef",
     "DashboardAttributesTypeDef",
+    "DashboardOptionsOutputTypeDef",
     "DashboardOptionsTypeDef",
     "DedicatedIpPoolTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteContactListRequestRequestTypeDef",
     "DeleteContactRequestRequestTypeDef",
     "DeleteCustomVerificationEmailTemplateRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityPolicyRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeleteEmailTemplateRequestRequestTypeDef",
     "DeleteSuppressedDestinationRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
+    "EmailTemplateContentOutputTypeDef",
     "EmailTemplateMetadataTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "PinpointDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "FailureInfoTypeDef",
     "SendQuotaTypeDef",
     "SuppressionAttributesTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SendingOptionsOutputTypeDef",
+    "SuppressionOptionsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "GetContactListRequestRequestTypeDef",
+    "TopicOutputTypeDef",
     "GetContactRequestRequestTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetDedicatedIpPoolRequestRequestTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
-    "GetEmailIdentityPoliciesResponseTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "GetEmailTemplateRequestRequestTypeDef",
     "GetImportJobRequestRequestTypeDef",
+    "ImportDataSourceOutputTypeDef",
     "GetSuppressedDestinationRequestRequestTypeDef",
+    "GuardianAttributesOutputTypeDef",
     "GuardianAttributesTypeDef",
+    "GuardianOptionsOutputTypeDef",
     "GuardianOptionsTypeDef",
     "IdentityInfoTypeDef",
+    "SuppressionListDestinationOutputTypeDef",
     "SuppressionListDestinationTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "ListContactListsRequestRequestTypeDef",
     "TopicFilterTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListEmailTemplatesRequestRequestTypeDef",
     "ListImportJobsRequestRequestTypeDef",
     "ListManagementOptionsTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
@@ -173,99 +189,109 @@
     "PutConfigurationSetSuppressionOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "PutSuppressedDestinationRequestRequestTypeDef",
     "ReplacementTemplateTypeDef",
-    "ResponseMetadataTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
     "SuppressedDestinationAttributesTypeDef",
     "TestRenderEmailTemplateRequestRequestTypeDef",
-    "TestRenderEmailTemplateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "UpdateEmailIdentityPolicyRequestRequestTypeDef",
     "AccountDetailsTypeDef",
     "BatchGetMetricDataRequestRequestTypeDef",
     "BatchGetMetricDataResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "CreateImportJobResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "TestRenderEmailTemplateResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
     "BulkEmailContentTypeDef",
     "SendBulkEmailResponseTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "ListContactListsResponseTypeDef",
     "ContactTypeDef",
-    "CreateContactRequestRequestTypeDef",
     "GetContactResponseTypeDef",
-    "UpdateContactRequestRequestTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateContactListRequestRequestTypeDef",
-    "GetContactListResponseTypeDef",
     "UpdateContactListRequestRequestTypeDef",
+    "CreateContactRequestRequestTypeDef",
+    "UpdateContactRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "CreateEmailTemplateRequestRequestTypeDef",
-    "GetEmailTemplateResponseTypeDef",
     "UpdateEmailTemplateRequestRequestTypeDef",
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpPoolResponseTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
+    "GetEmailTemplateResponseTypeDef",
     "ListEmailTemplatesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetContactListResponseTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
+    "VdmAttributesOutputTypeDef",
     "VdmAttributesTypeDef",
+    "VdmOptionsOutputTypeDef",
     "VdmOptionsTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
+    "ImportDestinationOutputTypeDef",
     "ImportDestinationTypeDef",
     "ListContactsFilterTypeDef",
     "ListRecommendationsResponseTypeDef",
     "ListSuppressedDestinationsResponseTypeDef",
     "ReplacementEmailContentTypeDef",
     "SuppressedDestinationTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "ListContactsResponseTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "GetAccountResponseTypeDef",
     "PutAccountVdmAttributesRequestRequestTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
     "GetConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
     "PutConfigurationSetVdmOptionsRequestRequestTypeDef",
-    "CreateImportJobRequestRequestTypeDef",
     "GetImportJobResponseTypeDef",
     "ImportJobSummaryTypeDef",
+    "CreateImportJobRequestRequestTypeDef",
     "ListContactsRequestRequestTypeDef",
     "BulkEmailEntryTypeDef",
     "GetSuppressedDestinationResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "ListImportJobsResponseTypeDef",
     "SendBulkEmailRequestRequestTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 ReviewDetailsTypeDef = TypedDict(
@@ -316,14 +342,25 @@
         "Id": str,
         "Timestamps": List[datetime],
         "Values": List[int],
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
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
         "RblName": str,
         "ListingTime": datetime,
         "Description": str,
     },
@@ -381,23 +418,40 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchDimensionConfigurationOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueSource": DimensionValueSourceType,
+        "DefaultDimensionValue": str,
+    },
+)
+
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
 )
 
+ContactListDestinationOutputTypeDef = TypedDict(
+    "ContactListDestinationOutputTypeDef",
+    {
+        "ContactListName": str,
+        "ContactListImportAction": ContactListImportActionType,
+    },
+)
+
 ContactListDestinationTypeDef = TypedDict(
     "ContactListDestinationTypeDef",
     {
         "ContactListName": str,
         "ContactListImportAction": ContactListImportActionType,
     },
 )
@@ -407,16 +461,16 @@
     {
         "ContactListName": str,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-TopicPreferenceTypeDef = TypedDict(
-    "TopicPreferenceTypeDef",
+TopicPreferenceOutputTypeDef = TypedDict(
+    "TopicPreferenceOutputTypeDef",
     {
         "TopicName": str,
         "SubscriptionStatus": SubscriptionStatusType,
     },
 )
 
 DeliveryOptionsTypeDef = TypedDict(
@@ -483,35 +537,34 @@
     },
     total=False,
 )
 
 class TopicTypeDef(_RequiredTopicTypeDef, _OptionalTopicTypeDef):
     pass
 
+TopicPreferenceTypeDef = TypedDict(
+    "TopicPreferenceTypeDef",
+    {
+        "TopicName": str,
+        "SubscriptionStatus": SubscriptionStatusType,
+    },
+)
+
 CreateCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
-    {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateEmailIdentityPolicyRequestRequestTypeDef = TypedDict(
     "CreateEmailIdentityPolicyRequestRequestTypeDef",
     {
         "EmailIdentity": str,
         "PolicyName": str,
         "Policy": str,
     },
@@ -555,22 +608,14 @@
     "ImportDataSourceTypeDef",
     {
         "S3Url": str,
         "DataFormat": DataFormatType,
     },
 )
 
-CreateImportJobResponseTypeDef = TypedDict(
-    "CreateImportJobResponseTypeDef",
-    {
-        "JobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomVerificationEmailTemplateMetadataTypeDef = TypedDict(
     "CustomVerificationEmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -598,22 +643,38 @@
         "SpamRawCount": int,
         "ProjectedInbox": int,
         "ProjectedSpam": int,
     },
     total=False,
 )
 
+DashboardAttributesOutputTypeDef = TypedDict(
+    "DashboardAttributesOutputTypeDef",
+    {
+        "EngagementMetrics": FeatureStatusType,
+    },
+    total=False,
+)
+
 DashboardAttributesTypeDef = TypedDict(
     "DashboardAttributesTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
 
+DashboardOptionsOutputTypeDef = TypedDict(
+    "DashboardOptionsOutputTypeDef",
+    {
+        "EngagementMetrics": FeatureStatusType,
+    },
+    total=False,
+)
+
 DashboardOptionsTypeDef = TypedDict(
     "DashboardOptionsTypeDef",
     {
         "EngagementMetrics": FeatureStatusType,
     },
     total=False,
 )
@@ -727,14 +788,23 @@
         "FromEmailAddress": str,
         "CreateDate": datetime,
         "DeliverabilityTestStatus": DeliverabilityTestStatusType,
     },
     total=False,
 )
 
+DeliveryOptionsOutputTypeDef = TypedDict(
+    "DeliveryOptionsOutputTypeDef",
+    {
+        "TlsPolicy": TlsPolicyType,
+        "SendingPoolName": str,
+    },
+    total=False,
+)
+
 DomainDeliverabilityCampaignTypeDef = TypedDict(
     "DomainDeliverabilityCampaignTypeDef",
     {
         "CampaignId": str,
         "ImageUrl": str,
         "Subject": str,
         "FromAddress": str,
@@ -748,30 +818,49 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
+InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
+    "InboxPlacementTrackingOptionOutputTypeDef",
+    {
+        "Global": bool,
+        "TrackedIsps": List[str],
+    },
+    total=False,
+)
+
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": List[str],
+        "TrackedIsps": Sequence[str],
     },
     total=False,
 )
 
 RawMessageTypeDef = TypedDict(
     "RawMessageTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
+EmailTemplateContentOutputTypeDef = TypedDict(
+    "EmailTemplateContentOutputTypeDef",
+    {
+        "Subject": str,
+        "Text": str,
+        "Html": str,
+    },
+    total=False,
+)
+
 EmailTemplateMetadataTypeDef = TypedDict(
     "EmailTemplateMetadataTypeDef",
     {
         "TemplateName": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
@@ -796,14 +885,37 @@
 SnsDestinationTypeDef = TypedDict(
     "SnsDestinationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
+    {
+        "IamRoleArn": str,
+        "DeliveryStreamArn": str,
+    },
+)
+
+PinpointDestinationOutputTypeDef = TypedDict(
+    "PinpointDestinationOutputTypeDef",
+    {
+        "ApplicationArn": str,
+    },
+    total=False,
+)
+
+SnsDestinationOutputTypeDef = TypedDict(
+    "SnsDestinationOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "FailedRecordsS3Url": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -844,21 +956,80 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
+ReputationOptionsOutputTypeDef = TypedDict(
+    "ReputationOptionsOutputTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": datetime,
+    },
+    total=False,
+)
+
+SendingOptionsOutputTypeDef = TypedDict(
+    "SendingOptionsOutputTypeDef",
+    {
+        "SendingEnabled": bool,
+    },
+    total=False,
+)
+
+SuppressionOptionsOutputTypeDef = TypedDict(
+    "SuppressionOptionsOutputTypeDef",
+    {
+        "SuppressedReasons": List[SuppressionListReasonType],
+    },
+    total=False,
+)
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+TrackingOptionsOutputTypeDef = TypedDict(
+    "TrackingOptionsOutputTypeDef",
+    {
+        "CustomRedirectDomain": str,
+    },
+)
+
 GetContactListRequestRequestTypeDef = TypedDict(
     "GetContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 
+_RequiredTopicOutputTypeDef = TypedDict(
+    "_RequiredTopicOutputTypeDef",
+    {
+        "TopicName": str,
+        "DisplayName": str,
+        "DefaultSubscriptionStatus": SubscriptionStatusType,
+    },
+)
+_OptionalTopicOutputTypeDef = TypedDict(
+    "_OptionalTopicOutputTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class TopicOutputTypeDef(_RequiredTopicOutputTypeDef, _OptionalTopicOutputTypeDef):
+    pass
+
 GetContactRequestRequestTypeDef = TypedDict(
     "GetContactRequestRequestTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
     },
 )
@@ -866,27 +1037,14 @@
 GetCustomVerificationEmailTemplateRequestRequestTypeDef = TypedDict(
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
-GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "FromEmailAddress": str,
-        "TemplateSubject": str,
-        "TemplateContent": str,
-        "SuccessRedirectionURL": str,
-        "FailureRedirectionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 
@@ -945,22 +1103,14 @@
 GetEmailIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityPoliciesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
-GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetEmailIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -983,29 +1133,53 @@
 GetImportJobRequestRequestTypeDef = TypedDict(
     "GetImportJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
+ImportDataSourceOutputTypeDef = TypedDict(
+    "ImportDataSourceOutputTypeDef",
+    {
+        "S3Url": str,
+        "DataFormat": DataFormatType,
+    },
+)
+
 GetSuppressedDestinationRequestRequestTypeDef = TypedDict(
     "GetSuppressedDestinationRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+GuardianAttributesOutputTypeDef = TypedDict(
+    "GuardianAttributesOutputTypeDef",
+    {
+        "OptimizedSharedDelivery": FeatureStatusType,
+    },
+    total=False,
+)
+
 GuardianAttributesTypeDef = TypedDict(
     "GuardianAttributesTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
 
+GuardianOptionsOutputTypeDef = TypedDict(
+    "GuardianOptionsOutputTypeDef",
+    {
+        "OptimizedSharedDelivery": FeatureStatusType,
+    },
+    total=False,
+)
+
 GuardianOptionsTypeDef = TypedDict(
     "GuardianOptionsTypeDef",
     {
         "OptimizedSharedDelivery": FeatureStatusType,
     },
     total=False,
 )
@@ -1017,14 +1191,21 @@
         "IdentityName": str,
         "SendingEnabled": bool,
         "VerificationStatus": VerificationStatusType,
     },
     total=False,
 )
 
+SuppressionListDestinationOutputTypeDef = TypedDict(
+    "SuppressionListDestinationOutputTypeDef",
+    {
+        "SuppressionListImportAction": SuppressionListImportActionType,
+    },
+)
+
 SuppressionListDestinationTypeDef = TypedDict(
     "SuppressionListDestinationTypeDef",
     {
         "SuppressionListImportAction": SuppressionListImportActionType,
     },
 )
 
@@ -1033,23 +1214,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListContactListsRequestRequestTypeDef = TypedDict(
     "ListContactListsRequestRequestTypeDef",
     {
         "PageSize": int,
         "NextToken": str,
     },
     total=False,
@@ -1078,23 +1250,14 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-ListDedicatedIpPoolsResponseTypeDef = TypedDict(
-    "ListDedicatedIpPoolsResponseTypeDef",
-    {
-        "DedicatedIpPools": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -1430,23 +1593,14 @@
 
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
-    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
-    {
-        "DkimStatus": DkimStatusType,
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
@@ -1496,25 +1650,14 @@
     "ReplacementTemplateTypeDef",
     {
         "ReplacementTemplateData": str,
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
 _RequiredSendCustomVerificationEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "EmailAddress": str,
         "TemplateName": str,
     },
 )
@@ -1528,30 +1671,14 @@
 
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-SendCustomVerificationEmailResponseTypeDef = TypedDict(
-    "SendCustomVerificationEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SuppressedDestinationAttributesTypeDef = TypedDict(
     "SuppressedDestinationAttributesTypeDef",
     {
         "MessageId": str,
         "FeedbackId": str,
     },
     total=False,
@@ -1561,22 +1688,14 @@
     "TestRenderEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderEmailTemplateResponseTypeDef = TypedDict(
-    "TestRenderEmailTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1623,23 +1742,112 @@
 )
 
 BatchGetMetricDataResponseTypeDef = TypedDict(
     "BatchGetMetricDataResponseTypeDef",
     {
         "Results": List[MetricDataResultTypeDef],
         "Errors": List[MetricDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImportJobResponseTypeDef = TypedDict(
+    "CreateImportJobResponseTypeDef",
+    {
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomVerificationEmailTemplateResponseTypeDef = TypedDict(
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "FromEmailAddress": str,
+        "TemplateSubject": str,
+        "TemplateContent": str,
+        "SuccessRedirectionURL": str,
+        "FailureRedirectionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEmailIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetEmailIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDedicatedIpPoolsResponseTypeDef = TypedDict(
+    "ListDedicatedIpPoolsResponseTypeDef",
+    {
+        "DedicatedIpPools": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEmailIdentityDkimSigningAttributesResponseTypeDef = TypedDict(
+    "PutEmailIdentityDkimSigningAttributesResponseTypeDef",
+    {
+        "DkimStatus": DkimStatusType,
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendCustomVerificationEmailResponseTypeDef = TypedDict(
+    "SendCustomVerificationEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderEmailTemplateResponseTypeDef = TypedDict(
+    "TestRenderEmailTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlacklistReportsResponseTypeDef = TypedDict(
     "GetBlacklistReportsResponseTypeDef",
     {
         "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
@@ -1656,15 +1864,22 @@
     total=False,
 )
 
 SendBulkEmailResponseTypeDef = TypedDict(
     "SendBulkEmailResponseTypeDef",
     {
         "BulkEmailEntryResults": List[BulkEmailEntryResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
     },
 )
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
@@ -1672,89 +1887,45 @@
 )
 
 ListContactListsResponseTypeDef = TypedDict(
     "ListContactListsResponseTypeDef",
     {
         "ContactLists": List[ContactListTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
+        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
         "UnsubscribeAll": bool,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-_RequiredCreateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalCreateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-class CreateContactRequestRequestTypeDef(
-    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
-):
-    pass
-
 GetContactResponseTypeDef = TypedDict(
     "GetContactResponseTypeDef",
     {
         "ContactListName": str,
         "EmailAddress": str,
-        "TopicPreferences": List[TopicPreferenceTypeDef],
-        "TopicDefaultPreferences": List[TopicPreferenceTypeDef],
+        "TopicPreferences": List[TopicPreferenceOutputTypeDef],
+        "TopicDefaultPreferences": List[TopicPreferenceOutputTypeDef],
         "UnsubscribeAll": bool,
         "AttributesData": str,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateContactRequestRequestTypeDef",
-    {
-        "ContactListName": str,
-        "EmailAddress": str,
-    },
-)
-_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateContactRequestRequestTypeDef",
-    {
-        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
-        "UnsubscribeAll": bool,
-        "AttributesData": str,
-    },
-    total=False,
-)
-
-class UpdateContactRequestRequestTypeDef(
-    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "PoolName": str,
     },
 )
 _OptionalCreateDedicatedIpPoolRequestRequestTypeDef = TypedDict(
@@ -1768,22 +1939,14 @@
 
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1805,27 +1968,14 @@
 )
 
 class CreateContactListRequestRequestTypeDef(
     _RequiredCreateContactListRequestRequestTypeDef, _OptionalCreateContactListRequestRequestTypeDef
 ):
     pass
 
-GetContactListResponseTypeDef = TypedDict(
-    "GetContactListResponseTypeDef",
-    {
-        "ContactListName": str,
-        "Topics": List[TopicTypeDef],
-        "Description": str,
-        "CreatedTimestamp": datetime,
-        "LastUpdatedTimestamp": datetime,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateContactListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContactListRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalUpdateContactListRequestRequestTypeDef = TypedDict(
@@ -1838,14 +1988,58 @@
 )
 
 class UpdateContactListRequestRequestTypeDef(
     _RequiredUpdateContactListRequestRequestTypeDef, _OptionalUpdateContactListRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalCreateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+class CreateContactRequestRequestTypeDef(
+    _RequiredCreateContactRequestRequestTypeDef, _OptionalCreateContactRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateContactRequestRequestTypeDef",
+    {
+        "ContactListName": str,
+        "EmailAddress": str,
+    },
+)
+_OptionalUpdateContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateContactRequestRequestTypeDef",
+    {
+        "TopicPreferences": Sequence[TopicPreferenceTypeDef],
+        "UnsubscribeAll": bool,
+        "AttributesData": str,
+    },
+    total=False,
+)
+
+class UpdateContactRequestRequestTypeDef(
+    _RequiredUpdateContactRequestRequestTypeDef, _OptionalUpdateContactRequestRequestTypeDef
+):
+    pass
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
@@ -1887,49 +2081,40 @@
 
 CreateEmailIdentityResponseTypeDef = TypedDict(
     "CreateEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEmailTemplateRequestRequestTypeDef = TypedDict(
     "CreateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
-GetEmailTemplateResponseTypeDef = TypedDict(
-    "GetEmailTemplateResponseTypeDef",
-    {
-        "TemplateName": str,
-        "TemplateContent": EmailTemplateContentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEmailTemplateRequestRequestTypeDef = TypedDict(
     "UpdateEmailTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateContent": EmailTemplateContentTypeDef,
     },
 )
 
 ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesResponseTypeDef",
     {
         "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1949,77 +2134,117 @@
     total=False,
 )
 
 GetDedicatedIpPoolResponseTypeDef = TypedDict(
     "GetDedicatedIpPoolResponseTypeDef",
     {
         "DedicatedIpPool": DedicatedIpPoolTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpResponseTypeDef = TypedDict(
     "GetDedicatedIpResponseTypeDef",
     {
         "DedicatedIp": DedicatedIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDedicatedIpsResponseTypeDef = TypedDict(
     "GetDedicatedIpsResponseTypeDef",
     {
         "DedicatedIps": List[DedicatedIpTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeliverabilityTestReportsResponseTypeDef = TypedDict(
     "ListDeliverabilityTestReportsResponseTypeDef",
     {
         "DeliverabilityTestReports": List[DeliverabilityTestReportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainDeliverabilityCampaignResponseTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     {
         "DomainDeliverabilityCampaign": DomainDeliverabilityCampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainDeliverabilityCampaignsResponseTypeDef = TypedDict(
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
+    {
+        "Domain": str,
+        "SubscriptionStartDate": datetime,
+        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
+    },
+    total=False,
+)
+
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": datetime,
+        "SubscriptionStartDate": Union[datetime, str],
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
+GetEmailTemplateResponseTypeDef = TypedDict(
+    "GetEmailTemplateResponseTypeDef",
+    {
+        "TemplateName": str,
+        "TemplateContent": EmailTemplateContentOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListEmailTemplatesResponseTypeDef = TypedDict(
     "ListEmailTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[EmailTemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContactListResponseTypeDef = TypedDict(
+    "GetContactListResponseTypeDef",
+    {
+        "ContactListName": str,
+        "Topics": List[TopicOutputTypeDef],
+        "Description": str,
+        "CreatedTimestamp": datetime,
+        "LastUpdatedTimestamp": datetime,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
@@ -2033,21 +2258,41 @@
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
         "Policies": Dict[str, str],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "ConfigurationSetName": str,
         "VerificationStatus": VerificationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredVdmAttributesOutputTypeDef = TypedDict(
+    "_RequiredVdmAttributesOutputTypeDef",
+    {
+        "VdmEnabled": FeatureStatusType,
+    },
+)
+_OptionalVdmAttributesOutputTypeDef = TypedDict(
+    "_OptionalVdmAttributesOutputTypeDef",
+    {
+        "DashboardAttributes": DashboardAttributesOutputTypeDef,
+        "GuardianAttributes": GuardianAttributesOutputTypeDef,
+    },
+    total=False,
+)
+
+class VdmAttributesOutputTypeDef(
+    _RequiredVdmAttributesOutputTypeDef, _OptionalVdmAttributesOutputTypeDef
+):
+    pass
+
 _RequiredVdmAttributesTypeDef = TypedDict(
     "_RequiredVdmAttributesTypeDef",
     {
         "VdmEnabled": FeatureStatusType,
     },
 )
 _OptionalVdmAttributesTypeDef = TypedDict(
@@ -2058,32 +2303,50 @@
     },
     total=False,
 )
 
 class VdmAttributesTypeDef(_RequiredVdmAttributesTypeDef, _OptionalVdmAttributesTypeDef):
     pass
 
+VdmOptionsOutputTypeDef = TypedDict(
+    "VdmOptionsOutputTypeDef",
+    {
+        "DashboardOptions": DashboardOptionsOutputTypeDef,
+        "GuardianOptions": GuardianOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 VdmOptionsTypeDef = TypedDict(
     "VdmOptionsTypeDef",
     {
         "DashboardOptions": DashboardOptionsTypeDef,
         "GuardianOptions": GuardianOptionsTypeDef,
     },
     total=False,
 )
 
 ListEmailIdentitiesResponseTypeDef = TypedDict(
     "ListEmailIdentitiesResponseTypeDef",
     {
         "EmailIdentities": List[IdentityInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportDestinationOutputTypeDef = TypedDict(
+    "ImportDestinationOutputTypeDef",
+    {
+        "SuppressionListDestination": SuppressionListDestinationOutputTypeDef,
+        "ContactListDestination": ContactListDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImportDestinationTypeDef = TypedDict(
     "ImportDestinationTypeDef",
     {
         "SuppressionListDestination": SuppressionListDestinationTypeDef,
         "ContactListDestination": ContactListDestinationTypeDef,
     },
     total=False,
@@ -2099,24 +2362,24 @@
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSuppressedDestinationsResponseTypeDef = TypedDict(
     "ListSuppressedDestinationsResponseTypeDef",
     {
         "SuppressedDestinationSummaries": List[SuppressedDestinationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplacementEmailContentTypeDef = TypedDict(
     "ReplacementEmailContentTypeDef",
     {
         "ReplacementTemplate": ReplacementTemplateTypeDef,
@@ -2149,76 +2412,76 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SnsDestination": SnsDestinationOutputTypeDef,
+        "PinpointDestination": PinpointDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
-class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
-    pass
-
 ListContactsResponseTypeDef = TypedDict(
     "ListContactsResponseTypeDef",
     {
         "Contacts": List[ContactTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
     "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "DashboardEnabled": bool,
@@ -2241,41 +2504,56 @@
 GetDeliverabilityTestReportResponseTypeDef = TypedDict(
     "GetDeliverabilityTestReportResponseTypeDef",
     {
         "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
         "OverallPlacement": PlacementStatisticsTypeDef,
         "IspPlacements": List[IspPlacementTypeDef],
         "Message": str,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "SuppressionAttributes": SuppressionAttributesTypeDef,
         "Details": AccountDetailsTypeDef,
-        "VdmAttributes": VdmAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VdmAttributes": VdmAttributesOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountVdmAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountVdmAttributesRequestRequestTypeDef",
     {
         "VdmAttributes": VdmAttributesTypeDef,
     },
 )
 
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsOutputTypeDef,
+        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "SendingOptions": SendingOptionsOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "SuppressionOptions": SuppressionOptionsOutputTypeDef,
+        "VdmOptions": VdmOptionsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -2294,29 +2572,14 @@
 
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "SuppressionOptions": SuppressionOptionsTypeDef,
-        "VdmOptions": VdmOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef = TypedDict(
@@ -2329,51 +2592,51 @@
 
 class PutConfigurationSetVdmOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetVdmOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetVdmOptionsRequestRequestTypeDef,
 ):
     pass
 
-CreateImportJobRequestRequestTypeDef = TypedDict(
-    "CreateImportJobRequestRequestTypeDef",
-    {
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
-    },
-)
-
 GetImportJobResponseTypeDef = TypedDict(
     "GetImportJobResponseTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationTypeDef,
-        "ImportDataSource": ImportDataSourceTypeDef,
+        "ImportDestination": ImportDestinationOutputTypeDef,
+        "ImportDataSource": ImportDataSourceOutputTypeDef,
         "FailureInfo": FailureInfoTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "CompletedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportJobSummaryTypeDef = TypedDict(
     "ImportJobSummaryTypeDef",
     {
         "JobId": str,
-        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDestination": ImportDestinationOutputTypeDef,
         "JobStatus": JobStatusType,
         "CreatedTimestamp": datetime,
         "ProcessedRecordsCount": int,
         "FailedRecordsCount": int,
     },
     total=False,
 )
 
+CreateImportJobRequestRequestTypeDef = TypedDict(
+    "CreateImportJobRequestRequestTypeDef",
+    {
+        "ImportDestination": ImportDestinationTypeDef,
+        "ImportDataSource": ImportDataSourceTypeDef,
+    },
+)
+
 _RequiredListContactsRequestRequestTypeDef = TypedDict(
     "_RequiredListContactsRequestRequestTypeDef",
     {
         "ContactListName": str,
     },
 )
 _OptionalListContactsRequestRequestTypeDef = TypedDict(
@@ -2409,28 +2672,36 @@
 class BulkEmailEntryTypeDef(_RequiredBulkEmailEntryTypeDef, _OptionalBulkEmailEntryTypeDef):
     pass
 
 GetSuppressedDestinationResponseTypeDef = TypedDict(
     "GetSuppressedDestinationResponseTypeDef",
     {
         "SuppressedDestination": SuppressedDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
+    {
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -2441,28 +2712,20 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListImportJobsResponseTypeDef = TypedDict(
     "ListImportJobsResponseTypeDef",
     {
         "ImportJobs": List[ImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendBulkEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendBulkEmailRequestRequestTypeDef",
     {
         "DefaultContent": BulkEmailContentTypeDef,
```

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/PKG-INFO` & `mypy-boto3-sesv2-1.28.12/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sesv2
-Version: 1.28.0
-Summary: Type annotations for boto3.SESV2 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sesv2 type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-sesv2"></a>
 
 # mypy-boto3-sesv2
 
 [![PyPI - mypy-boto3-sesv2](https://img.shields.io/pypi/v/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sesv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-sesv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sesv2?color=blue)](https://pypistats.org/packages/mypy-boto3-sesv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sesv2)](https://pepy.tech/project/mypy-boto3-sesv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SESV2 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
+[boto3.SESV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#SESV2)
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
 [mypy-boto3-sesv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sesv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,99 +301,115 @@
 
 ```python
 from mypy_boto3_sesv2.type_defs import (
     ReviewDetailsTypeDef,
     BatchGetMetricDataQueryTypeDef,
     MetricDataErrorTypeDef,
     MetricDataResultTypeDef,
+    ResponseMetadataTypeDef,
     BlacklistEntryTypeDef,
     ContentTypeDef,
     TemplateTypeDef,
     BulkEmailEntryResultTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ContactListDestinationOutputTypeDef,
     ContactListDestinationTypeDef,
     ContactListTypeDef,
-    TopicPreferenceTypeDef,
+    TopicPreferenceOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     SuppressionOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
     TopicTypeDef,
+    TopicPreferenceTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityPolicyRequestRequestTypeDef,
     DkimSigningAttributesTypeDef,
     DkimAttributesTypeDef,
     EmailTemplateContentTypeDef,
     ImportDataSourceTypeDef,
-    CreateImportJobResponseTypeDef,
     CustomVerificationEmailTemplateMetadataTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
+    DashboardAttributesOutputTypeDef,
     DashboardAttributesTypeDef,
+    DashboardOptionsOutputTypeDef,
     DashboardOptionsTypeDef,
     DedicatedIpPoolTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteContactListRequestRequestTypeDef,
     DeleteContactRequestRequestTypeDef,
     DeleteCustomVerificationEmailTemplateRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityPolicyRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeleteEmailTemplateRequestRequestTypeDef,
     DeleteSuppressedDestinationRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
+    EmailTemplateContentOutputTypeDef,
     EmailTemplateMetadataTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     FailureInfoTypeDef,
     SendQuotaTypeDef,
     SuppressionAttributesTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    SuppressionOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetContactListRequestRequestTypeDef,
+    TopicOutputTypeDef,
     GetContactRequestRequestTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetDedicatedIpPoolRequestRequestTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityPoliciesRequestRequestTypeDef,
-    GetEmailIdentityPoliciesResponseTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     GetEmailTemplateRequestRequestTypeDef,
     GetImportJobRequestRequestTypeDef,
+    ImportDataSourceOutputTypeDef,
     GetSuppressedDestinationRequestRequestTypeDef,
+    GuardianAttributesOutputTypeDef,
     GuardianAttributesTypeDef,
+    GuardianOptionsOutputTypeDef,
     GuardianOptionsTypeDef,
     IdentityInfoTypeDef,
+    SuppressionListDestinationOutputTypeDef,
     SuppressionListDestinationTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     ListContactListsRequestRequestTypeDef,
     TopicFilterTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListEmailTemplatesRequestRequestTypeDef,
     ListImportJobsRequestRequestTypeDef,
     ListManagementOptionsTypeDef,
     ListRecommendationsRequestRequestTypeDef,
@@ -443,99 +427,109 @@
     PutConfigurationSetSuppressionOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpPoolScalingAttributesRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityConfigurationSetAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
-    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     PutSuppressedDestinationRequestRequestTypeDef,
     ReplacementTemplateTypeDef,
-    ResponseMetadataTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
     SuppressedDestinationAttributesTypeDef,
     TestRenderEmailTemplateRequestRequestTypeDef,
-    TestRenderEmailTemplateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     UpdateEmailIdentityPolicyRequestRequestTypeDef,
     AccountDetailsTypeDef,
     BatchGetMetricDataRequestRequestTypeDef,
     BatchGetMetricDataResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    CreateImportJobResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetEmailIdentityPoliciesResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    PutEmailIdentityDkimSigningAttributesResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    TestRenderEmailTemplateResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
     BulkEmailContentTypeDef,
     SendBulkEmailResponseTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     ListContactListsResponseTypeDef,
     ContactTypeDef,
-    CreateContactRequestRequestTypeDef,
     GetContactResponseTypeDef,
-    UpdateContactRequestRequestTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateContactListRequestRequestTypeDef,
-    GetContactListResponseTypeDef,
     UpdateContactListRequestRequestTypeDef,
+    CreateContactRequestRequestTypeDef,
+    UpdateContactRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
     PutEmailIdentityDkimSigningAttributesRequestRequestTypeDef,
     CreateEmailIdentityResponseTypeDef,
     CreateEmailTemplateRequestRequestTypeDef,
-    GetEmailTemplateResponseTypeDef,
     UpdateEmailTemplateRequestRequestTypeDef,
     ListCustomVerificationEmailTemplatesResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpPoolResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
+    GetEmailTemplateResponseTypeDef,
     ListEmailTemplatesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetContactListResponseTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
+    VdmAttributesOutputTypeDef,
     VdmAttributesTypeDef,
+    VdmOptionsOutputTypeDef,
     VdmOptionsTypeDef,
     ListEmailIdentitiesResponseTypeDef,
+    ImportDestinationOutputTypeDef,
     ImportDestinationTypeDef,
     ListContactsFilterTypeDef,
     ListRecommendationsResponseTypeDef,
     ListSuppressedDestinationsResponseTypeDef,
     ReplacementEmailContentTypeDef,
     SuppressedDestinationTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     ListContactsResponseTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     GetAccountResponseTypeDef,
     PutAccountVdmAttributesRequestRequestTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
     GetConfigurationSetResponseTypeDef,
+    CreateConfigurationSetRequestRequestTypeDef,
     PutConfigurationSetVdmOptionsRequestRequestTypeDef,
-    CreateImportJobRequestRequestTypeDef,
     GetImportJobResponseTypeDef,
     ImportJobSummaryTypeDef,
+    CreateImportJobRequestRequestTypeDef,
     ListContactsRequestRequestTypeDef,
     BulkEmailEntryTypeDef,
     GetSuppressedDestinationResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     ListImportJobsResponseTypeDef,
     SendBulkEmailRequestRequestTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-sesv2-1.28.0/mypy_boto3_sesv2.egg-info/SOURCES.txt` & `mypy-boto3-sesv2-1.28.12/mypy_boto3_sesv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sesv2-1.28.0/setup.py` & `mypy-boto3-sesv2-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sesv2",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sesv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SESV2 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SESV2 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

