# Comparing `tmp/mypy-boto3-backup-1.28.0.tar.gz` & `tmp/mypy-boto3-backup-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backup-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-backup-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-backup-1.28.0.tar` & `mypy-boto3-backup-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.270228 mypy-boto3-backup-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-06 20:59:02.262228 mypy-boto3-backup-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.258228 mypy-boto3-backup-1.28.0/mypy_boto3_backup/
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-06 20:34:05.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-06 20:34:05.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-06 20:34:05.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-07-06 20:34:05.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-06 20:34:05.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67854 2023-07-06 20:34:08.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67779 2023-07-06 20:34:07.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.262228 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 20:59:02.000000 mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.270228 mypy-boto3-backup-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-07-06 20:34:04.000000 mypy-boto3-backup-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20994 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/mypy_boto3_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54908 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54816 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:52.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72958 2023-07-27 05:17:54.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72873 2023-07-27 05:17:53.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22477 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:20.000000 mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.828572 mypy-boto3-backup-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:17:51.000000 mypy-boto3-backup-1.28.12/setup.py
```

### Comparing `mypy-boto3-backup-1.28.0/LICENSE` & `mypy-boto3-backup-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/PKG-INFO` & `mypy-boto3-backup-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.0
-Summary: Type annotations for boto3.Backup 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,33 +378,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
+    LifecycleOutputTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
+    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
+    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     CreateReportPlanOutputTypeDef,
+    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
@@ -480,15 +487,17 @@
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     ListTagsOutputTypeDef,
     PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
+    ReportSettingOutputTypeDef,
     ResponseMetadataTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
     StartRestoreJobOutputTypeDef,
@@ -506,64 +515,69 @@
     CopyJobTypeDef,
     DescribeBackupJobOutputTypeDef,
     ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
+    CopyActionOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
     DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
+    CreateFrameworkInputRequestTypeDef,
     UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_structure() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.0/README.md` & `mypy-boto3-backup-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,33 +346,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
+    LifecycleOutputTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
+    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
+    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     CreateReportPlanOutputTypeDef,
+    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
@@ -448,15 +455,17 @@
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     ListTagsOutputTypeDef,
     PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
+    ReportSettingOutputTypeDef,
     ResponseMetadataTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
     StartRestoreJobOutputTypeDef,
@@ -474,64 +483,69 @@
     CopyJobTypeDef,
     DescribeBackupJobOutputTypeDef,
     ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
+    CopyActionOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
     DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
+    CreateFrameworkInputRequestTypeDef,
     UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_structure() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/__init__.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/__init__.pyi` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/__main__.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Backup 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Backup 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup\nOther"
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

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/client.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/client.pyi` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/literals.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -300,26 +301,28 @@
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

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/literals.pyi` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/literals.pyi`

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

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/paginator.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/paginator.pyi` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/type_defs.py` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_backup.type_defs import AdvancedBackupSettingTypeDef
+    from mypy_boto3_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -32,33 +32,40 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
+    "LifecycleOutputTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
+    "ConditionParameterOutputTypeDef",
     "ConditionParameterTypeDef",
+    "ControlInputParameterOutputTypeDef",
     "ControlInputParameterTypeDef",
+    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "CreateBackupVaultOutputTypeDef",
     "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
     "CreateReportPlanOutputTypeDef",
+    "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
@@ -134,15 +141,17 @@
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "ListTagsOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
+    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
+    "ReportSettingOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartBackupJobOutputTypeDef",
     "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
     "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
     "StartRestoreJobOutputTypeDef",
@@ -160,62 +169,76 @@
     "CopyJobTypeDef",
     "DescribeBackupJobOutputTypeDef",
     "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
+    "CopyActionOutputTypeDef",
     "ListBackupSelectionsOutputTypeDef",
     "ListBackupVaultsOutputTypeDef",
     "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
+    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
     "CreateReportPlanInputRequestTypeDef",
-    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
+    "RecoveryPointSelectionOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
+    "ReportPlanTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
+    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
     "UpdateFrameworkInputRequestTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "CreateBackupSelectionInputRequestTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "CreateBackupSelectionInputRequestTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
+AdvancedBackupSettingOutputTypeDef = TypedDict(
+    "AdvancedBackupSettingOutputTypeDef",
+    {
+        "ResourceType": str,
+        "BackupOptions": Dict[str, str],
+    },
+    total=False,
+)
+
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -246,14 +269,32 @@
     {
         "MoveToColdStorageAfterDays": int,
         "DeleteAfterDays": int,
     },
     total=False,
 )
 
+LifecycleOutputTypeDef = TypedDict(
+    "LifecycleOutputTypeDef",
+    {
+        "MoveToColdStorageAfterDays": int,
+        "DeleteAfterDays": int,
+    },
+    total=False,
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "ConditionType": Literal["STRINGEQUALS"],
+        "ConditionKey": str,
+        "ConditionValue": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ConditionType": Literal["STRINGEQUALS"],
         "ConditionKey": str,
         "ConditionValue": str,
     },
@@ -316,32 +357,60 @@
 
 class CancelLegalHoldInputRequestTypeDef(
     _RequiredCancelLegalHoldInputRequestTypeDef, _OptionalCancelLegalHoldInputRequestTypeDef
 ):
     pass
 
 
+ConditionParameterOutputTypeDef = TypedDict(
+    "ConditionParameterOutputTypeDef",
+    {
+        "ConditionKey": str,
+        "ConditionValue": str,
+    },
+    total=False,
+)
+
 ConditionParameterTypeDef = TypedDict(
     "ConditionParameterTypeDef",
     {
         "ConditionKey": str,
         "ConditionValue": str,
     },
     total=False,
 )
 
+ControlInputParameterOutputTypeDef = TypedDict(
+    "ControlInputParameterOutputTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+    },
+    total=False,
+)
+
 ControlInputParameterTypeDef = TypedDict(
     "ControlInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
+ControlScopeOutputTypeDef = TypedDict(
+    "ControlScopeOutputTypeDef",
+    {
+        "ComplianceResourceIds": List[str],
+        "ComplianceResourceTypes": List[str],
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
@@ -451,14 +520,22 @@
         "ReportPlanName": str,
         "ReportPlanArn": str,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DateRangeOutputTypeDef = TypedDict(
+    "DateRangeOutputTypeDef",
+    {
+        "FromDate": datetime,
+        "ToDate": datetime,
+    },
+)
+
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": Union[datetime, str],
         "ToDate": Union[datetime, str],
     },
 )
@@ -1454,23 +1531,70 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
+_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_RequiredReportDeliveryChannelOutputTypeDef",
+    {
+        "S3BucketName": str,
+    },
+)
+_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_OptionalReportDeliveryChannelOutputTypeDef",
+    {
+        "S3KeyPrefix": str,
+        "Formats": List[str],
+    },
+    total=False,
+)
+
+
+class ReportDeliveryChannelOutputTypeDef(
+    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
+):
+    pass
+
+
 ReportDestinationTypeDef = TypedDict(
     "ReportDestinationTypeDef",
     {
         "S3BucketName": str,
         "S3Keys": List[str],
     },
     total=False,
 )
 
+_RequiredReportSettingOutputTypeDef = TypedDict(
+    "_RequiredReportSettingOutputTypeDef",
+    {
+        "ReportTemplate": str,
+    },
+)
+_OptionalReportSettingOutputTypeDef = TypedDict(
+    "_OptionalReportSettingOutputTypeDef",
+    {
+        "FrameworkArns": List[str],
+        "NumberOfFrameworks": int,
+        "Accounts": List[str],
+        "OrganizationUnits": List[str],
+        "Regions": List[str],
+    },
+    total=False,
+)
+
+
+class ReportSettingOutputTypeDef(
+    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
+):
+    pass
+
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1628,39 +1752,39 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 CreateBackupPlanOutputTypeDef = TypedDict(
     "CreateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBackupPlanOutputTypeDef = TypedDict(
     "UpdateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
@@ -1851,14 +1975,33 @@
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredCopyActionOutputTypeDef = TypedDict(
+    "_RequiredCopyActionOutputTypeDef",
+    {
+        "DestinationBackupVaultArn": str,
+    },
+)
+_OptionalCopyActionOutputTypeDef = TypedDict(
+    "_OptionalCopyActionOutputTypeDef",
+    {
+        "Lifecycle": LifecycleOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CopyActionOutputTypeDef(_RequiredCopyActionOutputTypeDef, _OptionalCopyActionOutputTypeDef):
+    pass
+
+
 ListBackupSelectionsOutputTypeDef = TypedDict(
     "ListBackupSelectionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1886,15 +2029,15 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
@@ -1916,15 +2059,15 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
@@ -1933,31 +2076,64 @@
 )
 
 UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "StringEquals": List[ConditionParameterOutputTypeDef],
+        "StringNotEquals": List[ConditionParameterOutputTypeDef],
+        "StringLike": List[ConditionParameterOutputTypeDef],
+        "StringNotLike": List[ConditionParameterOutputTypeDef],
+    },
+    total=False,
+)
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "StringEquals": Sequence[ConditionParameterTypeDef],
         "StringNotEquals": Sequence[ConditionParameterTypeDef],
         "StringLike": Sequence[ConditionParameterTypeDef],
         "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterOutputTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
+    pass
+
+
 _RequiredFrameworkControlTypeDef = TypedDict(
     "_RequiredFrameworkControlTypeDef",
     {
         "ControlName": str,
     },
 )
 _OptionalFrameworkControlTypeDef = TypedDict(
@@ -1995,30 +2171,14 @@
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -2035,14 +2195,24 @@
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
 
+RecoveryPointSelectionOutputTypeDef = TypedDict(
+    "RecoveryPointSelectionOutputTypeDef",
+    {
+        "VaultNames": List[str],
+        "ResourceIdentifiers": List[str],
+        "DateRange": DateRangeOutputTypeDef,
+    },
+    total=False,
+)
+
 RecoveryPointSelectionTypeDef = TypedDict(
     "RecoveryPointSelectionTypeDef",
     {
         "VaultNames": Sequence[str],
         "ResourceIdentifiers": Sequence[str],
         "DateRange": DateRangeTypeDef,
     },
@@ -2114,14 +2284,30 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingOutputTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2197,18 +2383,18 @@
 )
 _OptionalBackupRuleTypeDef = TypedDict(
     "_OptionalBackupRuleTypeDef",
     {
         "ScheduleExpression": str,
         "StartWindowMinutes": int,
         "CompletionWindowMinutes": int,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "RecoveryPointTags": Dict[str, str],
         "RuleId": str,
-        "CopyActions": List[CopyActionTypeDef],
+        "CopyActions": List[CopyActionOutputTypeDef],
         "EnableContinuousBackup": bool,
     },
     total=False,
 )
 
 
 class BackupRuleTypeDef(_RequiredBackupRuleTypeDef, _OptionalBackupRuleTypeDef):
@@ -2220,14 +2406,39 @@
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBackupSelectionOutputTypeDef = TypedDict(
+    "_RequiredBackupSelectionOutputTypeDef",
+    {
+        "SelectionName": str,
+        "IamRoleArn": str,
+    },
+)
+_OptionalBackupSelectionOutputTypeDef = TypedDict(
+    "_OptionalBackupSelectionOutputTypeDef",
+    {
+        "Resources": List[str],
+        "ListOfTags": List[ConditionOutputTypeDef],
+        "NotResources": List[str],
+        "Conditions": ConditionsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class BackupSelectionOutputTypeDef(
+    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
+):
+    pass
+
+
 _RequiredBackupSelectionTypeDef = TypedDict(
     "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
@@ -2243,14 +2454,29 @@
 )
 
 
 class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
 
+DescribeFrameworkOutputTypeDef = TypedDict(
+    "DescribeFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "FrameworkDescription": str,
+        "FrameworkControls": List[FrameworkControlOutputTypeDef],
+        "CreationTime": datetime,
+        "DeploymentStatus": str,
+        "FrameworkStatus": str,
+        "IdempotencyToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
         "FrameworkControls": Sequence[FrameworkControlTypeDef],
     },
 )
@@ -2267,29 +2493,14 @@
 
 class CreateFrameworkInputRequestTypeDef(
     _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
 ):
     pass
 
 
-DescribeFrameworkOutputTypeDef = TypedDict(
-    "DescribeFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlTypeDef],
-        "CreationTime": datetime,
-        "DeploymentStatus": str,
-        "FrameworkStatus": str,
-        "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 _OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
@@ -2305,27 +2516,41 @@
 
 class UpdateFrameworkInputRequestTypeDef(
     _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
 ):
     pass
 
 
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
+CreateLegalHoldOutputTypeDef = TypedDict(
+    "CreateLegalHoldOutputTypeDef",
     {
-        "ReportPlan": ReportPlanTypeDef,
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
+GetLegalHoldOutputTypeDef = TypedDict(
+    "GetLegalHoldOutputTypeDef",
     {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "CancelDescription": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "CancellationDate": datetime,
+        "RetainRecordUntil": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
@@ -2346,57 +2571,43 @@
 
 class CreateLegalHoldInputRequestTypeDef(
     _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
 ):
     pass
 
 
-CreateLegalHoldOutputTypeDef = TypedDict(
-    "CreateLegalHoldOutputTypeDef",
+DescribeReportJobOutputTypeDef = TypedDict(
+    "DescribeReportJobOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ReportJob": ReportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLegalHoldOutputTypeDef = TypedDict(
-    "GetLegalHoldOutputTypeDef",
+ListReportJobsOutputTypeDef = TypedDict(
+    "ListReportJobsOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "CancelDescription": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "CancellationDate": datetime,
-        "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ReportJobs": List[ReportJobTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReportJobOutputTypeDef = TypedDict(
-    "DescribeReportJobOutputTypeDef",
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
     {
-        "ReportJob": ReportJobTypeDef,
+        "ReportPlan": ReportPlanTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListReportJobsOutputTypeDef = TypedDict(
-    "ListReportJobsOutputTypeDef",
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
     {
-        "ReportJobs": List[ReportJobTypeDef],
+        "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
@@ -2424,24 +2635,36 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
 
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
+    {
+        "BackupSelection": BackupSelectionOutputTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2457,26 +2680,14 @@
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
-    {
-        "BackupSelection": BackupSelectionTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2526,11 +2737,11 @@
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup/type_defs.pyi` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for backup service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_backup.type_defs import AdvancedBackupSettingTypeDef
+    from mypy_boto3_backup.type_defs import AdvancedBackupSettingOutputTypeDef
 
-    data: AdvancedBackupSettingTypeDef = {...}
+    data: AdvancedBackupSettingOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -31,33 +31,40 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AdvancedBackupSettingOutputTypeDef",
     "AdvancedBackupSettingTypeDef",
     "RecoveryPointCreatorTypeDef",
     "BackupPlanTemplatesListMemberTypeDef",
     "LifecycleTypeDef",
+    "LifecycleOutputTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "BackupSelectionsListMemberTypeDef",
     "BackupVaultListMemberTypeDef",
     "CalculatedLifecycleTypeDef",
     "CancelLegalHoldInputRequestTypeDef",
+    "ConditionParameterOutputTypeDef",
     "ConditionParameterTypeDef",
+    "ControlInputParameterOutputTypeDef",
     "ControlInputParameterTypeDef",
+    "ControlScopeOutputTypeDef",
     "ControlScopeTypeDef",
     "CreateBackupSelectionOutputTypeDef",
     "CreateBackupVaultInputRequestTypeDef",
     "CreateBackupVaultOutputTypeDef",
     "CreateFrameworkOutputTypeDef",
     "ReportDeliveryChannelTypeDef",
     "ReportSettingTypeDef",
     "CreateReportPlanOutputTypeDef",
+    "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeleteBackupPlanInputRequestTypeDef",
     "DeleteBackupPlanOutputTypeDef",
     "DeleteBackupSelectionInputRequestTypeDef",
     "DeleteBackupVaultAccessPolicyInputRequestTypeDef",
     "DeleteBackupVaultInputRequestTypeDef",
     "DeleteBackupVaultLockConfigurationInputRequestTypeDef",
@@ -133,15 +140,17 @@
     "RestoreJobsListMemberTypeDef",
     "ListTagsInputRequestTypeDef",
     "ListTagsOutputTypeDef",
     "PaginatorConfigTypeDef",
     "PutBackupVaultAccessPolicyInputRequestTypeDef",
     "PutBackupVaultLockConfigurationInputRequestTypeDef",
     "PutBackupVaultNotificationsInputRequestTypeDef",
+    "ReportDeliveryChannelOutputTypeDef",
     "ReportDestinationTypeDef",
+    "ReportSettingOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartBackupJobOutputTypeDef",
     "StartCopyJobOutputTypeDef",
     "StartReportJobInputRequestTypeDef",
     "StartReportJobOutputTypeDef",
     "StartRestoreJobInputRequestTypeDef",
     "StartRestoreJobOutputTypeDef",
@@ -159,62 +168,76 @@
     "CopyJobTypeDef",
     "DescribeBackupJobOutputTypeDef",
     "ListBackupPlanTemplatesOutputTypeDef",
     "CopyActionTypeDef",
     "StartBackupJobInputRequestTypeDef",
     "StartCopyJobInputRequestTypeDef",
     "UpdateRecoveryPointLifecycleInputRequestTypeDef",
+    "CopyActionOutputTypeDef",
     "ListBackupSelectionsOutputTypeDef",
     "ListBackupVaultsOutputTypeDef",
     "DescribeRecoveryPointOutputTypeDef",
     "RecoveryPointByBackupVaultTypeDef",
     "UpdateRecoveryPointLifecycleOutputTypeDef",
+    "ConditionsOutputTypeDef",
     "ConditionsTypeDef",
+    "FrameworkControlOutputTypeDef",
     "FrameworkControlTypeDef",
     "CreateReportPlanInputRequestTypeDef",
-    "ReportPlanTypeDef",
     "UpdateReportPlanInputRequestTypeDef",
+    "RecoveryPointSelectionOutputTypeDef",
     "RecoveryPointSelectionTypeDef",
     "ListFrameworksOutputTypeDef",
     "ListLegalHoldsOutputTypeDef",
     "ListProtectedResourcesOutputTypeDef",
     "ListRecoveryPointsByLegalHoldOutputTypeDef",
     "ListRecoveryPointsByResourceOutputTypeDef",
     "ListRestoreJobsOutputTypeDef",
     "ReportJobTypeDef",
+    "ReportPlanTypeDef",
     "ListBackupPlanVersionsOutputTypeDef",
     "ListBackupPlansOutputTypeDef",
     "ListBackupJobsOutputTypeDef",
     "DescribeCopyJobOutputTypeDef",
     "ListCopyJobsOutputTypeDef",
     "BackupRuleInputTypeDef",
     "BackupRuleTypeDef",
     "ListRecoveryPointsByBackupVaultOutputTypeDef",
+    "BackupSelectionOutputTypeDef",
     "BackupSelectionTypeDef",
-    "CreateFrameworkInputRequestTypeDef",
     "DescribeFrameworkOutputTypeDef",
+    "CreateFrameworkInputRequestTypeDef",
     "UpdateFrameworkInputRequestTypeDef",
-    "DescribeReportPlanOutputTypeDef",
-    "ListReportPlansOutputTypeDef",
-    "CreateLegalHoldInputRequestTypeDef",
     "CreateLegalHoldOutputTypeDef",
     "GetLegalHoldOutputTypeDef",
+    "CreateLegalHoldInputRequestTypeDef",
     "DescribeReportJobOutputTypeDef",
     "ListReportJobsOutputTypeDef",
+    "DescribeReportPlanOutputTypeDef",
+    "ListReportPlansOutputTypeDef",
     "BackupPlanInputTypeDef",
     "BackupPlanTypeDef",
-    "CreateBackupSelectionInputRequestTypeDef",
     "GetBackupSelectionOutputTypeDef",
+    "CreateBackupSelectionInputRequestTypeDef",
     "CreateBackupPlanInputRequestTypeDef",
     "UpdateBackupPlanInputRequestTypeDef",
     "GetBackupPlanFromJSONOutputTypeDef",
     "GetBackupPlanFromTemplateOutputTypeDef",
     "GetBackupPlanOutputTypeDef",
 )
 
+AdvancedBackupSettingOutputTypeDef = TypedDict(
+    "AdvancedBackupSettingOutputTypeDef",
+    {
+        "ResourceType": str,
+        "BackupOptions": Dict[str, str],
+    },
+    total=False,
+)
+
 AdvancedBackupSettingTypeDef = TypedDict(
     "AdvancedBackupSettingTypeDef",
     {
         "ResourceType": str,
         "BackupOptions": Mapping[str, str],
     },
     total=False,
@@ -245,14 +268,32 @@
     {
         "MoveToColdStorageAfterDays": int,
         "DeleteAfterDays": int,
     },
     total=False,
 )
 
+LifecycleOutputTypeDef = TypedDict(
+    "LifecycleOutputTypeDef",
+    {
+        "MoveToColdStorageAfterDays": int,
+        "DeleteAfterDays": int,
+    },
+    total=False,
+)
+
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "ConditionType": Literal["STRINGEQUALS"],
+        "ConditionKey": str,
+        "ConditionValue": str,
+    },
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "ConditionType": Literal["STRINGEQUALS"],
         "ConditionKey": str,
         "ConditionValue": str,
     },
@@ -313,32 +354,60 @@
 )
 
 class CancelLegalHoldInputRequestTypeDef(
     _RequiredCancelLegalHoldInputRequestTypeDef, _OptionalCancelLegalHoldInputRequestTypeDef
 ):
     pass
 
+ConditionParameterOutputTypeDef = TypedDict(
+    "ConditionParameterOutputTypeDef",
+    {
+        "ConditionKey": str,
+        "ConditionValue": str,
+    },
+    total=False,
+)
+
 ConditionParameterTypeDef = TypedDict(
     "ConditionParameterTypeDef",
     {
         "ConditionKey": str,
         "ConditionValue": str,
     },
     total=False,
 )
 
+ControlInputParameterOutputTypeDef = TypedDict(
+    "ControlInputParameterOutputTypeDef",
+    {
+        "ParameterName": str,
+        "ParameterValue": str,
+    },
+    total=False,
+)
+
 ControlInputParameterTypeDef = TypedDict(
     "ControlInputParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
 )
 
+ControlScopeOutputTypeDef = TypedDict(
+    "ControlScopeOutputTypeDef",
+    {
+        "ComplianceResourceIds": List[str],
+        "ComplianceResourceTypes": List[str],
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
 ControlScopeTypeDef = TypedDict(
     "ControlScopeTypeDef",
     {
         "ComplianceResourceIds": Sequence[str],
         "ComplianceResourceTypes": Sequence[str],
         "Tags": Mapping[str, str],
     },
@@ -442,14 +511,22 @@
         "ReportPlanName": str,
         "ReportPlanArn": str,
         "CreationTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DateRangeOutputTypeDef = TypedDict(
+    "DateRangeOutputTypeDef",
+    {
+        "FromDate": datetime,
+        "ToDate": datetime,
+    },
+)
+
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "FromDate": Union[datetime, str],
         "ToDate": Union[datetime, str],
     },
 )
@@ -1417,23 +1494,66 @@
     {
         "BackupVaultName": str,
         "SNSTopicArn": str,
         "BackupVaultEvents": Sequence[BackupVaultEventType],
     },
 )
 
+_RequiredReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_RequiredReportDeliveryChannelOutputTypeDef",
+    {
+        "S3BucketName": str,
+    },
+)
+_OptionalReportDeliveryChannelOutputTypeDef = TypedDict(
+    "_OptionalReportDeliveryChannelOutputTypeDef",
+    {
+        "S3KeyPrefix": str,
+        "Formats": List[str],
+    },
+    total=False,
+)
+
+class ReportDeliveryChannelOutputTypeDef(
+    _RequiredReportDeliveryChannelOutputTypeDef, _OptionalReportDeliveryChannelOutputTypeDef
+):
+    pass
+
 ReportDestinationTypeDef = TypedDict(
     "ReportDestinationTypeDef",
     {
         "S3BucketName": str,
         "S3Keys": List[str],
     },
     total=False,
 )
 
+_RequiredReportSettingOutputTypeDef = TypedDict(
+    "_RequiredReportSettingOutputTypeDef",
+    {
+        "ReportTemplate": str,
+    },
+)
+_OptionalReportSettingOutputTypeDef = TypedDict(
+    "_OptionalReportSettingOutputTypeDef",
+    {
+        "FrameworkArns": List[str],
+        "NumberOfFrameworks": int,
+        "Accounts": List[str],
+        "OrganizationUnits": List[str],
+        "Regions": List[str],
+    },
+    total=False,
+)
+
+class ReportSettingOutputTypeDef(
+    _RequiredReportSettingOutputTypeDef, _OptionalReportSettingOutputTypeDef
+):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -1587,39 +1707,39 @@
         "BackupPlanId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "VersionId": str,
         "BackupPlanName": str,
         "CreatorRequestId": str,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 CreateBackupPlanOutputTypeDef = TypedDict(
     "CreateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBackupPlanOutputTypeDef = TypedDict(
     "UpdateBackupPlanOutputTypeDef",
     {
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "CreationDate": datetime,
         "VersionId": str,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BackupJobTypeDef = TypedDict(
     "BackupJobTypeDef",
     {
@@ -1802,14 +1922,31 @@
 
 class UpdateRecoveryPointLifecycleInputRequestTypeDef(
     _RequiredUpdateRecoveryPointLifecycleInputRequestTypeDef,
     _OptionalUpdateRecoveryPointLifecycleInputRequestTypeDef,
 ):
     pass
 
+_RequiredCopyActionOutputTypeDef = TypedDict(
+    "_RequiredCopyActionOutputTypeDef",
+    {
+        "DestinationBackupVaultArn": str,
+    },
+)
+_OptionalCopyActionOutputTypeDef = TypedDict(
+    "_OptionalCopyActionOutputTypeDef",
+    {
+        "Lifecycle": LifecycleOutputTypeDef,
+    },
+    total=False,
+)
+
+class CopyActionOutputTypeDef(_RequiredCopyActionOutputTypeDef, _OptionalCopyActionOutputTypeDef):
+    pass
+
 ListBackupSelectionsOutputTypeDef = TypedDict(
     "ListBackupSelectionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupSelectionsList": List[BackupSelectionsListMemberTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1837,15 +1974,15 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "StorageClass": StorageClassType,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
@@ -1867,15 +2004,15 @@
         "IamRoleArn": str,
         "Status": RecoveryPointStatusType,
         "StatusMessage": str,
         "CreationDate": datetime,
         "CompletionDate": datetime,
         "BackupSizeInBytes": int,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "EncryptionKeyArn": str,
         "IsEncrypted": bool,
         "LastRestoreTime": datetime,
         "ParentRecoveryPointArn": str,
         "CompositeMemberIdentifier": str,
         "IsParent": bool,
         "ResourceName": str,
@@ -1884,31 +2021,62 @@
 )
 
 UpdateRecoveryPointLifecycleOutputTypeDef = TypedDict(
     "UpdateRecoveryPointLifecycleOutputTypeDef",
     {
         "BackupVaultArn": str,
         "RecoveryPointArn": str,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "CalculatedLifecycle": CalculatedLifecycleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ConditionsOutputTypeDef = TypedDict(
+    "ConditionsOutputTypeDef",
+    {
+        "StringEquals": List[ConditionParameterOutputTypeDef],
+        "StringNotEquals": List[ConditionParameterOutputTypeDef],
+        "StringLike": List[ConditionParameterOutputTypeDef],
+        "StringNotLike": List[ConditionParameterOutputTypeDef],
+    },
+    total=False,
+)
+
 ConditionsTypeDef = TypedDict(
     "ConditionsTypeDef",
     {
         "StringEquals": Sequence[ConditionParameterTypeDef],
         "StringNotEquals": Sequence[ConditionParameterTypeDef],
         "StringLike": Sequence[ConditionParameterTypeDef],
         "StringNotLike": Sequence[ConditionParameterTypeDef],
     },
     total=False,
 )
 
+_RequiredFrameworkControlOutputTypeDef = TypedDict(
+    "_RequiredFrameworkControlOutputTypeDef",
+    {
+        "ControlName": str,
+    },
+)
+_OptionalFrameworkControlOutputTypeDef = TypedDict(
+    "_OptionalFrameworkControlOutputTypeDef",
+    {
+        "ControlInputParameters": List[ControlInputParameterOutputTypeDef],
+        "ControlScope": ControlScopeOutputTypeDef,
+    },
+    total=False,
+)
+
+class FrameworkControlOutputTypeDef(
+    _RequiredFrameworkControlOutputTypeDef, _OptionalFrameworkControlOutputTypeDef
+):
+    pass
+
 _RequiredFrameworkControlTypeDef = TypedDict(
     "_RequiredFrameworkControlTypeDef",
     {
         "ControlName": str,
     },
 )
 _OptionalFrameworkControlTypeDef = TypedDict(
@@ -1942,30 +2110,14 @@
 )
 
 class CreateReportPlanInputRequestTypeDef(
     _RequiredCreateReportPlanInputRequestTypeDef, _OptionalCreateReportPlanInputRequestTypeDef
 ):
     pass
 
-ReportPlanTypeDef = TypedDict(
-    "ReportPlanTypeDef",
-    {
-        "ReportPlanArn": str,
-        "ReportPlanName": str,
-        "ReportPlanDescription": str,
-        "ReportSetting": ReportSettingTypeDef,
-        "ReportDeliveryChannel": ReportDeliveryChannelTypeDef,
-        "DeploymentStatus": str,
-        "CreationTime": datetime,
-        "LastAttemptedExecutionTime": datetime,
-        "LastSuccessfulExecutionTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredUpdateReportPlanInputRequestTypeDef = TypedDict(
     "_RequiredUpdateReportPlanInputRequestTypeDef",
     {
         "ReportPlanName": str,
     },
 )
 _OptionalUpdateReportPlanInputRequestTypeDef = TypedDict(
@@ -1980,14 +2132,24 @@
 )
 
 class UpdateReportPlanInputRequestTypeDef(
     _RequiredUpdateReportPlanInputRequestTypeDef, _OptionalUpdateReportPlanInputRequestTypeDef
 ):
     pass
 
+RecoveryPointSelectionOutputTypeDef = TypedDict(
+    "RecoveryPointSelectionOutputTypeDef",
+    {
+        "VaultNames": List[str],
+        "ResourceIdentifiers": List[str],
+        "DateRange": DateRangeOutputTypeDef,
+    },
+    total=False,
+)
+
 RecoveryPointSelectionTypeDef = TypedDict(
     "RecoveryPointSelectionTypeDef",
     {
         "VaultNames": Sequence[str],
         "ResourceIdentifiers": Sequence[str],
         "DateRange": DateRangeTypeDef,
     },
@@ -2059,14 +2221,30 @@
         "Status": str,
         "StatusMessage": str,
         "ReportDestination": ReportDestinationTypeDef,
     },
     total=False,
 )
 
+ReportPlanTypeDef = TypedDict(
+    "ReportPlanTypeDef",
+    {
+        "ReportPlanArn": str,
+        "ReportPlanName": str,
+        "ReportPlanDescription": str,
+        "ReportSetting": ReportSettingOutputTypeDef,
+        "ReportDeliveryChannel": ReportDeliveryChannelOutputTypeDef,
+        "DeploymentStatus": str,
+        "CreationTime": datetime,
+        "LastAttemptedExecutionTime": datetime,
+        "LastSuccessfulExecutionTime": datetime,
+    },
+    total=False,
+)
+
 ListBackupPlanVersionsOutputTypeDef = TypedDict(
     "ListBackupPlanVersionsOutputTypeDef",
     {
         "NextToken": str,
         "BackupPlanVersionsList": List[BackupPlansListMemberTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -2140,18 +2318,18 @@
 )
 _OptionalBackupRuleTypeDef = TypedDict(
     "_OptionalBackupRuleTypeDef",
     {
         "ScheduleExpression": str,
         "StartWindowMinutes": int,
         "CompletionWindowMinutes": int,
-        "Lifecycle": LifecycleTypeDef,
+        "Lifecycle": LifecycleOutputTypeDef,
         "RecoveryPointTags": Dict[str, str],
         "RuleId": str,
-        "CopyActions": List[CopyActionTypeDef],
+        "CopyActions": List[CopyActionOutputTypeDef],
         "EnableContinuousBackup": bool,
     },
     total=False,
 )
 
 class BackupRuleTypeDef(_RequiredBackupRuleTypeDef, _OptionalBackupRuleTypeDef):
     pass
@@ -2161,14 +2339,37 @@
     {
         "NextToken": str,
         "RecoveryPoints": List[RecoveryPointByBackupVaultTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBackupSelectionOutputTypeDef = TypedDict(
+    "_RequiredBackupSelectionOutputTypeDef",
+    {
+        "SelectionName": str,
+        "IamRoleArn": str,
+    },
+)
+_OptionalBackupSelectionOutputTypeDef = TypedDict(
+    "_OptionalBackupSelectionOutputTypeDef",
+    {
+        "Resources": List[str],
+        "ListOfTags": List[ConditionOutputTypeDef],
+        "NotResources": List[str],
+        "Conditions": ConditionsOutputTypeDef,
+    },
+    total=False,
+)
+
+class BackupSelectionOutputTypeDef(
+    _RequiredBackupSelectionOutputTypeDef, _OptionalBackupSelectionOutputTypeDef
+):
+    pass
+
 _RequiredBackupSelectionTypeDef = TypedDict(
     "_RequiredBackupSelectionTypeDef",
     {
         "SelectionName": str,
         "IamRoleArn": str,
     },
 )
@@ -2182,14 +2383,29 @@
     },
     total=False,
 )
 
 class BackupSelectionTypeDef(_RequiredBackupSelectionTypeDef, _OptionalBackupSelectionTypeDef):
     pass
 
+DescribeFrameworkOutputTypeDef = TypedDict(
+    "DescribeFrameworkOutputTypeDef",
+    {
+        "FrameworkName": str,
+        "FrameworkArn": str,
+        "FrameworkDescription": str,
+        "FrameworkControls": List[FrameworkControlOutputTypeDef],
+        "CreationTime": datetime,
+        "DeploymentStatus": str,
+        "FrameworkStatus": str,
+        "IdempotencyToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredCreateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
         "FrameworkControls": Sequence[FrameworkControlTypeDef],
     },
 )
@@ -2204,29 +2420,14 @@
 )
 
 class CreateFrameworkInputRequestTypeDef(
     _RequiredCreateFrameworkInputRequestTypeDef, _OptionalCreateFrameworkInputRequestTypeDef
 ):
     pass
 
-DescribeFrameworkOutputTypeDef = TypedDict(
-    "DescribeFrameworkOutputTypeDef",
-    {
-        "FrameworkName": str,
-        "FrameworkArn": str,
-        "FrameworkDescription": str,
-        "FrameworkControls": List[FrameworkControlTypeDef],
-        "CreationTime": datetime,
-        "DeploymentStatus": str,
-        "FrameworkStatus": str,
-        "IdempotencyToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFrameworkInputRequestTypeDef = TypedDict(
     "_RequiredUpdateFrameworkInputRequestTypeDef",
     {
         "FrameworkName": str,
     },
 )
 _OptionalUpdateFrameworkInputRequestTypeDef = TypedDict(
@@ -2240,27 +2441,41 @@
 )
 
 class UpdateFrameworkInputRequestTypeDef(
     _RequiredUpdateFrameworkInputRequestTypeDef, _OptionalUpdateFrameworkInputRequestTypeDef
 ):
     pass
 
-DescribeReportPlanOutputTypeDef = TypedDict(
-    "DescribeReportPlanOutputTypeDef",
+CreateLegalHoldOutputTypeDef = TypedDict(
+    "CreateLegalHoldOutputTypeDef",
     {
-        "ReportPlan": ReportPlanTypeDef,
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListReportPlansOutputTypeDef = TypedDict(
-    "ListReportPlansOutputTypeDef",
+GetLegalHoldOutputTypeDef = TypedDict(
+    "GetLegalHoldOutputTypeDef",
     {
-        "ReportPlans": List[ReportPlanTypeDef],
-        "NextToken": str,
+        "Title": str,
+        "Status": LegalHoldStatusType,
+        "Description": str,
+        "CancelDescription": str,
+        "LegalHoldId": str,
+        "LegalHoldArn": str,
+        "CreationDate": datetime,
+        "CancellationDate": datetime,
+        "RetainRecordUntil": datetime,
+        "RecoveryPointSelection": RecoveryPointSelectionOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateLegalHoldInputRequestTypeDef = TypedDict(
     "_RequiredCreateLegalHoldInputRequestTypeDef",
     {
@@ -2279,57 +2494,43 @@
 )
 
 class CreateLegalHoldInputRequestTypeDef(
     _RequiredCreateLegalHoldInputRequestTypeDef, _OptionalCreateLegalHoldInputRequestTypeDef
 ):
     pass
 
-CreateLegalHoldOutputTypeDef = TypedDict(
-    "CreateLegalHoldOutputTypeDef",
+DescribeReportJobOutputTypeDef = TypedDict(
+    "DescribeReportJobOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ReportJob": ReportJobTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLegalHoldOutputTypeDef = TypedDict(
-    "GetLegalHoldOutputTypeDef",
+ListReportJobsOutputTypeDef = TypedDict(
+    "ListReportJobsOutputTypeDef",
     {
-        "Title": str,
-        "Status": LegalHoldStatusType,
-        "Description": str,
-        "CancelDescription": str,
-        "LegalHoldId": str,
-        "LegalHoldArn": str,
-        "CreationDate": datetime,
-        "CancellationDate": datetime,
-        "RetainRecordUntil": datetime,
-        "RecoveryPointSelection": RecoveryPointSelectionTypeDef,
+        "ReportJobs": List[ReportJobTypeDef],
+        "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeReportJobOutputTypeDef = TypedDict(
-    "DescribeReportJobOutputTypeDef",
+DescribeReportPlanOutputTypeDef = TypedDict(
+    "DescribeReportPlanOutputTypeDef",
     {
-        "ReportJob": ReportJobTypeDef,
+        "ReportPlan": ReportPlanTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListReportJobsOutputTypeDef = TypedDict(
-    "ListReportJobsOutputTypeDef",
+ListReportPlansOutputTypeDef = TypedDict(
+    "ListReportPlansOutputTypeDef",
     {
-        "ReportJobs": List[ReportJobTypeDef],
+        "ReportPlans": List[ReportPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredBackupPlanInputTypeDef = TypedDict(
     "_RequiredBackupPlanInputTypeDef",
@@ -2355,22 +2556,34 @@
         "BackupPlanName": str,
         "Rules": List[BackupRuleTypeDef],
     },
 )
 _OptionalBackupPlanTypeDef = TypedDict(
     "_OptionalBackupPlanTypeDef",
     {
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
     },
     total=False,
 )
 
 class BackupPlanTypeDef(_RequiredBackupPlanTypeDef, _OptionalBackupPlanTypeDef):
     pass
 
+GetBackupSelectionOutputTypeDef = TypedDict(
+    "GetBackupSelectionOutputTypeDef",
+    {
+        "BackupSelection": BackupSelectionOutputTypeDef,
+        "SelectionId": str,
+        "BackupPlanId": str,
+        "CreationDate": datetime,
+        "CreatorRequestId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBackupSelectionInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupSelectionInputRequestTypeDef",
     {
         "BackupPlanId": str,
         "BackupSelection": BackupSelectionTypeDef,
     },
 )
@@ -2384,26 +2597,14 @@
 
 class CreateBackupSelectionInputRequestTypeDef(
     _RequiredCreateBackupSelectionInputRequestTypeDef,
     _OptionalCreateBackupSelectionInputRequestTypeDef,
 ):
     pass
 
-GetBackupSelectionOutputTypeDef = TypedDict(
-    "GetBackupSelectionOutputTypeDef",
-    {
-        "BackupSelection": BackupSelectionTypeDef,
-        "SelectionId": str,
-        "BackupPlanId": str,
-        "CreationDate": datetime,
-        "CreatorRequestId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBackupPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateBackupPlanInputRequestTypeDef",
     {
         "BackupPlan": BackupPlanInputTypeDef,
     },
 )
 _OptionalCreateBackupPlanInputRequestTypeDef = TypedDict(
@@ -2451,11 +2652,11 @@
         "BackupPlanId": str,
         "BackupPlanArn": str,
         "VersionId": str,
         "CreatorRequestId": str,
         "CreationDate": datetime,
         "DeletionDate": datetime,
         "LastExecutionDate": datetime,
-        "AdvancedBackupSettings": List[AdvancedBackupSettingTypeDef],
+        "AdvancedBackupSettings": List[AdvancedBackupSettingOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/PKG-INFO` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backup
-Version: 1.28.0
-Summary: Type annotations for boto3.Backup 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-backup"></a>
 
 # mypy-boto3-backup
 
 [![PyPI - mypy-boto3-backup](https://img.shields.io/pypi/v/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backup.svg?color=blue)](https://pypi.org/project/mypy-boto3-backup)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-backup?color=blue)](https://pypistats.org/packages/mypy-boto3-backup)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backup)](https://pepy.tech/project/mypy-boto3-backup)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Backup 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
+[boto3.Backup 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
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
 [mypy-boto3-backup docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backup/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,33 +378,40 @@
 ### Typed dictionaries
 
 `mypy_boto3_backup.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backup.type_defs import (
+    AdvancedBackupSettingOutputTypeDef,
     AdvancedBackupSettingTypeDef,
     RecoveryPointCreatorTypeDef,
     BackupPlanTemplatesListMemberTypeDef,
     LifecycleTypeDef,
+    LifecycleOutputTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     BackupSelectionsListMemberTypeDef,
     BackupVaultListMemberTypeDef,
     CalculatedLifecycleTypeDef,
     CancelLegalHoldInputRequestTypeDef,
+    ConditionParameterOutputTypeDef,
     ConditionParameterTypeDef,
+    ControlInputParameterOutputTypeDef,
     ControlInputParameterTypeDef,
+    ControlScopeOutputTypeDef,
     ControlScopeTypeDef,
     CreateBackupSelectionOutputTypeDef,
     CreateBackupVaultInputRequestTypeDef,
     CreateBackupVaultOutputTypeDef,
     CreateFrameworkOutputTypeDef,
     ReportDeliveryChannelTypeDef,
     ReportSettingTypeDef,
     CreateReportPlanOutputTypeDef,
+    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeleteBackupPlanInputRequestTypeDef,
     DeleteBackupPlanOutputTypeDef,
     DeleteBackupSelectionInputRequestTypeDef,
     DeleteBackupVaultAccessPolicyInputRequestTypeDef,
     DeleteBackupVaultInputRequestTypeDef,
     DeleteBackupVaultLockConfigurationInputRequestTypeDef,
@@ -480,15 +487,17 @@
     RestoreJobsListMemberTypeDef,
     ListTagsInputRequestTypeDef,
     ListTagsOutputTypeDef,
     PaginatorConfigTypeDef,
     PutBackupVaultAccessPolicyInputRequestTypeDef,
     PutBackupVaultLockConfigurationInputRequestTypeDef,
     PutBackupVaultNotificationsInputRequestTypeDef,
+    ReportDeliveryChannelOutputTypeDef,
     ReportDestinationTypeDef,
+    ReportSettingOutputTypeDef,
     ResponseMetadataTypeDef,
     StartBackupJobOutputTypeDef,
     StartCopyJobOutputTypeDef,
     StartReportJobInputRequestTypeDef,
     StartReportJobOutputTypeDef,
     StartRestoreJobInputRequestTypeDef,
     StartRestoreJobOutputTypeDef,
@@ -506,64 +515,69 @@
     CopyJobTypeDef,
     DescribeBackupJobOutputTypeDef,
     ListBackupPlanTemplatesOutputTypeDef,
     CopyActionTypeDef,
     StartBackupJobInputRequestTypeDef,
     StartCopyJobInputRequestTypeDef,
     UpdateRecoveryPointLifecycleInputRequestTypeDef,
+    CopyActionOutputTypeDef,
     ListBackupSelectionsOutputTypeDef,
     ListBackupVaultsOutputTypeDef,
     DescribeRecoveryPointOutputTypeDef,
     RecoveryPointByBackupVaultTypeDef,
     UpdateRecoveryPointLifecycleOutputTypeDef,
+    ConditionsOutputTypeDef,
     ConditionsTypeDef,
+    FrameworkControlOutputTypeDef,
     FrameworkControlTypeDef,
     CreateReportPlanInputRequestTypeDef,
-    ReportPlanTypeDef,
     UpdateReportPlanInputRequestTypeDef,
+    RecoveryPointSelectionOutputTypeDef,
     RecoveryPointSelectionTypeDef,
     ListFrameworksOutputTypeDef,
     ListLegalHoldsOutputTypeDef,
     ListProtectedResourcesOutputTypeDef,
     ListRecoveryPointsByLegalHoldOutputTypeDef,
     ListRecoveryPointsByResourceOutputTypeDef,
     ListRestoreJobsOutputTypeDef,
     ReportJobTypeDef,
+    ReportPlanTypeDef,
     ListBackupPlanVersionsOutputTypeDef,
     ListBackupPlansOutputTypeDef,
     ListBackupJobsOutputTypeDef,
     DescribeCopyJobOutputTypeDef,
     ListCopyJobsOutputTypeDef,
     BackupRuleInputTypeDef,
     BackupRuleTypeDef,
     ListRecoveryPointsByBackupVaultOutputTypeDef,
+    BackupSelectionOutputTypeDef,
     BackupSelectionTypeDef,
-    CreateFrameworkInputRequestTypeDef,
     DescribeFrameworkOutputTypeDef,
+    CreateFrameworkInputRequestTypeDef,
     UpdateFrameworkInputRequestTypeDef,
-    DescribeReportPlanOutputTypeDef,
-    ListReportPlansOutputTypeDef,
-    CreateLegalHoldInputRequestTypeDef,
     CreateLegalHoldOutputTypeDef,
     GetLegalHoldOutputTypeDef,
+    CreateLegalHoldInputRequestTypeDef,
     DescribeReportJobOutputTypeDef,
     ListReportJobsOutputTypeDef,
+    DescribeReportPlanOutputTypeDef,
+    ListReportPlansOutputTypeDef,
     BackupPlanInputTypeDef,
     BackupPlanTypeDef,
-    CreateBackupSelectionInputRequestTypeDef,
     GetBackupSelectionOutputTypeDef,
+    CreateBackupSelectionInputRequestTypeDef,
     CreateBackupPlanInputRequestTypeDef,
     UpdateBackupPlanInputRequestTypeDef,
     GetBackupPlanFromJSONOutputTypeDef,
     GetBackupPlanFromTemplateOutputTypeDef,
     GetBackupPlanOutputTypeDef,
 )
 
 
-def get_structure() -> AdvancedBackupSettingTypeDef:
+def get_structure() -> AdvancedBackupSettingOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-backup-1.28.0/mypy_boto3_backup.egg-info/SOURCES.txt` & `mypy-boto3-backup-1.28.12/mypy_boto3_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backup-1.28.0/setup.py` & `mypy-boto3-backup-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backup",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_backup"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Backup 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Backup 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

