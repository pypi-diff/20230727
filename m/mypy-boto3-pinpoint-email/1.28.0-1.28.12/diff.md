# Comparing `tmp/mypy-boto3-pinpoint-email-1.28.0.tar.gz` & `tmp/mypy-boto3-pinpoint-email-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.0.tar", last modified: Thu Jul  6 21:00:19 2023, max compression
+gzip compressed data, was "mypy-boto3-pinpoint-email-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
```

## Comparing `mypy-boto3-pinpoint-email-1.28.0.tar` & `mypy-boto3-pinpoint-email-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.138393 mypy-boto3-pinpoint-email-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-06 21:00:19.138393 mypy-boto3-pinpoint-email-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.130393 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-07-06 20:49:33.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34951 2023-07-06 20:49:33.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:19.138393 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:18.000000 mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:19.138393 mypy-boto3-pinpoint-email-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-06 20:49:32.000000 mypy-boto3-pinpoint-email-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32917 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9938 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-07-27 11:41:34.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37666 2023-07-27 11:41:35.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37632 2023-07-27 11:41:35.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18826 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:24.000000 mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.885162 mypy-boto3-pinpoint-email-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 11:41:33.000000 mypy-boto3-pinpoint-email-1.28.12/setup.py
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/LICENSE` & `mypy-boto3-pinpoint-email-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointEmail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,113 +354,125 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
+    ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    GetBlacklistReportsResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetConfigurationSetResponseTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BlacklistEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/README.md` & `mypy-boto3-pinpoint-email-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,113 +322,125 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
+    ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    GetBlacklistReportsResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetConfigurationSetResponseTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BlacklistEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__init__.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__init__.pyi` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/__main__.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PinpointEmail 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.PinpointEmail 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/client.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/client.pyi` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/literals.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BehaviorOnMxFailureType",
     "DeliverabilityDashboardAccountStatusType",
     "DeliverabilityTestStatusType",
     "DimensionValueSourceType",
     "DkimStatusType",
     "EventTypeType",
@@ -38,15 +37,14 @@
     "PinpointEmailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 DeliverabilityDashboardAccountStatusType = Literal["ACTIVE", "DISABLED", "PENDING_EXPIRATION"]
 DeliverabilityTestStatusType = Literal["COMPLETED", "IN_PROGRESS"]
 DimensionValueSourceType = Literal["EMAIL_HEADER", "LINK_TAG", "MESSAGE_TAG"]
 DkimStatusType = Literal["FAILED", "NOT_STARTED", "PENDING", "SUCCESS", "TEMPORARY_FAILURE"]
 EventTypeType = Literal[
     "BOUNCE", "CLICK", "COMPLAINT", "DELIVERY", "OPEN", "REJECT", "RENDERING_FAILURE", "SEND"
@@ -176,14 +174,15 @@
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
@@ -262,26 +261,28 @@
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

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/literals.pyi` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BehaviorOnMxFailureType",
     "DeliverabilityDashboardAccountStatusType",
     "DeliverabilityTestStatusType",
     "DimensionValueSourceType",
     "DkimStatusType",
     "EventTypeType",
@@ -37,14 +38,15 @@
     "PinpointEmailServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 BehaviorOnMxFailureType = Literal["REJECT_MESSAGE", "USE_DEFAULT_VALUE"]
 DeliverabilityDashboardAccountStatusType = Literal["ACTIVE", "DISABLED", "PENDING_EXPIRATION"]
 DeliverabilityTestStatusType = Literal["COMPLETED", "IN_PROGRESS"]
 DimensionValueSourceType = Literal["EMAIL_HEADER", "LINK_TAG", "MESSAGE_TAG"]
 DkimStatusType = Literal["FAILED", "NOT_STARTED", "PENDING", "SUCCESS", "TEMPORARY_FAILURE"]
 EventTypeType = Literal[
     "BOUNCE", "CLICK", "COMPLAINT", "DELIVERY", "OPEN", "REJECT", "RENDERING_FAILURE", "SEND"
@@ -174,14 +176,15 @@
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
@@ -260,26 +263,28 @@
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

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/paginator.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class GetDedicatedIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
     """
 
     def paginate(
-        self, *, PoolName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDedicatedIpsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
         """
 
 
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
         """
 
 
 class ListDedicatedIpPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDedicatedIpPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
         """
 
 
 class ListDeliverabilityTestReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeliverabilityTestReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
         """
 
 
 class ListEmailIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEmailIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/paginator.pyi` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class GetDedicatedIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
     """
 
     def paginate(
-        self, *, PoolName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDedicatedIpsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#getdedicatedipspaginator)
         """
 
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listconfigurationsetspaginator)
         """
 
 class ListDedicatedIpPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDedicatedIpPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdedicatedippoolspaginator)
         """
 
 class ListDeliverabilityTestReportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeliverabilityTestReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listdeliverabilitytestreportspaginator)
         """
 
 class ListEmailIdentitiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEmailIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/paginators/#listemailidentitiespaginator)
         """
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/type_defs.py` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -31,117 +31,128 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "PinpointDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SendingOptionsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendEmailResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "GetConfigurationSetResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "GetBlacklistReportsResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetConfigurationSetResponseTypeDef",
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
@@ -162,18 +173,25 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+CloudWatchDimensionConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchDimensionConfigurationOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueSource": DimensionValueSourceType,
+        "DefaultDimensionValue": str,
+    },
+)
 
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
@@ -217,20 +235,22 @@
 TrackingOptionsTypeDef = TypedDict(
     "TrackingOptionsTypeDef",
     {
         "CustomRedirectDomain": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DkimAttributesTypeDef = TypedDict(
     "DkimAttributesTypeDef",
     {
         "SigningEnabled": bool,
@@ -275,19 +295,17 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
-
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
-
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -322,14 +340,23 @@
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
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "ToAddresses": Sequence[str],
         "CcAddresses": Sequence[str],
         "BccAddresses": Sequence[str],
     },
@@ -353,19 +380,28 @@
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
@@ -401,14 +437,37 @@
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
 SendQuotaTypeDef = TypedDict(
     "SendQuotaTypeDef",
     {
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
     },
@@ -432,26 +491,59 @@
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
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
-GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PoolName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDedicatedIpsRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpsRequestRequestTypeDef",
     {
@@ -519,74 +611,32 @@
         "IdentityType": IdentityTypeType,
         "IdentityName": str,
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
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
-ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDedicatedIpPoolsRequestRequestTypeDef = TypedDict(
     "ListDedicatedIpPoolsRequestRequestTypeDef",
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
-ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -605,30 +655,20 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
-
-ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -645,24 +685,14 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
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
 PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "AutoWarmupEnabled": bool,
     },
     total=False,
 )
@@ -686,88 +716,80 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -790,44 +812,40 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -835,66 +853,44 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
-
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
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
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
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
 
-GetBlacklistReportsResponseTypeDef = TypedDict(
-    "GetBlacklistReportsResponseTypeDef",
-    {
-        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+    },
+)
+
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
@@ -908,52 +904,40 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-
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
@@ -972,42 +956,70 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    {
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
+GetBlacklistReportsResponseTypeDef = TypedDict(
+    "GetBlacklistReportsResponseTypeDef",
     {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
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
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1027,73 +1039,145 @@
     total=False,
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
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
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
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsOutputTypeDef,
+        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsOutputTypeDef,
+        "SendingOptions": SendingOptionsOutputTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    {
+        "PoolName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
@@ -1105,91 +1189,89 @@
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
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
 
 MessageTypeDef = TypedDict(
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
 
-
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
@@ -1199,44 +1281,50 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
-
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
-
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
@@ -1247,22 +1335,14 @@
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
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1271,22 +1351,20 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1298,12 +1376,11 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email/type_defs.pyi` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,116 +31,129 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BlacklistEntryTypeDef",
     "ContentTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "ReputationOptionsTypeDef",
     "SendingOptionsTypeDef",
     "TagTypeDef",
     "TrackingOptionsTypeDef",
-    "CreateDeliverabilityTestReportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DkimAttributesTypeDef",
     "DomainIspPlacementTypeDef",
     "VolumeStatisticsTypeDef",
     "DedicatedIpTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
+    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
     "RawMessageTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "PinpointDestinationOutputTypeDef",
+    "SnsDestinationOutputTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
+    "ReputationOptionsOutputTypeDef",
+    "SendingOptionsOutputTypeDef",
+    "TagOutputTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     "GetDomainStatisticsReportRequestRequestTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
-    "ListDedicatedIpPoolsResponseTypeDef",
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MessageTagTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutAccountSendingAttributesRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     "PutConfigurationSetReputationOptionsRequestRequestTypeDef",
     "PutConfigurationSetSendingOptionsRequestRequestTypeDef",
     "PutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendEmailResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "GetBlacklistReportsResponseTypeDef",
     "BodyTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "GetConfigurationSetResponseTypeDef",
+    "CreateDeliverabilityTestReportResponseTypeDef",
+    "GetBlacklistReportsResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListDedicatedIpPoolsResponseTypeDef",
+    "SendEmailResponseTypeDef",
     "CreateEmailIdentityResponseTypeDef",
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
+    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
     "GetAccountResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetConfigurationSetResponseTypeDef",
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
-    "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "EventDestinationDefinitionTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
     "EmailContentTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
@@ -161,17 +174,28 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
+
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+
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
@@ -214,20 +238,22 @@
 TrackingOptionsTypeDef = TypedDict(
     "TrackingOptionsTypeDef",
     {
         "CustomRedirectDomain": str,
     },
 )
 
-CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "CreateDeliverabilityTestReportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ReportId": str,
-        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DkimAttributesTypeDef = TypedDict(
     "DkimAttributesTypeDef",
     {
         "SigningEnabled": bool,
@@ -272,17 +298,19 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
+
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
+
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -317,14 +345,23 @@
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
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "ToAddresses": Sequence[str],
         "CcAddresses": Sequence[str],
         "BccAddresses": Sequence[str],
     },
@@ -348,19 +385,28 @@
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
@@ -396,14 +442,37 @@
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
 SendQuotaTypeDef = TypedDict(
     "SendQuotaTypeDef",
     {
         "Max24HourSend": float,
         "MaxSendRate": float,
         "SentLast24Hours": float,
     },
@@ -427,26 +496,59 @@
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
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
-GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
-    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PoolName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetDedicatedIpsRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpsRequestRequestTypeDef",
     {
@@ -514,74 +616,32 @@
         "IdentityType": IdentityTypeType,
         "IdentityName": str,
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
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
-ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
-    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDedicatedIpPoolsRequestRequestTypeDef = TypedDict(
     "ListDedicatedIpPoolsRequestRequestTypeDef",
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
-ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
-    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeliverabilityTestReportsRequestRequestTypeDef = TypedDict(
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
@@ -600,27 +660,21 @@
     {
         "NextToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
+
 class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
     _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
     _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
 ):
     pass
 
-ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
-    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListEmailIdentitiesRequestRequestTypeDef = TypedDict(
     "ListEmailIdentitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "PageSize": int,
     },
@@ -638,24 +692,14 @@
     "MessageTagTypeDef",
     {
         "Name": str,
         "Value": str,
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
 PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef = TypedDict(
     "PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef",
     {
         "AutoWarmupEnabled": bool,
     },
     total=False,
 )
@@ -679,80 +723,88 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -775,40 +827,44 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -816,64 +872,46 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
+
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
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
-
-SendEmailResponseTypeDef = TypedDict(
-    "SendEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-GetBlacklistReportsResponseTypeDef = TypedDict(
-    "GetBlacklistReportsResponseTypeDef",
-    {
-        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BodyTypeDef = TypedDict(
     "BodyTypeDef",
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+    },
+)
+
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
@@ -887,47 +925,43 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
@@ -947,40 +981,72 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
+
+CreateDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "CreateDeliverabilityTestReportResponseTypeDef",
     {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ReportId": str,
+        "DeliverabilityTestStatus": DeliverabilityTestStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBlacklistReportsResponseTypeDef = TypedDict(
+    "GetBlacklistReportsResponseTypeDef",
+    {
+        "BlacklistReport": Dict[str, List[BlacklistEntryTypeDef]],
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
+SendEmailResponseTypeDef = TypedDict(
+    "SendEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 DailyVolumeTypeDef = TypedDict(
     "DailyVolumeTypeDef",
     {
         "StartDate": datetime,
@@ -1000,75 +1066,147 @@
     total=False,
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
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
+    "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
+    {
+        "PoolName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = TypedDict(
+    "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = TypedDict(
+    "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = TypedDict(
+    "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 IspPlacementTypeDef = TypedDict(
     "IspPlacementTypeDef",
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
@@ -1078,89 +1216,91 @@
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
         "MailFromAttributes": MailFromAttributesTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
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
 
 MessageTypeDef = TypedDict(
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
+
+class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
+    pass
+
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
@@ -1170,42 +1310,52 @@
     "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
     {
         "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
     },
     total=False,
 )
 
+
 class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
     _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
     _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
 ):
     pass
 
+
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
@@ -1216,22 +1366,14 @@
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
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1240,20 +1382,22 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1265,11 +1409,12 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/PKG-INFO` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-pinpoint-email
-Version: 1.28.0
-Summary: Type annotations for boto3.PinpointEmail 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-pinpoint-email"></a>
 
 # mypy-boto3-pinpoint-email
 
 [![PyPI - mypy-boto3-pinpoint-email](https://img.shields.io/pypi/v/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-pinpoint-email.svg?color=blue)](https://pypi.org/project/mypy-boto3-pinpoint-email)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-pinpoint-email?color=blue)](https://pypistats.org/packages/mypy-boto3-pinpoint-email)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-pinpoint-email)](https://pepy.tech/project/mypy-boto3-pinpoint-email)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PinpointEmail 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
+[boto3.PinpointEmail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
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
 [mypy-boto3-pinpoint-email docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_pinpoint_email/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,113 +354,125 @@
 `mypy_boto3_pinpoint_email.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_pinpoint_email.type_defs import (
     BlacklistEntryTypeDef,
     ContentTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
     DeliveryOptionsTypeDef,
     ReputationOptionsTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TrackingOptionsTypeDef,
-    CreateDeliverabilityTestReportResponseTypeDef,
+    ResponseMetadataTypeDef,
     DkimAttributesTypeDef,
     DomainIspPlacementTypeDef,
     VolumeStatisticsTypeDef,
     DedicatedIpTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     DeleteDedicatedIpPoolRequestRequestTypeDef,
     DeleteEmailIdentityRequestRequestTypeDef,
     DeliverabilityTestReportTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DestinationTypeDef,
     DomainDeliverabilityCampaignTypeDef,
+    InboxPlacementTrackingOptionOutputTypeDef,
     InboxPlacementTrackingOptionTypeDef,
     RawMessageTypeDef,
     TemplateTypeDef,
     KinesisFirehoseDestinationTypeDef,
     PinpointDestinationTypeDef,
     SnsDestinationTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    PinpointDestinationOutputTypeDef,
+    SnsDestinationOutputTypeDef,
     SendQuotaTypeDef,
     GetBlacklistReportsRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
     GetConfigurationSetRequestRequestTypeDef,
+    ReputationOptionsOutputTypeDef,
+    SendingOptionsOutputTypeDef,
+    TagOutputTypeDef,
+    TrackingOptionsOutputTypeDef,
     GetDedicatedIpRequestRequestTypeDef,
-    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetDedicatedIpsRequestRequestTypeDef,
     GetDeliverabilityTestReportRequestRequestTypeDef,
     PlacementStatisticsTypeDef,
     GetDomainDeliverabilityCampaignRequestRequestTypeDef,
     GetDomainStatisticsReportRequestRequestTypeDef,
     GetEmailIdentityRequestRequestTypeDef,
     MailFromAttributesTypeDef,
     IdentityInfoTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
     ListDedicatedIpPoolsRequestRequestTypeDef,
-    ListDedicatedIpPoolsResponseTypeDef,
-    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
     ListDeliverabilityTestReportsRequestRequestTypeDef,
     ListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     ListEmailIdentitiesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MessageTagTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutAccountSendingAttributesRequestRequestTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     PutConfigurationSetReputationOptionsRequestRequestTypeDef,
     PutConfigurationSetSendingOptionsRequestRequestTypeDef,
     PutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     PutDedicatedIpInPoolRequestRequestTypeDef,
     PutDedicatedIpWarmupAttributesRequestRequestTypeDef,
     PutEmailIdentityDkimAttributesRequestRequestTypeDef,
     PutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     PutEmailIdentityMailFromAttributesRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendEmailResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    GetBlacklistReportsResponseTypeDef,
     BodyTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateDedicatedIpPoolRequestRequestTypeDef,
     CreateEmailIdentityRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    GetConfigurationSetResponseTypeDef,
+    CreateDeliverabilityTestReportResponseTypeDef,
+    GetBlacklistReportsResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListDedicatedIpPoolsResponseTypeDef,
+    SendEmailResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DailyVolumeTypeDef,
     OverallVolumeTypeDef,
     GetDedicatedIpResponseTypeDef,
     GetDedicatedIpsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     GetDomainDeliverabilityCampaignResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
+    DomainDeliverabilityTrackingOptionOutputTypeDef,
     DomainDeliverabilityTrackingOptionTypeDef,
     GetAccountResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetConfigurationSetResponseTypeDef,
+    GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef,
+    ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef,
+    ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef,
     IspPlacementTypeDef,
     GetEmailIdentityResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     MessageTypeDef,
-    EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    EventDestinationDefinitionTypeDef,
     GetDomainStatisticsReportResponseTypeDef,
     GetDeliverabilityDashboardOptionsResponseTypeDef,
     PutDeliverabilityDashboardOptionRequestRequestTypeDef,
     GetDeliverabilityTestReportResponseTypeDef,
     EmailContentTypeDef,
+    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
     CreateDeliverabilityTestReportRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
 )
 
 
 def get_structure() -> BlacklistEntryTypeDef:
     return {...}
```

### Comparing `mypy-boto3-pinpoint-email-1.28.0/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt` & `mypy-boto3-pinpoint-email-1.28.12/mypy_boto3_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-pinpoint-email-1.28.0/setup.py` & `mypy-boto3-pinpoint-email-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-pinpoint-email",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PinpointEmail 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.PinpointEmail 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

