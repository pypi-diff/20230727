# Comparing `tmp/mypy-boto3-wellarchitected-1.28.0.tar.gz` & `tmp/mypy-boto3-wellarchitected-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wellarchitected-1.28.0.tar", last modified: Thu Jul  6 21:00:51 2023, max compression
+gzip compressed data, was "mypy-boto3-wellarchitected-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-wellarchitected-1.28.0.tar` & `mypy-boto3-wellarchitected-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.114459 mypy-boto3-wellarchitected-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-07-06 21:00:51.114459 mypy-boto3-wellarchitected-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16558 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.114459 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38027 2023-07-06 20:58:00.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37965 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-07-06 20:58:00.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-07-06 20:58:00.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53113 2023-07-06 20:58:01.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53056 2023-07-06 20:58:01.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:51.114459 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 21:00:50.000000 mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:51.114459 mypy-boto3-wellarchitected-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 20:57:59.000000 mypy-boto3-wellarchitected-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.421491 mypy-boto3-wellarchitected-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-27 11:49:49.421491 mypy-boto3-wellarchitected-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16585 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.417491 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38027 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37965 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53350 2023-07-27 11:48:46.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53293 2023-07-27 11:48:45.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.421491 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:49.000000 mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.421491 mypy-boto3-wellarchitected-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-27 11:48:42.000000 mypy-boto3-wellarchitected-1.28.12/setup.py
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/LICENSE` & `mypy-boto3-wellarchitected-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.0/PKG-INFO` & `mypy-boto3-wellarchitected-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.28.0
-Summary: Type annotations for boto3.WellArchitected 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WellArchitected 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,51 +338,42 @@
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -398,85 +389,95 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/README.md` & `mypy-boto3-wellarchitected-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,51 +306,42 @@
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -366,85 +357,95 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/__main__.py` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WellArchitected 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.WellArchitected 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
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

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/client.py` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/client.pyi` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/literals.py` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,15 @@
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
@@ -299,26 +300,28 @@
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

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/literals.pyi` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,15 @@
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
@@ -297,26 +298,28 @@
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

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/type_defs.py` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,51 +64,42 @@
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
-    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "CreateMilestoneOutputTypeDef",
     "ProfileQuestionUpdateTypeDef",
-    "CreateProfileOutputTypeDef",
     "CreateProfileShareInputRequestTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
-    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "DisassociateProfilesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
-    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
     "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
     "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "ImportLensOutputTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -124,85 +115,95 @@
     "ListProfileSharesInputRequestTypeDef",
     "ProfileShareSummaryTypeDef",
     "ListProfilesInputRequestTypeDef",
     "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
-    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
+    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
-    "ListCheckDetailsOutputTypeDef",
-    "ListCheckSummariesOutputTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
+    "CreateLensShareOutputTypeDef",
+    "CreateLensVersionOutputTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareOutputTypeDef",
+    "CreateWorkloadOutputTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportLensOutputTypeDef",
+    "ImportLensOutputTypeDef",
+    "ListCheckDetailsOutputTypeDef",
+    "ListCheckSummariesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -334,19 +335,22 @@
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -365,114 +369,60 @@
 
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
 
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
-    {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProfileQuestionUpdateTypeDef = TypedDict(
     "ProfileQuestionUpdateTypeDef",
     {
         "QuestionId": str,
         "SelectedChoiceIds": Sequence[str],
     },
     total=False,
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProfileShareInputRequestTypeDef = TypedDict(
     "CreateProfileShareInputRequestTypeDef",
     {
         "ProfileArn": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
         "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -533,21 +483,14 @@
     "DisassociateProfilesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ProfileArns": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -561,22 +504,14 @@
 
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
 
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
-    {
-        "LensJSON": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
     },
@@ -787,23 +722,14 @@
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
 
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
-    {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": str,
         "ProfileVersion": str,
     },
     total=False,
@@ -1176,22 +1102,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -1260,25 +1178,14 @@
         "ChoiceId": str,
         "ChoiceTitle": str,
         "ChoiceDescription": str,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
@@ -1410,14 +1317,23 @@
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
 
+WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
+    "WorkloadDiscoveryConfigOutputTypeDef",
+    {
+        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": List[DefinitionTypeType],
+    },
+    total=False,
+)
+
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1429,32 +1345,14 @@
         "QuestionId": str,
         "Risk": RiskType,
         "BestPractices": List[BestPracticeTypeDef],
     },
     total=False,
 )
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
-    {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
-    {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1487,14 +1385,126 @@
 
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
 
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
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
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
+    {
+        "LensArn": str,
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateProfileInputRequestTypeDef = TypedDict(
     "_RequiredCreateProfileInputRequestTypeDef",
     {
         "ProfileName": str,
         "ProfileDescription": str,
         "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
         "ClientRequestToken": str,
@@ -1610,25 +1620,25 @@
     pass
 
 
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensReviewReportOutputTypeDef = TypedDict(
     "GetLensReviewReportOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": str,
@@ -1657,48 +1667,14 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1715,24 +1691,24 @@
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
@@ -1742,52 +1718,52 @@
 )
 
 ListProfileNotificationsOutputTypeDef = TypedDict(
     "ListProfileNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileSharesOutputTypeDef = TypedDict(
     "ListProfileSharesOutputTypeDef",
     {
         "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesOutputTypeDef = TypedDict(
     "ListProfilesOutputTypeDef",
     {
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PillarDifferenceTypeDef = TypedDict(
     "PillarDifferenceTypeDef",
     {
         "PillarId": str,
@@ -1825,25 +1801,59 @@
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
+    total=False,
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
@@ -1870,101 +1880,74 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadsOutputTypeDef = TypedDict(
     "ListWorkloadsOutputTypeDef",
     {
         "WorkloadSummaries": List[WorkloadSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MilestoneSummaryTypeDef = TypedDict(
     "MilestoneSummaryTypeDef",
     {
         "MilestoneNumber": int,
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VersionDifferencesTypeDef = TypedDict(
     "VersionDifferencesTypeDef",
     {
         "PillarDifferences": List[PillarDifferenceTypeDef],
@@ -1996,14 +1979,41 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -2050,97 +2060,97 @@
 
 ListMilestonesOutputTypeDef = TypedDict(
     "ListMilestonesOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileOutputTypeDef = TypedDict(
     "GetProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfileOutputTypeDef = TypedDict(
     "UpdateProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConsolidatedReportMetricTypeDef = TypedDict(
     "ConsolidatedReportMetricTypeDef",
     {
         "MetricType": Literal["WORKLOAD"],
@@ -2157,10 +2167,10 @@
 
 GetConsolidatedReportOutputTypeDef = TypedDict(
     "GetConsolidatedReportOutputTypeDef",
     {
         "Metrics": List[ConsolidatedReportMetricTypeDef],
         "NextToken": str,
         "Base64String": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected/type_defs.pyi` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,51 +63,42 @@
     "AssociateProfilesInputRequestTypeDef",
     "BestPracticeTypeDef",
     "CheckDetailTypeDef",
     "CheckSummaryTypeDef",
     "ChoiceImprovementPlanTypeDef",
     "ChoiceUpdateTypeDef",
     "CreateLensShareInputRequestTypeDef",
-    "CreateLensShareOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLensVersionInputRequestTypeDef",
-    "CreateLensVersionOutputTypeDef",
     "CreateMilestoneInputRequestTypeDef",
-    "CreateMilestoneOutputTypeDef",
     "ProfileQuestionUpdateTypeDef",
-    "CreateProfileOutputTypeDef",
     "CreateProfileShareInputRequestTypeDef",
-    "CreateProfileShareOutputTypeDef",
     "WorkloadDiscoveryConfigTypeDef",
-    "CreateWorkloadOutputTypeDef",
     "CreateWorkloadShareInputRequestTypeDef",
-    "CreateWorkloadShareOutputTypeDef",
     "DeleteLensInputRequestTypeDef",
     "DeleteLensShareInputRequestTypeDef",
     "DeleteProfileInputRequestTypeDef",
     "DeleteProfileShareInputRequestTypeDef",
     "DeleteWorkloadInputRequestTypeDef",
     "DeleteWorkloadShareInputRequestTypeDef",
     "DisassociateLensesInputRequestTypeDef",
     "DisassociateProfilesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportLensInputRequestTypeDef",
-    "ExportLensOutputTypeDef",
     "GetAnswerInputRequestTypeDef",
     "GetConsolidatedReportInputRequestTypeDef",
     "GetLensInputRequestTypeDef",
     "LensTypeDef",
     "GetLensReviewInputRequestTypeDef",
     "GetLensReviewReportInputRequestTypeDef",
     "LensReviewReportTypeDef",
     "GetLensVersionDifferenceInputRequestTypeDef",
     "GetMilestoneInputRequestTypeDef",
     "GetProfileInputRequestTypeDef",
     "GetWorkloadInputRequestTypeDef",
     "ImportLensInputRequestTypeDef",
-    "ImportLensOutputTypeDef",
     "WorkloadProfileTypeDef",
     "PillarReviewSummaryTypeDef",
     "LensShareSummaryTypeDef",
     "LensSummaryTypeDef",
     "LensUpgradeSummaryTypeDef",
     "ListAnswersInputRequestTypeDef",
     "ListCheckDetailsInputRequestTypeDef",
@@ -123,85 +114,95 @@
     "ListProfileSharesInputRequestTypeDef",
     "ProfileShareSummaryTypeDef",
     "ListProfilesInputRequestTypeDef",
     "ProfileSummaryTypeDef",
     "ListShareInvitationsInputRequestTypeDef",
     "ShareInvitationSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListWorkloadSharesInputRequestTypeDef",
     "WorkloadShareSummaryTypeDef",
     "ListWorkloadsInputRequestTypeDef",
     "QuestionDifferenceTypeDef",
     "ProfileChoiceTypeDef",
     "ProfileTemplateChoiceTypeDef",
-    "ResponseMetadataTypeDef",
     "ShareInvitationTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
+    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
-    "ListCheckDetailsOutputTypeDef",
-    "ListCheckSummariesOutputTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
+    "CreateLensShareOutputTypeDef",
+    "CreateLensVersionOutputTypeDef",
+    "CreateMilestoneOutputTypeDef",
+    "CreateProfileOutputTypeDef",
+    "CreateProfileShareOutputTypeDef",
+    "CreateWorkloadOutputTypeDef",
+    "CreateWorkloadShareOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportLensOutputTypeDef",
+    "ImportLensOutputTypeDef",
+    "ListCheckDetailsOutputTypeDef",
+    "ListCheckSummariesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "CreateProfileInputRequestTypeDef",
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
-    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
+    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -331,19 +332,22 @@
     {
         "LensAlias": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateLensShareOutputTypeDef = TypedDict(
-    "CreateLensShareOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLensVersionInputRequestTypeDef = TypedDict(
     "_RequiredCreateLensVersionInputRequestTypeDef",
     {
         "LensAlias": str,
@@ -360,114 +364,60 @@
 )
 
 class CreateLensVersionInputRequestTypeDef(
     _RequiredCreateLensVersionInputRequestTypeDef, _OptionalCreateLensVersionInputRequestTypeDef
 ):
     pass
 
-CreateLensVersionOutputTypeDef = TypedDict(
-    "CreateLensVersionOutputTypeDef",
-    {
-        "LensArn": str,
-        "LensVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMilestoneInputRequestTypeDef = TypedDict(
     "CreateMilestoneInputRequestTypeDef",
     {
         "WorkloadId": str,
         "MilestoneName": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateMilestoneOutputTypeDef = TypedDict(
-    "CreateMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "MilestoneNumber": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ProfileQuestionUpdateTypeDef = TypedDict(
     "ProfileQuestionUpdateTypeDef",
     {
         "QuestionId": str,
         "SelectedChoiceIds": Sequence[str],
     },
     total=False,
 )
 
-CreateProfileOutputTypeDef = TypedDict(
-    "CreateProfileOutputTypeDef",
-    {
-        "ProfileArn": str,
-        "ProfileVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProfileShareInputRequestTypeDef = TypedDict(
     "CreateProfileShareInputRequestTypeDef",
     {
         "ProfileArn": str,
         "SharedWith": str,
         "ClientRequestToken": str,
     },
 )
 
-CreateProfileShareOutputTypeDef = TypedDict(
-    "CreateProfileShareOutputTypeDef",
-    {
-        "ShareId": str,
-        "ProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadDiscoveryConfigTypeDef = TypedDict(
     "WorkloadDiscoveryConfigTypeDef",
     {
         "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
         "WorkloadResourceDefinition": Sequence[DefinitionTypeType],
     },
     total=False,
 )
 
-CreateWorkloadOutputTypeDef = TypedDict(
-    "CreateWorkloadOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWorkloadShareInputRequestTypeDef = TypedDict(
     "CreateWorkloadShareInputRequestTypeDef",
     {
         "WorkloadId": str,
         "SharedWith": str,
         "PermissionType": PermissionTypeType,
         "ClientRequestToken": str,
     },
 )
 
-CreateWorkloadShareOutputTypeDef = TypedDict(
-    "CreateWorkloadShareOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "ShareId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLensInputRequestTypeDef = TypedDict(
     "DeleteLensInputRequestTypeDef",
     {
         "LensAlias": str,
         "ClientRequestToken": str,
         "LensStatus": LensStatusTypeType,
     },
@@ -528,21 +478,14 @@
     "DisassociateProfilesInputRequestTypeDef",
     {
         "WorkloadId": str,
         "ProfileArns": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExportLensInputRequestTypeDef = TypedDict(
     "_RequiredExportLensInputRequestTypeDef",
     {
         "LensAlias": str,
     },
 )
 _OptionalExportLensInputRequestTypeDef = TypedDict(
@@ -554,22 +497,14 @@
 )
 
 class ExportLensInputRequestTypeDef(
     _RequiredExportLensInputRequestTypeDef, _OptionalExportLensInputRequestTypeDef
 ):
     pass
 
-ExportLensOutputTypeDef = TypedDict(
-    "ExportLensOutputTypeDef",
-    {
-        "LensJSON": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetAnswerInputRequestTypeDef = TypedDict(
     "_RequiredGetAnswerInputRequestTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "QuestionId": str,
     },
@@ -764,23 +699,14 @@
 )
 
 class ImportLensInputRequestTypeDef(
     _RequiredImportLensInputRequestTypeDef, _OptionalImportLensInputRequestTypeDef
 ):
     pass
 
-ImportLensOutputTypeDef = TypedDict(
-    "ImportLensOutputTypeDef",
-    {
-        "LensArn": str,
-        "Status": ImportLensStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkloadProfileTypeDef = TypedDict(
     "WorkloadProfileTypeDef",
     {
         "ProfileArn": str,
         "ProfileVersion": str,
     },
     total=False,
@@ -1137,22 +1063,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "WorkloadArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListWorkloadSharesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkloadSharesInputRequestTypeDef",
     {
         "WorkloadId": str,
     },
 )
 _OptionalListWorkloadSharesInputRequestTypeDef = TypedDict(
@@ -1219,25 +1137,14 @@
         "ChoiceId": str,
         "ChoiceTitle": str,
         "ChoiceDescription": str,
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
 ShareInvitationTypeDef = TypedDict(
     "ShareInvitationTypeDef",
     {
         "ShareInvitationId": str,
         "ShareResourceType": ShareResourceTypeType,
         "WorkloadId": str,
         "LensAlias": str,
@@ -1363,14 +1270,23 @@
 
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
+WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
+    "WorkloadDiscoveryConfigOutputTypeDef",
+    {
+        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
+        "WorkloadResourceDefinition": List[DefinitionTypeType],
+    },
+    total=False,
+)
+
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1382,32 +1298,14 @@
         "QuestionId": str,
         "Risk": RiskType,
         "BestPractices": List[BestPracticeTypeDef],
     },
     total=False,
 )
 
-ListCheckDetailsOutputTypeDef = TypedDict(
-    "ListCheckDetailsOutputTypeDef",
-    {
-        "CheckDetails": List[CheckDetailTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCheckSummariesOutputTypeDef = TypedDict(
-    "ListCheckSummariesOutputTypeDef",
-    {
-        "CheckSummaries": List[CheckSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImprovementSummaryTypeDef = TypedDict(
     "ImprovementSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Risk": RiskType,
@@ -1438,14 +1336,126 @@
 )
 
 class UpdateAnswerInputRequestTypeDef(
     _RequiredUpdateAnswerInputRequestTypeDef, _OptionalUpdateAnswerInputRequestTypeDef
 ):
     pass
 
+CreateLensShareOutputTypeDef = TypedDict(
+    "CreateLensShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLensVersionOutputTypeDef = TypedDict(
+    "CreateLensVersionOutputTypeDef",
+    {
+        "LensArn": str,
+        "LensVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMilestoneOutputTypeDef = TypedDict(
+    "CreateMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "MilestoneNumber": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileOutputTypeDef = TypedDict(
+    "CreateProfileOutputTypeDef",
+    {
+        "ProfileArn": str,
+        "ProfileVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProfileShareOutputTypeDef = TypedDict(
+    "CreateProfileShareOutputTypeDef",
+    {
+        "ShareId": str,
+        "ProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadOutputTypeDef = TypedDict(
+    "CreateWorkloadOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkloadShareOutputTypeDef = TypedDict(
+    "CreateWorkloadShareOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "ShareId": str,
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
+ExportLensOutputTypeDef = TypedDict(
+    "ExportLensOutputTypeDef",
+    {
+        "LensJSON": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportLensOutputTypeDef = TypedDict(
+    "ImportLensOutputTypeDef",
+    {
+        "LensArn": str,
+        "Status": ImportLensStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckDetailsOutputTypeDef = TypedDict(
+    "ListCheckDetailsOutputTypeDef",
+    {
+        "CheckDetails": List[CheckDetailTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCheckSummariesOutputTypeDef = TypedDict(
+    "ListCheckSummariesOutputTypeDef",
+    {
+        "CheckSummaries": List[CheckSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateProfileInputRequestTypeDef = TypedDict(
     "_RequiredCreateProfileInputRequestTypeDef",
     {
         "ProfileName": str,
         "ProfileDescription": str,
         "ProfileQuestions": Sequence[ProfileQuestionUpdateTypeDef],
         "ClientRequestToken": str,
@@ -1553,25 +1563,25 @@
 ):
     pass
 
 GetLensOutputTypeDef = TypedDict(
     "GetLensOutputTypeDef",
     {
         "Lens": LensTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensReviewReportOutputTypeDef = TypedDict(
     "GetLensReviewReportOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewReport": LensReviewReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LensReviewSummaryTypeDef = TypedDict(
     "LensReviewSummaryTypeDef",
     {
         "LensAlias": str,
@@ -1600,48 +1610,14 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1658,24 +1634,24 @@
 )
 
 ListLensSharesOutputTypeDef = TypedDict(
     "ListLensSharesOutputTypeDef",
     {
         "LensShareSummaries": List[LensShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensesOutputTypeDef = TypedDict(
     "ListLensesOutputTypeDef",
     {
         "LensSummaries": List[LensSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotificationSummaryTypeDef = TypedDict(
     "NotificationSummaryTypeDef",
     {
         "Type": NotificationTypeType,
@@ -1685,52 +1661,52 @@
 )
 
 ListProfileNotificationsOutputTypeDef = TypedDict(
     "ListProfileNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[ProfileNotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfileSharesOutputTypeDef = TypedDict(
     "ListProfileSharesOutputTypeDef",
     {
         "ProfileShareSummaries": List[ProfileShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilesOutputTypeDef = TypedDict(
     "ListProfilesOutputTypeDef",
     {
         "ProfileSummaries": List[ProfileSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListShareInvitationsOutputTypeDef = TypedDict(
     "ListShareInvitationsOutputTypeDef",
     {
         "ShareInvitationSummaries": List[ShareInvitationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadSharesOutputTypeDef = TypedDict(
     "ListWorkloadSharesOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShareSummaries": List[WorkloadShareSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PillarDifferenceTypeDef = TypedDict(
     "PillarDifferenceTypeDef",
     {
         "PillarId": str,
@@ -1768,25 +1744,59 @@
     total=False,
 )
 
 UpdateShareInvitationOutputTypeDef = TypedDict(
     "UpdateShareInvitationOutputTypeDef",
     {
         "ShareInvitation": ShareInvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWorkloadShareOutputTypeDef = TypedDict(
     "UpdateWorkloadShareOutputTypeDef",
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
     },
+    total=False,
 )
 
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
@@ -1813,101 +1823,74 @@
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "ImprovementSummaries": List[ImprovementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLensReviewsOutputTypeDef = TypedDict(
     "ListLensReviewsOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReviewSummaries": List[LensReviewSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkloadsOutputTypeDef = TypedDict(
     "ListWorkloadsOutputTypeDef",
     {
         "WorkloadSummaries": List[WorkloadSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MilestoneSummaryTypeDef = TypedDict(
     "MilestoneSummaryTypeDef",
     {
         "MilestoneNumber": int,
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLensReviewOutputTypeDef = TypedDict(
     "UpdateLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "LensReview": LensReviewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsOutputTypeDef = TypedDict(
     "ListNotificationsOutputTypeDef",
     {
         "NotificationSummaries": List[NotificationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VersionDifferencesTypeDef = TypedDict(
     "VersionDifferencesTypeDef",
     {
         "PillarDifferences": List[PillarDifferenceTypeDef],
@@ -1939,14 +1922,41 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -1993,97 +2003,97 @@
 
 ListMilestonesOutputTypeDef = TypedDict(
     "ListMilestonesOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
         "LatestLensVersion": str,
         "VersionDifferences": VersionDifferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileOutputTypeDef = TypedDict(
     "GetProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfileOutputTypeDef = TypedDict(
     "UpdateProfileOutputTypeDef",
     {
         "Profile": ProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProfileTemplateOutputTypeDef = TypedDict(
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "AnswerSummaries": List[AnswerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnswerOutputTypeDef = TypedDict(
     "GetAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAnswerOutputTypeDef = TypedDict(
     "UpdateAnswerOutputTypeDef",
     {
         "WorkloadId": str,
         "LensAlias": str,
         "LensArn": str,
         "Answer": AnswerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConsolidatedReportMetricTypeDef = TypedDict(
     "ConsolidatedReportMetricTypeDef",
     {
         "MetricType": Literal["WORKLOAD"],
@@ -2100,10 +2110,10 @@
 
 GetConsolidatedReportOutputTypeDef = TypedDict(
     "GetConsolidatedReportOutputTypeDef",
     {
         "Metrics": List[ConsolidatedReportMetricTypeDef],
         "NextToken": str,
         "Base64String": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/PKG-INFO` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wellarchitected
-Version: 1.28.0
-Summary: Type annotations for boto3.WellArchitected 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.WellArchitected 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wellarchitected"></a>
 
 # mypy-boto3-wellarchitected
 
 [![PyPI - mypy-boto3-wellarchitected](https://img.shields.io/pypi/v/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wellarchitected.svg?color=blue)](https://pypi.org/project/mypy-boto3-wellarchitected)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wellarchitected?color=blue)](https://pypistats.org/packages/mypy-boto3-wellarchitected)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wellarchitected)](https://pepy.tech/project/mypy-boto3-wellarchitected)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WellArchitected 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
+[boto3.WellArchitected 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected)
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
 [mypy-boto3-wellarchitected docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wellarchitected/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,51 +338,42 @@
     AssociateProfilesInputRequestTypeDef,
     BestPracticeTypeDef,
     CheckDetailTypeDef,
     CheckSummaryTypeDef,
     ChoiceImprovementPlanTypeDef,
     ChoiceUpdateTypeDef,
     CreateLensShareInputRequestTypeDef,
-    CreateLensShareOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateLensVersionInputRequestTypeDef,
-    CreateLensVersionOutputTypeDef,
     CreateMilestoneInputRequestTypeDef,
-    CreateMilestoneOutputTypeDef,
     ProfileQuestionUpdateTypeDef,
-    CreateProfileOutputTypeDef,
     CreateProfileShareInputRequestTypeDef,
-    CreateProfileShareOutputTypeDef,
     WorkloadDiscoveryConfigTypeDef,
-    CreateWorkloadOutputTypeDef,
     CreateWorkloadShareInputRequestTypeDef,
-    CreateWorkloadShareOutputTypeDef,
     DeleteLensInputRequestTypeDef,
     DeleteLensShareInputRequestTypeDef,
     DeleteProfileInputRequestTypeDef,
     DeleteProfileShareInputRequestTypeDef,
     DeleteWorkloadInputRequestTypeDef,
     DeleteWorkloadShareInputRequestTypeDef,
     DisassociateLensesInputRequestTypeDef,
     DisassociateProfilesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportLensInputRequestTypeDef,
-    ExportLensOutputTypeDef,
     GetAnswerInputRequestTypeDef,
     GetConsolidatedReportInputRequestTypeDef,
     GetLensInputRequestTypeDef,
     LensTypeDef,
     GetLensReviewInputRequestTypeDef,
     GetLensReviewReportInputRequestTypeDef,
     LensReviewReportTypeDef,
     GetLensVersionDifferenceInputRequestTypeDef,
     GetMilestoneInputRequestTypeDef,
     GetProfileInputRequestTypeDef,
     GetWorkloadInputRequestTypeDef,
     ImportLensInputRequestTypeDef,
-    ImportLensOutputTypeDef,
     WorkloadProfileTypeDef,
     PillarReviewSummaryTypeDef,
     LensShareSummaryTypeDef,
     LensSummaryTypeDef,
     LensUpgradeSummaryTypeDef,
     ListAnswersInputRequestTypeDef,
     ListCheckDetailsInputRequestTypeDef,
@@ -398,85 +389,95 @@
     ListProfileSharesInputRequestTypeDef,
     ProfileShareSummaryTypeDef,
     ListProfilesInputRequestTypeDef,
     ProfileSummaryTypeDef,
     ListShareInvitationsInputRequestTypeDef,
     ShareInvitationSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListWorkloadSharesInputRequestTypeDef,
     WorkloadShareSummaryTypeDef,
     ListWorkloadsInputRequestTypeDef,
     QuestionDifferenceTypeDef,
     ProfileChoiceTypeDef,
     ProfileTemplateChoiceTypeDef,
-    ResponseMetadataTypeDef,
     ShareInvitationTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateGlobalSettingsInputRequestTypeDef,
     UpdateLensReviewInputRequestTypeDef,
     UpdateShareInvitationInputRequestTypeDef,
     UpdateWorkloadShareInputRequestTypeDef,
     WorkloadShareTypeDef,
     UpgradeLensReviewInputRequestTypeDef,
     UpgradeProfileVersionInputRequestTypeDef,
+    WorkloadDiscoveryConfigOutputTypeDef,
     AdditionalResourcesTypeDef,
     QuestionMetricTypeDef,
-    ListCheckDetailsOutputTypeDef,
-    ListCheckSummariesOutputTypeDef,
     ImprovementSummaryTypeDef,
     UpdateAnswerInputRequestTypeDef,
+    CreateLensShareOutputTypeDef,
+    CreateLensVersionOutputTypeDef,
+    CreateMilestoneOutputTypeDef,
+    CreateProfileOutputTypeDef,
+    CreateProfileShareOutputTypeDef,
+    CreateWorkloadOutputTypeDef,
+    CreateWorkloadShareOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportLensOutputTypeDef,
+    ImportLensOutputTypeDef,
+    ListCheckDetailsOutputTypeDef,
+    ListCheckSummariesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     CreateProfileInputRequestTypeDef,
     UpdateProfileInputRequestTypeDef,
     CreateWorkloadInputRequestTypeDef,
     UpdateWorkloadInputRequestTypeDef,
     GetLensOutputTypeDef,
     GetLensReviewReportOutputTypeDef,
     LensReviewSummaryTypeDef,
     WorkloadSummaryTypeDef,
-    WorkloadTypeDef,
     LensReviewTypeDef,
     ListLensSharesOutputTypeDef,
     ListLensesOutputTypeDef,
     NotificationSummaryTypeDef,
     ListProfileNotificationsOutputTypeDef,
     ListProfileSharesOutputTypeDef,
     ListProfilesOutputTypeDef,
     ListShareInvitationsOutputTypeDef,
     ListWorkloadSharesOutputTypeDef,
     PillarDifferenceTypeDef,
     ProfileQuestionTypeDef,
     ProfileTemplateQuestionTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
+    WorkloadTypeDef,
     ChoiceTypeDef,
     PillarMetricTypeDef,
     ListLensReviewImprovementsOutputTypeDef,
     ListLensReviewsOutputTypeDef,
     ListWorkloadsOutputTypeDef,
     MilestoneSummaryTypeDef,
-    GetWorkloadOutputTypeDef,
-    MilestoneTypeDef,
-    UpdateWorkloadOutputTypeDef,
     GetLensReviewOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     ListNotificationsOutputTypeDef,
     VersionDifferencesTypeDef,
     ProfileTypeDef,
     ProfileTemplateTypeDef,
+    GetWorkloadOutputTypeDef,
+    MilestoneTypeDef,
+    UpdateWorkloadOutputTypeDef,
     AnswerSummaryTypeDef,
     AnswerTypeDef,
     LensMetricTypeDef,
     ListMilestonesOutputTypeDef,
-    GetMilestoneOutputTypeDef,
     GetLensVersionDifferenceOutputTypeDef,
     GetProfileOutputTypeDef,
     UpdateProfileOutputTypeDef,
     GetProfileTemplateOutputTypeDef,
+    GetMilestoneOutputTypeDef,
     ListAnswersOutputTypeDef,
     GetAnswerOutputTypeDef,
     UpdateAnswerOutputTypeDef,
     ConsolidatedReportMetricTypeDef,
     GetConsolidatedReportOutputTypeDef,
 )
```

### Comparing `mypy-boto3-wellarchitected-1.28.0/mypy_boto3_wellarchitected.egg-info/SOURCES.txt` & `mypy-boto3-wellarchitected-1.28.12/mypy_boto3_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wellarchitected-1.28.0/setup.py` & `mypy-boto3-wellarchitected-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wellarchitected",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.WellArchitected 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.WellArchitected 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

