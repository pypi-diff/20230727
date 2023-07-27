# Comparing `tmp/mypy-boto3-connectcampaigns-1.28.0.tar.gz` & `tmp/mypy-boto3-connectcampaigns-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.0.tar", last modified: Thu Jul  6 20:59:19 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
```

## Comparing `mypy-boto3-connectcampaigns-1.28.0.tar` & `mypy-boto3-connectcampaigns-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.574267 mypy-boto3-connectcampaigns-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-06 20:59:19.570267 mypy-boto3-connectcampaigns-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.566267 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-06 20:37:08.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-06 20:37:08.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:19.570267 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:59:19.000000 mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:19.574267 mypy-boto3-connectcampaigns-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:37:07.000000 mypy-boto3-connectcampaigns-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.520542 mypy-boto3-connectcampaigns-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.520542 mypy-boto3-connectcampaigns-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/setup.py
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/LICENSE` & `mypy-boto3-connectcampaigns-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,26 +327,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
+    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
+    PredictiveDialerConfigOutputTypeDef,
+    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
     GetCampaignStateResponseTypeDef,
@@ -361,19 +365,21 @@
     ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
+    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     ListCampaignsResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
+    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -383,15 +389,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/README.md` & `mypy-boto3-connectcampaigns-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,26 +295,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
+    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
+    PredictiveDialerConfigOutputTypeDef,
+    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
     GetCampaignStateResponseTypeDef,
@@ -329,19 +333,21 @@
     ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
+    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     ListCampaignsResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
+    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -351,15 +357,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__init__.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__init__.pyi` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/__main__.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCampaignService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ConnectCampaignService 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/client.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/client.pyi` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/literals.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.pyi`

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
     "CampaignStateType",
     "EncryptionTypeType",
     "FailureCodeType",
     "GetCampaignStateBatchFailureCodeType",
     "InstanceIdFilterOperatorType",
     "InstanceOnboardingJobFailureCodeType",
@@ -31,15 +30,14 @@
     "ConnectCampaignServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CampaignStateType = Literal["Failed", "Initialized", "Paused", "Running", "Stopped"]
 EncryptionTypeType = Literal["KMS"]
 FailureCodeType = Literal["InvalidInput", "RequestThrottled", "UnknownError"]
 GetCampaignStateBatchFailureCodeType = Literal["ResourceNotFound", "UnknownError"]
 InstanceIdFilterOperatorType = Literal["Eq"]
 InstanceOnboardingJobFailureCodeType = Literal[
     "EVENT_BRIDGE_ACCESS_DENIED",
@@ -167,14 +165,15 @@
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
@@ -253,26 +252,28 @@
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

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/literals.pyi` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.py`

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
     "CampaignStateType",
     "EncryptionTypeType",
     "FailureCodeType",
     "GetCampaignStateBatchFailureCodeType",
     "InstanceIdFilterOperatorType",
     "InstanceOnboardingJobFailureCodeType",
@@ -30,14 +31,15 @@
     "ConnectCampaignServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 CampaignStateType = Literal["Failed", "Initialized", "Paused", "Running", "Stopped"]
 EncryptionTypeType = Literal["KMS"]
 FailureCodeType = Literal["InvalidInput", "RequestThrottled", "UnknownError"]
 GetCampaignStateBatchFailureCodeType = Literal["ResourceNotFound", "UnknownError"]
 InstanceIdFilterOperatorType = Literal["Eq"]
 InstanceOnboardingJobFailureCodeType = Literal[
     "EVENT_BRIDGE_ACCESS_DENIED",
@@ -165,14 +167,15 @@
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
@@ -251,26 +254,28 @@
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

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/paginator.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/paginator.pyi` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/type_defs.py` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connectcampaigns service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
+    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigOutputTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -28,28 +28,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AnswerMachineDetectionConfigOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
+    "PredictiveDialerConfigOutputTypeDef",
+    "ProgressiveDialerConfigOutputTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
     "GetCampaignStateResponseTypeDef",
@@ -64,19 +67,21 @@
     "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
+    "OutboundCallConfigOutputTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
     "ListCampaignsResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
+    "DialerConfigOutputTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
@@ -85,14 +90,21 @@
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
+AnswerMachineDetectionConfigOutputTypeDef = TypedDict(
+    "AnswerMachineDetectionConfigOutputTypeDef",
+    {
+        "enableAnswerMachineDetection": bool,
+    },
+)
+
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
     },
 )
 
@@ -158,14 +170,28 @@
         "attributes": Mapping[str, str],
         "clientToken": str,
         "expirationTime": Union[datetime, str],
         "phoneNumber": str,
     },
 )
 
+PredictiveDialerConfigOutputTypeDef = TypedDict(
+    "PredictiveDialerConfigOutputTypeDef",
+    {
+        "bandwidthAllocation": float,
+    },
+)
+
+ProgressiveDialerConfigOutputTypeDef = TypedDict(
+    "ProgressiveDialerConfigOutputTypeDef",
+    {
+        "bandwidthAllocation": float,
+    },
+)
+
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
@@ -179,14 +205,34 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigOutputTypeDef",
+    {
+        "encryptionType": Literal["KMS"],
+        "keyArn": str,
+    },
+    total=False,
+)
+
+class EncryptionConfigOutputTypeDef(
+    _RequiredEncryptionConfigOutputTypeDef, _OptionalEncryptionConfigOutputTypeDef
+):
+    pass
+
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -194,19 +240,17 @@
     {
         "encryptionType": Literal["KMS"],
         "keyArn": str,
     },
     total=False,
 )
 
-
 class EncryptionConfigTypeDef(_RequiredEncryptionConfigTypeDef, _OptionalEncryptionConfigTypeDef):
     pass
 
-
 FailedCampaignStateResponseTypeDef = TypedDict(
     "FailedCampaignStateResponseTypeDef",
     {
         "campaignId": str,
         "failureCode": GetCampaignStateBatchFailureCodeType,
     },
     total=False,
@@ -278,21 +322,19 @@
     "_OptionalInstanceOnboardingJobStatusTypeDef",
     {
         "failureCode": InstanceOnboardingJobFailureCodeType,
     },
     total=False,
 )
 
-
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -382,14 +424,35 @@
     "UpdateCampaignNameRequestRequestTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
 
+_RequiredOutboundCallConfigOutputTypeDef = TypedDict(
+    "_RequiredOutboundCallConfigOutputTypeDef",
+    {
+        "connectContactFlowId": str,
+        "connectQueueId": str,
+    },
+)
+_OptionalOutboundCallConfigOutputTypeDef = TypedDict(
+    "_OptionalOutboundCallConfigOutputTypeDef",
+    {
+        "answerMachineDetectionConfig": AnswerMachineDetectionConfigOutputTypeDef,
+        "connectSourcePhoneNumber": str,
+    },
+    total=False,
+)
+
+class OutboundCallConfigOutputTypeDef(
+    _RequiredOutboundCallConfigOutputTypeDef, _OptionalOutboundCallConfigOutputTypeDef
+):
+    pass
+
 _RequiredOutboundCallConfigTypeDef = TypedDict(
     "_RequiredOutboundCallConfigTypeDef",
     {
         "connectContactFlowId": str,
         "connectQueueId": str,
     },
 )
@@ -398,21 +461,19 @@
     {
         "answerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "connectSourcePhoneNumber": str,
     },
     total=False,
 )
 
-
 class OutboundCallConfigTypeDef(
     _RequiredOutboundCallConfigTypeDef, _OptionalOutboundCallConfigTypeDef
 ):
     pass
 
-
 _RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateCampaignOutboundCallConfigRequestRequestTypeDef = TypedDict(
@@ -421,22 +482,20 @@
         "answerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "connectContactFlowId": str,
         "connectSourcePhoneNumber": str,
     },
     total=False,
 )
 
-
 class UpdateCampaignOutboundCallConfigRequestRequestTypeDef(
     _RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     _OptionalUpdateCampaignOutboundCallConfigRequestRequestTypeDef,
 ):
     pass
 
-
 CampaignFiltersTypeDef = TypedDict(
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
@@ -454,28 +513,37 @@
     "PutDialRequestBatchRequestRequestTypeDef",
     {
         "dialRequests": Sequence[DialRequestTypeDef],
         "id": str,
     },
 )
 
+DialerConfigOutputTypeDef = TypedDict(
+    "DialerConfigOutputTypeDef",
+    {
+        "predictiveDialerConfig": PredictiveDialerConfigOutputTypeDef,
+        "progressiveDialerConfig": ProgressiveDialerConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
         "progressiveDialerConfig": ProgressiveDialerConfigTypeDef,
     },
     total=False,
 )
 
 InstanceConfigTypeDef = TypedDict(
     "InstanceConfigTypeDef",
     {
         "connectInstanceId": str,
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "serviceLinkedRoleArn": str,
     },
 )
 
 StartInstanceOnboardingJobRequestRequestTypeDef = TypedDict(
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     {
@@ -538,33 +606,31 @@
 )
 
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
-        "dialerConfig": DialerConfigTypeDef,
+        "dialerConfig": DialerConfigOutputTypeDef,
         "id": str,
         "name": str,
-        "outboundCallConfig": OutboundCallConfigTypeDef,
+        "outboundCallConfig": OutboundCallConfigOutputTypeDef,
     },
 )
 _OptionalCampaignTypeDef = TypedDict(
     "_OptionalCampaignTypeDef",
     {
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class CampaignTypeDef(_RequiredCampaignTypeDef, _OptionalCampaignTypeDef):
     pass
 
-
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "name": str,
         "outboundCallConfig": OutboundCallConfigTypeDef,
@@ -574,21 +640,19 @@
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
-
 UpdateCampaignDialerConfigRequestRequestTypeDef = TypedDict(
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     {
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
     },
 )
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns/type_defs.pyi` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connectcampaigns service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
+    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigOutputTypeDef
 
-    data: AnswerMachineDetectionConfigTypeDef = {...}
+    data: AnswerMachineDetectionConfigOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -28,27 +28,32 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AnswerMachineDetectionConfigOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
     "CreateCampaignResponseTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
+    "PredictiveDialerConfigOutputTypeDef",
+    "ProgressiveDialerConfigOutputTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
     "GetCampaignStateResponseTypeDef",
@@ -63,19 +68,21 @@
     "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
+    "OutboundCallConfigOutputTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
     "ListCampaignsResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
+    "DialerConfigOutputTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
@@ -84,14 +91,21 @@
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
+AnswerMachineDetectionConfigOutputTypeDef = TypedDict(
+    "AnswerMachineDetectionConfigOutputTypeDef",
+    {
+        "enableAnswerMachineDetection": bool,
+    },
+)
+
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
     },
 )
 
@@ -157,14 +171,28 @@
         "attributes": Mapping[str, str],
         "clientToken": str,
         "expirationTime": Union[datetime, str],
         "phoneNumber": str,
     },
 )
 
+PredictiveDialerConfigOutputTypeDef = TypedDict(
+    "PredictiveDialerConfigOutputTypeDef",
+    {
+        "bandwidthAllocation": float,
+    },
+)
+
+ProgressiveDialerConfigOutputTypeDef = TypedDict(
+    "ProgressiveDialerConfigOutputTypeDef",
+    {
+        "bandwidthAllocation": float,
+    },
+)
+
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
@@ -178,14 +206,36 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredEncryptionConfigOutputTypeDef = TypedDict(
+    "_RequiredEncryptionConfigOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalEncryptionConfigOutputTypeDef = TypedDict(
+    "_OptionalEncryptionConfigOutputTypeDef",
+    {
+        "encryptionType": Literal["KMS"],
+        "keyArn": str,
+    },
+    total=False,
+)
+
+
+class EncryptionConfigOutputTypeDef(
+    _RequiredEncryptionConfigOutputTypeDef, _OptionalEncryptionConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -193,17 +243,19 @@
     {
         "encryptionType": Literal["KMS"],
         "keyArn": str,
     },
     total=False,
 )
 
+
 class EncryptionConfigTypeDef(_RequiredEncryptionConfigTypeDef, _OptionalEncryptionConfigTypeDef):
     pass
 
+
 FailedCampaignStateResponseTypeDef = TypedDict(
     "FailedCampaignStateResponseTypeDef",
     {
         "campaignId": str,
         "failureCode": GetCampaignStateBatchFailureCodeType,
     },
     total=False,
@@ -275,19 +327,21 @@
     "_OptionalInstanceOnboardingJobStatusTypeDef",
     {
         "failureCode": InstanceOnboardingJobFailureCodeType,
     },
     total=False,
 )
 
+
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -377,14 +431,37 @@
     "UpdateCampaignNameRequestRequestTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
 
+_RequiredOutboundCallConfigOutputTypeDef = TypedDict(
+    "_RequiredOutboundCallConfigOutputTypeDef",
+    {
+        "connectContactFlowId": str,
+        "connectQueueId": str,
+    },
+)
+_OptionalOutboundCallConfigOutputTypeDef = TypedDict(
+    "_OptionalOutboundCallConfigOutputTypeDef",
+    {
+        "answerMachineDetectionConfig": AnswerMachineDetectionConfigOutputTypeDef,
+        "connectSourcePhoneNumber": str,
+    },
+    total=False,
+)
+
+
+class OutboundCallConfigOutputTypeDef(
+    _RequiredOutboundCallConfigOutputTypeDef, _OptionalOutboundCallConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredOutboundCallConfigTypeDef = TypedDict(
     "_RequiredOutboundCallConfigTypeDef",
     {
         "connectContactFlowId": str,
         "connectQueueId": str,
     },
 )
@@ -393,19 +470,21 @@
     {
         "answerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "connectSourcePhoneNumber": str,
     },
     total=False,
 )
 
+
 class OutboundCallConfigTypeDef(
     _RequiredOutboundCallConfigTypeDef, _OptionalOutboundCallConfigTypeDef
 ):
     pass
 
+
 _RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateCampaignOutboundCallConfigRequestRequestTypeDef = TypedDict(
@@ -414,20 +493,22 @@
         "answerMachineDetectionConfig": AnswerMachineDetectionConfigTypeDef,
         "connectContactFlowId": str,
         "connectSourcePhoneNumber": str,
     },
     total=False,
 )
 
+
 class UpdateCampaignOutboundCallConfigRequestRequestTypeDef(
     _RequiredUpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     _OptionalUpdateCampaignOutboundCallConfigRequestRequestTypeDef,
 ):
     pass
 
+
 CampaignFiltersTypeDef = TypedDict(
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
@@ -445,28 +526,37 @@
     "PutDialRequestBatchRequestRequestTypeDef",
     {
         "dialRequests": Sequence[DialRequestTypeDef],
         "id": str,
     },
 )
 
+DialerConfigOutputTypeDef = TypedDict(
+    "DialerConfigOutputTypeDef",
+    {
+        "predictiveDialerConfig": PredictiveDialerConfigOutputTypeDef,
+        "progressiveDialerConfig": ProgressiveDialerConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
         "progressiveDialerConfig": ProgressiveDialerConfigTypeDef,
     },
     total=False,
 )
 
 InstanceConfigTypeDef = TypedDict(
     "InstanceConfigTypeDef",
     {
         "connectInstanceId": str,
-        "encryptionConfig": EncryptionConfigTypeDef,
+        "encryptionConfig": EncryptionConfigOutputTypeDef,
         "serviceLinkedRoleArn": str,
     },
 )
 
 StartInstanceOnboardingJobRequestRequestTypeDef = TypedDict(
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     {
@@ -529,31 +619,33 @@
 )
 
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
-        "dialerConfig": DialerConfigTypeDef,
+        "dialerConfig": DialerConfigOutputTypeDef,
         "id": str,
         "name": str,
-        "outboundCallConfig": OutboundCallConfigTypeDef,
+        "outboundCallConfig": OutboundCallConfigOutputTypeDef,
     },
 )
 _OptionalCampaignTypeDef = TypedDict(
     "_OptionalCampaignTypeDef",
     {
         "tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class CampaignTypeDef(_RequiredCampaignTypeDef, _OptionalCampaignTypeDef):
     pass
 
+
 _RequiredCreateCampaignRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCampaignRequestRequestTypeDef",
     {
         "connectInstanceId": str,
         "dialerConfig": DialerConfigTypeDef,
         "name": str,
         "outboundCallConfig": OutboundCallConfigTypeDef,
@@ -563,19 +655,21 @@
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCampaignRequestRequestTypeDef(
     _RequiredCreateCampaignRequestRequestTypeDef, _OptionalCreateCampaignRequestRequestTypeDef
 ):
     pass
 
+
 UpdateCampaignDialerConfigRequestRequestTypeDef = TypedDict(
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     {
         "dialerConfig": DialerConfigTypeDef,
         "id": str,
     },
 )
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.0
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-connectcampaigns"></a>
 
 # mypy-boto3-connectcampaigns
 
 [![PyPI - mypy-boto3-connectcampaigns](https://img.shields.io/pypi/v/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-connectcampaigns?color=blue)](https://pypistats.org/packages/mypy-boto3-connectcampaigns)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,26 +327,30 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
+    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
     CreateCampaignResponseTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
+    PredictiveDialerConfigOutputTypeDef,
+    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
     EmptyResponseMetadataTypeDef,
+    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
     GetCampaignStateResponseTypeDef,
@@ -361,19 +365,21 @@
     ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
+    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
     ListCampaignsResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
+    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -383,15 +389,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.0/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt` & `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.0/setup.py` & `mypy-boto3-connectcampaigns-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcampaigns",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCampaignService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

