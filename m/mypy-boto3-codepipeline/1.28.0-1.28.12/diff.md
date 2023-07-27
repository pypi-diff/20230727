# Comparing `tmp/mypy-boto3-codepipeline-1.28.0.tar.gz` & `tmp/mypy-boto3-codepipeline-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codepipeline-1.28.0.tar", last modified: Thu Jul  6 20:59:15 2023, max compression
+gzip compressed data, was "mypy-boto3-codepipeline-1.28.12.tar", last modified: Thu Jul 27 05:34:29 2023, max compression
```

## Comparing `mypy-boto3-codepipeline-1.28.0.tar` & `mypy-boto3-codepipeline-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.754258 mypy-boto3-codepipeline-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-06 20:59:15.754258 mypy-boto3-codepipeline-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17645 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.754258 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-06 20:36:11.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-07-06 20:36:11.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46243 2023-07-06 20:36:12.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46182 2023-07-06 20:36:11.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:15.754258 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:15.000000 mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:15.754258 mypy-boto3-codepipeline-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:36:10.000000 mypy-boto3-codepipeline-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18628 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32307 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32255 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10845 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56295 2023-07-27 05:19:13.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56216 2023-07-27 05:19:12.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20135 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:29.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:28.000000 mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:29.160550 mypy-boto3-codepipeline-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:11.000000 mypy-boto3-codepipeline-1.28.12/setup.py
```

### Comparing `mypy-boto3-codepipeline-1.28.0/LICENSE` & `mypy-boto3-codepipeline-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/PKG-INFO` & `mypy-boto3-codepipeline-1.28.12/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codepipeline
-Version: 1.28.0
-Summary: Type annotations for boto3.CodePipeline 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,48 +365,65 @@
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
+    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
+    ActionTypeIdOutputTypeDef,
+    InputArtifactOutputTypeDef,
+    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
+    ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
+    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
+    ActionTypeIdentifierOutputTypeDef,
+    ActionTypePermissionsOutputTypeDef,
+    ActionTypePropertyOutputTypeDef,
+    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypeSettingsOutputTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsTypeDef,
+    ArtifactDetailsOutputTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
+    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
+    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
+    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
+    LambdaExecutorConfigurationOutputTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
@@ -438,67 +455,77 @@
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
     StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
+    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
+    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
+    ActionDeclarationOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
+    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
     UpdateActionTypeInputRequestTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.0/README.md` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-codepipeline
+Version: 1.28.12
+Summary: Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,48 +365,65 @@
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
+    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
+    ActionTypeIdOutputTypeDef,
+    InputArtifactOutputTypeDef,
+    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
+    ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
+    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
+    ActionTypeIdentifierOutputTypeDef,
+    ActionTypePermissionsOutputTypeDef,
+    ActionTypePropertyOutputTypeDef,
+    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypeSettingsOutputTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsTypeDef,
+    ArtifactDetailsOutputTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
+    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
+    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
+    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
+    LambdaExecutorConfigurationOutputTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
@@ -406,67 +455,77 @@
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
     StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
+    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
+    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
+    ActionDeclarationOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
+    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
     UpdateActionTypeInputRequestTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__init__.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__init__.pyi` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/__main__.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodePipeline 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodePipeline 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/client.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/client.pyi` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/literals.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -298,26 +299,28 @@
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

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/literals.pyi` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/literals.pyi`

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

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/paginator.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/paginator.pyi` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/type_defs.py` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,48 +43,65 @@
 
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
     "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     "AcknowledgeThirdPartyJobOutputTypeDef",
+    "ActionConfigurationPropertyOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
+    "ActionTypeIdOutputTypeDef",
+    "InputArtifactOutputTypeDef",
+    "OutputArtifactOutputTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
+    "ActionRevisionOutputTypeDef",
     "ActionRevisionTypeDef",
+    "ActionTypeArtifactDetailsOutputTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
+    "ActionTypeIdentifierOutputTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
+    "ActionTypePropertyOutputTypeDef",
+    "ActionTypeUrlsOutputTypeDef",
     "ActionTypeIdentifierTypeDef",
     "ActionTypePermissionsTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypeSettingsOutputTypeDef",
     "ActionTypeSettingsTypeDef",
-    "ArtifactDetailsTypeDef",
+    "ArtifactDetailsOutputTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
+    "ArtifactDetailsTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "EncryptionKeyTypeDef",
+    "BlockerDeclarationOutputTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
+    "LambdaExecutorConfigurationOutputTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
@@ -116,67 +133,77 @@
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "WebhookAuthConfigurationOutputTypeDef",
     "WebhookAuthConfigurationTypeDef",
+    "WebhookFilterRuleOutputTypeDef",
     "WebhookFilterRuleTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
+    "ArtifactStoreOutputTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
@@ -223,14 +250,41 @@
     "AcknowledgeThirdPartyJobOutputTypeDef",
     {
         "status": JobStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredActionConfigurationPropertyOutputTypeDef = TypedDict(
+    "_RequiredActionConfigurationPropertyOutputTypeDef",
+    {
+        "name": str,
+        "required": bool,
+        "key": bool,
+        "secret": bool,
+    },
+)
+_OptionalActionConfigurationPropertyOutputTypeDef = TypedDict(
+    "_OptionalActionConfigurationPropertyOutputTypeDef",
+    {
+        "queryable": bool,
+        "description": str,
+        "type": ActionConfigurationPropertyTypeType,
+    },
+    total=False,
+)
+
+
+class ActionConfigurationPropertyOutputTypeDef(
+    _RequiredActionConfigurationPropertyOutputTypeDef,
+    _OptionalActionConfigurationPropertyOutputTypeDef,
+):
+    pass
+
+
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -266,14 +320,38 @@
     {
         "name": str,
         "actionExecutionId": str,
     },
     total=False,
 )
 
+ActionTypeIdOutputTypeDef = TypedDict(
+    "ActionTypeIdOutputTypeDef",
+    {
+        "category": ActionCategoryType,
+        "owner": ActionOwnerType,
+        "provider": str,
+        "version": str,
+    },
+)
+
+InputArtifactOutputTypeDef = TypedDict(
+    "InputArtifactOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
+OutputArtifactOutputTypeDef = TypedDict(
+    "OutputArtifactOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ActionTypeIdTypeDef = TypedDict(
     "ActionTypeIdTypeDef",
     {
         "category": ActionCategoryType,
         "owner": ActionOwnerType,
         "provider": str,
         "version": str,
@@ -317,45 +395,115 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
+    {
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": datetime,
+    },
+)
+
 ActionRevisionTypeDef = TypedDict(
     "ActionRevisionTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
-        "created": datetime,
+        "created": Union[datetime, str],
+    },
+)
+
+ActionTypeArtifactDetailsOutputTypeDef = TypedDict(
+    "ActionTypeArtifactDetailsOutputTypeDef",
+    {
+        "minimumCount": int,
+        "maximumCount": int,
     },
 )
 
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
+ActionTypeIdentifierOutputTypeDef = TypedDict(
+    "ActionTypeIdentifierOutputTypeDef",
+    {
+        "category": ActionCategoryType,
+        "owner": str,
+        "provider": str,
+        "version": str,
+    },
+)
+
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
+    {
+        "allowedAccounts": List[str],
+    },
+)
+
+_RequiredActionTypePropertyOutputTypeDef = TypedDict(
+    "_RequiredActionTypePropertyOutputTypeDef",
+    {
+        "name": str,
+        "optional": bool,
+        "key": bool,
+        "noEcho": bool,
+    },
+)
+_OptionalActionTypePropertyOutputTypeDef = TypedDict(
+    "_OptionalActionTypePropertyOutputTypeDef",
+    {
+        "queryable": bool,
+        "description": str,
+    },
+    total=False,
+)
+
+
+class ActionTypePropertyOutputTypeDef(
+    _RequiredActionTypePropertyOutputTypeDef, _OptionalActionTypePropertyOutputTypeDef
+):
+    pass
+
+
+ActionTypeUrlsOutputTypeDef = TypedDict(
+    "ActionTypeUrlsOutputTypeDef",
+    {
+        "configurationUrl": str,
+        "entityUrlTemplate": str,
+        "executionUrlTemplate": str,
+        "revisionUrlTemplate": str,
+    },
+    total=False,
+)
+
 ActionTypeIdentifierTypeDef = TypedDict(
     "ActionTypeIdentifierTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
 ActionTypePermissionsTypeDef = TypedDict(
     "ActionTypePermissionsTypeDef",
     {
-        "allowedAccounts": List[str],
+        "allowedAccounts": Sequence[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
     {
         "name": str,
@@ -387,27 +535,38 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
+ActionTypeSettingsOutputTypeDef = TypedDict(
+    "ActionTypeSettingsOutputTypeDef",
+    {
+        "thirdPartyConfigurationUrl": str,
+        "entityUrlTemplate": str,
+        "executionUrlTemplate": str,
+        "revisionUrlTemplate": str,
+    },
+    total=False,
+)
+
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ArtifactDetailsTypeDef = TypedDict(
-    "ArtifactDetailsTypeDef",
+ArtifactDetailsOutputTypeDef = TypedDict(
+    "ArtifactDetailsOutputTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
 ApprovalResultTypeDef = TypedDict(
@@ -423,14 +582,22 @@
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
+ArtifactDetailsTypeDef = TypedDict(
+    "ArtifactDetailsTypeDef",
+    {
+        "minimumCount": int,
+        "maximumCount": int,
+    },
+)
+
 S3ArtifactLocationTypeDef = TypedDict(
     "S3ArtifactLocationTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -444,22 +611,38 @@
         "revisionSummary": str,
         "created": datetime,
         "revisionUrl": str,
     },
     total=False,
 )
 
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "id": str,
+        "type": Literal["KMS"],
+    },
+)
+
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "id": str,
         "type": Literal["KMS"],
     },
 )
 
+BlockerDeclarationOutputTypeDef = TypedDict(
+    "BlockerDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "type": Literal["Schedule"],
+    },
+)
+
 BlockerDeclarationTypeDef = TypedDict(
     "BlockerDeclarationTypeDef",
     {
         "name": str,
         "type": Literal["Schedule"],
     },
 )
@@ -468,14 +651,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredCurrentRevisionTypeDef = TypedDict(
     "_RequiredCurrentRevisionTypeDef",
     {
         "revision": str,
         "changeIdentifier": str,
     },
 )
@@ -565,23 +756,39 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
+LambdaExecutorConfigurationOutputTypeDef = TypedDict(
+    "LambdaExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaFunctionArn": str,
+    },
+)
+
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": Sequence[str],
+        "pollingServicePrincipals": Sequence[str],
+    },
+    total=False,
+)
+
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
@@ -1026,23 +1233,53 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WebhookAuthConfigurationOutputTypeDef = TypedDict(
+    "WebhookAuthConfigurationOutputTypeDef",
+    {
+        "AllowedIPRange": str,
+        "SecretToken": str,
+    },
+    total=False,
+)
+
 WebhookAuthConfigurationTypeDef = TypedDict(
     "WebhookAuthConfigurationTypeDef",
     {
         "AllowedIPRange": str,
         "SecretToken": str,
     },
     total=False,
 )
 
+_RequiredWebhookFilterRuleOutputTypeDef = TypedDict(
+    "_RequiredWebhookFilterRuleOutputTypeDef",
+    {
+        "jsonPath": str,
+    },
+)
+_OptionalWebhookFilterRuleOutputTypeDef = TypedDict(
+    "_OptionalWebhookFilterRuleOutputTypeDef",
+    {
+        "matchEquals": str,
+    },
+    total=False,
+)
+
+
+class WebhookFilterRuleOutputTypeDef(
+    _RequiredWebhookFilterRuleOutputTypeDef, _OptionalWebhookFilterRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredWebhookFilterRuleTypeDef = TypedDict(
     "_RequiredWebhookFilterRuleTypeDef",
     {
         "jsonPath": str,
     },
 )
 _OptionalWebhookFilterRuleTypeDef = TypedDict(
@@ -1056,14 +1293,42 @@
 
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
 
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
+    },
+)
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
+    {
+        "runOrder": int,
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactOutputTypeDef],
+        "inputArtifacts": List[InputArtifactOutputTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
+    },
+    total=False,
+)
+
+
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForJobsInputRequestTypeDef = TypedDict(
@@ -1205,24 +1470,24 @@
         "actionRevision": ActionRevisionTypeDef,
     },
 )
 
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
-        "id": ActionTypeIdTypeDef,
-        "inputArtifactDetails": ArtifactDetailsTypeDef,
-        "outputArtifactDetails": ArtifactDetailsTypeDef,
+        "id": ActionTypeIdOutputTypeDef,
+        "inputArtifactDetails": ArtifactDetailsOutputTypeDef,
+        "outputArtifactDetails": ArtifactDetailsOutputTypeDef,
     },
 )
 _OptionalActionTypeTypeDef = TypedDict(
     "_OptionalActionTypeTypeDef",
     {
-        "settings": ActionTypeSettingsTypeDef,
-        "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
+        "settings": ActionTypeSettingsOutputTypeDef,
+        "actionConfigurationProperties": List[ActionConfigurationPropertyOutputTypeDef],
     },
     total=False,
 )
 
 
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
@@ -1266,14 +1531,36 @@
         "status": PipelineExecutionStatusType,
         "statusSummary": str,
         "artifactRevisions": List[ArtifactRevisionTypeDef],
     },
     total=False,
 )
 
+_RequiredArtifactStoreOutputTypeDef = TypedDict(
+    "_RequiredArtifactStoreOutputTypeDef",
+    {
+        "type": Literal["S3"],
+        "location": str,
+    },
+)
+_OptionalArtifactStoreOutputTypeDef = TypedDict(
+    "_OptionalArtifactStoreOutputTypeDef",
+    {
+        "encryptionKey": EncryptionKeyOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ArtifactStoreOutputTypeDef(
+    _RequiredArtifactStoreOutputTypeDef, _OptionalArtifactStoreOutputTypeDef
+):
+    pass
+
+
 _RequiredArtifactStoreTypeDef = TypedDict(
     "_RequiredArtifactStoreTypeDef",
     {
         "type": Literal["S3"],
         "location": str,
     },
 )
@@ -1314,31 +1601,31 @@
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
@@ -1380,14 +1667,23 @@
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
 
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationOutputTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1449,26 +1745,60 @@
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleOutputTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationOutputTypeDef,
+    },
+)
+
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
+_RequiredStageDeclarationOutputTypeDef = TypedDict(
+    "_RequiredStageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+    },
+)
+_OptionalStageDeclarationOutputTypeDef = TypedDict(
+    "_OptionalStageDeclarationOutputTypeDef",
+    {
+        "blockers": List[BlockerDeclarationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class StageDeclarationOutputTypeDef(
+    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1485,27 +1815,27 @@
     pass
 
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionTypeDef,
+        "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
@@ -1514,15 +1844,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "configuration": Dict[str, str],
         "resolvedConfiguration": Dict[str, str],
         "roleArn": str,
         "region": str,
         "inputArtifacts": List[ArtifactDetailTypeDef],
         "namespace": str,
     },
@@ -1553,14 +1883,37 @@
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
+    "_RequiredActionTypeExecutorOutputTypeDef",
+    {
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+    },
+)
+_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
+    "_OptionalActionTypeExecutorOutputTypeDef",
+    {
+        "policyStatementsTemplate": str,
+        "jobTimeout": int,
+    },
+    total=False,
+)
+
+
+class ActionTypeExecutorOutputTypeDef(
+    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+):
+    pass
+
+
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1588,26 +1941,26 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
         "errorCode": str,
         "lastTriggered": datetime,
         "arn": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
@@ -1630,14 +1983,39 @@
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
 
+_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
+    "_RequiredPipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+    },
+)
+_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
+    "_OptionalPipelineDeclarationOutputTypeDef",
+    {
+        "artifactStore": ArtifactStoreOutputTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreOutputTypeDef],
+        "version": int,
+    },
+    total=False,
+)
+
+
+class PipelineDeclarationOutputTypeDef(
+    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1687,56 +2065,83 @@
     },
     total=False,
 )
 
 JobDataTypeDef = TypedDict(
     "JobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyTypeDef,
+        "encryptionKey": EncryptionKeyOutputTypeDef,
     },
     total=False,
 )
 
 ThirdPartyJobDataTypeDef = TypedDict(
     "ThirdPartyJobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyTypeDef,
+        "encryptionKey": EncryptionKeyOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierOutputTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+    },
+)
+_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionTypeDeclarationOutputTypeDef",
+    {
+        "description": str,
+        "permissions": ActionTypePermissionsOutputTypeDef,
+        "properties": List[ActionTypePropertyOutputTypeDef],
+        "urls": ActionTypeUrlsOutputTypeDef,
     },
     total=False,
 )
 
+
+class ActionTypeDeclarationOutputTypeDef(
+    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
+        "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 
 class ActionTypeDeclarationTypeDef(
@@ -1758,14 +2163,40 @@
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 _OptionalCreatePipelineInputRequestTypeDef = TypedDict(
@@ -1779,47 +2210,21 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
@@ -1867,15 +2272,15 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
+        "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline/type_defs.pyi` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -42,48 +42,65 @@
 
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
     "AcknowledgeJobOutputTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     "AcknowledgeThirdPartyJobOutputTypeDef",
+    "ActionConfigurationPropertyOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
+    "ActionTypeIdOutputTypeDef",
+    "InputArtifactOutputTypeDef",
+    "OutputArtifactOutputTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
+    "ActionRevisionOutputTypeDef",
     "ActionRevisionTypeDef",
+    "ActionTypeArtifactDetailsOutputTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
+    "ActionTypeIdentifierOutputTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
+    "ActionTypePropertyOutputTypeDef",
+    "ActionTypeUrlsOutputTypeDef",
     "ActionTypeIdentifierTypeDef",
     "ActionTypePermissionsTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypeSettingsOutputTypeDef",
     "ActionTypeSettingsTypeDef",
-    "ArtifactDetailsTypeDef",
+    "ArtifactDetailsOutputTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
+    "ArtifactDetailsTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
+    "EncryptionKeyOutputTypeDef",
     "EncryptionKeyTypeDef",
+    "BlockerDeclarationOutputTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
+    "TagOutputTypeDef",
     "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
+    "LambdaExecutorConfigurationOutputTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
     "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
@@ -115,67 +132,77 @@
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "WebhookAuthConfigurationOutputTypeDef",
     "WebhookAuthConfigurationTypeDef",
+    "WebhookFilterRuleOutputTypeDef",
     "WebhookFilterRuleTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
     "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
+    "ArtifactStoreOutputTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "PutJobSuccessResultInputRequestTypeDef",
     "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
@@ -222,14 +249,39 @@
     "AcknowledgeThirdPartyJobOutputTypeDef",
     {
         "status": JobStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredActionConfigurationPropertyOutputTypeDef = TypedDict(
+    "_RequiredActionConfigurationPropertyOutputTypeDef",
+    {
+        "name": str,
+        "required": bool,
+        "key": bool,
+        "secret": bool,
+    },
+)
+_OptionalActionConfigurationPropertyOutputTypeDef = TypedDict(
+    "_OptionalActionConfigurationPropertyOutputTypeDef",
+    {
+        "queryable": bool,
+        "description": str,
+        "type": ActionConfigurationPropertyTypeType,
+    },
+    total=False,
+)
+
+class ActionConfigurationPropertyOutputTypeDef(
+    _RequiredActionConfigurationPropertyOutputTypeDef,
+    _OptionalActionConfigurationPropertyOutputTypeDef,
+):
+    pass
+
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -263,14 +315,38 @@
     {
         "name": str,
         "actionExecutionId": str,
     },
     total=False,
 )
 
+ActionTypeIdOutputTypeDef = TypedDict(
+    "ActionTypeIdOutputTypeDef",
+    {
+        "category": ActionCategoryType,
+        "owner": ActionOwnerType,
+        "provider": str,
+        "version": str,
+    },
+)
+
+InputArtifactOutputTypeDef = TypedDict(
+    "InputArtifactOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
+OutputArtifactOutputTypeDef = TypedDict(
+    "OutputArtifactOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+
 ActionTypeIdTypeDef = TypedDict(
     "ActionTypeIdTypeDef",
     {
         "category": ActionCategoryType,
         "owner": ActionOwnerType,
         "provider": str,
         "version": str,
@@ -314,45 +390,113 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
+    {
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": datetime,
+    },
+)
+
 ActionRevisionTypeDef = TypedDict(
     "ActionRevisionTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
-        "created": datetime,
+        "created": Union[datetime, str],
+    },
+)
+
+ActionTypeArtifactDetailsOutputTypeDef = TypedDict(
+    "ActionTypeArtifactDetailsOutputTypeDef",
+    {
+        "minimumCount": int,
+        "maximumCount": int,
     },
 )
 
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
+ActionTypeIdentifierOutputTypeDef = TypedDict(
+    "ActionTypeIdentifierOutputTypeDef",
+    {
+        "category": ActionCategoryType,
+        "owner": str,
+        "provider": str,
+        "version": str,
+    },
+)
+
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
+    {
+        "allowedAccounts": List[str],
+    },
+)
+
+_RequiredActionTypePropertyOutputTypeDef = TypedDict(
+    "_RequiredActionTypePropertyOutputTypeDef",
+    {
+        "name": str,
+        "optional": bool,
+        "key": bool,
+        "noEcho": bool,
+    },
+)
+_OptionalActionTypePropertyOutputTypeDef = TypedDict(
+    "_OptionalActionTypePropertyOutputTypeDef",
+    {
+        "queryable": bool,
+        "description": str,
+    },
+    total=False,
+)
+
+class ActionTypePropertyOutputTypeDef(
+    _RequiredActionTypePropertyOutputTypeDef, _OptionalActionTypePropertyOutputTypeDef
+):
+    pass
+
+ActionTypeUrlsOutputTypeDef = TypedDict(
+    "ActionTypeUrlsOutputTypeDef",
+    {
+        "configurationUrl": str,
+        "entityUrlTemplate": str,
+        "executionUrlTemplate": str,
+        "revisionUrlTemplate": str,
+    },
+    total=False,
+)
+
 ActionTypeIdentifierTypeDef = TypedDict(
     "ActionTypeIdentifierTypeDef",
     {
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
 ActionTypePermissionsTypeDef = TypedDict(
     "ActionTypePermissionsTypeDef",
     {
-        "allowedAccounts": List[str],
+        "allowedAccounts": Sequence[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
     {
         "name": str,
@@ -382,27 +526,38 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
+ActionTypeSettingsOutputTypeDef = TypedDict(
+    "ActionTypeSettingsOutputTypeDef",
+    {
+        "thirdPartyConfigurationUrl": str,
+        "entityUrlTemplate": str,
+        "executionUrlTemplate": str,
+        "revisionUrlTemplate": str,
+    },
+    total=False,
+)
+
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ArtifactDetailsTypeDef = TypedDict(
-    "ArtifactDetailsTypeDef",
+ArtifactDetailsOutputTypeDef = TypedDict(
+    "ArtifactDetailsOutputTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
 
 ApprovalResultTypeDef = TypedDict(
@@ -418,14 +573,22 @@
     {
         "bucket": str,
         "key": str,
     },
     total=False,
 )
 
+ArtifactDetailsTypeDef = TypedDict(
+    "ArtifactDetailsTypeDef",
+    {
+        "minimumCount": int,
+        "maximumCount": int,
+    },
+)
+
 S3ArtifactLocationTypeDef = TypedDict(
     "S3ArtifactLocationTypeDef",
     {
         "bucketName": str,
         "objectKey": str,
     },
 )
@@ -439,22 +602,38 @@
         "revisionSummary": str,
         "created": datetime,
         "revisionUrl": str,
     },
     total=False,
 )
 
+EncryptionKeyOutputTypeDef = TypedDict(
+    "EncryptionKeyOutputTypeDef",
+    {
+        "id": str,
+        "type": Literal["KMS"],
+    },
+)
+
 EncryptionKeyTypeDef = TypedDict(
     "EncryptionKeyTypeDef",
     {
         "id": str,
         "type": Literal["KMS"],
     },
 )
 
+BlockerDeclarationOutputTypeDef = TypedDict(
+    "BlockerDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "type": Literal["Schedule"],
+    },
+)
+
 BlockerDeclarationTypeDef = TypedDict(
     "BlockerDeclarationTypeDef",
     {
         "name": str,
         "type": Literal["Schedule"],
     },
 )
@@ -463,14 +642,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredCurrentRevisionTypeDef = TypedDict(
     "_RequiredCurrentRevisionTypeDef",
     {
         "revision": str,
         "changeIdentifier": str,
     },
 )
@@ -558,23 +745,39 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
+LambdaExecutorConfigurationOutputTypeDef = TypedDict(
+    "LambdaExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaFunctionArn": str,
+    },
+)
+
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": Sequence[str],
+        "pollingServicePrincipals": Sequence[str],
+    },
+    total=False,
+)
+
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
@@ -1001,23 +1204,51 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+WebhookAuthConfigurationOutputTypeDef = TypedDict(
+    "WebhookAuthConfigurationOutputTypeDef",
+    {
+        "AllowedIPRange": str,
+        "SecretToken": str,
+    },
+    total=False,
+)
+
 WebhookAuthConfigurationTypeDef = TypedDict(
     "WebhookAuthConfigurationTypeDef",
     {
         "AllowedIPRange": str,
         "SecretToken": str,
     },
     total=False,
 )
 
+_RequiredWebhookFilterRuleOutputTypeDef = TypedDict(
+    "_RequiredWebhookFilterRuleOutputTypeDef",
+    {
+        "jsonPath": str,
+    },
+)
+_OptionalWebhookFilterRuleOutputTypeDef = TypedDict(
+    "_OptionalWebhookFilterRuleOutputTypeDef",
+    {
+        "matchEquals": str,
+    },
+    total=False,
+)
+
+class WebhookFilterRuleOutputTypeDef(
+    _RequiredWebhookFilterRuleOutputTypeDef, _OptionalWebhookFilterRuleOutputTypeDef
+):
+    pass
+
 _RequiredWebhookFilterRuleTypeDef = TypedDict(
     "_RequiredWebhookFilterRuleTypeDef",
     {
         "jsonPath": str,
     },
 )
 _OptionalWebhookFilterRuleTypeDef = TypedDict(
@@ -1029,14 +1260,40 @@
 )
 
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
+    },
+)
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
+    {
+        "runOrder": int,
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactOutputTypeDef],
+        "inputArtifacts": List[InputArtifactOutputTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
+    },
+    total=False,
+)
+
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForJobsInputRequestTypeDef = TypedDict(
@@ -1168,24 +1425,24 @@
         "actionRevision": ActionRevisionTypeDef,
     },
 )
 
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
-        "id": ActionTypeIdTypeDef,
-        "inputArtifactDetails": ArtifactDetailsTypeDef,
-        "outputArtifactDetails": ArtifactDetailsTypeDef,
+        "id": ActionTypeIdOutputTypeDef,
+        "inputArtifactDetails": ArtifactDetailsOutputTypeDef,
+        "outputArtifactDetails": ArtifactDetailsOutputTypeDef,
     },
 )
 _OptionalActionTypeTypeDef = TypedDict(
     "_OptionalActionTypeTypeDef",
     {
-        "settings": ActionTypeSettingsTypeDef,
-        "actionConfigurationProperties": List[ActionConfigurationPropertyTypeDef],
+        "settings": ActionTypeSettingsOutputTypeDef,
+        "actionConfigurationProperties": List[ActionConfigurationPropertyOutputTypeDef],
     },
     total=False,
 )
 
 class ActionTypeTypeDef(_RequiredActionTypeTypeDef, _OptionalActionTypeTypeDef):
     pass
 
@@ -1227,14 +1484,34 @@
         "status": PipelineExecutionStatusType,
         "statusSummary": str,
         "artifactRevisions": List[ArtifactRevisionTypeDef],
     },
     total=False,
 )
 
+_RequiredArtifactStoreOutputTypeDef = TypedDict(
+    "_RequiredArtifactStoreOutputTypeDef",
+    {
+        "type": Literal["S3"],
+        "location": str,
+    },
+)
+_OptionalArtifactStoreOutputTypeDef = TypedDict(
+    "_OptionalArtifactStoreOutputTypeDef",
+    {
+        "encryptionKey": EncryptionKeyOutputTypeDef,
+    },
+    total=False,
+)
+
+class ArtifactStoreOutputTypeDef(
+    _RequiredArtifactStoreOutputTypeDef, _OptionalArtifactStoreOutputTypeDef
+):
+    pass
+
 _RequiredArtifactStoreTypeDef = TypedDict(
     "_RequiredArtifactStoreTypeDef",
     {
         "type": Literal["S3"],
         "location": str,
     },
 )
@@ -1271,31 +1548,31 @@
 
 class CreateCustomActionTypeInputRequestTypeDef(
     _RequiredCreateCustomActionTypeInputRequestTypeDef,
     _OptionalCreateCustomActionTypeInputRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
     "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
@@ -1333,14 +1610,23 @@
 
 class PutThirdPartyJobSuccessResultInputRequestTypeDef(
     _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
     _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationOutputTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1402,26 +1688,58 @@
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleOutputTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationOutputTypeDef,
+    },
+)
+
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
+_RequiredStageDeclarationOutputTypeDef = TypedDict(
+    "_RequiredStageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+    },
+)
+_OptionalStageDeclarationOutputTypeDef = TypedDict(
+    "_OptionalStageDeclarationOutputTypeDef",
+    {
+        "blockers": List[BlockerDeclarationOutputTypeDef],
+    },
+    total=False,
+)
+
+class StageDeclarationOutputTypeDef(
+    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1436,27 +1754,27 @@
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionTypeDef,
+        "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
@@ -1465,15 +1783,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "configuration": Dict[str, str],
         "resolvedConfiguration": Dict[str, str],
         "roleArn": str,
         "region": str,
         "inputArtifacts": List[ArtifactDetailTypeDef],
         "namespace": str,
     },
@@ -1504,14 +1822,35 @@
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
+    "_RequiredActionTypeExecutorOutputTypeDef",
+    {
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+    },
+)
+_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
+    "_OptionalActionTypeExecutorOutputTypeDef",
+    {
+        "policyStatementsTemplate": str,
+        "jobTimeout": int,
+    },
+    total=False,
+)
+
+class ActionTypeExecutorOutputTypeDef(
+    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+):
+    pass
+
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1537,26 +1876,26 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
         "errorCode": str,
         "lastTriggered": datetime,
         "arn": str,
-        "tags": List[TagTypeDef],
+        "tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 class ListWebhookItemTypeDef(_RequiredListWebhookItemTypeDef, _OptionalListWebhookItemTypeDef):
     pass
 
@@ -1575,14 +1914,37 @@
 )
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
+_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
+    "_RequiredPipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+    },
+)
+_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
+    "_OptionalPipelineDeclarationOutputTypeDef",
+    {
+        "artifactStore": ArtifactStoreOutputTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreOutputTypeDef],
+        "version": int,
+    },
+    total=False,
+)
+
+class PipelineDeclarationOutputTypeDef(
+    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1630,56 +1992,81 @@
     },
     total=False,
 )
 
 JobDataTypeDef = TypedDict(
     "JobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyTypeDef,
+        "encryptionKey": EncryptionKeyOutputTypeDef,
     },
     total=False,
 )
 
 ThirdPartyJobDataTypeDef = TypedDict(
     "ThirdPartyJobDataTypeDef",
     {
-        "actionTypeId": ActionTypeIdTypeDef,
+        "actionTypeId": ActionTypeIdOutputTypeDef,
         "actionConfiguration": ActionConfigurationTypeDef,
         "pipelineContext": PipelineContextTypeDef,
         "inputArtifacts": List[ArtifactTypeDef],
         "outputArtifacts": List[ArtifactTypeDef],
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
-        "encryptionKey": EncryptionKeyTypeDef,
+        "encryptionKey": EncryptionKeyOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierOutputTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsOutputTypeDef,
+    },
+)
+_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionTypeDeclarationOutputTypeDef",
+    {
+        "description": str,
+        "permissions": ActionTypePermissionsOutputTypeDef,
+        "properties": List[ActionTypePropertyOutputTypeDef],
+        "urls": ActionTypeUrlsOutputTypeDef,
+    },
+    total=False,
+)
+
+class ActionTypeDeclarationOutputTypeDef(
+    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
+        "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
@@ -1699,14 +2086,40 @@
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 _OptionalCreatePipelineInputRequestTypeDef = TypedDict(
@@ -1718,47 +2131,21 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
@@ -1806,15 +2193,15 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
+        "actionType": ActionTypeDeclarationOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/PKG-INFO` & `mypy-boto3-codepipeline-1.28.12/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-codepipeline
-Version: 1.28.0
-Summary: Type annotations for boto3.CodePipeline 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-codepipeline"></a>
 
 # mypy-boto3-codepipeline
 
 [![PyPI - mypy-boto3-codepipeline](https://img.shields.io/pypi/v/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codepipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codepipeline?color=blue)](https://pypistats.org/packages/mypy-boto3-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codepipeline)](https://pepy.tech/project/mypy-boto3-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodePipeline 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
+[boto3.CodePipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [mypy-boto3-codepipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codepipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -365,48 +333,65 @@
 ```python
 from mypy_boto3_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
+    ActionConfigurationPropertyOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
+    ActionTypeIdOutputTypeDef,
+    InputArtifactOutputTypeDef,
+    OutputArtifactOutputTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
+    ActionRevisionOutputTypeDef,
     ActionRevisionTypeDef,
+    ActionTypeArtifactDetailsOutputTypeDef,
     ActionTypeArtifactDetailsTypeDef,
+    ActionTypeIdentifierOutputTypeDef,
+    ActionTypePermissionsOutputTypeDef,
+    ActionTypePropertyOutputTypeDef,
+    ActionTypeUrlsOutputTypeDef,
     ActionTypeIdentifierTypeDef,
     ActionTypePermissionsTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypeSettingsOutputTypeDef,
     ActionTypeSettingsTypeDef,
-    ArtifactDetailsTypeDef,
+    ArtifactDetailsOutputTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
+    ArtifactDetailsTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
+    EncryptionKeyOutputTypeDef,
     EncryptionKeyTypeDef,
+    BlockerDeclarationOutputTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
+    TagOutputTypeDef,
     CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
+    LambdaExecutorConfigurationOutputTypeDef,
     JobWorkerExecutorConfigurationTypeDef,
     LambdaExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
@@ -438,67 +423,77 @@
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
     StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
+    WebhookAuthConfigurationOutputTypeDef,
     WebhookAuthConfigurationTypeDef,
+    WebhookFilterRuleOutputTypeDef,
     WebhookFilterRuleTypeDef,
+    ActionDeclarationOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
     ActionDeclarationTypeDef,
     ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
     PutActionRevisionInputRequestTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
+    ArtifactStoreOutputTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     PutJobSuccessResultInputRequestTypeDef,
     PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
     UpdateActionTypeInputRequestTypeDef,
```

### Comparing `mypy-boto3-codepipeline-1.28.0/mypy_boto3_codepipeline.egg-info/SOURCES.txt` & `mypy-boto3-codepipeline-1.28.12/mypy_boto3_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codepipeline-1.28.0/setup.py` & `mypy-boto3-codepipeline-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codepipeline",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodePipeline 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodePipeline 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

