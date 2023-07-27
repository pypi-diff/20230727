# Comparing `tmp/mypy-boto3-sns-1.28.0.tar.gz` & `tmp/mypy-boto3-sns-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sns-1.28.0.tar", last modified: Thu Jul  6 21:00:40 2023, max compression
+gzip compressed data, was "mypy-boto3-sns-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
```

## Comparing `mypy-boto3-sns-1.28.0.tar` & `mypy-boto3-sns-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.770438 mypy-boto3-sns-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-06 21:00:40.762437 mypy-boto3-sns-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.758437 mypy-boto3-sns-1.28.0/mypy_boto3_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-06 20:56:10.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-06 20:56:10.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-07-06 20:56:14.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-06 20:56:14.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-06 20:56:14.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-07-06 20:56:14.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-06 20:56:13.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-06 20:56:10.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34610 2023-07-06 20:56:15.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-07-06 20:56:14.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:40.758437 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 21:00:40.000000 mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:40.770438 mypy-boto3-sns-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-06 20:56:09.000000 mypy-boto3-sns-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.477319 mypy-boto3-sns-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-07-27 11:49:41.473318 mypy-boto3-sns-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.469318 mypy-boto3-sns-1.28.12/mypy_boto3_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-07-27 11:47:11.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-07-27 11:47:11.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.473318 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.477319 mypy-boto3-sns-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/setup.py
```

### Comparing `mypy-boto3-sns-1.28.0/LICENSE` & `mypy-boto3-sns-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/PKG-INFO` & `mypy-boto3-sns-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.0
-Summary: Type annotations for boto3.SNS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -437,103 +437,104 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
-    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
-    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
+    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
-    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
-    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
+    CreateTopicResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
+    GetEndpointAttributesResponseTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    PublishResponseTypeDef,
+    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.0/README.md` & `mypy-boto3-sns-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,103 +405,104 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
-    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
-    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
+    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
-    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
-    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
+    CreateTopicResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
+    GetEndpointAttributesResponseTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    PublishResponseTypeDef,
+    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/__init__.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/__init__.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/__main__.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SNS 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SNS 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/client.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/client.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/literals.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
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
@@ -268,26 +269,28 @@
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

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/literals.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,15 @@
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
@@ -266,26 +267,28 @@
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

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/paginator.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,136 +56,126 @@
     "ListPlatformApplicationsPaginator",
     "ListSMSSandboxPhoneNumbersPaginator",
     "ListSubscriptionsPaginator",
     "ListSubscriptionsByTopicPaginator",
     "ListTopicsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEndpointsByPlatformApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
     """
 
     def paginate(
-        self, *, PlatformApplicationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PlatformApplicationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
         """
 
-
 class ListOriginationNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
         """
 
-
 class ListPhoneNumbersOptedOutPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPhoneNumbersOptedOutResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
         """
 
-
 class ListPlatformApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlatformApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
         """
 
-
 class ListSMSSandboxPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
         """
 
-
 class ListSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
         """
 
-
 class ListSubscriptionsByTopicPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
     """
 
     def paginate(
-        self, *, TopicArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TopicArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionsByTopicResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
         """
 
-
 class ListTopicsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
         """
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/paginator.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,126 +56,136 @@
     "ListPlatformApplicationsPaginator",
     "ListSMSSandboxPhoneNumbersPaginator",
     "ListSubscriptionsPaginator",
     "ListSubscriptionsByTopicPaginator",
     "ListTopicsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEndpointsByPlatformApplicationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
     """
 
     def paginate(
-        self, *, PlatformApplicationArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PlatformApplicationArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointsByPlatformApplicationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListEndpointsByPlatformApplication.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listendpointsbyplatformapplicationpaginator)
         """
 
+
 class ListOriginationNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOriginationNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListOriginationNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listoriginationnumberspaginator)
         """
 
+
 class ListPhoneNumbersOptedOutPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPhoneNumbersOptedOutResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPhoneNumbersOptedOut.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listphonenumbersoptedoutpaginator)
         """
 
+
 class ListPlatformApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlatformApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListPlatformApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listplatformapplicationspaginator)
         """
 
+
 class ListSMSSandboxPhoneNumbersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSMSSandboxPhoneNumbersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSMSSandboxPhoneNumbers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsmssandboxphonenumberspaginator)
         """
 
+
 class ListSubscriptionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionspaginator)
         """
 
+
 class ListSubscriptionsByTopicPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
     """
 
     def paginate(
-        self, *, TopicArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TopicArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSubscriptionsByTopicResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListSubscriptionsByTopic.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listsubscriptionsbytopicpaginator)
         """
 
+
 class ListTopicsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Paginator.ListTopics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/paginators/#listtopicspaginator)
         """
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/service_resource.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/service_resource.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/type_defs.py` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,103 +31,104 @@
 
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
-    "ConfirmSubscriptionResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
-    "CreatePlatformApplicationResponseTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     "CreatePlatformEndpointInputRequestTypeDef",
     "CreateSMSSandboxPhoneNumberInputRequestTypeDef",
     "TagTypeDef",
-    "CreateTopicResponseTypeDef",
     "DeleteEndpointInputRequestTypeDef",
     "DeletePlatformApplicationInputRequestTypeDef",
     "DeleteSMSSandboxPhoneNumberInputRequestTypeDef",
     "DeleteTopicInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
     "GetDataProtectionPolicyInputRequestTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
     "GetEndpointAttributesInputRequestTypeDef",
-    "GetEndpointAttributesResponseTypeDef",
     "GetPlatformApplicationAttributesInputRequestTypeDef",
-    "GetPlatformApplicationAttributesResponseTypeDef",
     "GetSMSAttributesInputRequestTypeDef",
-    "GetSMSAttributesResponseTypeDef",
-    "GetSMSSandboxAccountStatusResultTypeDef",
     "GetSubscriptionAttributesInputRequestTypeDef",
-    "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesInputRequestTypeDef",
-    "GetTopicAttributesResponseTypeDef",
-    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointsByPlatformApplicationInputRequestTypeDef",
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListOriginationNumbersRequestRequestTypeDef",
     "PhoneNumberInformationTypeDef",
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListPlatformApplicationsInputRequestTypeDef",
     "PlatformApplicationTypeDef",
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
-    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTopicsInputListTopicsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishBatchResultEntryTypeDef",
-    "PublishResponseTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
-    "ResponseMetadataTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
     "SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef",
     "SetPlatformApplicationAttributesInputRequestTypeDef",
     "SetSMSAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef",
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
-    "SubscribeResponseTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    "ConfirmSubscriptionResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreatePlatformApplicationResponseTypeDef",
+    "CreateTopicResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
+    "GetEndpointAttributesResponseTypeDef",
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    "GetSMSAttributesResponseTypeDef",
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    "GetSubscriptionAttributesResponseTypeDef",
+    "GetTopicAttributesResponseTypeDef",
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    "PublishResponseTypeDef",
+    "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
+    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
     "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
@@ -178,19 +179,22 @@
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
-CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "isOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredConfirmSubscriptionInputRequestTypeDef = TypedDict(
     "_RequiredConfirmSubscriptionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -230,30 +234,14 @@
 class ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef(
     _RequiredConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     _OptionalConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
 ):
     pass
 
 
-ConfirmSubscriptionResponseTypeDef = TypedDict(
-    "ConfirmSubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePlatformApplicationInputRequestTypeDef = TypedDict(
     "CreatePlatformApplicationInputRequestTypeDef",
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
@@ -264,22 +252,14 @@
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
 )
 
-CreatePlatformApplicationResponseTypeDef = TypedDict(
-    "CreatePlatformApplicationResponseTypeDef",
-    {
-        "PlatformApplicationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
     "_RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     {
         "Token": str,
     },
 )
 _OptionalCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
@@ -349,22 +329,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateTopicResponseTypeDef = TypedDict(
-    "CreateTopicResponseTypeDef",
-    {
-        "TopicArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEndpointInputRequestTypeDef = TypedDict(
     "DeleteEndpointInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
@@ -385,21 +357,14 @@
 DeleteTopicInputRequestTypeDef = TypedDict(
     "DeleteTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
@@ -408,128 +373,60 @@
 GetDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "DataProtectionPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAttributesInputRequestTypeDef = TypedDict(
     "GetEndpointAttributesInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-GetEndpointAttributesResponseTypeDef = TypedDict(
-    "GetEndpointAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPlatformApplicationAttributesInputRequestTypeDef = TypedDict(
     "GetPlatformApplicationAttributesInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 
-GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSMSAttributesInputRequestTypeDef = TypedDict(
     "GetSMSAttributesInputRequestTypeDef",
     {
         "attributes": Sequence[str],
     },
     total=False,
 )
 
-GetSMSAttributesResponseTypeDef = TypedDict(
-    "GetSMSAttributesResponseTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    {
-        "IsInSandbox": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionAttributesInputRequestTypeDef = TypedDict(
     "GetSubscriptionAttributesInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
-GetSubscriptionAttributesResponseTypeDef = TypedDict(
-    "GetSubscriptionAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTopicAttributesInputRequestTypeDef = TypedDict(
     "GetTopicAttributesInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-GetTopicAttributesResponseTypeDef = TypedDict(
-    "GetTopicAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PlatformApplicationArn": str,
-    },
-)
-_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
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
-class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
-    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
     "_RequiredListEndpointsByPlatformApplicationInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
@@ -544,22 +441,14 @@
 class ListEndpointsByPlatformApplicationInputRequestTypeDef(
     _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef,
     _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef,
 ):
     pass
 
 
-ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOriginationNumbersRequestRequestTypeDef = TypedDict(
     "ListOriginationNumbersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -574,47 +463,22 @@
         "Iso2CountryCode": str,
         "RouteType": RouteTypeType,
         "NumberCapabilities": List[NumberCapabilityType],
     },
     total=False,
 )
 
-ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPhoneNumbersOptedOutInputRequestTypeDef = TypedDict(
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    {
-        "phoneNumbers": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlatformApplicationsInputRequestTypeDef = TypedDict(
     "ListPlatformApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -624,22 +488,14 @@
     {
         "PlatformApplicationArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSMSSandboxPhoneNumbersInputRequestTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -650,36 +506,14 @@
     {
         "PhoneNumber": str,
         "Status": SMSSandboxPhoneNumberVerificationStatusType,
     },
     total=False,
 )
 
-_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
-    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionsByTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
@@ -706,22 +540,14 @@
         "Protocol": str,
         "Endpoint": str,
         "TopicArn": str,
     },
     total=False,
 )
 
-ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscriptionsInputRequestTypeDef = TypedDict(
     "ListSubscriptionsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -729,20 +555,20 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
-    "ListTopicsInputListTopicsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
@@ -782,43 +608,24 @@
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
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
 PublishBatchResultEntryTypeDef = TypedDict(
     "PublishBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
-PublishResponseTypeDef = TypedDict(
-    "PublishResponseTypeDef",
-    {
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
         "DataProtectionPolicy": str,
     },
 )
@@ -834,25 +641,14 @@
 RemovePermissionInputTopicRemovePermissionTypeDef = TypedDict(
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     {
         "Label": str,
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
 SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef = TypedDict(
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     {
         "Attributes": Mapping[str, str],
     },
 )
 
@@ -1018,22 +814,14 @@
 
 class SubscribeInputTopicSubscribeTypeDef(
     _RequiredSubscribeInputTopicSubscribeTypeDef, _OptionalSubscribeInputTopicSubscribeTypeDef
 ):
     pass
 
 
-SubscribeResponseTypeDef = TypedDict(
-    "SubscribeResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeInputRequestTypeDef = TypedDict(
     "UnsubscribeInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
@@ -1049,14 +837,143 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
+CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    {
+        "isOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmSubscriptionResponseTypeDef = TypedDict(
+    "ConfirmSubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlatformApplicationResponseTypeDef = TypedDict(
+    "CreatePlatformApplicationResponseTypeDef",
+    {
+        "PlatformApplicationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTopicResponseTypeDef = TypedDict(
+    "CreateTopicResponseTypeDef",
+    {
+        "TopicArn": str,
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
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "DataProtectionPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointAttributesResponseTypeDef = TypedDict(
+    "GetEndpointAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSMSAttributesResponseTypeDef = TypedDict(
+    "GetSMSAttributesResponseTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    {
+        "IsInSandbox": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionAttributesResponseTypeDef = TypedDict(
+    "GetSubscriptionAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTopicAttributesResponseTypeDef = TypedDict(
+    "GetTopicAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    {
+        "phoneNumbers": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishResponseTypeDef = TypedDict(
+    "PublishResponseTypeDef",
+    {
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResponseTypeDef = TypedDict(
+    "SubscribeResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTopicInputRequestTypeDef = TypedDict(
     "_RequiredCreateTopicInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTopicInputRequestTypeDef = TypedDict(
@@ -1096,90 +1013,182 @@
 class CreateTopicInputServiceResourceCreateTopicTypeDef(
     _RequiredCreateTopicInputServiceResourceCreateTopicTypeDef,
     _OptionalCreateTopicInputServiceResourceCreateTopicTypeDef,
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
 
 ListEndpointsByPlatformApplicationResponseTypeDef = TypedDict(
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PlatformApplicationArn": str,
+    },
+)
+_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
+    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+):
+    pass
+
+
+ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
+    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+):
+    pass
+
+
+ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
+    "ListTopicsInputListTopicsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListOriginationNumbersResultTypeDef = TypedDict(
     "ListOriginationNumbersResultTypeDef",
     {
         "NextToken": str,
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformApplicationsResponseTypeDef = TypedDict(
     "ListPlatformApplicationsResponseTypeDef",
     {
         "PlatformApplications": List[PlatformApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSMSSandboxPhoneNumbersResultTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[SMSSandboxPhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionsByTopicResponseTypeDef = TypedDict(
     "ListSubscriptionsByTopicResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionsResponseTypeDef = TypedDict(
     "ListSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
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
     },
 )
 
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -1289,15 +1298,15 @@
 
 
 PublishBatchResponseTypeDef = TypedDict(
     "PublishBatchResponseTypeDef",
     {
         "Successful": List[PublishBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns/type_defs.pyi` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,103 +30,104 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionInputRequestTypeDef",
     "AddPermissionInputTopicAddPermissionTypeDef",
     "BatchResultErrorEntryTypeDef",
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfirmSubscriptionInputRequestTypeDef",
     "ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef",
-    "ConfirmSubscriptionResponseTypeDef",
-    "CreateEndpointResponseTypeDef",
     "CreatePlatformApplicationInputRequestTypeDef",
     "CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef",
-    "CreatePlatformApplicationResponseTypeDef",
     "CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     "CreatePlatformEndpointInputRequestTypeDef",
     "CreateSMSSandboxPhoneNumberInputRequestTypeDef",
     "TagTypeDef",
-    "CreateTopicResponseTypeDef",
     "DeleteEndpointInputRequestTypeDef",
     "DeletePlatformApplicationInputRequestTypeDef",
     "DeleteSMSSandboxPhoneNumberInputRequestTypeDef",
     "DeleteTopicInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EndpointTypeDef",
     "GetDataProtectionPolicyInputRequestTypeDef",
-    "GetDataProtectionPolicyResponseTypeDef",
     "GetEndpointAttributesInputRequestTypeDef",
-    "GetEndpointAttributesResponseTypeDef",
     "GetPlatformApplicationAttributesInputRequestTypeDef",
-    "GetPlatformApplicationAttributesResponseTypeDef",
     "GetSMSAttributesInputRequestTypeDef",
-    "GetSMSAttributesResponseTypeDef",
-    "GetSMSSandboxAccountStatusResultTypeDef",
     "GetSubscriptionAttributesInputRequestTypeDef",
-    "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesInputRequestTypeDef",
-    "GetTopicAttributesResponseTypeDef",
-    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEndpointsByPlatformApplicationInputRequestTypeDef",
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListOriginationNumbersRequestRequestTypeDef",
     "PhoneNumberInformationTypeDef",
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListPlatformApplicationsInputRequestTypeDef",
     "PlatformApplicationTypeDef",
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
-    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTopicsInputListTopicsPaginateTypeDef",
+    "TagOutputTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishBatchResultEntryTypeDef",
-    "PublishResponseTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
     "RemovePermissionInputTopicRemovePermissionTypeDef",
-    "ResponseMetadataTypeDef",
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     "SetEndpointAttributesInputRequestTypeDef",
     "SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef",
     "SetPlatformApplicationAttributesInputRequestTypeDef",
     "SetSMSAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputRequestTypeDef",
     "SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef",
     "SetTopicAttributesInputRequestTypeDef",
     "SetTopicAttributesInputTopicSetAttributesTypeDef",
     "SubscribeInputRequestTypeDef",
     "SubscribeInputTopicSubscribeTypeDef",
-    "SubscribeResponseTypeDef",
     "UnsubscribeInputRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    "ConfirmSubscriptionResponseTypeDef",
+    "CreateEndpointResponseTypeDef",
+    "CreatePlatformApplicationResponseTypeDef",
+    "CreateTopicResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDataProtectionPolicyResponseTypeDef",
+    "GetEndpointAttributesResponseTypeDef",
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    "GetSMSAttributesResponseTypeDef",
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    "GetSubscriptionAttributesResponseTypeDef",
+    "GetTopicAttributesResponseTypeDef",
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    "PublishResponseTypeDef",
+    "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
+    "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    "ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
     "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
@@ -175,19 +176,22 @@
 CheckIfPhoneNumberIsOptedOutInputRequestTypeDef = TypedDict(
     "CheckIfPhoneNumberIsOptedOutInputRequestTypeDef",
     {
         "phoneNumber": str,
     },
 )
 
-CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
-    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "isOptedOut": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredConfirmSubscriptionInputRequestTypeDef = TypedDict(
     "_RequiredConfirmSubscriptionInputRequestTypeDef",
     {
         "TopicArn": str,
@@ -223,30 +227,14 @@
 
 class ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef(
     _RequiredConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
     _OptionalConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
 ):
     pass
 
-ConfirmSubscriptionResponseTypeDef = TypedDict(
-    "ConfirmSubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEndpointResponseTypeDef = TypedDict(
-    "CreateEndpointResponseTypeDef",
-    {
-        "EndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePlatformApplicationInputRequestTypeDef = TypedDict(
     "CreatePlatformApplicationInputRequestTypeDef",
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
@@ -257,22 +245,14 @@
     {
         "Name": str,
         "Platform": str,
         "Attributes": Mapping[str, str],
     },
 )
 
-CreatePlatformApplicationResponseTypeDef = TypedDict(
-    "CreatePlatformApplicationResponseTypeDef",
-    {
-        "PlatformApplicationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
     "_RequiredCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef",
     {
         "Token": str,
     },
 )
 _OptionalCreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef = TypedDict(
@@ -336,22 +316,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateTopicResponseTypeDef = TypedDict(
-    "CreateTopicResponseTypeDef",
-    {
-        "TopicArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEndpointInputRequestTypeDef = TypedDict(
     "DeleteEndpointInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
@@ -372,21 +344,14 @@
 DeleteTopicInputRequestTypeDef = TypedDict(
     "DeleteTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "EndpointArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
@@ -395,126 +360,60 @@
 GetDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "GetDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetDataProtectionPolicyResponseTypeDef = TypedDict(
-    "GetDataProtectionPolicyResponseTypeDef",
-    {
-        "DataProtectionPolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEndpointAttributesInputRequestTypeDef = TypedDict(
     "GetEndpointAttributesInputRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 
-GetEndpointAttributesResponseTypeDef = TypedDict(
-    "GetEndpointAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPlatformApplicationAttributesInputRequestTypeDef = TypedDict(
     "GetPlatformApplicationAttributesInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 
-GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
-    "GetPlatformApplicationAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSMSAttributesInputRequestTypeDef = TypedDict(
     "GetSMSAttributesInputRequestTypeDef",
     {
         "attributes": Sequence[str],
     },
     total=False,
 )
 
-GetSMSAttributesResponseTypeDef = TypedDict(
-    "GetSMSAttributesResponseTypeDef",
-    {
-        "attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
-    "GetSMSSandboxAccountStatusResultTypeDef",
-    {
-        "IsInSandbox": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSubscriptionAttributesInputRequestTypeDef = TypedDict(
     "GetSubscriptionAttributesInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
-GetSubscriptionAttributesResponseTypeDef = TypedDict(
-    "GetSubscriptionAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTopicAttributesInputRequestTypeDef = TypedDict(
     "GetTopicAttributesInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 
-GetTopicAttributesResponseTypeDef = TypedDict(
-    "GetTopicAttributesResponseTypeDef",
-    {
-        "Attributes": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
-    {
-        "PlatformApplicationArn": str,
-    },
-)
-_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
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
 
-class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
-    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
-):
-    pass
-
 _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
     "_RequiredListEndpointsByPlatformApplicationInputRequestTypeDef",
     {
         "PlatformApplicationArn": str,
     },
 )
 _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef = TypedDict(
@@ -527,22 +426,14 @@
 
 class ListEndpointsByPlatformApplicationInputRequestTypeDef(
     _RequiredListEndpointsByPlatformApplicationInputRequestTypeDef,
     _OptionalListEndpointsByPlatformApplicationInputRequestTypeDef,
 ):
     pass
 
-ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
-    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOriginationNumbersRequestRequestTypeDef = TypedDict(
     "ListOriginationNumbersRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -557,47 +448,22 @@
         "Iso2CountryCode": str,
         "RouteType": RouteTypeType,
         "NumberCapabilities": List[NumberCapabilityType],
     },
     total=False,
 )
 
-ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPhoneNumbersOptedOutInputRequestTypeDef = TypedDict(
     "ListPhoneNumbersOptedOutInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
-    "ListPhoneNumbersOptedOutResponseTypeDef",
-    {
-        "phoneNumbers": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
-    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlatformApplicationsInputRequestTypeDef = TypedDict(
     "ListPlatformApplicationsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -607,22 +473,14 @@
     {
         "PlatformApplicationArn": str,
         "Attributes": Dict[str, str],
     },
     total=False,
 )
 
-ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
-    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSMSSandboxPhoneNumbersInputRequestTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -633,34 +491,14 @@
     {
         "PhoneNumber": str,
         "Status": SMSSandboxPhoneNumberVerificationStatusType,
     },
     total=False,
 )
 
-_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
-    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
-    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
-):
-    pass
-
 _RequiredListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
     "_RequiredListSubscriptionsByTopicInputRequestTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalListSubscriptionsByTopicInputRequestTypeDef = TypedDict(
@@ -685,22 +523,14 @@
         "Protocol": str,
         "Endpoint": str,
         "TopicArn": str,
     },
     total=False,
 )
 
-ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
-    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSubscriptionsInputRequestTypeDef = TypedDict(
     "ListSubscriptionsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -708,20 +538,20 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
-    "ListTopicsInputListTopicsPaginateTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
@@ -759,43 +589,24 @@
 OptInPhoneNumberInputRequestTypeDef = TypedDict(
     "OptInPhoneNumberInputRequestTypeDef",
     {
         "phoneNumber": str,
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
 PublishBatchResultEntryTypeDef = TypedDict(
     "PublishBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "SequenceNumber": str,
     },
     total=False,
 )
 
-PublishResponseTypeDef = TypedDict(
-    "PublishResponseTypeDef",
-    {
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutDataProtectionPolicyInputRequestTypeDef = TypedDict(
     "PutDataProtectionPolicyInputRequestTypeDef",
     {
         "ResourceArn": str,
         "DataProtectionPolicy": str,
     },
 )
@@ -811,25 +622,14 @@
 RemovePermissionInputTopicRemovePermissionTypeDef = TypedDict(
     "RemovePermissionInputTopicRemovePermissionTypeDef",
     {
         "Label": str,
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
 SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef = TypedDict(
     "SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef",
     {
         "Attributes": Mapping[str, str],
     },
 )
 
@@ -983,22 +783,14 @@
 )
 
 class SubscribeInputTopicSubscribeTypeDef(
     _RequiredSubscribeInputTopicSubscribeTypeDef, _OptionalSubscribeInputTopicSubscribeTypeDef
 ):
     pass
 
-SubscribeResponseTypeDef = TypedDict(
-    "SubscribeResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnsubscribeInputRequestTypeDef = TypedDict(
     "UnsubscribeInputRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 
@@ -1014,14 +806,143 @@
     "VerifySMSSandboxPhoneNumberInputRequestTypeDef",
     {
         "PhoneNumber": str,
         "OneTimePassword": str,
     },
 )
 
+CheckIfPhoneNumberIsOptedOutResponseTypeDef = TypedDict(
+    "CheckIfPhoneNumberIsOptedOutResponseTypeDef",
+    {
+        "isOptedOut": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmSubscriptionResponseTypeDef = TypedDict(
+    "ConfirmSubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEndpointResponseTypeDef = TypedDict(
+    "CreateEndpointResponseTypeDef",
+    {
+        "EndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlatformApplicationResponseTypeDef = TypedDict(
+    "CreatePlatformApplicationResponseTypeDef",
+    {
+        "PlatformApplicationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTopicResponseTypeDef = TypedDict(
+    "CreateTopicResponseTypeDef",
+    {
+        "TopicArn": str,
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
+GetDataProtectionPolicyResponseTypeDef = TypedDict(
+    "GetDataProtectionPolicyResponseTypeDef",
+    {
+        "DataProtectionPolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointAttributesResponseTypeDef = TypedDict(
+    "GetEndpointAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlatformApplicationAttributesResponseTypeDef = TypedDict(
+    "GetPlatformApplicationAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSMSAttributesResponseTypeDef = TypedDict(
+    "GetSMSAttributesResponseTypeDef",
+    {
+        "attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSMSSandboxAccountStatusResultTypeDef = TypedDict(
+    "GetSMSSandboxAccountStatusResultTypeDef",
+    {
+        "IsInSandbox": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSubscriptionAttributesResponseTypeDef = TypedDict(
+    "GetSubscriptionAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTopicAttributesResponseTypeDef = TypedDict(
+    "GetTopicAttributesResponseTypeDef",
+    {
+        "Attributes": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPhoneNumbersOptedOutResponseTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutResponseTypeDef",
+    {
+        "phoneNumbers": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishResponseTypeDef = TypedDict(
+    "PublishResponseTypeDef",
+    {
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubscribeResponseTypeDef = TypedDict(
+    "SubscribeResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateTopicInputRequestTypeDef = TypedDict(
     "_RequiredCreateTopicInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateTopicInputRequestTypeDef = TypedDict(
@@ -1057,90 +978,178 @@
 
 class CreateTopicInputServiceResourceCreateTopicTypeDef(
     _RequiredCreateTopicInputServiceResourceCreateTopicTypeDef,
     _OptionalCreateTopicInputServiceResourceCreateTopicTypeDef,
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
 
 ListEndpointsByPlatformApplicationResponseTypeDef = TypedDict(
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PlatformApplicationArn": str,
+    },
+)
+_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef(
+    _RequiredListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    _OptionalListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+):
+    pass
+
+ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef = TypedDict(
+    "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef = TypedDict(
+    "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef = TypedDict(
+    "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef = TypedDict(
+    "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "TopicArn": str,
+    },
+)
+_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef = TypedDict(
+    "_OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef(
+    _RequiredListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    _OptionalListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+):
+    pass
+
+ListSubscriptionsInputListSubscriptionsPaginateTypeDef = TypedDict(
+    "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicsInputListTopicsPaginateTypeDef = TypedDict(
+    "ListTopicsInputListTopicsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListOriginationNumbersResultTypeDef = TypedDict(
     "ListOriginationNumbersResultTypeDef",
     {
         "NextToken": str,
         "PhoneNumbers": List[PhoneNumberInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformApplicationsResponseTypeDef = TypedDict(
     "ListPlatformApplicationsResponseTypeDef",
     {
         "PlatformApplications": List[PlatformApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSMSSandboxPhoneNumbersResultTypeDef = TypedDict(
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     {
         "PhoneNumbers": List[SMSSandboxPhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionsByTopicResponseTypeDef = TypedDict(
     "ListSubscriptionsByTopicResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSubscriptionsResponseTypeDef = TypedDict(
     "ListSubscriptionsResponseTypeDef",
     {
         "Subscriptions": List[SubscriptionTypeDef],
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
     },
 )
 
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPublishBatchRequestEntryTypeDef = TypedDict(
     "_RequiredPublishBatchRequestEntryTypeDef",
     {
         "Id": str,
@@ -1242,15 +1251,15 @@
     pass
 
 PublishBatchResponseTypeDef = TypedDict(
     "PublishBatchResponseTypeDef",
     {
         "Successful": List[PublishBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishBatchInputRequestTypeDef = TypedDict(
     "PublishBatchInputRequestTypeDef",
     {
         "TopicArn": str,
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/PKG-INFO` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.0
-Summary: Type annotations for boto3.SNS 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sns"></a>
 
 # mypy-boto3-sns
 
 [![PyPI - mypy-boto3-sns](https://img.shields.io/pypi/v/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sns?color=blue)](https://pypistats.org/packages/mypy-boto3-sns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -437,103 +437,104 @@
 
 ```python
 from mypy_boto3_sns.type_defs import (
     AddPermissionInputRequestTypeDef,
     AddPermissionInputTopicAddPermissionTypeDef,
     BatchResultErrorEntryTypeDef,
     CheckIfPhoneNumberIsOptedOutInputRequestTypeDef,
-    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ResponseMetadataTypeDef,
     ConfirmSubscriptionInputRequestTypeDef,
     ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef,
-    ConfirmSubscriptionResponseTypeDef,
-    CreateEndpointResponseTypeDef,
     CreatePlatformApplicationInputRequestTypeDef,
     CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef,
-    CreatePlatformApplicationResponseTypeDef,
     CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef,
     CreatePlatformEndpointInputRequestTypeDef,
     CreateSMSSandboxPhoneNumberInputRequestTypeDef,
     TagTypeDef,
-    CreateTopicResponseTypeDef,
     DeleteEndpointInputRequestTypeDef,
     DeletePlatformApplicationInputRequestTypeDef,
     DeleteSMSSandboxPhoneNumberInputRequestTypeDef,
     DeleteTopicInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EndpointTypeDef,
     GetDataProtectionPolicyInputRequestTypeDef,
-    GetDataProtectionPolicyResponseTypeDef,
     GetEndpointAttributesInputRequestTypeDef,
-    GetEndpointAttributesResponseTypeDef,
     GetPlatformApplicationAttributesInputRequestTypeDef,
-    GetPlatformApplicationAttributesResponseTypeDef,
     GetSMSAttributesInputRequestTypeDef,
-    GetSMSAttributesResponseTypeDef,
-    GetSMSSandboxAccountStatusResultTypeDef,
     GetSubscriptionAttributesInputRequestTypeDef,
-    GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesInputRequestTypeDef,
-    GetTopicAttributesResponseTypeDef,
-    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEndpointsByPlatformApplicationInputRequestTypeDef,
-    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListOriginationNumbersRequestRequestTypeDef,
     PhoneNumberInformationTypeDef,
-    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPhoneNumbersOptedOutInputRequestTypeDef,
-    ListPhoneNumbersOptedOutResponseTypeDef,
-    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListPlatformApplicationsInputRequestTypeDef,
     PlatformApplicationTypeDef,
-    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
-    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
-    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTopicsInputListTopicsPaginateTypeDef,
+    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishBatchResultEntryTypeDef,
-    PublishResponseTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
     RemovePermissionInputTopicRemovePermissionTypeDef,
-    ResponseMetadataTypeDef,
     SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef,
     SetEndpointAttributesInputRequestTypeDef,
     SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef,
     SetPlatformApplicationAttributesInputRequestTypeDef,
     SetSMSAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputRequestTypeDef,
     SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef,
     SetTopicAttributesInputRequestTypeDef,
     SetTopicAttributesInputTopicSetAttributesTypeDef,
     SubscribeInputRequestTypeDef,
     SubscribeInputTopicSubscribeTypeDef,
-    SubscribeResponseTypeDef,
     UnsubscribeInputRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     VerifySMSSandboxPhoneNumberInputRequestTypeDef,
+    CheckIfPhoneNumberIsOptedOutResponseTypeDef,
+    ConfirmSubscriptionResponseTypeDef,
+    CreateEndpointResponseTypeDef,
+    CreatePlatformApplicationResponseTypeDef,
+    CreateTopicResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDataProtectionPolicyResponseTypeDef,
+    GetEndpointAttributesResponseTypeDef,
+    GetPlatformApplicationAttributesResponseTypeDef,
+    GetSMSAttributesResponseTypeDef,
+    GetSMSSandboxAccountStatusResultTypeDef,
+    GetSubscriptionAttributesResponseTypeDef,
+    GetTopicAttributesResponseTypeDef,
+    ListPhoneNumbersOptedOutResponseTypeDef,
+    PublishResponseTypeDef,
+    SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
+    ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
+    ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
+    ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
+    ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
+    ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
+    ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef,
+    ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
+    ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.0/mypy_boto3_sns.egg-info/SOURCES.txt` & `mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.0/setup.py` & `mypy-boto3-sns-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sns",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SNS 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

