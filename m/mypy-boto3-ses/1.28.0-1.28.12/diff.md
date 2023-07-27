# Comparing `tmp/mypy-boto3-ses-1.28.0.tar.gz` & `tmp/mypy-boto3-ses-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ses-1.28.0.tar", last modified: Thu Jul  6 21:00:38 2023, max compression
+gzip compressed data, was "mypy-boto3-ses-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-ses-1.28.0.tar` & `mypy-boto3-ses-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.578433 mypy-boto3-ses-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-07-06 21:00:38.574433 mypy-boto3-ses-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.570433 mypy-boto3-ses-1.28.0/mypy_boto3_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-06 20:55:48.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-06 20:55:48.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47976 2023-07-06 20:55:49.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47913 2023-07-06 20:55:48.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:38.574433 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:38.000000 mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:38.578433 mypy-boto3-ses-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:55:47.000000 mypy-boto3-ses-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.829293 mypy-boto3-ses-1.28.12/mypy_boto3_ses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49195 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49111 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54975 2023-07-27 11:46:53.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54894 2023-07-27 11:46:52.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-27 11:46:50.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:38.000000 mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.833293 mypy-boto3-ses-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:46:49.000000 mypy-boto3-ses-1.28.12/setup.py
```

### Comparing `mypy-boto3-ses-1.28.0/LICENSE` & `mypy-boto3-ses-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/PKG-INFO` & `mypy-boto3-ses-1.28.12/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.0
-Summary: Type annotations for boto3.SES 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,22 +375,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
+    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
+    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -400,140 +404,156 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
+    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
+    TemplateOutputTypeDef,
+    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
+    S3ActionOutputTypeDef,
+    SNSActionOutputTypeDef,
+    StopActionOutputTypeDef,
+    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
+    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
+    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
+    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
+    CreateReceiptFilterRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_structure() -> AddHeaderActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.0/README.md` & `mypy-boto3-ses-1.28.12/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,22 +343,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
+    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
+    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -368,140 +372,156 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
+    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
+    TemplateOutputTypeDef,
+    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
+    S3ActionOutputTypeDef,
+    SNSActionOutputTypeDef,
+    StopActionOutputTypeDef,
+    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
+    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
+    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
+    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
+    CreateReceiptFilterRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_structure() -> AddHeaderActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/__init__.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/__init__.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/__main__.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SES 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SES 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/client.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/client.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/literals.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,14 +217,15 @@
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
@@ -303,26 +304,28 @@
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

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/literals.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,15 @@
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
@@ -301,26 +302,28 @@
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

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/paginator.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,30 +63,30 @@
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
         """
 
 
 class ListCustomVerificationEmailTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 
@@ -96,43 +96,43 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
         """
 
 
 class ListReceiptRuleSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/paginator.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,29 +60,29 @@
 class ListConfigurationSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listconfigurationsetspaginator)
         """
 
 class ListCustomVerificationEmailTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listcustomverificationemailtemplatespaginator)
         """
 
 class ListIdentitiesPaginator(Paginator):
@@ -91,41 +91,41 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
     """
 
     def paginate(
         self,
         *,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listidentitiespaginator)
         """
 
 class ListReceiptRuleSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReceiptRuleSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listreceiptrulesetspaginator)
         """
 
 class ListTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/paginators/#listtemplatespaginator)
         """
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/type_defs.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ses service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
+    from mypy_boto3_ses.type_defs import AddHeaderActionOutputTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,24 +40,27 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AddHeaderActionOutputTypeDef",
     "AddHeaderActionTypeDef",
     "ContentTypeDef",
+    "BounceActionOutputTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
+    "ConfigurationSetOutputTypeDef",
     "ConfigurationSetTypeDef",
     "TrackingOptionsTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateReceiptRuleSetRequestRequestTypeDef",
     "TemplateTypeDef",
     "CustomVerificationEmailTemplateTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -67,138 +70,162 @@
     "DeleteIdentityPolicyRequestRequestTypeDef",
     "DeleteIdentityRequestRequestTypeDef",
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SNSDestinationOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "TemplateOutputTypeDef",
+    "LambdaActionOutputTypeDef",
     "LambdaActionTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
-    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
+    "S3ActionOutputTypeDef",
+    "SNSActionOutputTypeDef",
+    "StopActionOutputTypeDef",
+    "WorkmailActionOutputTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
+    "ReceiptIpFilterOutputTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
-    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "BodyTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
+    "GetSendQuotaResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    "ListIdentitiesResponseTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "SendBounceResponseTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
+    "TestRenderTemplateResponseTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
+    "GetTemplateResponseTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
+    "ReceiptActionOutputTypeDef",
     "ReceiptActionTypeDef",
+    "ReceiptFilterOutputTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
+    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
+    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
-    "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
+    "CreateReceiptFilterRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
+AddHeaderActionOutputTypeDef = TypedDict(
+    "AddHeaderActionOutputTypeDef",
+    {
+        "HeaderName": str,
+        "HeaderValue": str,
+    },
+)
+
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -213,18 +240,38 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+_RequiredBounceActionOutputTypeDef = TypedDict(
+    "_RequiredBounceActionOutputTypeDef",
+    {
+        "SmtpReplyCode": str,
+        "Message": str,
+        "Sender": str,
+    },
+)
+_OptionalBounceActionOutputTypeDef = TypedDict(
+    "_OptionalBounceActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "StatusCode": str,
+    },
+    total=False,
+)
+
+class BounceActionOutputTypeDef(
+    _RequiredBounceActionOutputTypeDef, _OptionalBounceActionOutputTypeDef
+):
+    pass
 
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
@@ -235,19 +282,17 @@
     {
         "TopicArn": str,
         "StatusCode": str,
     },
     total=False,
 )
 
-
 class BounceActionTypeDef(_RequiredBounceActionTypeDef, _OptionalBounceActionTypeDef):
     pass
 
-
 BulkEmailDestinationStatusTypeDef = TypedDict(
     "BulkEmailDestinationStatusTypeDef",
     {
         "Status": BulkEmailStatusType,
         "Error": str,
         "MessageId": str,
     },
@@ -276,23 +321,39 @@
     "CloneReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "OriginalRuleSetName": str,
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
 
+ConfigurationSetOutputTypeDef = TypedDict(
+    "ConfigurationSetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 ConfigurationSetTypeDef = TypedDict(
     "ConfigurationSetTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -335,19 +396,17 @@
         "SubjectPart": str,
         "TextPart": str,
         "HtmlPart": str,
     },
     total=False,
 )
 
-
 class TemplateTypeDef(_RequiredTemplateTypeDef, _OptionalTemplateTypeDef):
     pass
 
-
 CustomVerificationEmailTemplateTypeDef = TypedDict(
     "CustomVerificationEmailTemplateTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -432,14 +491,22 @@
 DeleteVerifiedEmailAddressRequestRequestTypeDef = TypedDict(
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+DeliveryOptionsOutputTypeDef = TypedDict(
+    "DeliveryOptionsOutputTypeDef",
+    {
+        "TlsPolicy": TlsPolicyType,
+    },
+    total=False,
+)
+
 DeliveryOptionsTypeDef = TypedDict(
     "DeliveryOptionsTypeDef",
     {
         "TlsPolicy": TlsPolicyType,
     },
     total=False,
 )
@@ -449,46 +516,63 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetAttributeNames": Sequence[ConfigurationSetAttributeType],
     },
     total=False,
 )
 
-
 class DescribeConfigurationSetRequestRequestTypeDef(
     _RequiredDescribeConfigurationSetRequestRequestTypeDef,
     _OptionalDescribeConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-
 ReputationOptionsTypeDef = TypedDict(
     "ReputationOptionsTypeDef",
     {
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
+TrackingOptionsOutputTypeDef = TypedDict(
+    "TrackingOptionsOutputTypeDef",
+    {
+        "CustomRedirectDomain": str,
+    },
+    total=False,
+)
+
 DescribeReceiptRuleRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -496,18 +580,26 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IAMRoleARN": str,
+        "DeliveryStreamARN": str,
+    },
+)
+
+SNSDestinationOutputTypeDef = TypedDict(
+    "SNSDestinationOutputTypeDef",
+    {
+        "TopicARN": str,
     },
 )
 
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
@@ -526,42 +618,21 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -576,21 +647,19 @@
     "_OptionalIdentityDkimAttributesTypeDef",
     {
         "DkimTokens": List[str],
     },
     total=False,
 )
 
-
 class IdentityDkimAttributesTypeDef(
     _RequiredIdentityDkimAttributesTypeDef, _OptionalIdentityDkimAttributesTypeDef
 ):
     pass
 
-
 GetIdentityMailFromDomainAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -625,37 +694,27 @@
         "HeadersInBounceNotificationsEnabled": bool,
         "HeadersInComplaintNotificationsEnabled": bool,
         "HeadersInDeliveryNotificationsEnabled": bool,
     },
     total=False,
 )
 
-
 class IdentityNotificationAttributesTypeDef(
     _RequiredIdentityNotificationAttributesTypeDef, _OptionalIdentityNotificationAttributesTypeDef
 ):
     pass
 
-
 GetIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -678,31 +737,19 @@
     "_OptionalIdentityVerificationAttributesTypeDef",
     {
         "VerificationToken": str,
     },
     total=False,
 )
 
-
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
-
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -714,14 +761,53 @@
 GetTemplateRequestRequestTypeDef = TypedDict(
     "GetTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
+_RequiredTemplateOutputTypeDef = TypedDict(
+    "_RequiredTemplateOutputTypeDef",
+    {
+        "TemplateName": str,
+    },
+)
+_OptionalTemplateOutputTypeDef = TypedDict(
+    "_OptionalTemplateOutputTypeDef",
+    {
+        "SubjectPart": str,
+        "TextPart": str,
+        "HtmlPart": str,
+    },
+    total=False,
+)
+
+class TemplateOutputTypeDef(_RequiredTemplateOutputTypeDef, _OptionalTemplateOutputTypeDef):
+    pass
+
+_RequiredLambdaActionOutputTypeDef = TypedDict(
+    "_RequiredLambdaActionOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+)
+_OptionalLambdaActionOutputTypeDef = TypedDict(
+    "_OptionalLambdaActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "InvocationType": InvocationTypeType,
+    },
+    total=False,
+)
+
+class LambdaActionOutputTypeDef(
+    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
+):
+    pass
+
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
@@ -729,120 +815,70 @@
     {
         "TopicArn": str,
         "InvocationType": InvocationTypeType,
     },
     total=False,
 )
 
-
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
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
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -853,47 +889,101 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
+PutIdentityPolicyRequestRequestTypeDef = TypedDict(
+    "PutIdentityPolicyRequestRequestTypeDef",
     {
-        "VerifiedEmailAddresses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Identity": str,
+        "PolicyName": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Data": Union[str, bytes, IO[Any], StreamingBody],
+    },
+)
+
+_RequiredS3ActionOutputTypeDef = TypedDict(
+    "_RequiredS3ActionOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalS3ActionOutputTypeDef = TypedDict(
+    "_OptionalS3ActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "ObjectKeyPrefix": str,
+        "KmsKeyArn": str,
     },
     total=False,
 )
 
-PutIdentityPolicyRequestRequestTypeDef = TypedDict(
-    "PutIdentityPolicyRequestRequestTypeDef",
+class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
+    pass
+
+_RequiredSNSActionOutputTypeDef = TypedDict(
+    "_RequiredSNSActionOutputTypeDef",
     {
-        "Identity": str,
-        "PolicyName": str,
-        "Policy": str,
+        "TopicArn": str,
+    },
+)
+_OptionalSNSActionOutputTypeDef = TypedDict(
+    "_OptionalSNSActionOutputTypeDef",
+    {
+        "Encoding": SNSActionEncodingType,
     },
+    total=False,
 )
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
+class SNSActionOutputTypeDef(_RequiredSNSActionOutputTypeDef, _OptionalSNSActionOutputTypeDef):
+    pass
+
+_RequiredStopActionOutputTypeDef = TypedDict(
+    "_RequiredStopActionOutputTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Scope": Literal["RuleSet"],
     },
 )
+_OptionalStopActionOutputTypeDef = TypedDict(
+    "_OptionalStopActionOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+    total=False,
+)
+
+class StopActionOutputTypeDef(_RequiredStopActionOutputTypeDef, _OptionalStopActionOutputTypeDef):
+    pass
+
+_RequiredWorkmailActionOutputTypeDef = TypedDict(
+    "_RequiredWorkmailActionOutputTypeDef",
+    {
+        "OrganizationArn": str,
+    },
+)
+_OptionalWorkmailActionOutputTypeDef = TypedDict(
+    "_OptionalWorkmailActionOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+    total=False,
+)
+
+class WorkmailActionOutputTypeDef(
+    _RequiredWorkmailActionOutputTypeDef, _OptionalWorkmailActionOutputTypeDef
+):
+    pass
 
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
@@ -903,75 +993,75 @@
         "TopicArn": str,
         "ObjectKeyPrefix": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3ActionTypeDef(_RequiredS3ActionTypeDef, _OptionalS3ActionTypeDef):
     pass
 
-
 _RequiredSNSActionTypeDef = TypedDict(
     "_RequiredSNSActionTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalSNSActionTypeDef = TypedDict(
     "_OptionalSNSActionTypeDef",
     {
         "Encoding": SNSActionEncodingType,
     },
     total=False,
 )
 
-
 class SNSActionTypeDef(_RequiredSNSActionTypeDef, _OptionalSNSActionTypeDef):
     pass
 
-
 _RequiredStopActionTypeDef = TypedDict(
     "_RequiredStopActionTypeDef",
     {
         "Scope": Literal["RuleSet"],
     },
 )
 _OptionalStopActionTypeDef = TypedDict(
     "_OptionalStopActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-
 class StopActionTypeDef(_RequiredStopActionTypeDef, _OptionalStopActionTypeDef):
     pass
 
-
 _RequiredWorkmailActionTypeDef = TypedDict(
     "_RequiredWorkmailActionTypeDef",
     {
         "OrganizationArn": str,
     },
 )
 _OptionalWorkmailActionTypeDef = TypedDict(
     "_OptionalWorkmailActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
+ReceiptIpFilterOutputTypeDef = TypedDict(
+    "ReceiptIpFilterOutputTypeDef",
+    {
+        "Policy": ReceiptFilterPolicyType,
+        "Cidr": str,
+    },
+)
 
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
@@ -981,33 +1071,14 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
     },
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
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1015,54 +1086,20 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-
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
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -1103,22 +1140,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMXFailure": BehaviorOnMXFailureType,
     },
     total=False,
 )
 
-
 class SetIdentityMailFromDomainRequestRequestTypeDef(
     _RequiredSetIdentityMailFromDomainRequestRequestTypeDef,
     _OptionalSetIdentityMailFromDomainRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSetIdentityNotificationTopicRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "Identity": str,
         "NotificationType": NotificationTypeType,
     },
 )
@@ -1126,22 +1161,20 @@
     "_OptionalSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "SnsTopic": str,
     },
     total=False,
 )
 
-
 class SetIdentityNotificationTopicRequestRequestTypeDef(
     _RequiredSetIdentityNotificationTopicRequestRequestTypeDef,
     _OptionalSetIdentityNotificationTopicRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSetReceiptRulePositionRequestRequestTypeDef = TypedDict(
     "_RequiredSetReceiptRulePositionRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -1149,38 +1182,28 @@
     "_OptionalSetReceiptRulePositionRequestRequestTypeDef",
     {
         "After": str,
     },
     total=False,
 )
 
-
 class SetReceiptRulePositionRequestRequestTypeDef(
     _RequiredSetReceiptRulePositionRequestRequestTypeDef,
     _OptionalSetReceiptRulePositionRequestRequestTypeDef,
 ):
     pass
 
-
 TestRenderTemplateRequestRequestTypeDef = TypedDict(
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1215,52 +1238,34 @@
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
     total=False,
 )
 
-
 class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
@@ -1276,22 +1281,14 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1299,21 +1296,19 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementTemplateData": str,
     },
     total=False,
 )
 
-
 class BulkEmailDestinationTypeDef(
     _RequiredBulkEmailDestinationTypeDef, _OptionalBulkEmailDestinationTypeDef
 ):
     pass
 
-
 _RequiredSendTemplatedEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendTemplatedEmailRequestRequestTypeDef",
     {
         "Source": str,
         "Destination": DestinationTypeDef,
         "Template": str,
         "TemplateData": str,
@@ -1329,21 +1324,26 @@
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "TemplateArn": str,
     },
     total=False,
 )
 
-
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+CloudWatchDestinationOutputTypeDef = TypedDict(
+    "CloudWatchDestinationOutputTypeDef",
+    {
+        "DimensionConfigurations": List[CloudWatchDimensionConfigurationOutputTypeDef],
+    },
+)
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
@@ -1351,23 +1351,14 @@
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1383,66 +1374,208 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "DeliveryOptions": DeliveryOptionsTypeDef,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
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
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    {
+        "VerifiedEmailAddresses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
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
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageDsnTypeDef = TypedDict(
     "_RequiredMessageDsnTypeDef",
     {
         "ReportingMta": str,
@@ -1453,19 +1586,17 @@
     {
         "ArrivalDate": Union[datetime, str],
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-
 class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
     pass
 
-
 _RequiredRecipientDsnFieldsTypeDef = TypedDict(
     "_RequiredRecipientDsnFieldsTypeDef",
     {
         "Action": DsnActionType,
         "Status": str,
     },
 )
@@ -1477,42 +1608,40 @@
         "DiagnosticCode": str,
         "LastAttemptDate": Union[datetime, str],
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-
 class RecipientDsnFieldsTypeDef(
     _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
-
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1522,44 +1651,91 @@
     "_OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef(
     _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     _OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
 ):
     pass
 
-
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
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
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendRawEmailRequestRequestTypeDef",
     {
         "RawMessage": RawMessageTypeDef,
@@ -1575,20 +1751,32 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
+ReceiptActionOutputTypeDef = TypedDict(
+    "ReceiptActionOutputTypeDef",
+    {
+        "S3Action": S3ActionOutputTypeDef,
+        "BounceAction": BounceActionOutputTypeDef,
+        "WorkmailAction": WorkmailActionOutputTypeDef,
+        "LambdaAction": LambdaActionOutputTypeDef,
+        "StopAction": StopActionOutputTypeDef,
+        "AddHeaderAction": AddHeaderActionOutputTypeDef,
+        "SNSAction": SNSActionOutputTypeDef,
+    },
+    total=False,
+)
 
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
@@ -1596,14 +1784,22 @@
         "StopAction": StopActionTypeDef,
         "AddHeaderAction": AddHeaderActionTypeDef,
         "SNSAction": SNSActionTypeDef,
     },
     total=False,
 )
 
+ReceiptFilterOutputTypeDef = TypedDict(
+    "ReceiptFilterOutputTypeDef",
+    {
+        "Name": str,
+        "IpFilter": ReceiptIpFilterOutputTypeDef,
+    },
+)
+
 ReceiptFilterTypeDef = TypedDict(
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
@@ -1635,21 +1831,42 @@
         "DefaultTags": Sequence[MessageTagTypeDef],
         "TemplateArn": str,
         "DefaultTemplateData": str,
     },
     total=False,
 )
 
-
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+_RequiredEventDestinationOutputTypeDef = TypedDict(
+    "_RequiredEventDestinationOutputTypeDef",
+    {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationOutputTypeDef = TypedDict(
+    "_OptionalEventDestinationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventDestinationOutputTypeDef(
+    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
+):
+    pass
 
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
@@ -1661,19 +1878,17 @@
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-
 _RequiredBouncedRecipientInfoTypeDef = TypedDict(
     "_RequiredBouncedRecipientInfoTypeDef",
     {
         "Recipient": str,
     },
 )
 _OptionalBouncedRecipientInfoTypeDef = TypedDict(
@@ -1682,20 +1897,41 @@
         "RecipientArn": str,
         "BounceType": BounceTypeType,
         "RecipientDsnFields": RecipientDsnFieldsTypeDef,
     },
     total=False,
 )
 
-
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
+_RequiredReceiptRuleOutputTypeDef = TypedDict(
+    "_RequiredReceiptRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalReceiptRuleOutputTypeDef = TypedDict(
+    "_OptionalReceiptRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+        "TlsPolicy": TlsPolicyType,
+        "Recipients": List[str],
+        "Actions": List[ReceiptActionOutputTypeDef],
+        "ScanEnabled": bool,
+    },
+    total=False,
+)
+
+class ReceiptRuleOutputTypeDef(
+    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
+):
+    pass
 
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
@@ -1707,31 +1943,29 @@
         "Recipients": Sequence[str],
         "Actions": Sequence[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
-
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
-
-CreateReceiptFilterRequestRequestTypeDef = TypedDict(
-    "CreateReceiptFilterRequestRequestTypeDef",
+ListReceiptFiltersResponseTypeDef = TypedDict(
+    "ListReceiptFiltersResponseTypeDef",
     {
-        "Filter": ReceiptFilterTypeDef,
+        "Filters": List[ReceiptFilterOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListReceiptFiltersResponseTypeDef = TypedDict(
-    "ListReceiptFiltersResponseTypeDef",
+CreateReceiptFilterRequestRequestTypeDef = TypedDict(
+    "CreateReceiptFilterRequestRequestTypeDef",
     {
-        "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Filter": ReceiptFilterTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1748,41 +1982,39 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
+DescribeConfigurationSetResponseTypeDef = TypedDict(
+    "DescribeConfigurationSetResponseTypeDef",
+    {
+        "ConfigurationSet": ConfigurationSetOutputTypeDef,
+        "EventDestinations": List[EventDestinationOutputTypeDef],
+        "TrackingOptions": TrackingOptionsOutputTypeDef,
+        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
 
-DescribeConfigurationSetResponseTypeDef = TypedDict(
-    "DescribeConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationTypeDef],
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1801,20 +2033,44 @@
         "Explanation": str,
         "MessageDsn": MessageDsnTypeDef,
         "BounceSenderArn": str,
     },
     total=False,
 )
 
-
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
+DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
+    "DescribeActiveReceiptRuleSetResponseTypeDef",
+    {
+        "Metadata": ReceiptRuleSetMetadataTypeDef,
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReceiptRuleResponseTypeDef = TypedDict(
+    "DescribeReceiptRuleResponseTypeDef",
+    {
+        "Rule": ReceiptRuleOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeReceiptRuleSetResponseTypeDef = TypedDict(
+    "DescribeReceiptRuleSetResponseTypeDef",
+    {
+        "Metadata": ReceiptRuleSetMetadataTypeDef,
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
@@ -1823,47 +2079,19 @@
     "_OptionalCreateReceiptRuleRequestRequestTypeDef",
     {
         "After": str,
     },
     total=False,
 )
 
-
 class CreateReceiptRuleRequestRequestTypeDef(
     _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
 ):
     pass
 
-
-DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
-    "DescribeActiveReceiptRuleSetResponseTypeDef",
-    {
-        "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReceiptRuleResponseTypeDef = TypedDict(
-    "DescribeReceiptRuleResponseTypeDef",
-    {
-        "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeReceiptRuleSetResponseTypeDef = TypedDict(
-    "DescribeReceiptRuleSetResponseTypeDef",
-    {
-        "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/type_defs.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ses service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ses.type_defs import AddHeaderActionTypeDef
+    from mypy_boto3_ses.type_defs import AddHeaderActionOutputTypeDef
 
-    data: AddHeaderActionTypeDef = {...}
+    data: AddHeaderActionOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -40,23 +40,28 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AddHeaderActionOutputTypeDef",
     "AddHeaderActionTypeDef",
     "ContentTypeDef",
+    "BounceActionOutputTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
     "MessageTagTypeDef",
     "CloneReceiptRuleSetRequestRequestTypeDef",
+    "CloudWatchDimensionConfigurationOutputTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
+    "ConfigurationSetOutputTypeDef",
     "ConfigurationSetTypeDef",
     "TrackingOptionsTypeDef",
     "CreateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "CreateReceiptRuleSetRequestRequestTypeDef",
     "TemplateTypeDef",
     "CustomVerificationEmailTemplateTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
@@ -66,138 +71,162 @@
     "DeleteIdentityPolicyRequestRequestTypeDef",
     "DeleteIdentityRequestRequestTypeDef",
     "DeleteReceiptFilterRequestRequestTypeDef",
     "DeleteReceiptRuleRequestRequestTypeDef",
     "DeleteReceiptRuleSetRequestRequestTypeDef",
     "DeleteTemplateRequestRequestTypeDef",
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
+    "DeliveryOptionsOutputTypeDef",
     "DeliveryOptionsTypeDef",
     "ReceiptRuleSetMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeConfigurationSetRequestRequestTypeDef",
     "ReputationOptionsTypeDef",
+    "TrackingOptionsOutputTypeDef",
     "DescribeReceiptRuleRequestRequestTypeDef",
     "DescribeReceiptRuleSetRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "KinesisFirehoseDestinationOutputTypeDef",
+    "SNSDestinationOutputTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SNSDestinationTypeDef",
     "ExtensionFieldTypeDef",
-    "GetAccountSendingEnabledResponseTypeDef",
     "GetCustomVerificationEmailTemplateRequestRequestTypeDef",
-    "GetCustomVerificationEmailTemplateResponseTypeDef",
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     "IdentityDkimAttributesTypeDef",
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     "IdentityMailFromDomainAttributesTypeDef",
     "GetIdentityNotificationAttributesRequestRequestTypeDef",
     "IdentityNotificationAttributesTypeDef",
     "GetIdentityPoliciesRequestRequestTypeDef",
-    "GetIdentityPoliciesResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetIdentityVerificationAttributesRequestRequestTypeDef",
     "IdentityVerificationAttributesTypeDef",
-    "GetSendQuotaResponseTypeDef",
     "SendDataPointTypeDef",
     "GetTemplateRequestRequestTypeDef",
+    "TemplateOutputTypeDef",
+    "LambdaActionOutputTypeDef",
     "LambdaActionTypeDef",
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
     "ListIdentitiesRequestRequestTypeDef",
-    "ListIdentitiesResponseTypeDef",
     "ListIdentityPoliciesRequestRequestTypeDef",
-    "ListIdentityPoliciesResponseTypeDef",
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
     "ListReceiptRuleSetsRequestRequestTypeDef",
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateMetadataTypeDef",
-    "ListVerifiedEmailAddressesResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutIdentityPolicyRequestRequestTypeDef",
     "RawMessageTypeDef",
+    "S3ActionOutputTypeDef",
+    "SNSActionOutputTypeDef",
+    "StopActionOutputTypeDef",
+    "WorkmailActionOutputTypeDef",
     "S3ActionTypeDef",
     "SNSActionTypeDef",
     "StopActionTypeDef",
     "WorkmailActionTypeDef",
+    "ReceiptIpFilterOutputTypeDef",
     "ReceiptIpFilterTypeDef",
     "ReorderReceiptRuleSetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendBounceResponseTypeDef",
     "SendCustomVerificationEmailRequestRequestTypeDef",
-    "SendCustomVerificationEmailResponseTypeDef",
-    "SendEmailResponseTypeDef",
-    "SendRawEmailResponseTypeDef",
-    "SendTemplatedEmailResponseTypeDef",
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     "SetIdentityDkimEnabledRequestRequestTypeDef",
     "SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef",
     "SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef",
     "SetIdentityMailFromDomainRequestRequestTypeDef",
     "SetIdentityNotificationTopicRequestRequestTypeDef",
     "SetReceiptRulePositionRequestRequestTypeDef",
     "TestRenderTemplateRequestRequestTypeDef",
-    "TestRenderTemplateResponseTypeDef",
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef",
     "UpdateConfigurationSetSendingEnabledRequestRequestTypeDef",
     "UpdateCustomVerificationEmailTemplateRequestRequestTypeDef",
     "VerifyDomainDkimRequestRequestTypeDef",
-    "VerifyDomainDkimResponseTypeDef",
     "VerifyDomainIdentityRequestRequestTypeDef",
-    "VerifyDomainIdentityResponseTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "BodyTypeDef",
-    "SendBulkTemplatedEmailResponseTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
+    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSendingEnabledResponseTypeDef",
+    "GetCustomVerificationEmailTemplateResponseTypeDef",
+    "GetIdentityPoliciesResponseTypeDef",
+    "GetSendQuotaResponseTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    "ListIdentitiesResponseTypeDef",
+    "ListIdentityPoliciesResponseTypeDef",
     "ListReceiptRuleSetsResponseTypeDef",
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    "SendBounceResponseTypeDef",
+    "SendBulkTemplatedEmailResponseTypeDef",
+    "SendCustomVerificationEmailResponseTypeDef",
+    "SendEmailResponseTypeDef",
+    "SendRawEmailResponseTypeDef",
+    "SendTemplatedEmailResponseTypeDef",
+    "TestRenderTemplateResponseTypeDef",
+    "VerifyDomainDkimResponseTypeDef",
+    "VerifyDomainIdentityResponseTypeDef",
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "GetIdentityDkimAttributesResponseTypeDef",
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     "GetIdentityNotificationAttributesResponseTypeDef",
     "GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     "GetIdentityVerificationAttributesResponseTypeDef",
     "GetSendStatisticsResponseTypeDef",
+    "GetTemplateResponseTypeDef",
+    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
     "ListTemplatesResponseTypeDef",
     "SendRawEmailRequestRequestTypeDef",
+    "ReceiptActionOutputTypeDef",
     "ReceiptActionTypeDef",
+    "ReceiptFilterOutputTypeDef",
     "ReceiptFilterTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
+    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
+    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
-    "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
+    "CreateReceiptFilterRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "DescribeConfigurationSetResponseTypeDef",
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
+AddHeaderActionOutputTypeDef = TypedDict(
+    "AddHeaderActionOutputTypeDef",
+    {
+        "HeaderName": str,
+        "HeaderValue": str,
+    },
+)
+
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
         "HeaderValue": str,
     },
 )
@@ -212,17 +241,43 @@
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
+_RequiredBounceActionOutputTypeDef = TypedDict(
+    "_RequiredBounceActionOutputTypeDef",
+    {
+        "SmtpReplyCode": str,
+        "Message": str,
+        "Sender": str,
+    },
+)
+_OptionalBounceActionOutputTypeDef = TypedDict(
+    "_OptionalBounceActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "StatusCode": str,
+    },
+    total=False,
+)
+
+
+class BounceActionOutputTypeDef(
+    _RequiredBounceActionOutputTypeDef, _OptionalBounceActionOutputTypeDef
+):
+    pass
+
+
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
     },
@@ -232,17 +287,19 @@
     {
         "TopicArn": str,
         "StatusCode": str,
     },
     total=False,
 )
 
+
 class BounceActionTypeDef(_RequiredBounceActionTypeDef, _OptionalBounceActionTypeDef):
     pass
 
+
 BulkEmailDestinationStatusTypeDef = TypedDict(
     "BulkEmailDestinationStatusTypeDef",
     {
         "Status": BulkEmailStatusType,
         "Error": str,
         "MessageId": str,
     },
@@ -271,23 +328,39 @@
     "CloneReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "OriginalRuleSetName": str,
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
 
+ConfigurationSetOutputTypeDef = TypedDict(
+    "ConfigurationSetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+
 ConfigurationSetTypeDef = TypedDict(
     "ConfigurationSetTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -330,17 +403,19 @@
         "SubjectPart": str,
         "TextPart": str,
         "HtmlPart": str,
     },
     total=False,
 )
 
+
 class TemplateTypeDef(_RequiredTemplateTypeDef, _OptionalTemplateTypeDef):
     pass
 
+
 CustomVerificationEmailTemplateTypeDef = TypedDict(
     "CustomVerificationEmailTemplateTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -425,14 +500,22 @@
 DeleteVerifiedEmailAddressRequestRequestTypeDef = TypedDict(
     "DeleteVerifiedEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
+DeliveryOptionsOutputTypeDef = TypedDict(
+    "DeliveryOptionsOutputTypeDef",
+    {
+        "TlsPolicy": TlsPolicyType,
+    },
+    total=False,
+)
+
 DeliveryOptionsTypeDef = TypedDict(
     "DeliveryOptionsTypeDef",
     {
         "TlsPolicy": TlsPolicyType,
     },
     total=False,
 )
@@ -442,44 +525,65 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
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
 _RequiredDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalDescribeConfigurationSetRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetAttributeNames": Sequence[ConfigurationSetAttributeType],
     },
     total=False,
 )
 
+
 class DescribeConfigurationSetRequestRequestTypeDef(
     _RequiredDescribeConfigurationSetRequestRequestTypeDef,
     _OptionalDescribeConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+
 ReputationOptionsTypeDef = TypedDict(
     "ReputationOptionsTypeDef",
     {
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
     total=False,
 )
 
+TrackingOptionsOutputTypeDef = TypedDict(
+    "TrackingOptionsOutputTypeDef",
+    {
+        "CustomRedirectDomain": str,
+    },
+    total=False,
+)
+
 DescribeReceiptRuleRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -487,18 +591,26 @@
 DescribeReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "DescribeReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+KinesisFirehoseDestinationOutputTypeDef = TypedDict(
+    "KinesisFirehoseDestinationOutputTypeDef",
+    {
+        "IAMRoleARN": str,
+        "DeliveryStreamARN": str,
+    },
+)
+
+SNSDestinationOutputTypeDef = TypedDict(
+    "SNSDestinationOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TopicARN": str,
     },
 )
 
 KinesisFirehoseDestinationTypeDef = TypedDict(
     "KinesisFirehoseDestinationTypeDef",
     {
         "IAMRoleARN": str,
@@ -517,42 +629,21 @@
     "ExtensionFieldTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-GetAccountSendingEnabledResponseTypeDef = TypedDict(
-    "GetAccountSendingEnabledResponseTypeDef",
-    {
-        "Enabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 GetIdentityDkimAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityDkimAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -567,19 +658,21 @@
     "_OptionalIdentityDkimAttributesTypeDef",
     {
         "DkimTokens": List[str],
     },
     total=False,
 )
 
+
 class IdentityDkimAttributesTypeDef(
     _RequiredIdentityDkimAttributesTypeDef, _OptionalIdentityDkimAttributesTypeDef
 ):
     pass
 
+
 GetIdentityMailFromDomainAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -614,35 +707,29 @@
         "HeadersInBounceNotificationsEnabled": bool,
         "HeadersInComplaintNotificationsEnabled": bool,
         "HeadersInDeliveryNotificationsEnabled": bool,
     },
     total=False,
 )
 
+
 class IdentityNotificationAttributesTypeDef(
     _RequiredIdentityNotificationAttributesTypeDef, _OptionalIdentityNotificationAttributesTypeDef
 ):
     pass
 
+
 GetIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
 
-GetIdentityPoliciesResponseTypeDef = TypedDict(
-    "GetIdentityPoliciesResponseTypeDef",
-    {
-        "Policies": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -665,28 +752,20 @@
     "_OptionalIdentityVerificationAttributesTypeDef",
     {
         "VerificationToken": str,
     },
     total=False,
 )
 
+
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
-GetSendQuotaResponseTypeDef = TypedDict(
-    "GetSendQuotaResponseTypeDef",
-    {
-        "Max24HourSend": float,
-        "MaxSendRate": float,
-        "SentLast24Hours": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
@@ -699,14 +778,57 @@
 GetTemplateRequestRequestTypeDef = TypedDict(
     "GetTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
     },
 )
 
+_RequiredTemplateOutputTypeDef = TypedDict(
+    "_RequiredTemplateOutputTypeDef",
+    {
+        "TemplateName": str,
+    },
+)
+_OptionalTemplateOutputTypeDef = TypedDict(
+    "_OptionalTemplateOutputTypeDef",
+    {
+        "SubjectPart": str,
+        "TextPart": str,
+        "HtmlPart": str,
+    },
+    total=False,
+)
+
+
+class TemplateOutputTypeDef(_RequiredTemplateOutputTypeDef, _OptionalTemplateOutputTypeDef):
+    pass
+
+
+_RequiredLambdaActionOutputTypeDef = TypedDict(
+    "_RequiredLambdaActionOutputTypeDef",
+    {
+        "FunctionArn": str,
+    },
+)
+_OptionalLambdaActionOutputTypeDef = TypedDict(
+    "_OptionalLambdaActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "InvocationType": InvocationTypeType,
+    },
+    total=False,
+)
+
+
+class LambdaActionOutputTypeDef(
+    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
+):
+    pass
+
+
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "FunctionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
@@ -714,118 +836,72 @@
     {
         "TopicArn": str,
         "InvocationType": InvocationTypeType,
     },
     total=False,
 )
 
+
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = TypedDict(
-    "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
+
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
 
 ListConfigurationSetsRequestRequestTypeDef = TypedDict(
     "ListConfigurationSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomVerificationEmailTemplatesRequestRequestTypeDef = TypedDict(
     "ListCustomVerificationEmailTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
-    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
-    {
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIdentitiesRequestRequestTypeDef = TypedDict(
     "ListIdentitiesRequestRequestTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListIdentitiesResponseTypeDef = TypedDict(
-    "ListIdentitiesResponseTypeDef",
-    {
-        "Identities": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "ListIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
     },
 )
 
-ListIdentityPoliciesResponseTypeDef = TypedDict(
-    "ListIdentityPoliciesResponseTypeDef",
-    {
-        "PolicyNames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
-    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReceiptRuleSetsRequestRequestTypeDef = TypedDict(
     "ListReceiptRuleSetsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
-    "ListTemplatesRequestListTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTemplatesRequestRequestTypeDef = TypedDict(
     "ListTemplatesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxItems": int,
     },
     total=False,
@@ -836,48 +912,110 @@
     {
         "Name": str,
         "CreatedTimestamp": datetime,
     },
     total=False,
 )
 
-ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
-    "ListVerifiedEmailAddressesResponseTypeDef",
+PutIdentityPolicyRequestRequestTypeDef = TypedDict(
+    "PutIdentityPolicyRequestRequestTypeDef",
     {
-        "VerifiedEmailAddresses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Identity": str,
+        "PolicyName": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RawMessageTypeDef = TypedDict(
+    "RawMessageTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Data": Union[str, bytes, IO[Any], StreamingBody],
+    },
+)
+
+_RequiredS3ActionOutputTypeDef = TypedDict(
+    "_RequiredS3ActionOutputTypeDef",
+    {
+        "BucketName": str,
+    },
+)
+_OptionalS3ActionOutputTypeDef = TypedDict(
+    "_OptionalS3ActionOutputTypeDef",
+    {
+        "TopicArn": str,
+        "ObjectKeyPrefix": str,
+        "KmsKeyArn": str,
     },
     total=False,
 )
 
-PutIdentityPolicyRequestRequestTypeDef = TypedDict(
-    "PutIdentityPolicyRequestRequestTypeDef",
+
+class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
+    pass
+
+
+_RequiredSNSActionOutputTypeDef = TypedDict(
+    "_RequiredSNSActionOutputTypeDef",
     {
-        "Identity": str,
-        "PolicyName": str,
-        "Policy": str,
+        "TopicArn": str,
     },
 )
+_OptionalSNSActionOutputTypeDef = TypedDict(
+    "_OptionalSNSActionOutputTypeDef",
+    {
+        "Encoding": SNSActionEncodingType,
+    },
+    total=False,
+)
 
-RawMessageTypeDef = TypedDict(
-    "RawMessageTypeDef",
+
+class SNSActionOutputTypeDef(_RequiredSNSActionOutputTypeDef, _OptionalSNSActionOutputTypeDef):
+    pass
+
+
+_RequiredStopActionOutputTypeDef = TypedDict(
+    "_RequiredStopActionOutputTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Scope": Literal["RuleSet"],
+    },
+)
+_OptionalStopActionOutputTypeDef = TypedDict(
+    "_OptionalStopActionOutputTypeDef",
+    {
+        "TopicArn": str,
     },
+    total=False,
 )
 
+
+class StopActionOutputTypeDef(_RequiredStopActionOutputTypeDef, _OptionalStopActionOutputTypeDef):
+    pass
+
+
+_RequiredWorkmailActionOutputTypeDef = TypedDict(
+    "_RequiredWorkmailActionOutputTypeDef",
+    {
+        "OrganizationArn": str,
+    },
+)
+_OptionalWorkmailActionOutputTypeDef = TypedDict(
+    "_OptionalWorkmailActionOutputTypeDef",
+    {
+        "TopicArn": str,
+    },
+    total=False,
+)
+
+
+class WorkmailActionOutputTypeDef(
+    _RequiredWorkmailActionOutputTypeDef, _OptionalWorkmailActionOutputTypeDef
+):
+    pass
+
+
 _RequiredS3ActionTypeDef = TypedDict(
     "_RequiredS3ActionTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ActionTypeDef = TypedDict(
@@ -886,68 +1024,84 @@
         "TopicArn": str,
         "ObjectKeyPrefix": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3ActionTypeDef(_RequiredS3ActionTypeDef, _OptionalS3ActionTypeDef):
     pass
 
+
 _RequiredSNSActionTypeDef = TypedDict(
     "_RequiredSNSActionTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalSNSActionTypeDef = TypedDict(
     "_OptionalSNSActionTypeDef",
     {
         "Encoding": SNSActionEncodingType,
     },
     total=False,
 )
 
+
 class SNSActionTypeDef(_RequiredSNSActionTypeDef, _OptionalSNSActionTypeDef):
     pass
 
+
 _RequiredStopActionTypeDef = TypedDict(
     "_RequiredStopActionTypeDef",
     {
         "Scope": Literal["RuleSet"],
     },
 )
 _OptionalStopActionTypeDef = TypedDict(
     "_OptionalStopActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
+
 class StopActionTypeDef(_RequiredStopActionTypeDef, _OptionalStopActionTypeDef):
     pass
 
+
 _RequiredWorkmailActionTypeDef = TypedDict(
     "_RequiredWorkmailActionTypeDef",
     {
         "OrganizationArn": str,
     },
 )
 _OptionalWorkmailActionTypeDef = TypedDict(
     "_OptionalWorkmailActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
+
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
+
+ReceiptIpFilterOutputTypeDef = TypedDict(
+    "ReceiptIpFilterOutputTypeDef",
+    {
+        "Policy": ReceiptFilterPolicyType,
+        "Cidr": str,
+    },
+)
+
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
 )
@@ -956,33 +1110,14 @@
     "ReorderReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleNames": Sequence[str],
     },
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
-SendBounceResponseTypeDef = TypedDict(
-    "SendBounceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -990,51 +1125,21 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
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
-SendRawEmailResponseTypeDef = TypedDict(
-    "SendRawEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendTemplatedEmailResponseTypeDef = TypedDict(
-    "SendTemplatedEmailResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
@@ -1076,20 +1181,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMXFailure": BehaviorOnMXFailureType,
     },
     total=False,
 )
 
+
 class SetIdentityMailFromDomainRequestRequestTypeDef(
     _RequiredSetIdentityMailFromDomainRequestRequestTypeDef,
     _OptionalSetIdentityMailFromDomainRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSetIdentityNotificationTopicRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "Identity": str,
         "NotificationType": NotificationTypeType,
     },
 )
@@ -1097,20 +1204,22 @@
     "_OptionalSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "SnsTopic": str,
     },
     total=False,
 )
 
+
 class SetIdentityNotificationTopicRequestRequestTypeDef(
     _RequiredSetIdentityNotificationTopicRequestRequestTypeDef,
     _OptionalSetIdentityNotificationTopicRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSetReceiptRulePositionRequestRequestTypeDef = TypedDict(
     "_RequiredSetReceiptRulePositionRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -1118,36 +1227,30 @@
     "_OptionalSetReceiptRulePositionRequestRequestTypeDef",
     {
         "After": str,
     },
     total=False,
 )
 
+
 class SetReceiptRulePositionRequestRequestTypeDef(
     _RequiredSetReceiptRulePositionRequestRequestTypeDef,
     _OptionalSetReceiptRulePositionRequestRequestTypeDef,
 ):
     pass
 
+
 TestRenderTemplateRequestRequestTypeDef = TypedDict(
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
 
-TestRenderTemplateResponseTypeDef = TypedDict(
-    "TestRenderTemplateResponseTypeDef",
-    {
-        "RenderedTemplate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSendingEnabledRequestRequestTypeDef = TypedDict(
     "UpdateAccountSendingEnabledRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -1182,50 +1285,36 @@
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
     total=False,
 )
 
+
 class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainDkimResponseTypeDef = TypedDict(
-    "VerifyDomainDkimResponseTypeDef",
-    {
-        "DkimTokens": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyDomainIdentityRequestRequestTypeDef = TypedDict(
     "VerifyDomainIdentityRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
-VerifyDomainIdentityResponseTypeDef = TypedDict(
-    "VerifyDomainIdentityResponseTypeDef",
-    {
-        "VerificationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyEmailAddressRequestRequestTypeDef = TypedDict(
     "VerifyEmailAddressRequestRequestTypeDef",
     {
         "EmailAddress": str,
     },
 )
 
@@ -1241,22 +1330,14 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
-SendBulkTemplatedEmailResponseTypeDef = TypedDict(
-    "SendBulkTemplatedEmailResponseTypeDef",
-    {
-        "Status": List[BulkEmailDestinationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredBulkEmailDestinationTypeDef = TypedDict(
     "_RequiredBulkEmailDestinationTypeDef",
     {
         "Destination": DestinationTypeDef,
     },
 )
 _OptionalBulkEmailDestinationTypeDef = TypedDict(
@@ -1264,19 +1345,21 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementTemplateData": str,
     },
     total=False,
 )
 
+
 class BulkEmailDestinationTypeDef(
     _RequiredBulkEmailDestinationTypeDef, _OptionalBulkEmailDestinationTypeDef
 ):
     pass
 
+
 _RequiredSendTemplatedEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendTemplatedEmailRequestRequestTypeDef",
     {
         "Source": str,
         "Destination": DestinationTypeDef,
         "Template": str,
         "TemplateData": str,
@@ -1292,43 +1375,43 @@
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "TemplateArn": str,
     },
     total=False,
 )
 
+
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+
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
 
 CreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
     },
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
-    {
-        "ConfigurationSets": List[ConfigurationSetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "TrackingOptions": TrackingOptionsTypeDef,
     },
 )
@@ -1344,64 +1427,210 @@
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-GetTemplateResponseTypeDef = TypedDict(
-    "GetTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "Template": TemplateTypeDef,
     },
 )
 
-ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
-    "ListCustomVerificationEmailTemplatesResponseTypeDef",
-    {
-        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "DeliveryOptions": DeliveryOptionsTypeDef,
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
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountSendingEnabledResponseTypeDef = TypedDict(
+    "GetAccountSendingEnabledResponseTypeDef",
+    {
+        "Enabled": bool,
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
+GetIdentityPoliciesResponseTypeDef = TypedDict(
+    "GetIdentityPoliciesResponseTypeDef",
+    {
+        "Policies": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSendQuotaResponseTypeDef = TypedDict(
+    "GetSendQuotaResponseTypeDef",
+    {
+        "Max24HourSend": float,
+        "MaxSendRate": float,
+        "SentLast24Hours": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[ConfigurationSetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomVerificationEmailTemplatesResponseTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesResponseTypeDef",
+    {
+        "CustomVerificationEmailTemplates": List[CustomVerificationEmailTemplateTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentitiesResponseTypeDef = TypedDict(
+    "ListIdentitiesResponseTypeDef",
+    {
+        "Identities": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIdentityPoliciesResponseTypeDef = TypedDict(
+    "ListIdentityPoliciesResponseTypeDef",
+    {
+        "PolicyNames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListReceiptRuleSetsResponseTypeDef = TypedDict(
     "ListReceiptRuleSetsResponseTypeDef",
     {
         "RuleSets": List[ReceiptRuleSetMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVerifiedEmailAddressesResponseTypeDef = TypedDict(
+    "ListVerifiedEmailAddressesResponseTypeDef",
+    {
+        "VerifiedEmailAddresses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendBounceResponseTypeDef = TypedDict(
+    "SendBounceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendBulkTemplatedEmailResponseTypeDef = TypedDict(
+    "SendBulkTemplatedEmailResponseTypeDef",
+    {
+        "Status": List[BulkEmailDestinationStatusTypeDef],
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
+SendRawEmailResponseTypeDef = TypedDict(
+    "SendRawEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendTemplatedEmailResponseTypeDef = TypedDict(
+    "SendTemplatedEmailResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestRenderTemplateResponseTypeDef = TypedDict(
+    "TestRenderTemplateResponseTypeDef",
+    {
+        "RenderedTemplate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainDkimResponseTypeDef = TypedDict(
+    "VerifyDomainDkimResponseTypeDef",
+    {
+        "DkimTokens": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifyDomainIdentityResponseTypeDef = TypedDict(
+    "VerifyDomainIdentityResponseTypeDef",
+    {
+        "VerificationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMessageDsnTypeDef = TypedDict(
     "_RequiredMessageDsnTypeDef",
     {
         "ReportingMta": str,
@@ -1412,17 +1641,19 @@
     {
         "ArrivalDate": Union[datetime, str],
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
+
 class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
     pass
 
+
 _RequiredRecipientDsnFieldsTypeDef = TypedDict(
     "_RequiredRecipientDsnFieldsTypeDef",
     {
         "Action": DsnActionType,
         "Status": str,
     },
 )
@@ -1434,40 +1665,42 @@
         "DiagnosticCode": str,
         "LastAttemptDate": Union[datetime, str],
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
+
 class RecipientDsnFieldsTypeDef(
     _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
+
 GetIdentityDkimAttributesResponseTypeDef = TypedDict(
     "GetIdentityDkimAttributesResponseTypeDef",
     {
         "DkimAttributes": Dict[str, IdentityDkimAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityMailFromDomainAttributesResponseTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesResponseTypeDef",
     {
         "MailFromDomainAttributes": Dict[str, IdentityMailFromDomainAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityNotificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityNotificationAttributesResponseTypeDef",
     {
         "NotificationAttributes": Dict[str, IdentityNotificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = TypedDict(
     "_RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "Identities": Sequence[str],
@@ -1477,42 +1710,93 @@
     "_OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef(
     _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     _OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
 ):
     pass
 
+
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSendStatisticsResponseTypeDef = TypedDict(
     "GetSendStatisticsResponseTypeDef",
     {
         "SendDataPoints": List[SendDataPointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateResponseTypeDef = TypedDict(
+    "GetTemplateResponseTypeDef",
+    {
+        "Template": TemplateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
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
+ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = TypedDict(
+    "ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListIdentitiesRequestListIdentitiesPaginateTypeDef = TypedDict(
+    "ListIdentitiesRequestListIdentitiesPaginateTypeDef",
+    {
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = TypedDict(
+    "ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTemplatesRequestListTemplatesPaginateTypeDef = TypedDict(
+    "ListTemplatesRequestListTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplatesMetadata": List[TemplateMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendRawEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendRawEmailRequestRequestTypeDef",
     {
         "RawMessage": RawMessageTypeDef,
@@ -1528,33 +1812,57 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
+
+ReceiptActionOutputTypeDef = TypedDict(
+    "ReceiptActionOutputTypeDef",
+    {
+        "S3Action": S3ActionOutputTypeDef,
+        "BounceAction": BounceActionOutputTypeDef,
+        "WorkmailAction": WorkmailActionOutputTypeDef,
+        "LambdaAction": LambdaActionOutputTypeDef,
+        "StopAction": StopActionOutputTypeDef,
+        "AddHeaderAction": AddHeaderActionOutputTypeDef,
+        "SNSAction": SNSActionOutputTypeDef,
+    },
+    total=False,
+)
+
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
         "LambdaAction": LambdaActionTypeDef,
         "StopAction": StopActionTypeDef,
         "AddHeaderAction": AddHeaderActionTypeDef,
         "SNSAction": SNSActionTypeDef,
     },
     total=False,
 )
 
+ReceiptFilterOutputTypeDef = TypedDict(
+    "ReceiptFilterOutputTypeDef",
+    {
+        "Name": str,
+        "IpFilter": ReceiptIpFilterOutputTypeDef,
+    },
+)
+
 ReceiptFilterTypeDef = TypedDict(
     "ReceiptFilterTypeDef",
     {
         "Name": str,
         "IpFilter": ReceiptIpFilterTypeDef,
     },
 )
@@ -1586,20 +1894,47 @@
         "DefaultTags": Sequence[MessageTagTypeDef],
         "TemplateArn": str,
         "DefaultTemplateData": str,
     },
     total=False,
 )
 
+
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
+
+_RequiredEventDestinationOutputTypeDef = TypedDict(
+    "_RequiredEventDestinationOutputTypeDef",
+    {
+        "Name": str,
+        "MatchingEventTypes": List[EventTypeType],
+    },
+)
+_OptionalEventDestinationOutputTypeDef = TypedDict(
+    "_OptionalEventDestinationOutputTypeDef",
+    {
+        "Enabled": bool,
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "SNSDestination": SNSDestinationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EventDestinationOutputTypeDef(
+    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
+):
+    pass
+
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
 )
@@ -1610,17 +1945,19 @@
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+
 _RequiredBouncedRecipientInfoTypeDef = TypedDict(
     "_RequiredBouncedRecipientInfoTypeDef",
     {
         "Recipient": str,
     },
 )
 _OptionalBouncedRecipientInfoTypeDef = TypedDict(
@@ -1629,19 +1966,46 @@
         "RecipientArn": str,
         "BounceType": BounceTypeType,
         "RecipientDsnFields": RecipientDsnFieldsTypeDef,
     },
     total=False,
 )
 
+
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
+
+_RequiredReceiptRuleOutputTypeDef = TypedDict(
+    "_RequiredReceiptRuleOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalReceiptRuleOutputTypeDef = TypedDict(
+    "_OptionalReceiptRuleOutputTypeDef",
+    {
+        "Enabled": bool,
+        "TlsPolicy": TlsPolicyType,
+        "Recipients": List[str],
+        "Actions": List[ReceiptActionOutputTypeDef],
+        "ScanEnabled": bool,
+    },
+    total=False,
+)
+
+
+class ReceiptRuleOutputTypeDef(
+    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalReceiptRuleTypeDef = TypedDict(
@@ -1652,29 +2016,31 @@
         "Recipients": Sequence[str],
         "Actions": Sequence[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
+
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
-CreateReceiptFilterRequestRequestTypeDef = TypedDict(
-    "CreateReceiptFilterRequestRequestTypeDef",
+
+ListReceiptFiltersResponseTypeDef = TypedDict(
+    "ListReceiptFiltersResponseTypeDef",
     {
-        "Filter": ReceiptFilterTypeDef,
+        "Filters": List[ReceiptFilterOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListReceiptFiltersResponseTypeDef = TypedDict(
-    "ListReceiptFiltersResponseTypeDef",
+CreateReceiptFilterRequestRequestTypeDef = TypedDict(
+    "CreateReceiptFilterRequestRequestTypeDef",
     {
-        "Filters": List[ReceiptFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Filter": ReceiptFilterTypeDef,
     },
 )
 
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Source": str,
@@ -1691,36 +2057,38 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
-CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "EventDestination": EventDestinationTypeDef,
-    },
-)
 
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
-        "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationTypeDef],
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ConfigurationSet": ConfigurationSetOutputTypeDef,
+        "EventDestinations": List[EventDestinationOutputTypeDef],
+        "TrackingOptions": TrackingOptionsOutputTypeDef,
+        "DeliveryOptions": DeliveryOptionsOutputTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "EventDestination": EventDestinationTypeDef,
     },
 )
 
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
@@ -1742,65 +2110,69 @@
         "Explanation": str,
         "MessageDsn": MessageDsnTypeDef,
         "BounceSenderArn": str,
     },
     total=False,
 )
 
+
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "RuleSetName": str,
-        "Rule": ReceiptRuleTypeDef,
-    },
-)
-_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "After": str,
-    },
-    total=False,
-)
-
-class CreateReceiptRuleRequestRequestTypeDef(
-    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
-):
-    pass
 
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
-        "Rule": ReceiptRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rule": ReceiptRuleOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Rules": List[ReceiptRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "RuleSetName": str,
+        "Rule": ReceiptRuleTypeDef,
+    },
+)
+_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "After": str,
     },
+    total=False,
 )
 
+
+class CreateReceiptRuleRequestRequestTypeDef(
+    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
+):
+    pass
+
+
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/waiter.py` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses/waiter.pyi` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/PKG-INFO` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ses
-Version: 1.28.0
-Summary: Type annotations for boto3.SES 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ses"></a>
 
 # mypy-boto3-ses
 
 [![PyPI - mypy-boto3-ses](https://img.shields.io/pypi/v/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ses.svg?color=blue)](https://pypi.org/project/mypy-boto3-ses)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ses?color=blue)](https://pypistats.org/packages/mypy-boto3-ses)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ses)](https://pepy.tech/project/mypy-boto3-ses)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SES 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
+[boto3.SES 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
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
 [mypy-boto3-ses docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ses/).
 
 See how it helps to find and fix potential bugs:
 
@@ -375,22 +375,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ses.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ses.type_defs import (
+    AddHeaderActionOutputTypeDef,
     AddHeaderActionTypeDef,
     ContentTypeDef,
+    BounceActionOutputTypeDef,
     BounceActionTypeDef,
     BulkEmailDestinationStatusTypeDef,
     DestinationTypeDef,
     MessageTagTypeDef,
     CloneReceiptRuleSetRequestRequestTypeDef,
+    CloudWatchDimensionConfigurationOutputTypeDef,
     CloudWatchDimensionConfigurationTypeDef,
+    ConfigurationSetOutputTypeDef,
     ConfigurationSetTypeDef,
     TrackingOptionsTypeDef,
     CreateCustomVerificationEmailTemplateRequestRequestTypeDef,
     CreateReceiptRuleSetRequestRequestTypeDef,
     TemplateTypeDef,
     CustomVerificationEmailTemplateTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
@@ -400,140 +404,156 @@
     DeleteIdentityPolicyRequestRequestTypeDef,
     DeleteIdentityRequestRequestTypeDef,
     DeleteReceiptFilterRequestRequestTypeDef,
     DeleteReceiptRuleRequestRequestTypeDef,
     DeleteReceiptRuleSetRequestRequestTypeDef,
     DeleteTemplateRequestRequestTypeDef,
     DeleteVerifiedEmailAddressRequestRequestTypeDef,
+    DeliveryOptionsOutputTypeDef,
     DeliveryOptionsTypeDef,
     ReceiptRuleSetMetadataTypeDef,
+    ResponseMetadataTypeDef,
     DescribeConfigurationSetRequestRequestTypeDef,
     ReputationOptionsTypeDef,
+    TrackingOptionsOutputTypeDef,
     DescribeReceiptRuleRequestRequestTypeDef,
     DescribeReceiptRuleSetRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    KinesisFirehoseDestinationOutputTypeDef,
+    SNSDestinationOutputTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SNSDestinationTypeDef,
     ExtensionFieldTypeDef,
-    GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateRequestRequestTypeDef,
-    GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesRequestRequestTypeDef,
     IdentityDkimAttributesTypeDef,
     GetIdentityMailFromDomainAttributesRequestRequestTypeDef,
     IdentityMailFromDomainAttributesTypeDef,
     GetIdentityNotificationAttributesRequestRequestTypeDef,
     IdentityNotificationAttributesTypeDef,
     GetIdentityPoliciesRequestRequestTypeDef,
-    GetIdentityPoliciesResponseTypeDef,
     WaiterConfigTypeDef,
     GetIdentityVerificationAttributesRequestRequestTypeDef,
     IdentityVerificationAttributesTypeDef,
-    GetSendQuotaResponseTypeDef,
     SendDataPointTypeDef,
     GetTemplateRequestRequestTypeDef,
+    TemplateOutputTypeDef,
+    LambdaActionOutputTypeDef,
     LambdaActionTypeDef,
-    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
     ListCustomVerificationEmailTemplatesRequestRequestTypeDef,
-    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
     ListIdentitiesRequestRequestTypeDef,
-    ListIdentitiesResponseTypeDef,
     ListIdentityPoliciesRequestRequestTypeDef,
-    ListIdentityPoliciesResponseTypeDef,
-    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
     ListReceiptRuleSetsRequestRequestTypeDef,
-    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateMetadataTypeDef,
-    ListVerifiedEmailAddressesResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutIdentityPolicyRequestRequestTypeDef,
     RawMessageTypeDef,
+    S3ActionOutputTypeDef,
+    SNSActionOutputTypeDef,
+    StopActionOutputTypeDef,
+    WorkmailActionOutputTypeDef,
     S3ActionTypeDef,
     SNSActionTypeDef,
     StopActionTypeDef,
     WorkmailActionTypeDef,
+    ReceiptIpFilterOutputTypeDef,
     ReceiptIpFilterTypeDef,
     ReorderReceiptRuleSetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendBounceResponseTypeDef,
     SendCustomVerificationEmailRequestRequestTypeDef,
-    SendCustomVerificationEmailResponseTypeDef,
-    SendEmailResponseTypeDef,
-    SendRawEmailResponseTypeDef,
-    SendTemplatedEmailResponseTypeDef,
     SetActiveReceiptRuleSetRequestRequestTypeDef,
     SetIdentityDkimEnabledRequestRequestTypeDef,
     SetIdentityFeedbackForwardingEnabledRequestRequestTypeDef,
     SetIdentityHeadersInNotificationsEnabledRequestRequestTypeDef,
     SetIdentityMailFromDomainRequestRequestTypeDef,
     SetIdentityNotificationTopicRequestRequestTypeDef,
     SetReceiptRulePositionRequestRequestTypeDef,
     TestRenderTemplateRequestRequestTypeDef,
-    TestRenderTemplateResponseTypeDef,
     UpdateAccountSendingEnabledRequestRequestTypeDef,
     UpdateConfigurationSetReputationMetricsEnabledRequestRequestTypeDef,
     UpdateConfigurationSetSendingEnabledRequestRequestTypeDef,
     UpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     VerifyDomainDkimRequestRequestTypeDef,
-    VerifyDomainDkimResponseTypeDef,
     VerifyDomainIdentityRequestRequestTypeDef,
-    VerifyDomainIdentityResponseTypeDef,
     VerifyEmailAddressRequestRequestTypeDef,
     VerifyEmailIdentityRequestRequestTypeDef,
     BodyTypeDef,
-    SendBulkTemplatedEmailResponseTypeDef,
     BulkEmailDestinationTypeDef,
     SendTemplatedEmailRequestRequestTypeDef,
+    CloudWatchDestinationOutputTypeDef,
     CloudWatchDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     CreateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef,
     CreateTemplateRequestRequestTypeDef,
-    GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
-    ListCustomVerificationEmailTemplatesResponseTypeDef,
     PutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSendingEnabledResponseTypeDef,
+    GetCustomVerificationEmailTemplateResponseTypeDef,
+    GetIdentityPoliciesResponseTypeDef,
+    GetSendQuotaResponseTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    ListCustomVerificationEmailTemplatesResponseTypeDef,
+    ListIdentitiesResponseTypeDef,
+    ListIdentityPoliciesResponseTypeDef,
     ListReceiptRuleSetsResponseTypeDef,
+    ListVerifiedEmailAddressesResponseTypeDef,
+    SendBounceResponseTypeDef,
+    SendBulkTemplatedEmailResponseTypeDef,
+    SendCustomVerificationEmailResponseTypeDef,
+    SendEmailResponseTypeDef,
+    SendRawEmailResponseTypeDef,
+    SendTemplatedEmailResponseTypeDef,
+    TestRenderTemplateResponseTypeDef,
+    VerifyDomainDkimResponseTypeDef,
+    VerifyDomainIdentityResponseTypeDef,
     MessageDsnTypeDef,
     RecipientDsnFieldsTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
     GetSendStatisticsResponseTypeDef,
+    GetTemplateResponseTypeDef,
+    ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef,
+    ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef,
+    ListIdentitiesRequestListIdentitiesPaginateTypeDef,
+    ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef,
+    ListTemplatesRequestListTemplatesPaginateTypeDef,
     ListTemplatesResponseTypeDef,
     SendRawEmailRequestRequestTypeDef,
+    ReceiptActionOutputTypeDef,
     ReceiptActionTypeDef,
+    ReceiptFilterOutputTypeDef,
     ReceiptFilterTypeDef,
     MessageTypeDef,
     SendBulkTemplatedEmailRequestRequestTypeDef,
+    EventDestinationOutputTypeDef,
     EventDestinationTypeDef,
     BouncedRecipientInfoTypeDef,
+    ReceiptRuleOutputTypeDef,
     ReceiptRuleTypeDef,
-    CreateReceiptFilterRequestRequestTypeDef,
     ListReceiptFiltersResponseTypeDef,
+    CreateReceiptFilterRequestRequestTypeDef,
     SendEmailRequestRequestTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     DescribeConfigurationSetResponseTypeDef,
+    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     SendBounceRequestRequestTypeDef,
-    CreateReceiptRuleRequestRequestTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
+    CreateReceiptRuleRequestRequestTypeDef,
     UpdateReceiptRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddHeaderActionTypeDef:
+def get_structure() -> AddHeaderActionOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ses-1.28.0/mypy_boto3_ses.egg-info/SOURCES.txt` & `mypy-boto3-ses-1.28.12/mypy_boto3_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ses-1.28.0/setup.py` & `mypy-boto3-ses-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ses",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SES 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SES 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

