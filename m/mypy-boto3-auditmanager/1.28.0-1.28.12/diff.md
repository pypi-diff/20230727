# Comparing `tmp/mypy-boto3-auditmanager-1.28.0.tar.gz` & `tmp/mypy-boto3-auditmanager-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.28.0.tar` & `mypy-boto3-auditmanager-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.114228 mypy-boto3-auditmanager-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-06 20:59:02.114228 mypy-boto3-auditmanager-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.114228 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-06 20:33:53.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-06 20:33:53.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10637 2023-07-06 20:33:53.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10635 2023-07-06 20:33:53.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57825 2023-07-06 20:33:55.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57780 2023-07-06 20:33:54.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.114228 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19626 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 20:59:01.000000 mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.114228 mypy-boto3-auditmanager-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:33:52.000000 mypy-boto3-auditmanager-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60586 2023-07-27 05:17:46.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60541 2023-07-27 05:17:45.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.28.0/LICENSE` & `mypy-boto3-auditmanager-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.0/PKG-INFO` & `mypy-boto3-auditmanager-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.0
-Summary: Type annotations for boto3.AuditManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,49 +321,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
+    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
+    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleTypeDef,
+    RoleOutputTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationTypeDef,
+    AssessmentReportsDestinationOutputTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    CreateDelegationRequestOutputTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
+    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    RoleTypeDef,
+    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
     DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
+    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
     GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
@@ -410,14 +419,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
@@ -433,14 +443,15 @@
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
+    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -486,15 +497,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_structure() -> AWSAccountOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.0/README.md` & `mypy-boto3-auditmanager-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,49 +289,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
+    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
+    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleTypeDef,
+    RoleOutputTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationTypeDef,
+    AssessmentReportsDestinationOutputTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    CreateDelegationRequestOutputTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
+    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    RoleTypeDef,
+    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
     DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
+    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
     GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
@@ -378,14 +387,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
@@ -401,14 +411,15 @@
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
+    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -454,15 +465,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_structure() -> AWSAccountOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,15 @@
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
@@ -305,26 +306,28 @@
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

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for auditmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
+    from mypy_boto3_auditmanager.type_defs import AWSAccountOutputTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -46,51 +46,59 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AWSAccountOutputTypeDef",
     "AWSAccountTypeDef",
+    "AWSServiceOutputTypeDef",
     "AWSServiceTypeDef",
     "DelegationTypeDef",
-    "RoleTypeDef",
+    "RoleOutputTypeDef",
     "ControlCommentTypeDef",
     "AssessmentEvidenceFolderTypeDef",
     "AssessmentFrameworkMetadataTypeDef",
     "AssessmentFrameworkShareRequestTypeDef",
     "FrameworkMetadataTypeDef",
-    "AssessmentReportsDestinationTypeDef",
+    "AssessmentReportsDestinationOutputTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
+    "AssessmentReportsDestinationTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "CreateDelegationRequestOutputTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "ManualEvidenceOutputTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
+    "SourceKeywordOutputTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
+    "RoleTypeDef",
+    "DefaultExportDestinationOutputTypeDef",
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
     "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
+    "DeregistrationPolicyOutputTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
     "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
@@ -137,14 +145,15 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     "ListAssessmentFrameworksResponseTypeDef",
@@ -160,14 +169,15 @@
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
     "ControlInsightsMetadataByAssessmentItemTypeDef",
     "ControlInsightsMetadataItemTypeDef",
+    "ControlMappingSourceOutputTypeDef",
     "ControlMappingSourceTypeDef",
     "CreateControlMappingSourceTypeDef",
     "ListControlsResponseTypeDef",
     "CreateAssessmentFrameworkControlSetTypeDef",
     "UpdateAssessmentFrameworkControlSetTypeDef",
     "GetDelegationsResponseTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
@@ -212,24 +222,42 @@
     "UpdateAssessmentResponseTypeDef",
     "UpdateAssessmentStatusResponseTypeDef",
     "CreateAssessmentFrameworkResponseTypeDef",
     "GetAssessmentFrameworkResponseTypeDef",
     "UpdateAssessmentFrameworkResponseTypeDef",
 )
 
+AWSAccountOutputTypeDef = TypedDict(
+    "AWSAccountOutputTypeDef",
+    {
+        "id": str,
+        "emailAddress": str,
+        "name": str,
+    },
+    total=False,
+)
+
 AWSAccountTypeDef = TypedDict(
     "AWSAccountTypeDef",
     {
         "id": str,
         "emailAddress": str,
         "name": str,
     },
     total=False,
 )
 
+AWSServiceOutputTypeDef = TypedDict(
+    "AWSServiceOutputTypeDef",
+    {
+        "serviceName": str,
+    },
+    total=False,
+)
+
 AWSServiceTypeDef = TypedDict(
     "AWSServiceTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
@@ -248,16 +276,16 @@
         "controlSetId": str,
         "comment": str,
         "createdBy": str,
     },
     total=False,
 )
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
+RoleOutputTypeDef = TypedDict(
+    "RoleOutputTypeDef",
     {
         "roleType": RoleTypeType,
         "roleArn": str,
     },
 )
 
 ControlCommentTypeDef = TypedDict(
@@ -342,16 +370,16 @@
         "description": str,
         "logo": str,
         "complianceType": str,
     },
     total=False,
 )
 
-AssessmentReportsDestinationTypeDef = TypedDict(
-    "AssessmentReportsDestinationTypeDef",
+AssessmentReportsDestinationOutputTypeDef = TypedDict(
+    "AssessmentReportsDestinationOutputTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
 )
 
@@ -392,14 +420,23 @@
         "author": str,
         "status": AssessmentReportStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
+AssessmentReportsDestinationTypeDef = TypedDict(
+    "AssessmentReportsDestinationTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
+
 AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef = TypedDict(
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "evidenceFolderId": str,
     },
 )
@@ -409,14 +446,25 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
+CreateDelegationRequestOutputTypeDef = TypedDict(
+    "CreateDelegationRequestOutputTypeDef",
+    {
+        "comment": str,
+        "controlSetId": str,
+        "roleArn": str,
+        "roleType": RoleTypeType,
+    },
+    total=False,
+)
+
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -447,14 +495,24 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
+ManualEvidenceOutputTypeDef = TypedDict(
+    "ManualEvidenceOutputTypeDef",
+    {
+        "s3ResourcePath": str,
+        "textResponse": str,
+        "evidenceFileName": str,
+    },
+    total=False,
+)
+
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
         "textResponse": str,
         "evidenceFileName": str,
     },
@@ -479,14 +537,23 @@
         "noncompliantEvidenceCount": int,
         "compliantEvidenceCount": int,
         "inconclusiveEvidenceCount": int,
     },
     total=False,
 )
 
+SourceKeywordOutputTypeDef = TypedDict(
+    "SourceKeywordOutputTypeDef",
+    {
+        "keywordInputType": KeywordInputTypeType,
+        "keywordValue": str,
+    },
+    total=False,
+)
+
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
         "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
@@ -524,21 +591,36 @@
     {
         "description": str,
         "queryStatement": str,
     },
     total=False,
 )
 
-
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
+    {
+        "roleType": RoleTypeType,
+        "roleArn": str,
+    },
+)
+
+DefaultExportDestinationOutputTypeDef = TypedDict(
+    "DefaultExportDestinationOutputTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
 
 DefaultExportDestinationTypeDef = TypedDict(
     "DefaultExportDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
@@ -608,14 +690,22 @@
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
 
+DeregistrationPolicyOutputTypeDef = TypedDict(
+    "DeregistrationPolicyOutputTypeDef",
+    {
+        "deleteResources": DeleteResourcesType,
+    },
+    total=False,
+)
+
 DeregistrationPolicyTypeDef = TypedDict(
     "DeregistrationPolicyTypeDef",
     {
         "deleteResources": DeleteResourcesType,
     },
     total=False,
 )
@@ -701,21 +791,19 @@
         "controlId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetChangeLogsRequestRequestTypeDef(
     _RequiredGetChangeLogsRequestRequestTypeDef, _OptionalGetChangeLogsRequestRequestTypeDef
 ):
     pass
 
-
 GetControlRequestRequestTypeDef = TypedDict(
     "GetControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
@@ -741,22 +829,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetEvidenceByEvidenceFolderRequestRequestTypeDef(
     _RequiredGetEvidenceByEvidenceFolderRequestRequestTypeDef,
     _OptionalGetEvidenceByEvidenceFolderRequestRequestTypeDef,
 ):
     pass
 
-
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -791,22 +877,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef(
     _RequiredGetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     _OptionalGetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 _OptionalGetEvidenceFoldersByAssessmentRequestRequestTypeDef = TypedDict(
@@ -814,22 +898,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetEvidenceFoldersByAssessmentRequestRequestTypeDef(
     _RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     _OptionalGetEvidenceFoldersByAssessmentRequestRequestTypeDef,
 ):
     pass
 
-
 GetEvidenceRequestRequestTypeDef = TypedDict(
     "GetEvidenceRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
         "evidenceId": str,
@@ -909,22 +991,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef(
     _RequiredListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     _OptionalListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     {
         "requestType": ShareRequestTypeType,
     },
 )
 _OptionalListAssessmentFrameworkShareRequestsRequestRequestTypeDef = TypedDict(
@@ -932,22 +1012,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentFrameworkShareRequestsRequestRequestTypeDef(
     _RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     _OptionalListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssessmentFrameworksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentFrameworksRequestRequestTypeDef",
     {
         "frameworkType": FrameworkTypeType,
     },
 )
 _OptionalListAssessmentFrameworksRequestRequestTypeDef = TypedDict(
@@ -955,22 +1033,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAssessmentFrameworksRequestRequestTypeDef(
     _RequiredListAssessmentFrameworksRequestRequestTypeDef,
     _OptionalListAssessmentFrameworksRequestRequestTypeDef,
 ):
     pass
 
-
 ListAssessmentReportsRequestRequestTypeDef = TypedDict(
     "ListAssessmentReportsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -997,22 +1073,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListControlDomainInsightsByAssessmentRequestRequestTypeDef(
     _RequiredListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     _OptionalListControlDomainInsightsByAssessmentRequestRequestTypeDef,
 ):
     pass
 
-
 ListControlDomainInsightsRequestRequestTypeDef = TypedDict(
     "ListControlDomainInsightsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1029,22 +1103,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListControlInsightsByControlDomainRequestRequestTypeDef(
     _RequiredListControlInsightsByControlDomainRequestRequestTypeDef,
     _OptionalListControlInsightsByControlDomainRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListControlsRequestRequestTypeDef",
     {
         "controlType": ControlTypeType,
     },
 )
 _OptionalListControlsRequestRequestTypeDef = TypedDict(
@@ -1052,21 +1124,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListControlsRequestRequestTypeDef(
     _RequiredListControlsRequestRequestTypeDef, _OptionalListControlsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListKeywordsForDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredListKeywordsForDataSourceRequestRequestTypeDef",
     {
         "source": SourceTypeType,
     },
 )
 _OptionalListKeywordsForDataSourceRequestRequestTypeDef = TypedDict(
@@ -1074,22 +1144,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
-
 ListKeywordsForDataSourceResponseTypeDef = TypedDict(
     "ListKeywordsForDataSourceResponseTypeDef",
     {
         "keywords": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1190,22 +1258,20 @@
     "_OptionalStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
-
 class StartAssessmentFrameworkShareRequestRequestTypeDef(
     _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef,
     _OptionalStartAssessmentFrameworkShareRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1231,22 +1297,20 @@
     {
         "controlStatus": ControlStatusType,
         "commentBody": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentControlRequestRequestTypeDef(
     _RequiredUpdateAssessmentControlRequestRequestTypeDef,
     _OptionalUpdateAssessmentControlRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateAssessmentControlSetStatusRequestRequestTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "status": ControlSetStatusType,
         "comment": str,
@@ -1285,14 +1349,23 @@
         "signatureDateTime": str,
         "signatureKeyId": str,
         "validationErrors": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "awsAccounts": List[AWSAccountOutputTypeDef],
+        "awsServices": List[AWSServiceOutputTypeDef],
+    },
+    total=False,
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1301,15 +1374,15 @@
 AssessmentMetadataItemTypeDef = TypedDict(
     "AssessmentMetadataItemTypeDef",
     {
         "name": str,
         "id": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "roles": List[RoleTypeDef],
+        "roles": List[RoleOutputTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1423,15 +1496,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
-        "createDelegationRequest": CreateDelegationRequestTypeDef,
+        "createDelegationRequest": CreateDelegationRequestOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchCreateDelegationByAssessmentRequestRequestTypeDef = TypedDict(
@@ -1449,15 +1522,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
-        "manualEvidence": ManualEvidenceTypeDef,
+        "manualEvidence": ManualEvidenceOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchImportEvidenceToAssessmentControlRequestRequestTypeDef = TypedDict(
@@ -1511,14 +1584,29 @@
         "id": str,
         "evidenceInsights": EvidenceInsightsTypeDef,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
+ControlMappingSourceOutputTypeDef = TypedDict(
+    "ControlMappingSourceOutputTypeDef",
+    {
+        "sourceId": str,
+        "sourceName": str,
+        "sourceDescription": str,
+        "sourceSetUpOption": SourceSetUpOptionType,
+        "sourceType": SourceTypeType,
+        "sourceKeyword": SourceKeywordOutputTypeDef,
+        "sourceFrequency": SourceFrequencyType,
+        "troubleshootingText": str,
+    },
+    total=False,
+)
+
 ControlMappingSourceTypeDef = TypedDict(
     "ControlMappingSourceTypeDef",
     {
         "sourceId": str,
         "sourceName": str,
         "sourceDescription": str,
         "sourceSetUpOption": SourceSetUpOptionType,
@@ -1563,22 +1651,20 @@
     "_OptionalCreateAssessmentFrameworkControlSetTypeDef",
     {
         "controls": Sequence[CreateAssessmentFrameworkControlTypeDef],
     },
     total=False,
 )
 
-
 class CreateAssessmentFrameworkControlSetTypeDef(
     _RequiredCreateAssessmentFrameworkControlSetTypeDef,
     _OptionalCreateAssessmentFrameworkControlSetTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredUpdateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
         "controls": Sequence[CreateAssessmentFrameworkControlTypeDef],
     },
 )
@@ -1586,22 +1672,20 @@
     "_OptionalUpdateAssessmentFrameworkControlSetTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentFrameworkControlSetTypeDef(
     _RequiredUpdateAssessmentFrameworkControlSetTypeDef,
     _OptionalUpdateAssessmentFrameworkControlSetTypeDef,
 ):
     pass
 
-
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1622,20 +1706,20 @@
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
-        "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "defaultProcessOwners": List[RoleTypeDef],
+        "defaultAssessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "defaultProcessOwners": List[RoleOutputTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
-        "deregistrationPolicy": DeregistrationPolicyTypeDef,
-        "defaultExportDestination": DefaultExportDestinationTypeDef,
+        "deregistrationPolicy": DeregistrationPolicyOutputTypeDef,
+        "defaultExportDestination": DefaultExportDestinationOutputTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1703,17 +1787,17 @@
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeTypeDef,
-        "roles": List[RoleTypeDef],
+        "assessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "scope": ScopeOutputTypeDef,
+        "roles": List[RoleOutputTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1732,21 +1816,19 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
@@ -1757,21 +1839,19 @@
         "assessmentDescription": str,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "roles": Sequence[RoleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateAssessmentRequestRequestTypeDef(
     _RequiredUpdateAssessmentRequestRequestTypeDef, _OptionalUpdateAssessmentRequestRequestTypeDef
 ):
     pass
 
-
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1779,15 +1859,15 @@
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
         "description": str,
         "status": ControlSetStatusType,
-        "roles": List[RoleTypeDef],
+        "roles": List[RoleOutputTypeDef],
         "controls": List[AssessmentControlTypeDef],
         "delegations": List[DelegationTypeDef],
         "systemEvidenceCount": int,
         "manualEvidenceCount": int,
     },
     total=False,
 )
@@ -1861,15 +1941,15 @@
         "type": ControlTypeType,
         "name": str,
         "description": str,
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "controlSources": str,
-        "controlMappingSources": List[ControlMappingSourceTypeDef],
+        "controlMappingSources": List[ControlMappingSourceOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
     },
     total=False,
@@ -1890,21 +1970,19 @@
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
     },
     total=False,
 )
 
-
 class UpdateControlRequestRequestTypeDef(
     _RequiredUpdateControlRequestRequestTypeDef, _OptionalUpdateControlRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateControlRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlRequestRequestTypeDef",
     {
         "name": str,
         "controlMappingSources": Sequence[CreateControlMappingSourceTypeDef],
     },
 )
@@ -1916,21 +1994,19 @@
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateControlRequestRequestTypeDef(
     _RequiredCreateControlRequestRequestTypeDef, _OptionalCreateControlRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkRequestRequestTypeDef",
     {
         "name": str,
         "controlSets": Sequence[CreateAssessmentFrameworkControlSetTypeDef],
     },
 )
@@ -1940,22 +2016,20 @@
         "description": str,
         "complianceType": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAssessmentFrameworkRequestRequestTypeDef(
     _RequiredCreateAssessmentFrameworkRequestRequestTypeDef,
     _OptionalCreateAssessmentFrameworkRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
         "name": str,
         "controlSets": Sequence[UpdateAssessmentFrameworkControlSetTypeDef],
     },
@@ -1965,22 +2039,20 @@
     {
         "description": str,
         "complianceType": str,
     },
     total=False,
 )
 
-
 class UpdateAssessmentFrameworkRequestRequestTypeDef(
     _RequiredUpdateAssessmentFrameworkRequestRequestTypeDef,
     _OptionalUpdateAssessmentFrameworkRequestRequestTypeDef,
 ):
     pass
 
-
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2063,15 +2135,15 @@
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
-        "awsAccount": AWSAccountTypeDef,
+        "awsAccount": AWSAccountOutputTypeDef,
         "metadata": AssessmentMetadataTypeDef,
         "framework": AssessmentFrameworkTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
@@ -2104,15 +2176,15 @@
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "userRole": RoleTypeDef,
+        "userRole": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
```

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for auditmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
+    from mypy_boto3_auditmanager.type_defs import AWSAccountOutputTypeDef
 
-    data: AWSAccountTypeDef = {...}
+    data: AWSAccountOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -46,50 +46,60 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AWSAccountOutputTypeDef",
     "AWSAccountTypeDef",
+    "AWSServiceOutputTypeDef",
     "AWSServiceTypeDef",
     "DelegationTypeDef",
-    "RoleTypeDef",
+    "RoleOutputTypeDef",
     "ControlCommentTypeDef",
     "AssessmentEvidenceFolderTypeDef",
     "AssessmentFrameworkMetadataTypeDef",
     "AssessmentFrameworkShareRequestTypeDef",
     "FrameworkMetadataTypeDef",
-    "AssessmentReportsDestinationTypeDef",
+    "AssessmentReportsDestinationOutputTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
+    "AssessmentReportsDestinationTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "CreateDelegationRequestOutputTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
+    "ManualEvidenceOutputTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
+    "SourceKeywordOutputTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
+    "RoleTypeDef",
+    "DefaultExportDestinationOutputTypeDef",
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
     "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
+    "DeregistrationPolicyOutputTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
     "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
@@ -136,14 +146,15 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityResponseTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     "ListAssessmentFrameworksResponseTypeDef",
@@ -159,14 +170,15 @@
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
     "ControlInsightsMetadataByAssessmentItemTypeDef",
     "ControlInsightsMetadataItemTypeDef",
+    "ControlMappingSourceOutputTypeDef",
     "ControlMappingSourceTypeDef",
     "CreateControlMappingSourceTypeDef",
     "ListControlsResponseTypeDef",
     "CreateAssessmentFrameworkControlSetTypeDef",
     "UpdateAssessmentFrameworkControlSetTypeDef",
     "GetDelegationsResponseTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
@@ -211,24 +223,42 @@
     "UpdateAssessmentResponseTypeDef",
     "UpdateAssessmentStatusResponseTypeDef",
     "CreateAssessmentFrameworkResponseTypeDef",
     "GetAssessmentFrameworkResponseTypeDef",
     "UpdateAssessmentFrameworkResponseTypeDef",
 )
 
+AWSAccountOutputTypeDef = TypedDict(
+    "AWSAccountOutputTypeDef",
+    {
+        "id": str,
+        "emailAddress": str,
+        "name": str,
+    },
+    total=False,
+)
+
 AWSAccountTypeDef = TypedDict(
     "AWSAccountTypeDef",
     {
         "id": str,
         "emailAddress": str,
         "name": str,
     },
     total=False,
 )
 
+AWSServiceOutputTypeDef = TypedDict(
+    "AWSServiceOutputTypeDef",
+    {
+        "serviceName": str,
+    },
+    total=False,
+)
+
 AWSServiceTypeDef = TypedDict(
     "AWSServiceTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
@@ -247,16 +277,16 @@
         "controlSetId": str,
         "comment": str,
         "createdBy": str,
     },
     total=False,
 )
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
+RoleOutputTypeDef = TypedDict(
+    "RoleOutputTypeDef",
     {
         "roleType": RoleTypeType,
         "roleArn": str,
     },
 )
 
 ControlCommentTypeDef = TypedDict(
@@ -341,16 +371,16 @@
         "description": str,
         "logo": str,
         "complianceType": str,
     },
     total=False,
 )
 
-AssessmentReportsDestinationTypeDef = TypedDict(
-    "AssessmentReportsDestinationTypeDef",
+AssessmentReportsDestinationOutputTypeDef = TypedDict(
+    "AssessmentReportsDestinationOutputTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
 )
 
@@ -391,14 +421,23 @@
         "author": str,
         "status": AssessmentReportStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
+AssessmentReportsDestinationTypeDef = TypedDict(
+    "AssessmentReportsDestinationTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
+
 AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef = TypedDict(
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "evidenceFolderId": str,
     },
 )
@@ -408,14 +447,25 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
+CreateDelegationRequestOutputTypeDef = TypedDict(
+    "CreateDelegationRequestOutputTypeDef",
+    {
+        "comment": str,
+        "controlSetId": str,
+        "roleArn": str,
+        "roleType": RoleTypeType,
+    },
+    total=False,
+)
+
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
         "roleArn": str,
         "roleType": RoleTypeType,
@@ -446,14 +496,24 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
+ManualEvidenceOutputTypeDef = TypedDict(
+    "ManualEvidenceOutputTypeDef",
+    {
+        "s3ResourcePath": str,
+        "textResponse": str,
+        "evidenceFileName": str,
+    },
+    total=False,
+)
+
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
         "textResponse": str,
         "evidenceFileName": str,
     },
@@ -478,14 +538,23 @@
         "noncompliantEvidenceCount": int,
         "compliantEvidenceCount": int,
         "inconclusiveEvidenceCount": int,
     },
     total=False,
 )
 
+SourceKeywordOutputTypeDef = TypedDict(
+    "SourceKeywordOutputTypeDef",
+    {
+        "keywordInputType": KeywordInputTypeType,
+        "keywordValue": str,
+    },
+    total=False,
+)
+
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
         "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
@@ -523,20 +592,39 @@
     {
         "description": str,
         "queryStatement": str,
     },
     total=False,
 )
 
+
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
+
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
+    {
+        "roleType": RoleTypeType,
+        "roleArn": str,
+    },
+)
+
+DefaultExportDestinationOutputTypeDef = TypedDict(
+    "DefaultExportDestinationOutputTypeDef",
+    {
+        "destinationType": Literal["S3"],
+        "destination": str,
+    },
+    total=False,
+)
+
 DefaultExportDestinationTypeDef = TypedDict(
     "DefaultExportDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
@@ -605,14 +693,22 @@
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
 
+DeregistrationPolicyOutputTypeDef = TypedDict(
+    "DeregistrationPolicyOutputTypeDef",
+    {
+        "deleteResources": DeleteResourcesType,
+    },
+    total=False,
+)
+
 DeregistrationPolicyTypeDef = TypedDict(
     "DeregistrationPolicyTypeDef",
     {
         "deleteResources": DeleteResourcesType,
     },
     total=False,
 )
@@ -698,19 +794,21 @@
         "controlId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetChangeLogsRequestRequestTypeDef(
     _RequiredGetChangeLogsRequestRequestTypeDef, _OptionalGetChangeLogsRequestRequestTypeDef
 ):
     pass
 
+
 GetControlRequestRequestTypeDef = TypedDict(
     "GetControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
@@ -736,20 +834,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetEvidenceByEvidenceFolderRequestRequestTypeDef(
     _RequiredGetEvidenceByEvidenceFolderRequestRequestTypeDef,
     _OptionalGetEvidenceByEvidenceFolderRequestRequestTypeDef,
 ):
     pass
 
+
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
@@ -784,20 +884,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef(
     _RequiredGetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     _OptionalGetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 _OptionalGetEvidenceFoldersByAssessmentRequestRequestTypeDef = TypedDict(
@@ -805,20 +907,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetEvidenceFoldersByAssessmentRequestRequestTypeDef(
     _RequiredGetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     _OptionalGetEvidenceFoldersByAssessmentRequestRequestTypeDef,
 ):
     pass
 
+
 GetEvidenceRequestRequestTypeDef = TypedDict(
     "GetEvidenceRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
         "evidenceId": str,
@@ -898,20 +1002,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef(
     _RequiredListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     _OptionalListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     {
         "requestType": ShareRequestTypeType,
     },
 )
 _OptionalListAssessmentFrameworkShareRequestsRequestRequestTypeDef = TypedDict(
@@ -919,20 +1025,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentFrameworkShareRequestsRequestRequestTypeDef(
     _RequiredListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     _OptionalListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssessmentFrameworksRequestRequestTypeDef = TypedDict(
     "_RequiredListAssessmentFrameworksRequestRequestTypeDef",
     {
         "frameworkType": FrameworkTypeType,
     },
 )
 _OptionalListAssessmentFrameworksRequestRequestTypeDef = TypedDict(
@@ -940,20 +1048,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAssessmentFrameworksRequestRequestTypeDef(
     _RequiredListAssessmentFrameworksRequestRequestTypeDef,
     _OptionalListAssessmentFrameworksRequestRequestTypeDef,
 ):
     pass
 
+
 ListAssessmentReportsRequestRequestTypeDef = TypedDict(
     "ListAssessmentReportsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -980,20 +1090,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListControlDomainInsightsByAssessmentRequestRequestTypeDef(
     _RequiredListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     _OptionalListControlDomainInsightsByAssessmentRequestRequestTypeDef,
 ):
     pass
 
+
 ListControlDomainInsightsRequestRequestTypeDef = TypedDict(
     "ListControlDomainInsightsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1010,20 +1122,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListControlInsightsByControlDomainRequestRequestTypeDef(
     _RequiredListControlInsightsByControlDomainRequestRequestTypeDef,
     _OptionalListControlInsightsByControlDomainRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListControlsRequestRequestTypeDef = TypedDict(
     "_RequiredListControlsRequestRequestTypeDef",
     {
         "controlType": ControlTypeType,
     },
 )
 _OptionalListControlsRequestRequestTypeDef = TypedDict(
@@ -1031,19 +1145,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListControlsRequestRequestTypeDef(
     _RequiredListControlsRequestRequestTypeDef, _OptionalListControlsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListKeywordsForDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredListKeywordsForDataSourceRequestRequestTypeDef",
     {
         "source": SourceTypeType,
     },
 )
 _OptionalListKeywordsForDataSourceRequestRequestTypeDef = TypedDict(
@@ -1051,20 +1167,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
+
 ListKeywordsForDataSourceResponseTypeDef = TypedDict(
     "ListKeywordsForDataSourceResponseTypeDef",
     {
         "keywords": List[str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1165,20 +1283,22 @@
     "_OptionalStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "comment": str,
     },
     total=False,
 )
 
+
 class StartAssessmentFrameworkShareRequestRequestTypeDef(
     _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef,
     _OptionalStartAssessmentFrameworkShareRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1204,20 +1324,22 @@
     {
         "controlStatus": ControlStatusType,
         "commentBody": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentControlRequestRequestTypeDef(
     _RequiredUpdateAssessmentControlRequestRequestTypeDef,
     _OptionalUpdateAssessmentControlRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateAssessmentControlSetStatusRequestRequestTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "status": ControlSetStatusType,
         "comment": str,
@@ -1256,14 +1378,23 @@
         "signatureDateTime": str,
         "signatureKeyId": str,
         "validationErrors": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "awsAccounts": List[AWSAccountOutputTypeDef],
+        "awsServices": List[AWSServiceOutputTypeDef],
+    },
+    total=False,
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1272,15 +1403,15 @@
 AssessmentMetadataItemTypeDef = TypedDict(
     "AssessmentMetadataItemTypeDef",
     {
         "name": str,
         "id": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "roles": List[RoleTypeDef],
+        "roles": List[RoleOutputTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1394,15 +1525,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
-        "createDelegationRequest": CreateDelegationRequestTypeDef,
+        "createDelegationRequest": CreateDelegationRequestOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchCreateDelegationByAssessmentRequestRequestTypeDef = TypedDict(
@@ -1420,15 +1551,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
-        "manualEvidence": ManualEvidenceTypeDef,
+        "manualEvidence": ManualEvidenceOutputTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchImportEvidenceToAssessmentControlRequestRequestTypeDef = TypedDict(
@@ -1482,14 +1613,29 @@
         "id": str,
         "evidenceInsights": EvidenceInsightsTypeDef,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
+ControlMappingSourceOutputTypeDef = TypedDict(
+    "ControlMappingSourceOutputTypeDef",
+    {
+        "sourceId": str,
+        "sourceName": str,
+        "sourceDescription": str,
+        "sourceSetUpOption": SourceSetUpOptionType,
+        "sourceType": SourceTypeType,
+        "sourceKeyword": SourceKeywordOutputTypeDef,
+        "sourceFrequency": SourceFrequencyType,
+        "troubleshootingText": str,
+    },
+    total=False,
+)
+
 ControlMappingSourceTypeDef = TypedDict(
     "ControlMappingSourceTypeDef",
     {
         "sourceId": str,
         "sourceName": str,
         "sourceDescription": str,
         "sourceSetUpOption": SourceSetUpOptionType,
@@ -1534,20 +1680,22 @@
     "_OptionalCreateAssessmentFrameworkControlSetTypeDef",
     {
         "controls": Sequence[CreateAssessmentFrameworkControlTypeDef],
     },
     total=False,
 )
 
+
 class CreateAssessmentFrameworkControlSetTypeDef(
     _RequiredCreateAssessmentFrameworkControlSetTypeDef,
     _OptionalCreateAssessmentFrameworkControlSetTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredUpdateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
         "controls": Sequence[CreateAssessmentFrameworkControlTypeDef],
     },
 )
@@ -1555,20 +1703,22 @@
     "_OptionalUpdateAssessmentFrameworkControlSetTypeDef",
     {
         "id": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentFrameworkControlSetTypeDef(
     _RequiredUpdateAssessmentFrameworkControlSetTypeDef,
     _OptionalUpdateAssessmentFrameworkControlSetTypeDef,
 ):
     pass
 
+
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1589,20 +1739,20 @@
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
-        "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "defaultProcessOwners": List[RoleTypeDef],
+        "defaultAssessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "defaultProcessOwners": List[RoleOutputTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
-        "deregistrationPolicy": DeregistrationPolicyTypeDef,
-        "defaultExportDestination": DefaultExportDestinationTypeDef,
+        "deregistrationPolicy": DeregistrationPolicyOutputTypeDef,
+        "defaultExportDestination": DefaultExportDestinationOutputTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1670,17 +1820,17 @@
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeTypeDef,
-        "roles": List[RoleTypeDef],
+        "assessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "scope": ScopeOutputTypeDef,
+        "roles": List[RoleOutputTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1699,19 +1849,21 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
@@ -1722,19 +1874,21 @@
         "assessmentDescription": str,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "roles": Sequence[RoleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateAssessmentRequestRequestTypeDef(
     _RequiredUpdateAssessmentRequestRequestTypeDef, _OptionalUpdateAssessmentRequestRequestTypeDef
 ):
     pass
 
+
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1742,15 +1896,15 @@
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
         "description": str,
         "status": ControlSetStatusType,
-        "roles": List[RoleTypeDef],
+        "roles": List[RoleOutputTypeDef],
         "controls": List[AssessmentControlTypeDef],
         "delegations": List[DelegationTypeDef],
         "systemEvidenceCount": int,
         "manualEvidenceCount": int,
     },
     total=False,
 )
@@ -1824,15 +1978,15 @@
         "type": ControlTypeType,
         "name": str,
         "description": str,
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "controlSources": str,
-        "controlMappingSources": List[ControlMappingSourceTypeDef],
+        "controlMappingSources": List[ControlMappingSourceOutputTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
     },
     total=False,
@@ -1853,19 +2007,21 @@
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
     },
     total=False,
 )
 
+
 class UpdateControlRequestRequestTypeDef(
     _RequiredUpdateControlRequestRequestTypeDef, _OptionalUpdateControlRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateControlRequestRequestTypeDef = TypedDict(
     "_RequiredCreateControlRequestRequestTypeDef",
     {
         "name": str,
         "controlMappingSources": Sequence[CreateControlMappingSourceTypeDef],
     },
 )
@@ -1877,19 +2033,21 @@
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateControlRequestRequestTypeDef(
     _RequiredCreateControlRequestRequestTypeDef, _OptionalCreateControlRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkRequestRequestTypeDef",
     {
         "name": str,
         "controlSets": Sequence[CreateAssessmentFrameworkControlSetTypeDef],
     },
 )
@@ -1899,20 +2057,22 @@
         "description": str,
         "complianceType": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAssessmentFrameworkRequestRequestTypeDef(
     _RequiredCreateAssessmentFrameworkRequestRequestTypeDef,
     _OptionalCreateAssessmentFrameworkRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
         "name": str,
         "controlSets": Sequence[UpdateAssessmentFrameworkControlSetTypeDef],
     },
@@ -1922,20 +2082,22 @@
     {
         "description": str,
         "complianceType": str,
     },
     total=False,
 )
 
+
 class UpdateAssessmentFrameworkRequestRequestTypeDef(
     _RequiredUpdateAssessmentFrameworkRequestRequestTypeDef,
     _OptionalUpdateAssessmentFrameworkRequestRequestTypeDef,
 ):
     pass
 
+
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2018,15 +2180,15 @@
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
-        "awsAccount": AWSAccountTypeDef,
+        "awsAccount": AWSAccountOutputTypeDef,
         "metadata": AssessmentMetadataTypeDef,
         "framework": AssessmentFrameworkTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
@@ -2059,15 +2221,15 @@
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "userRole": RoleTypeDef,
+        "userRole": RoleOutputTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
```

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.0
-Summary: Type annotations for boto3.AuditManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-auditmanager"></a>
 
 # mypy-boto3-auditmanager
 
 [![PyPI - mypy-boto3-auditmanager](https://img.shields.io/pypi/v/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-auditmanager?color=blue)](https://pypistats.org/packages/mypy-boto3-auditmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,49 +321,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
+    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
+    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleTypeDef,
+    RoleOutputTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationTypeDef,
+    AssessmentReportsDestinationOutputTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
+    CreateDelegationRequestOutputTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
+    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
+    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
+    RoleTypeDef,
+    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
     DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
+    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
     GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
@@ -410,14 +419,15 @@
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityResponseTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
     ListAssessmentFrameworksResponseTypeDef,
@@ -433,14 +443,15 @@
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
+    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -486,15 +497,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountTypeDef:
+def get_structure() -> AWSAccountOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.0/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.0/setup.py` & `mypy-boto3-auditmanager-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AuditManager 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

