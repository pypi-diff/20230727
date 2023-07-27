# Comparing `tmp/mypy-boto3-iotevents-1.28.0.tar.gz` & `tmp/mypy-boto3-iotevents-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-1.28.0.tar", last modified: Thu Jul  6 20:59:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
```

## Comparing `mypy-boto3-iotevents-1.28.0.tar` & `mypy-boto3-iotevents-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.146330 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37394 2023-07-06 20:43:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-07-06 20:43:45.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15927 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:59:47.000000 mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:48.158330 mypy-boto3-iotevents-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:43:44.000000 mypy-boto3-iotevents-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53782 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53679 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.640482 mypy-boto3-iotevents-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:24:02.000000 mypy-boto3-iotevents-1.28.12/setup.py
```

### Comparing `mypy-boto3-iotevents-1.28.0/LICENSE` & `mypy-boto3-iotevents-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.0/PKG-INFO` & `mypy-boto3-iotevents-1.28.12/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents
-Version: 1.28.0
-Summary: Type annotations for boto3.IoTEvents 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,127 +304,173 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
+    AcknowledgeFlowOutputTypeDef,
     AcknowledgeFlowTypeDef,
+    ClearTimerActionOutputTypeDef,
+    ResetTimerActionOutputTypeDef,
+    SetTimerActionOutputTypeDef,
+    SetVariableActionOutputTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
     SetVariableActionTypeDef,
+    InitializationConfigurationOutputTypeDef,
     InitializationConfigurationTypeDef,
     AlarmModelSummaryTypeDef,
     AlarmModelVersionSummaryTypeDef,
+    SimpleRuleOutputTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
+    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
+    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     TagTypeDef,
     CreateAlarmModelResponseTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
+    DetectorDebugOptionOutputTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
+    PayloadOutputTypeDef,
     PayloadTypeDef,
+    EmailContentOutputTypeDef,
     EmailContentTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    SSOIdentityOutputTypeDef,
     SSOIdentityTypeDef,
     ResponseMetadataTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAlarmModelResponseTypeDef,
+    AlarmCapabilitiesOutputTypeDef,
     AlarmCapabilitiesTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
+    AlarmRuleOutputTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
+    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
+    DynamoDBActionOutputTypeDef,
+    DynamoDBv2ActionOutputTypeDef,
+    FirehoseActionOutputTypeDef,
+    IotEventsActionOutputTypeDef,
+    IotTopicPublishActionOutputTypeDef,
+    LambdaActionOutputTypeDef,
+    SNSTopicPublishActionOutputTypeDef,
+    SqsActionOutputTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
     IotTopicPublishActionTypeDef,
     LambdaActionTypeDef,
     SNSTopicPublishActionTypeDef,
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RecipientDetailOutputTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
-    CreateInputRequestRequestTypeDef,
     InputTypeDef,
+    CreateInputRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
+    NotificationTargetActionsOutputTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
+    EmailRecipientsOutputTypeDef,
+    SMSConfigurationOutputTypeDef,
     EmailRecipientsTypeDef,
     SMSConfigurationTypeDef,
+    ActionOutputTypeDef,
+    AlarmActionOutputTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
+    EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
+    EventOutputTypeDef,
+    TransitionEventOutputTypeDef,
+    AlarmEventActionsOutputTypeDef,
     EventTypeDef,
     TransitionEventTypeDef,
     AlarmEventActionsTypeDef,
+    NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
+    OnEnterLifecycleOutputTypeDef,
+    OnExitLifecycleOutputTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
+    StateOutputTypeDef,
     StateTypeDef,
-    CreateAlarmModelRequestRequestTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
-    CreateDetectorModelRequestRequestTypeDef,
     DetectorModelTypeDef,
+    CreateDetectorModelRequestRequestTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_structure() -> AcknowledgeFlowOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.0/README.md` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iotevents
+Version: 1.28.12
+Summary: Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iotevents type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iotevents"></a>
 
 # mypy-boto3-iotevents
 
 [![PyPI - mypy-boto3-iotevents](https://img.shields.io/pypi/v/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotevents?color=blue)](https://pypistats.org/packages/mypy-boto3-iotevents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents)](https://pepy.tech/project/mypy-boto3-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[boto3.IoTEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [mypy-boto3-iotevents docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,127 +304,173 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotevents.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotevents.type_defs import (
+    AcknowledgeFlowOutputTypeDef,
     AcknowledgeFlowTypeDef,
+    ClearTimerActionOutputTypeDef,
+    ResetTimerActionOutputTypeDef,
+    SetTimerActionOutputTypeDef,
+    SetVariableActionOutputTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
     SetVariableActionTypeDef,
+    InitializationConfigurationOutputTypeDef,
     InitializationConfigurationTypeDef,
     AlarmModelSummaryTypeDef,
     AlarmModelVersionSummaryTypeDef,
+    SimpleRuleOutputTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
+    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
+    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     TagTypeDef,
     CreateAlarmModelResponseTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
+    DetectorDebugOptionOutputTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
+    PayloadOutputTypeDef,
     PayloadTypeDef,
+    EmailContentOutputTypeDef,
     EmailContentTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
+    SSOIdentityOutputTypeDef,
     SSOIdentityTypeDef,
     ResponseMetadataTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAlarmModelResponseTypeDef,
+    AlarmCapabilitiesOutputTypeDef,
     AlarmCapabilitiesTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
+    AlarmRuleOutputTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
+    AssetPropertyValueOutputTypeDef,
     AssetPropertyValueTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
+    DynamoDBActionOutputTypeDef,
+    DynamoDBv2ActionOutputTypeDef,
+    FirehoseActionOutputTypeDef,
+    IotEventsActionOutputTypeDef,
+    IotTopicPublishActionOutputTypeDef,
+    LambdaActionOutputTypeDef,
+    SNSTopicPublishActionOutputTypeDef,
+    SqsActionOutputTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
     IotTopicPublishActionTypeDef,
     LambdaActionTypeDef,
     SNSTopicPublishActionTypeDef,
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RecipientDetailOutputTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
+    IotSiteWiseActionOutputTypeDef,
     IotSiteWiseActionTypeDef,
-    CreateInputRequestRequestTypeDef,
     InputTypeDef,
+    CreateInputRequestRequestTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
+    NotificationTargetActionsOutputTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
+    EmailRecipientsOutputTypeDef,
+    SMSConfigurationOutputTypeDef,
     EmailRecipientsTypeDef,
     SMSConfigurationTypeDef,
+    ActionOutputTypeDef,
+    AlarmActionOutputTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
+    EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
+    EventOutputTypeDef,
+    TransitionEventOutputTypeDef,
+    AlarmEventActionsOutputTypeDef,
     EventTypeDef,
     TransitionEventTypeDef,
     AlarmEventActionsTypeDef,
+    NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
+    OnEnterLifecycleOutputTypeDef,
+    OnExitLifecycleOutputTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
+    StateOutputTypeDef,
     StateTypeDef,
-    CreateAlarmModelRequestRequestTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
-    CreateDetectorModelRequestRequestTypeDef,
     DetectorModelTypeDef,
+    CreateDetectorModelRequestRequestTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_structure() -> AcknowledgeFlowOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/__main__.py` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEvents 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.IoTEvents 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.py` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/client.pyi` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.py` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,15 @@
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
@@ -251,26 +252,28 @@
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

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/literals.pyi` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
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
@@ -249,26 +250,28 @@
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

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents/type_defs.py` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotevents service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowTypeDef
+    from mypy_boto3_iotevents.type_defs import AcknowledgeFlowOutputTypeDef
 
-    data: AcknowledgeFlowTypeDef = {...}
+    data: AcknowledgeFlowOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -28,134 +28,228 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AcknowledgeFlowOutputTypeDef",
     "AcknowledgeFlowTypeDef",
+    "ClearTimerActionOutputTypeDef",
+    "ResetTimerActionOutputTypeDef",
+    "SetTimerActionOutputTypeDef",
+    "SetVariableActionOutputTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
+    "InitializationConfigurationOutputTypeDef",
     "InitializationConfigurationTypeDef",
     "AlarmModelSummaryTypeDef",
     "AlarmModelVersionSummaryTypeDef",
+    "SimpleRuleOutputTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
+    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
+    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
     "CreateAlarmModelResponseTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
+    "DetectorDebugOptionOutputTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
+    "PayloadOutputTypeDef",
     "PayloadTypeDef",
+    "EmailContentOutputTypeDef",
     "EmailContentTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
+    "SSOIdentityOutputTypeDef",
     "SSOIdentityTypeDef",
     "ResponseMetadataTypeDef",
     "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAlarmModelResponseTypeDef",
+    "AlarmCapabilitiesOutputTypeDef",
     "AlarmCapabilitiesTypeDef",
     "ListAlarmModelsResponseTypeDef",
     "ListAlarmModelVersionsResponseTypeDef",
+    "AlarmRuleOutputTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
+    "AssetPropertyValueOutputTypeDef",
     "AssetPropertyValueTypeDef",
+    "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
+    "DynamoDBActionOutputTypeDef",
+    "DynamoDBv2ActionOutputTypeDef",
+    "FirehoseActionOutputTypeDef",
+    "IotEventsActionOutputTypeDef",
+    "IotTopicPublishActionOutputTypeDef",
+    "LambdaActionOutputTypeDef",
+    "SNSTopicPublishActionOutputTypeDef",
+    "SqsActionOutputTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
     "IotTopicPublishActionTypeDef",
     "LambdaActionTypeDef",
     "SNSTopicPublishActionTypeDef",
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RecipientDetailOutputTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
+    "IotSiteWiseActionOutputTypeDef",
     "IotSiteWiseActionTypeDef",
-    "CreateInputRequestRequestTypeDef",
     "InputTypeDef",
+    "CreateInputRequestRequestTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
+    "NotificationTargetActionsOutputTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
+    "EmailRecipientsOutputTypeDef",
+    "SMSConfigurationOutputTypeDef",
     "EmailRecipientsTypeDef",
     "SMSConfigurationTypeDef",
+    "ActionOutputTypeDef",
+    "AlarmActionOutputTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
+    "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
+    "EventOutputTypeDef",
+    "TransitionEventOutputTypeDef",
+    "AlarmEventActionsOutputTypeDef",
     "EventTypeDef",
     "TransitionEventTypeDef",
     "AlarmEventActionsTypeDef",
+    "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
+    "OnEnterLifecycleOutputTypeDef",
+    "OnExitLifecycleOutputTypeDef",
+    "OnInputLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
     "OnInputLifecycleTypeDef",
+    "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
+    "StateOutputTypeDef",
     "StateTypeDef",
-    "CreateAlarmModelRequestRequestTypeDef",
     "DescribeAlarmModelResponseTypeDef",
+    "CreateAlarmModelRequestRequestTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
+    "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
-    "CreateDetectorModelRequestRequestTypeDef",
     "DetectorModelTypeDef",
+    "CreateDetectorModelRequestRequestTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
+AcknowledgeFlowOutputTypeDef = TypedDict(
+    "AcknowledgeFlowOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
     {
         "enabled": bool,
     },
 )
 
+ClearTimerActionOutputTypeDef = TypedDict(
+    "ClearTimerActionOutputTypeDef",
+    {
+        "timerName": str,
+    },
+)
+
+ResetTimerActionOutputTypeDef = TypedDict(
+    "ResetTimerActionOutputTypeDef",
+    {
+        "timerName": str,
+    },
+)
+
+_RequiredSetTimerActionOutputTypeDef = TypedDict(
+    "_RequiredSetTimerActionOutputTypeDef",
+    {
+        "timerName": str,
+    },
+)
+_OptionalSetTimerActionOutputTypeDef = TypedDict(
+    "_OptionalSetTimerActionOutputTypeDef",
+    {
+        "seconds": int,
+        "durationExpression": str,
+    },
+    total=False,
+)
+
+class SetTimerActionOutputTypeDef(
+    _RequiredSetTimerActionOutputTypeDef, _OptionalSetTimerActionOutputTypeDef
+):
+    pass
+
+SetVariableActionOutputTypeDef = TypedDict(
+    "SetVariableActionOutputTypeDef",
+    {
+        "variableName": str,
+        "value": str,
+    },
+)
+
 ClearTimerActionTypeDef = TypedDict(
     "ClearTimerActionTypeDef",
     {
         "timerName": str,
     },
 )
 
@@ -177,27 +271,32 @@
     {
         "seconds": int,
         "durationExpression": str,
     },
     total=False,
 )
 
-
 class SetTimerActionTypeDef(_RequiredSetTimerActionTypeDef, _OptionalSetTimerActionTypeDef):
     pass
 
-
 SetVariableActionTypeDef = TypedDict(
     "SetVariableActionTypeDef",
     {
         "variableName": str,
         "value": str,
     },
 )
 
+InitializationConfigurationOutputTypeDef = TypedDict(
+    "InitializationConfigurationOutputTypeDef",
+    {
+        "disabledOnInitialization": bool,
+    },
+)
+
 InitializationConfigurationTypeDef = TypedDict(
     "InitializationConfigurationTypeDef",
     {
         "disabledOnInitialization": bool,
     },
 )
 
@@ -222,14 +321,23 @@
         "lastUpdateTime": datetime,
         "status": AlarmModelVersionStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
+SimpleRuleOutputTypeDef = TypedDict(
+    "SimpleRuleOutputTypeDef",
+    {
+        "inputProperty": str,
+        "comparisonOperator": ComparisonOperatorType,
+        "threshold": str,
+    },
+)
+
 SimpleRuleTypeDef = TypedDict(
     "SimpleRuleTypeDef",
     {
         "inputProperty": str,
         "comparisonOperator": ComparisonOperatorType,
         "threshold": str,
     },
@@ -239,46 +347,81 @@
     "AnalysisResultLocationTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
+_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_RequiredAssetPropertyTimestampOutputTypeDef",
+    {
+        "timeInSeconds": str,
+    },
+)
+_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
+    "_OptionalAssetPropertyTimestampOutputTypeDef",
+    {
+        "offsetInNanos": str,
+    },
+    total=False,
+)
+
+class AssetPropertyTimestampOutputTypeDef(
+    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
+):
+    pass
+
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
     "_OptionalAssetPropertyTimestampTypeDef",
     {
         "offsetInNanos": str,
     },
     total=False,
 )
 
-
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
+AssetPropertyVariantOutputTypeDef = TypedDict(
+    "AssetPropertyVariantOutputTypeDef",
+    {
+        "stringValue": str,
+        "integerValue": str,
+        "doubleValue": str,
+        "booleanValue": str,
+    },
+    total=False,
+)
 
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
     },
     total=False,
 )
 
+AttributeOutputTypeDef = TypedDict(
+    "AttributeOutputTypeDef",
+    {
+        "jsonPath": str,
+    },
+)
+
 AttributeTypeDef = TypedDict(
     "AttributeTypeDef",
     {
         "jsonPath": str,
     },
 )
 
@@ -333,21 +476,19 @@
     "_OptionalInputConfigurationTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
-
 class InputConfigurationTypeDef(
     _RequiredInputConfigurationTypeDef, _OptionalInputConfigurationTypeDef
 ):
     pass
 
-
 DeleteAlarmModelRequestRequestTypeDef = TypedDict(
     "DeleteAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
     },
 )
 
@@ -375,22 +516,20 @@
     "_OptionalDescribeAlarmModelRequestRequestTypeDef",
     {
         "alarmModelVersion": str,
     },
     total=False,
 )
 
-
 class DescribeAlarmModelRequestRequestTypeDef(
     _RequiredDescribeAlarmModelRequestRequestTypeDef,
     _OptionalDescribeAlarmModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
@@ -412,50 +551,65 @@
     "_OptionalDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelVersion": str,
     },
     total=False,
 )
 
-
 class DescribeDetectorModelRequestRequestTypeDef(
     _RequiredDescribeDetectorModelRequestRequestTypeDef,
     _OptionalDescribeDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "inputName": str,
     },
 )
 
+_RequiredDetectorDebugOptionOutputTypeDef = TypedDict(
+    "_RequiredDetectorDebugOptionOutputTypeDef",
+    {
+        "detectorModelName": str,
+    },
+)
+_OptionalDetectorDebugOptionOutputTypeDef = TypedDict(
+    "_OptionalDetectorDebugOptionOutputTypeDef",
+    {
+        "keyValue": str,
+    },
+    total=False,
+)
+
+class DetectorDebugOptionOutputTypeDef(
+    _RequiredDetectorDebugOptionOutputTypeDef, _OptionalDetectorDebugOptionOutputTypeDef
+):
+    pass
+
 _RequiredDetectorDebugOptionTypeDef = TypedDict(
     "_RequiredDetectorDebugOptionTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDetectorDebugOptionTypeDef = TypedDict(
     "_OptionalDetectorDebugOptionTypeDef",
     {
         "keyValue": str,
     },
     total=False,
 )
 
-
 class DetectorDebugOptionTypeDef(
     _RequiredDetectorDebugOptionTypeDef, _OptionalDetectorDebugOptionTypeDef
 ):
     pass
 
-
 DetectorModelSummaryTypeDef = TypedDict(
     "DetectorModelSummaryTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDescription": str,
         "creationTime": datetime,
     },
@@ -473,22 +627,39 @@
         "lastUpdateTime": datetime,
         "status": DetectorModelVersionStatusType,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
+PayloadOutputTypeDef = TypedDict(
+    "PayloadOutputTypeDef",
+    {
+        "contentExpression": str,
+        "type": PayloadTypeType,
+    },
+)
+
 PayloadTypeDef = TypedDict(
     "PayloadTypeDef",
     {
         "contentExpression": str,
         "type": PayloadTypeType,
     },
 )
 
+EmailContentOutputTypeDef = TypedDict(
+    "EmailContentOutputTypeDef",
+    {
+        "subject": str,
+        "additionalMessage": str,
+    },
+    total=False,
+)
+
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
     {
         "subject": str,
         "additionalMessage": str,
     },
     total=False,
@@ -512,22 +683,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetDetectorModelAnalysisResultsRequestRequestTypeDef(
     _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef,
     _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef,
 ):
     pass
 
-
 IotEventsInputIdentifierTypeDef = TypedDict(
     "IotEventsInputIdentifierTypeDef",
     {
         "inputName": str,
     },
 )
 
@@ -563,22 +732,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAlarmModelVersionsRequestRequestTypeDef(
     _RequiredListAlarmModelVersionsRequestRequestTypeDef,
     _OptionalListAlarmModelVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAlarmModelsRequestRequestTypeDef = TypedDict(
     "ListAlarmModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -595,22 +762,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDetectorModelVersionsRequestRequestTypeDef(
     _RequiredListDetectorModelVersionsRequestRequestTypeDef,
     _OptionalListDetectorModelVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDetectorModelsRequestRequestTypeDef = TypedDict(
     "ListDetectorModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -637,33 +802,58 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
+_RequiredSSOIdentityOutputTypeDef = TypedDict(
+    "_RequiredSSOIdentityOutputTypeDef",
+    {
+        "identityStoreId": str,
+    },
+)
+_OptionalSSOIdentityOutputTypeDef = TypedDict(
+    "_OptionalSSOIdentityOutputTypeDef",
+    {
+        "userId": str,
+    },
+    total=False,
+)
+
+class SSOIdentityOutputTypeDef(
+    _RequiredSSOIdentityOutputTypeDef, _OptionalSSOIdentityOutputTypeDef
+):
+    pass
+
 _RequiredSSOIdentityTypeDef = TypedDict(
     "_RequiredSSOIdentityTypeDef",
     {
         "identityStoreId": str,
     },
 )
 _OptionalSSOIdentityTypeDef = TypedDict(
     "_OptionalSSOIdentityTypeDef",
     {
         "userId": str,
     },
     total=False,
 )
 
-
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -695,14 +885,23 @@
         "alarmModelVersion": str,
         "lastUpdateTime": datetime,
         "status": AlarmModelVersionStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AlarmCapabilitiesOutputTypeDef = TypedDict(
+    "AlarmCapabilitiesOutputTypeDef",
+    {
+        "initializationConfiguration": InitializationConfigurationOutputTypeDef,
+        "acknowledgeFlow": AcknowledgeFlowOutputTypeDef,
+    },
+    total=False,
+)
+
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
@@ -722,14 +921,22 @@
     {
         "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+AlarmRuleOutputTypeDef = TypedDict(
+    "AlarmRuleOutputTypeDef",
+    {
+        "simpleRule": SimpleRuleOutputTypeDef,
+    },
+    total=False,
+)
+
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -741,36 +948,45 @@
         "level": AnalysisResultLevelType,
         "message": str,
         "locations": List[AnalysisResultLocationTypeDef],
     },
     total=False,
 )
 
+AssetPropertyValueOutputTypeDef = TypedDict(
+    "AssetPropertyValueOutputTypeDef",
+    {
+        "value": AssetPropertyVariantOutputTypeDef,
+        "timestamp": AssetPropertyTimestampOutputTypeDef,
+        "quality": str,
+    },
+    total=False,
+)
+
 AssetPropertyValueTypeDef = TypedDict(
     "AssetPropertyValueTypeDef",
     {
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
-InputDefinitionTypeDef = TypedDict(
-    "InputDefinitionTypeDef",
+InputDefinitionOutputTypeDef = TypedDict(
+    "InputDefinitionOutputTypeDef",
     {
-        "attributes": Sequence[AttributeTypeDef],
+        "attributes": List[AttributeOutputTypeDef],
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+InputDefinitionTypeDef = TypedDict(
+    "InputDefinitionTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "attributes": Sequence[AttributeTypeDef],
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -806,35 +1022,54 @@
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredLoggingOptionsOutputTypeDef = TypedDict(
+    "_RequiredLoggingOptionsOutputTypeDef",
+    {
+        "roleArn": str,
+        "level": LoggingLevelType,
+        "enabled": bool,
+    },
+)
+_OptionalLoggingOptionsOutputTypeDef = TypedDict(
+    "_OptionalLoggingOptionsOutputTypeDef",
+    {
+        "detectorDebugOptions": List[DetectorDebugOptionOutputTypeDef],
+    },
+    total=False,
+)
+
+class LoggingOptionsOutputTypeDef(
+    _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
+):
+    pass
+
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsTypeDef = TypedDict(
     "_OptionalLoggingOptionsTypeDef",
     {
-        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
+        "detectorDebugOptions": Sequence[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
-
 class LoggingOptionsTypeDef(_RequiredLoggingOptionsTypeDef, _OptionalLoggingOptionsTypeDef):
     pass
 
-
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -845,14 +1080,174 @@
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDynamoDBActionOutputTypeDef = TypedDict(
+    "_RequiredDynamoDBActionOutputTypeDef",
+    {
+        "hashKeyField": str,
+        "hashKeyValue": str,
+        "tableName": str,
+    },
+)
+_OptionalDynamoDBActionOutputTypeDef = TypedDict(
+    "_OptionalDynamoDBActionOutputTypeDef",
+    {
+        "hashKeyType": str,
+        "rangeKeyType": str,
+        "rangeKeyField": str,
+        "rangeKeyValue": str,
+        "operation": str,
+        "payloadField": str,
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class DynamoDBActionOutputTypeDef(
+    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
+):
+    pass
+
+_RequiredDynamoDBv2ActionOutputTypeDef = TypedDict(
+    "_RequiredDynamoDBv2ActionOutputTypeDef",
+    {
+        "tableName": str,
+    },
+)
+_OptionalDynamoDBv2ActionOutputTypeDef = TypedDict(
+    "_OptionalDynamoDBv2ActionOutputTypeDef",
+    {
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class DynamoDBv2ActionOutputTypeDef(
+    _RequiredDynamoDBv2ActionOutputTypeDef, _OptionalDynamoDBv2ActionOutputTypeDef
+):
+    pass
+
+_RequiredFirehoseActionOutputTypeDef = TypedDict(
+    "_RequiredFirehoseActionOutputTypeDef",
+    {
+        "deliveryStreamName": str,
+    },
+)
+_OptionalFirehoseActionOutputTypeDef = TypedDict(
+    "_OptionalFirehoseActionOutputTypeDef",
+    {
+        "separator": str,
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class FirehoseActionOutputTypeDef(
+    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
+):
+    pass
+
+_RequiredIotEventsActionOutputTypeDef = TypedDict(
+    "_RequiredIotEventsActionOutputTypeDef",
+    {
+        "inputName": str,
+    },
+)
+_OptionalIotEventsActionOutputTypeDef = TypedDict(
+    "_OptionalIotEventsActionOutputTypeDef",
+    {
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class IotEventsActionOutputTypeDef(
+    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
+):
+    pass
+
+_RequiredIotTopicPublishActionOutputTypeDef = TypedDict(
+    "_RequiredIotTopicPublishActionOutputTypeDef",
+    {
+        "mqttTopic": str,
+    },
+)
+_OptionalIotTopicPublishActionOutputTypeDef = TypedDict(
+    "_OptionalIotTopicPublishActionOutputTypeDef",
+    {
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class IotTopicPublishActionOutputTypeDef(
+    _RequiredIotTopicPublishActionOutputTypeDef, _OptionalIotTopicPublishActionOutputTypeDef
+):
+    pass
+
+_RequiredLambdaActionOutputTypeDef = TypedDict(
+    "_RequiredLambdaActionOutputTypeDef",
+    {
+        "functionArn": str,
+    },
+)
+_OptionalLambdaActionOutputTypeDef = TypedDict(
+    "_OptionalLambdaActionOutputTypeDef",
+    {
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class LambdaActionOutputTypeDef(
+    _RequiredLambdaActionOutputTypeDef, _OptionalLambdaActionOutputTypeDef
+):
+    pass
+
+_RequiredSNSTopicPublishActionOutputTypeDef = TypedDict(
+    "_RequiredSNSTopicPublishActionOutputTypeDef",
+    {
+        "targetArn": str,
+    },
+)
+_OptionalSNSTopicPublishActionOutputTypeDef = TypedDict(
+    "_OptionalSNSTopicPublishActionOutputTypeDef",
+    {
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class SNSTopicPublishActionOutputTypeDef(
+    _RequiredSNSTopicPublishActionOutputTypeDef, _OptionalSNSTopicPublishActionOutputTypeDef
+):
+    pass
+
+_RequiredSqsActionOutputTypeDef = TypedDict(
+    "_RequiredSqsActionOutputTypeDef",
+    {
+        "queueUrl": str,
+    },
+)
+_OptionalSqsActionOutputTypeDef = TypedDict(
+    "_OptionalSqsActionOutputTypeDef",
+    {
+        "useBase64": bool,
+        "payload": PayloadOutputTypeDef,
+    },
+    total=False,
+)
+
+class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
+    pass
+
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
         "hashKeyValue": str,
         "tableName": str,
     },
@@ -867,38 +1262,34 @@
         "operation": str,
         "payloadField": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class DynamoDBActionTypeDef(_RequiredDynamoDBActionTypeDef, _OptionalDynamoDBActionTypeDef):
     pass
 
-
 _RequiredDynamoDBv2ActionTypeDef = TypedDict(
     "_RequiredDynamoDBv2ActionTypeDef",
     {
         "tableName": str,
     },
 )
 _OptionalDynamoDBv2ActionTypeDef = TypedDict(
     "_OptionalDynamoDBv2ActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class DynamoDBv2ActionTypeDef(_RequiredDynamoDBv2ActionTypeDef, _OptionalDynamoDBv2ActionTypeDef):
     pass
 
-
 _RequiredFirehoseActionTypeDef = TypedDict(
     "_RequiredFirehoseActionTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 _OptionalFirehoseActionTypeDef = TypedDict(
@@ -906,99 +1297,89 @@
     {
         "separator": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class FirehoseActionTypeDef(_RequiredFirehoseActionTypeDef, _OptionalFirehoseActionTypeDef):
     pass
 
-
 _RequiredIotEventsActionTypeDef = TypedDict(
     "_RequiredIotEventsActionTypeDef",
     {
         "inputName": str,
     },
 )
 _OptionalIotEventsActionTypeDef = TypedDict(
     "_OptionalIotEventsActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
-
 _RequiredIotTopicPublishActionTypeDef = TypedDict(
     "_RequiredIotTopicPublishActionTypeDef",
     {
         "mqttTopic": str,
     },
 )
 _OptionalIotTopicPublishActionTypeDef = TypedDict(
     "_OptionalIotTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class IotTopicPublishActionTypeDef(
     _RequiredIotTopicPublishActionTypeDef, _OptionalIotTopicPublishActionTypeDef
 ):
     pass
 
-
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "functionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
     "_OptionalLambdaActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-
 _RequiredSNSTopicPublishActionTypeDef = TypedDict(
     "_RequiredSNSTopicPublishActionTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalSNSTopicPublishActionTypeDef = TypedDict(
     "_OptionalSNSTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class SNSTopicPublishActionTypeDef(
     _RequiredSNSTopicPublishActionTypeDef, _OptionalSNSTopicPublishActionTypeDef
 ):
     pass
 
-
 _RequiredSqsActionTypeDef = TypedDict(
     "_RequiredSqsActionTypeDef",
     {
         "queueUrl": str,
     },
 )
 _OptionalSqsActionTypeDef = TypedDict(
@@ -1006,19 +1387,17 @@
     {
         "useBase64": bool,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class SqsActionTypeDef(_RequiredSqsActionTypeDef, _OptionalSqsActionTypeDef):
     pass
 
-
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1037,14 +1416,30 @@
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+RecipientDetailOutputTypeDef = TypedDict(
+    "RecipientDetailOutputTypeDef",
+    {
+        "ssoIdentity": SSOIdentityOutputTypeDef,
+    },
+    total=False,
+)
+
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
     },
     total=False,
 )
@@ -1054,26 +1449,47 @@
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+IotSiteWiseActionOutputTypeDef = TypedDict(
+    "IotSiteWiseActionOutputTypeDef",
+    {
+        "entryId": str,
+        "assetId": str,
+        "propertyId": str,
+        "propertyAlias": str,
+        "propertyValue": AssetPropertyValueOutputTypeDef,
+    },
+    total=False,
+)
+
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
         "assetId": str,
         "propertyId": str,
         "propertyAlias": str,
         "propertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
+InputTypeDef = TypedDict(
+    "InputTypeDef",
+    {
+        "inputConfiguration": InputConfigurationTypeDef,
+        "inputDefinition": InputDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1082,30 +1498,19 @@
     {
         "inputDescription": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
-
-InputTypeDef = TypedDict(
-    "InputTypeDef",
-    {
-        "inputConfiguration": InputConfigurationTypeDef,
-        "inputDefinition": InputDefinitionTypeDef,
-    },
-    total=False,
-)
-
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1113,36 +1518,42 @@
     "_OptionalUpdateInputRequestRequestTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
-
 class UpdateInputRequestRequestTypeDef(
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
-
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
+        "loggingOptions": LoggingOptionsOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
+NotificationTargetActionsOutputTypeDef = TypedDict(
+    "NotificationTargetActionsOutputTypeDef",
+    {
+        "lambdaAction": LambdaActionOutputTypeDef,
+    },
+    total=False,
+)
+
 NotificationTargetActionsTypeDef = TypedDict(
     "NotificationTargetActionsTypeDef",
     {
         "lambdaAction": LambdaActionTypeDef,
     },
     total=False,
 )
@@ -1152,14 +1563,42 @@
     {
         "iotEventsInputIdentifier": IotEventsInputIdentifierTypeDef,
         "iotSiteWiseInputIdentifier": IotSiteWiseInputIdentifierTypeDef,
     },
     total=False,
 )
 
+EmailRecipientsOutputTypeDef = TypedDict(
+    "EmailRecipientsOutputTypeDef",
+    {
+        "to": List[RecipientDetailOutputTypeDef],
+    },
+    total=False,
+)
+
+_RequiredSMSConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSMSConfigurationOutputTypeDef",
+    {
+        "recipients": List[RecipientDetailOutputTypeDef],
+    },
+)
+_OptionalSMSConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSMSConfigurationOutputTypeDef",
+    {
+        "senderId": str,
+        "additionalMessage": str,
+    },
+    total=False,
+)
+
+class SMSConfigurationOutputTypeDef(
+    _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
+):
+    pass
+
 EmailRecipientsTypeDef = TypedDict(
     "EmailRecipientsTypeDef",
     {
         "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
@@ -1175,18 +1614,52 @@
     {
         "senderId": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
-
 class SMSConfigurationTypeDef(_RequiredSMSConfigurationTypeDef, _OptionalSMSConfigurationTypeDef):
     pass
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "setVariable": SetVariableActionOutputTypeDef,
+        "sns": SNSTopicPublishActionOutputTypeDef,
+        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
+        "setTimer": SetTimerActionOutputTypeDef,
+        "clearTimer": ClearTimerActionOutputTypeDef,
+        "resetTimer": ResetTimerActionOutputTypeDef,
+        "lambda": LambdaActionOutputTypeDef,
+        "iotEvents": IotEventsActionOutputTypeDef,
+        "sqs": SqsActionOutputTypeDef,
+        "firehose": FirehoseActionOutputTypeDef,
+        "dynamoDB": DynamoDBActionOutputTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+    },
+    total=False,
+)
+
+AlarmActionOutputTypeDef = TypedDict(
+    "AlarmActionOutputTypeDef",
+    {
+        "sns": SNSTopicPublishActionOutputTypeDef,
+        "iotTopicPublish": IotTopicPublishActionOutputTypeDef,
+        "lambda": LambdaActionOutputTypeDef,
+        "iotEvents": IotEventsActionOutputTypeDef,
+        "sqs": SqsActionOutputTypeDef,
+        "firehose": FirehoseActionOutputTypeDef,
+        "dynamoDB": DynamoDBActionOutputTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
+        "iotSiteWise": IotSiteWiseActionOutputTypeDef,
+    },
+    total=False,
+)
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "setVariable": SetVariableActionTypeDef,
         "sns": SNSTopicPublishActionTypeDef,
         "iotTopicPublish": IotTopicPublishActionTypeDef,
@@ -1239,20 +1712,38 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListInputRoutingsRequestRequestTypeDef(
     _RequiredListInputRoutingsRequestRequestTypeDef, _OptionalListInputRoutingsRequestRequestTypeDef
 ):
     pass
 
+_RequiredEmailConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEmailConfigurationOutputTypeDef",
+    {
+        "from": str,
+        "recipients": EmailRecipientsOutputTypeDef,
+    },
+)
+_OptionalEmailConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEmailConfigurationOutputTypeDef",
+    {
+        "content": EmailContentOutputTypeDef,
+    },
+    total=False,
+)
+
+class EmailConfigurationOutputTypeDef(
+    _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
+):
+    pass
 
 _RequiredEmailConfigurationTypeDef = TypedDict(
     "_RequiredEmailConfigurationTypeDef",
     {
         "from": str,
         "recipients": EmailRecipientsTypeDef,
     },
@@ -1261,20 +1752,65 @@
     "_OptionalEmailConfigurationTypeDef",
     {
         "content": EmailContentTypeDef,
     },
     total=False,
 )
 
-
 class EmailConfigurationTypeDef(
     _RequiredEmailConfigurationTypeDef, _OptionalEmailConfigurationTypeDef
 ):
     pass
 
+_RequiredEventOutputTypeDef = TypedDict(
+    "_RequiredEventOutputTypeDef",
+    {
+        "eventName": str,
+    },
+)
+_OptionalEventOutputTypeDef = TypedDict(
+    "_OptionalEventOutputTypeDef",
+    {
+        "condition": str,
+        "actions": List[ActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
+    pass
+
+_RequiredTransitionEventOutputTypeDef = TypedDict(
+    "_RequiredTransitionEventOutputTypeDef",
+    {
+        "eventName": str,
+        "condition": str,
+        "nextState": str,
+    },
+)
+_OptionalTransitionEventOutputTypeDef = TypedDict(
+    "_OptionalTransitionEventOutputTypeDef",
+    {
+        "actions": List[ActionOutputTypeDef],
+    },
+    total=False,
+)
+
+class TransitionEventOutputTypeDef(
+    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
+):
+    pass
+
+AlarmEventActionsOutputTypeDef = TypedDict(
+    "AlarmEventActionsOutputTypeDef",
+    {
+        "alarmActions": List[AlarmActionOutputTypeDef],
+    },
+    total=False,
+)
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventName": str,
     },
 )
@@ -1283,19 +1819,17 @@
     {
         "condition": str,
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
         "nextState": str,
     },
@@ -1304,27 +1838,45 @@
     "_OptionalTransitionEventTypeDef",
     {
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
-
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationActionOutputTypeDef = TypedDict(
+    "_RequiredNotificationActionOutputTypeDef",
+    {
+        "action": NotificationTargetActionsOutputTypeDef,
+    },
+)
+_OptionalNotificationActionOutputTypeDef = TypedDict(
+    "_OptionalNotificationActionOutputTypeDef",
+    {
+        "smsConfigurations": List[SMSConfigurationOutputTypeDef],
+        "emailConfigurations": List[EmailConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+class NotificationActionOutputTypeDef(
+    _RequiredNotificationActionOutputTypeDef, _OptionalNotificationActionOutputTypeDef
+):
+    pass
+
 _RequiredNotificationActionTypeDef = TypedDict(
     "_RequiredNotificationActionTypeDef",
     {
         "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionTypeDef = TypedDict(
@@ -1332,20 +1884,43 @@
     {
         "smsConfigurations": Sequence[SMSConfigurationTypeDef],
         "emailConfigurations": Sequence[EmailConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class NotificationActionTypeDef(
     _RequiredNotificationActionTypeDef, _OptionalNotificationActionTypeDef
 ):
     pass
 
+OnEnterLifecycleOutputTypeDef = TypedDict(
+    "OnEnterLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
+OnExitLifecycleOutputTypeDef = TypedDict(
+    "OnExitLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
+OnInputLifecycleOutputTypeDef = TypedDict(
+    "OnInputLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+        "transitionEvents": List[TransitionEventOutputTypeDef],
+    },
+    total=False,
+)
 
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
@@ -1364,22 +1939,49 @@
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
+AlarmNotificationOutputTypeDef = TypedDict(
+    "AlarmNotificationOutputTypeDef",
+    {
+        "notificationActions": List[NotificationActionOutputTypeDef],
+    },
+    total=False,
+)
+
 AlarmNotificationTypeDef = TypedDict(
     "AlarmNotificationTypeDef",
     {
         "notificationActions": Sequence[NotificationActionTypeDef],
     },
     total=False,
 )
 
+_RequiredStateOutputTypeDef = TypedDict(
+    "_RequiredStateOutputTypeDef",
+    {
+        "stateName": str,
+    },
+)
+_OptionalStateOutputTypeDef = TypedDict(
+    "_OptionalStateOutputTypeDef",
+    {
+        "onInput": OnInputLifecycleOutputTypeDef,
+        "onEnter": OnEnterLifecycleOutputTypeDef,
+        "onExit": OnExitLifecycleOutputTypeDef,
+    },
+    total=False,
+)
+
+class StateOutputTypeDef(_RequiredStateOutputTypeDef, _OptionalStateOutputTypeDef):
+    pass
+
 _RequiredStateTypeDef = TypedDict(
     "_RequiredStateTypeDef",
     {
         "stateName": str,
     },
 )
 _OptionalStateTypeDef = TypedDict(
@@ -1388,18 +1990,38 @@
         "onInput": OnInputLifecycleTypeDef,
         "onEnter": OnEnterLifecycleTypeDef,
         "onExit": OnExitLifecycleTypeDef,
     },
     total=False,
 )
 
-
 class StateTypeDef(_RequiredStateTypeDef, _OptionalStateTypeDef):
     pass
 
+DescribeAlarmModelResponseTypeDef = TypedDict(
+    "DescribeAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "statusMessage": str,
+        "alarmModelName": str,
+        "alarmModelDescription": str,
+        "roleArn": str,
+        "key": str,
+        "severity": int,
+        "alarmRule": AlarmRuleOutputTypeDef,
+        "alarmNotification": AlarmNotificationOutputTypeDef,
+        "alarmEventActions": AlarmEventActionsOutputTypeDef,
+        "alarmCapabilities": AlarmCapabilitiesOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
@@ -1415,43 +2037,19 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateAlarmModelRequestRequestTypeDef(
     _RequiredCreateAlarmModelRequestRequestTypeDef, _OptionalCreateAlarmModelRequestRequestTypeDef
 ):
     pass
 
-
-DescribeAlarmModelResponseTypeDef = TypedDict(
-    "DescribeAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "statusMessage": str,
-        "alarmModelName": str,
-        "alarmModelDescription": str,
-        "roleArn": str,
-        "key": str,
-        "severity": int,
-        "alarmRule": AlarmRuleTypeDef,
-        "alarmNotification": AlarmNotificationTypeDef,
-        "alarmEventActions": AlarmEventActionsTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1464,29 +2062,44 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAlarmModelRequestRequestTypeDef(
     _RequiredUpdateAlarmModelRequestRequestTypeDef, _OptionalUpdateAlarmModelRequestRequestTypeDef
 ):
     pass
 
+DetectorModelDefinitionOutputTypeDef = TypedDict(
+    "DetectorModelDefinitionOutputTypeDef",
+    {
+        "states": List[StateOutputTypeDef],
+        "initialStateName": str,
+    },
+)
 
 DetectorModelDefinitionTypeDef = TypedDict(
     "DetectorModelDefinitionTypeDef",
     {
         "states": Sequence[StateTypeDef],
         "initialStateName": str,
     },
 )
 
+DetectorModelTypeDef = TypedDict(
+    "DetectorModelTypeDef",
+    {
+        "detectorModelDefinition": DetectorModelDefinitionOutputTypeDef,
+        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
         "roleArn": str,
     },
@@ -1498,31 +2111,20 @@
         "key": str,
         "tags": Sequence[TagTypeDef],
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-
-DetectorModelTypeDef = TypedDict(
-    "DetectorModelTypeDef",
-    {
-        "detectorModelDefinition": DetectorModelDefinitionTypeDef,
-        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-    },
-    total=False,
-)
-
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
 
@@ -1539,22 +2141,20 @@
     {
         "detectorModelDescription": str,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-
 class UpdateDetectorModelRequestRequestTypeDef(
     _RequiredUpdateDetectorModelRequestRequestTypeDef,
     _OptionalUpdateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iotevents-1.28.0/mypy_boto3_iotevents.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-1.28.12/mypy_boto3_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-1.28.0/setup.py` & `mypy-boto3-iotevents-1.28.12/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEvents 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.IoTEvents 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

