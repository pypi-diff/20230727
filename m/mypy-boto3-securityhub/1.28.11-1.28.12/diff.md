# Comparing `tmp/mypy-boto3-securityhub-1.28.11.tar.gz` & `tmp/mypy-boto3-securityhub-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.28.12.tar", last modified: Thu Jul 27 11:49:36 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.28.11.tar` & `mypy-boto3-securityhub-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    82526 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    81023 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-07-25 19:48:45.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-07-25 19:48:45.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   508039 2023-07-25 19:48:57.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   507986 2023-07-25 19:48:51.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    82526 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 19:49:16.000000 mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.505065 mypy-boto3-securityhub-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-25 19:48:44.000000 mypy-boto3-securityhub-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    82510 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    81007 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.641272 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   522233 2023-07-27 11:46:33.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   522150 2023-07-27 11:46:25.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    82510 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/setup.py
```

### Comparing `mypy-boto3-securityhub-1.28.11/LICENSE` & `mypy-boto3-securityhub-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/PKG-INFO` & `mypy-boto3-securityhub-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.11
-Summary: Type annotations for boto3.SecurityHub 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.11/README.md` & `mypy-boto3-securityhub-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.28.11\nVersion:         1.28.11\nBuilder version:"
-        " 7.15.1\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.pyi`

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
     "AdminStatusType",
     "AssociationStatusType",
     "AutoEnableStandardsType",
     "AutomationRulesActionTypeType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
@@ -71,15 +70,14 @@
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
 AutomationRulesActionTypeType = Literal["FINDING_FIELDS_UPDATE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
@@ -276,14 +274,15 @@
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
@@ -362,14 +361,15 @@
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
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.py`

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
     "AdminStatusType",
     "AssociationStatusType",
     "AutoEnableStandardsType",
     "AutomationRulesActionTypeType",
     "AwsIamAccessKeyStatusType",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType",
@@ -70,14 +71,15 @@
     "SecurityHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AdminStatusType = Literal["DISABLE_IN_PROGRESS", "ENABLED"]
 AssociationStatusType = Literal["DISABLED", "ENABLED"]
 AutoEnableStandardsType = Literal["DEFAULT", "NONE"]
 AutomationRulesActionTypeType = Literal["FINDING_FIELDS_UPDATE"]
 AwsIamAccessKeyStatusType = Literal["Active", "Inactive"]
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal["Prefix", "Suffix"]
 ComplianceStatusType = Literal["FAILED", "NOT_AVAILABLE", "PASSED", "WARNING"]
@@ -274,14 +276,15 @@
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
@@ -360,14 +363,15 @@
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
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1397,14 +1397,15 @@
 
 
 ActionLocalIpDetailsOutputTypeDef = TypedDict(
     "ActionLocalIpDetailsOutputTypeDef",
     {
         "IpAddressV4": str,
     },
+    total=False,
 )
 
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
@@ -1413,14 +1414,15 @@
 
 ActionLocalPortDetailsOutputTypeDef = TypedDict(
     "ActionLocalPortDetailsOutputTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
+    total=False,
 )
 
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
@@ -1431,47 +1433,52 @@
 DnsRequestActionOutputTypeDef = TypedDict(
     "DnsRequestActionOutputTypeDef",
     {
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
+    total=False,
 )
 
 CityOutputTypeDef = TypedDict(
     "CityOutputTypeDef",
     {
         "CityName": str,
     },
+    total=False,
 )
 
 CountryOutputTypeDef = TypedDict(
     "CountryOutputTypeDef",
     {
         "CountryCode": str,
         "CountryName": str,
     },
+    total=False,
 )
 
 GeoLocationOutputTypeDef = TypedDict(
     "GeoLocationOutputTypeDef",
     {
         "Lon": float,
         "Lat": float,
     },
+    total=False,
 )
 
 IpOrganizationDetailsOutputTypeDef = TypedDict(
     "IpOrganizationDetailsOutputTypeDef",
     {
         "Asn": int,
         "AsnOrg": str,
         "Isp": str,
         "Org": str,
     },
+    total=False,
 )
 
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
@@ -1509,14 +1516,15 @@
 
 ActionRemotePortDetailsOutputTypeDef = TypedDict(
     "ActionRemotePortDetailsOutputTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
+    total=False,
 )
 
 ActionRemotePortDetailsTypeDef = TypedDict(
     "ActionRemotePortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
@@ -1545,14 +1553,15 @@
 
 AdjustmentOutputTypeDef = TypedDict(
     "AdjustmentOutputTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
+    total=False,
 )
 
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
@@ -1562,21 +1571,23 @@
 
 AdminAccountTypeDef = TypedDict(
     "AdminAccountTypeDef",
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
+    total=False,
 )
 
 AssociatedStandardOutputTypeDef = TypedDict(
     "AssociatedStandardOutputTypeDef",
     {
         "StandardsId": str,
     },
+    total=False,
 )
 
 AssociatedStandardTypeDef = TypedDict(
     "AssociatedStandardTypeDef",
     {
         "StandardsId": str,
     },
@@ -1585,14 +1596,15 @@
 
 AssociationStateDetailsOutputTypeDef = TypedDict(
     "AssociationStateDetailsOutputTypeDef",
     {
         "State": str,
         "StatusMessage": str,
     },
+    total=False,
 )
 
 AssociationStateDetailsTypeDef = TypedDict(
     "AssociationStateDetailsTypeDef",
     {
         "State": str,
         "StatusMessage": str,
@@ -1619,21 +1631,23 @@
 SeverityUpdateOutputTypeDef = TypedDict(
     "SeverityUpdateOutputTypeDef",
     {
         "Normalized": int,
         "Product": float,
         "Label": SeverityLabelType,
     },
+    total=False,
 )
 
 WorkflowUpdateOutputTypeDef = TypedDict(
     "WorkflowUpdateOutputTypeDef",
     {
         "Status": WorkflowStatusType,
     },
+    total=False,
 )
 
 NoteUpdateTypeDef = TypedDict(
     "NoteUpdateTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
@@ -1669,31 +1683,34 @@
 MapFilterOutputTypeDef = TypedDict(
     "MapFilterOutputTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparison": MapFilterComparisonType,
     },
+    total=False,
 )
 
 NumberFilterOutputTypeDef = TypedDict(
     "NumberFilterOutputTypeDef",
     {
         "Gte": float,
         "Lte": float,
         "Eq": float,
     },
+    total=False,
 )
 
 StringFilterOutputTypeDef = TypedDict(
     "StringFilterOutputTypeDef",
     {
         "Value": str,
         "Comparison": StringFilterComparisonType,
     },
+    total=False,
 )
 
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1730,22 +1747,24 @@
         "RuleName": str,
         "Description": str,
         "IsTerminal": bool,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
+    total=False,
 )
 
 AvailabilityZoneOutputTypeDef = TypedDict(
     "AvailabilityZoneOutputTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
@@ -1755,14 +1774,15 @@
 
 AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
@@ -1771,31 +1791,34 @@
         "RoleSearchSubtree": bool,
         "ServiceAccountUsername": str,
         "UserBase": str,
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
     {
         "DayOfWeek": str,
         "TimeOfDay": str,
         "TimeZone": str,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerUsersDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
     {
         "PendingChange": str,
         "Username": str,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
@@ -1841,14 +1864,15 @@
 
 AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
@@ -1857,14 +1881,15 @@
 )
 
 AwsApiCallActionDomainDetailsOutputTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsOutputTypeDef",
     {
         "Domain": str,
     },
+    total=False,
 )
 
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
@@ -1873,14 +1898,15 @@
 
 AwsApiGatewayAccessLogSettingsOutputTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsOutputTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
     },
+    total=False,
 )
 
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
@@ -1892,14 +1918,15 @@
     "AwsApiGatewayCanarySettingsOutputTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
         "StageVariableOverrides": Dict[str, str],
         "UseStageCache": bool,
     },
+    total=False,
 )
 
 AwsApiGatewayCanarySettingsTypeDef = TypedDict(
     "AwsApiGatewayCanarySettingsTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
@@ -1910,14 +1937,15 @@
 )
 
 AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     {
         "Types": List[str],
     },
+    total=False,
 )
 
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
@@ -1936,14 +1964,15 @@
         "CacheTtlInSeconds": int,
         "CacheDataEncrypted": bool,
         "RequireAuthorizationForCacheControl": bool,
         "UnauthorizedCacheControlHeaderStrategy": str,
         "HttpMethod": str,
         "ResourcePath": str,
     },
+    total=False,
 )
 
 AwsApiGatewayMethodSettingsTypeDef = TypedDict(
     "AwsApiGatewayMethodSettingsTypeDef",
     {
         "MetricsEnabled": bool,
         "LoggingLevel": str,
@@ -1967,14 +1996,15 @@
         "AllowOrigins": List[str],
         "AllowCredentials": bool,
         "ExposeHeaders": List[str],
         "MaxAge": int,
         "AllowMethods": List[str],
         "AllowHeaders": List[str],
     },
+    total=False,
 )
 
 AwsCorsConfigurationTypeDef = TypedDict(
     "AwsCorsConfigurationTypeDef",
     {
         "AllowOrigins": Sequence[str],
         "AllowCredentials": bool,
@@ -1991,14 +2021,15 @@
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
+    total=False,
 )
 
 AwsApiGatewayV2RouteSettingsTypeDef = TypedDict(
     "AwsApiGatewayV2RouteSettingsTypeDef",
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
@@ -2012,34 +2043,37 @@
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
         "IdentityValidationExpression": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
     {
         "AuthTtL": int,
         "ClientId": str,
         "IatTtL": int,
         "Issuer": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
     {
         "AppIdClientRegex": str,
         "AwsRegion": str,
         "DefaultAction": str,
         "UserPoolId": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
@@ -2073,14 +2107,15 @@
 AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
         "FieldLogLevel": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
@@ -2091,14 +2126,15 @@
 
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
@@ -2107,14 +2143,15 @@
 )
 
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
@@ -2124,14 +2161,15 @@
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -2146,14 +2184,15 @@
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
         "SpotInstancePools": int,
         "SpotMaxPrice": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
@@ -2168,22 +2207,24 @@
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -2207,14 +2248,15 @@
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -2227,23 +2269,25 @@
 )
 
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
     {
         "HttpEndpoint": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     {
         "Enabled": bool,
     },
@@ -2262,14 +2306,15 @@
 
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     {
         "BackupOptions": Dict[str, str],
         "ResourceType": str,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
@@ -2279,14 +2324,15 @@
 
 AwsBackupBackupPlanLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
@@ -2296,14 +2342,15 @@
 
 AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     {
         "BackupVaultEvents": List[str],
         "SnsTopicArn": str,
     },
+    total=False,
 )
 
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
@@ -2313,14 +2360,15 @@
 
 AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
@@ -2332,14 +2380,15 @@
     "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "BackupPlanVersion": str,
         "BackupRuleId": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointCreatedByDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
@@ -2351,14 +2400,15 @@
 
 AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
@@ -2368,28 +2418,31 @@
 
 AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
     {
         "Name": str,
         "OId": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateKeyUsageOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
     {
         "Name": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateOptionsOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateOptionsOutputTypeDef",
     {
         "CertificateTransparencyLoggingPreference": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateExtendedKeyUsageTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     {
         "Name": str,
         "OId": str,
@@ -2416,14 +2469,15 @@
 AwsCertificateManagerCertificateResourceRecordOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateResourceRecordTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -2433,23 +2487,25 @@
 )
 
 AwsCloudFormationStackDriftInformationDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
     {
         "StackDriftStatus": str,
     },
+    total=False,
 )
 
 AwsCloudFormationStackOutputsDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
     {
         "Description": str,
         "OutputKey": str,
         "OutputValue": str,
     },
+    total=False,
 )
 
 AwsCloudFormationStackDriftInformationDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     {
         "StackDriftStatus": str,
     },
@@ -2467,14 +2523,15 @@
 )
 
 AwsCloudFrontDistributionCacheBehaviorOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
@@ -2482,14 +2539,15 @@
 )
 
 AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
@@ -2500,27 +2558,29 @@
     "AwsCloudFrontDistributionLoggingOutputTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
         "IncludeCookies": bool,
         "Prefix": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionViewerCertificateOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
     {
         "AcmCertificateArn": str,
         "Certificate": str,
         "CertificateSource": str,
         "CloudFrontDefaultCertificate": bool,
         "IamCertificateId": str,
         "MinimumProtocolVersion": str,
         "SslSupportMethod": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionLoggingTypeDef = TypedDict(
     "AwsCloudFrontDistributionLoggingTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
@@ -2546,14 +2606,15 @@
 
 AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     {
         "Items": List[str],
         "Quantity": int,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": Sequence[str],
         "Quantity": int,
@@ -2563,14 +2624,15 @@
 
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     {
         "Items": List[int],
         "Quantity": int,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     {
         "Items": Sequence[int],
         "Quantity": int,
@@ -2579,14 +2641,15 @@
 )
 
 AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
     {
         "OriginAccessIdentity": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginS3OriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
@@ -2608,14 +2671,15 @@
         "Name": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "SnsTopicArn": str,
         "SnsTopicName": str,
         "TrailArn": str,
     },
+    total=False,
 )
 
 AwsCloudTrailTrailDetailsTypeDef = TypedDict(
     "AwsCloudTrailTrailDetailsTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "CloudWatchLogsRoleArn": str,
@@ -2638,14 +2702,15 @@
 
 AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCloudWatchAlarmDimensionsDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -2662,14 +2727,15 @@
         "Name": str,
         "NamespaceType": str,
         "OverrideArtifactName": bool,
         "Packaging": str,
         "Path": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectArtifactsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     {
         "ArtifactIdentifier": str,
         "EncryptionDisabled": bool,
@@ -2688,23 +2754,25 @@
     "AwsCodeBuildProjectSourceOutputTypeDef",
     {
         "Type": str,
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     {
         "VpcId": str,
         "Subnets": List[str],
         "SecurityGroupIds": List[str],
     },
+    total=False,
 )
 
 AwsCodeBuildProjectSourceTypeDef = TypedDict(
     "AwsCodeBuildProjectSourceTypeDef",
     {
         "Type": str,
         "Location": str,
@@ -2727,14 +2795,15 @@
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -2745,14 +2814,15 @@
 
 AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
@@ -2763,14 +2833,15 @@
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
     {
         "GroupName": str,
         "Status": str,
         "StreamName": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     {
         "GroupName": str,
         "Status": str,
@@ -2782,14 +2853,15 @@
 AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
@@ -2800,14 +2872,15 @@
 
 AwsDynamoDbTableAttributeDefinitionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableAttributeDefinitionTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
@@ -2817,14 +2890,15 @@
 
 AwsDynamoDbTableBillingModeSummaryOutputTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableBillingModeSummaryTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
@@ -2834,53 +2908,58 @@
 
 AwsDynamoDbTableKeySchemaOutputTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaOutputTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProvisionedThroughputOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
     {
         "LastDecreaseDateTime": str,
         "LastIncreaseDateTime": str,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 AwsDynamoDbTableRestoreSummaryOutputTypeDef = TypedDict(
     "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": str,
         "RestoreInProgress": bool,
     },
+    total=False,
 )
 
 AwsDynamoDbTableSseDescriptionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableSseDescriptionOutputTypeDef",
     {
         "InaccessibleEncryptionDateTime": str,
         "Status": str,
         "SseType": str,
         "KmsMasterKeyArn": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableStreamSpecificationOutputTypeDef = TypedDict(
     "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableKeySchemaTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
@@ -2933,14 +3012,15 @@
 
 AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionOutputTypeDef",
     {
         "NonKeyAttributes": List[str],
         "ProjectionType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
@@ -2949,14 +3029,15 @@
 )
 
 AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProvisionedThroughputOverrideTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
@@ -2973,14 +3054,15 @@
         "Domain": str,
         "PublicIpv4Pool": str,
         "NetworkBorderGroup": str,
         "NetworkInterfaceId": str,
         "NetworkInterfaceOwnerId": str,
         "PrivateIpAddress": str,
     },
+    total=False,
 )
 
 AwsEc2EipDetailsTypeDef = TypedDict(
     "AwsEc2EipDetailsTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
@@ -3001,28 +3083,31 @@
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
         "InstanceMetadataTags": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
     {
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef = TypedDict(
     "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
     {
         "NetworkInterfaceId": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceMetadataOptionsTypeDef = TypedDict(
     "AwsEc2InstanceMetadataOptionsTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
@@ -3057,14 +3142,15 @@
         "Iops": int,
         "KmsKeyId": str,
         "SnapshotId": str,
         "Throughput": int,
         "VolumeSize": int,
         "VolumeType": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -3080,14 +3166,15 @@
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
@@ -3097,14 +3184,15 @@
 
 AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
@@ -3113,14 +3201,15 @@
 )
 
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
     {
         "CpuCredits": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
     {
         "CpuCredits": str,
     },
@@ -3128,99 +3217,110 @@
 )
 
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
     {
         "Count": int,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
     {
         "Configured": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
     {
         "AutoRecovery": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpTokens": str,
         "HttpPutResponseHopLimit": int,
         "InstanceMetadataTags": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
     {
         "Affinity": str,
         "AvailabilityZone": str,
         "GroupName": str,
         "HostId": str,
         "HostResourceGroupArn": str,
         "PartitionNumber": int,
         "SpreadDomain": str,
         "Tenancy": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
     {
         "EnableResourceNameDnsAAAARecord": bool,
         "EnableResourceNameDnsARecord": bool,
         "HostnameType": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     {
         "Type": str,
     },
@@ -3327,14 +3427,15 @@
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
         "MaxPrice": str,
         "SpotInstanceType": str,
         "ValidUntil": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
@@ -3347,14 +3448,15 @@
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
@@ -3365,14 +3467,15 @@
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef = (
     TypedDict(
         "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
         {
             "Max": int,
             "Min": int,
         },
+        total=False,
     )
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
     {
         "Max": int,
@@ -3384,14 +3487,15 @@
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef = (
     TypedDict(
         "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
         {
             "Max": int,
             "Min": int,
         },
+        total=False,
     )
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
     {
         "Max": int,
@@ -3402,46 +3506,51 @@
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
     {
         "Max": float,
         "Min": float,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
     {
         "Max": float,
         "Min": float,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     {
         "Max": float,
         "Min": float,
@@ -3486,36 +3595,40 @@
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
     {
         "Ipv4Prefix": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
     {
         "Ipv6Address": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
     {
         "Ipv6Prefix": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
     {
         "Primary": bool,
         "PrivateIpAddress": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     {
         "Ipv4Prefix": str,
     },
@@ -3550,14 +3663,15 @@
 AwsEc2NetworkAclAssociationOutputTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationOutputTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
@@ -3568,22 +3682,24 @@
 
 IcmpTypeCodeOutputTypeDef = TypedDict(
     "IcmpTypeCodeOutputTypeDef",
     {
         "Code": int,
         "Type": int,
     },
+    total=False,
 )
 
 PortRangeFromToOutputTypeDef = TypedDict(
     "PortRangeFromToOutputTypeDef",
     {
         "From": int,
         "To": int,
     },
+    total=False,
 )
 
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
@@ -3607,14 +3723,15 @@
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceAttachmentTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": str,
         "AttachmentId": str,
@@ -3628,30 +3745,33 @@
 )
 
 AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
     {
         "IpV6Address": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
     {
         "PrivateIpAddress": str,
         "PrivateDnsName": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     {
         "IpV6Address": str,
     },
@@ -3677,14 +3797,15 @@
 )
 
 PropagatingVgwSetDetailsOutputTypeDef = TypedDict(
     "PropagatingVgwSetDetailsOutputTypeDef",
     {
         "GatewayId": str,
     },
+    total=False,
 )
 
 RouteSetDetailsOutputTypeDef = TypedDict(
     "RouteSetDetailsOutputTypeDef",
     {
         "CarrierGatewayId": str,
         "CoreNetworkArn": str,
@@ -3699,14 +3820,15 @@
         "NatGatewayId": str,
         "NetworkInterfaceId": str,
         "Origin": str,
         "State": str,
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 PropagatingVgwSetDetailsTypeDef = TypedDict(
     "PropagatingVgwSetDetailsTypeDef",
     {
         "GatewayId": str,
     },
@@ -3737,40 +3859,44 @@
 )
 
 AwsEc2SecurityGroupIpRangeOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeOutputTypeDef",
     {
         "CidrIp": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpv6RangeOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
     {
         "CidrIpv6": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupPrefixListIdOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
     {
         "PrefixListId": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
     {
         "GroupId": str,
         "GroupName": str,
         "PeeringStatus": str,
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
@@ -3809,14 +3935,15 @@
 Ipv6CidrBlockAssociationOutputTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationOutputTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
+    total=False,
 )
 
 Ipv6CidrBlockAssociationTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
@@ -3837,14 +3964,15 @@
         "AssociationDefaultRouteTableId": str,
         "PropagationDefaultRouteTableId": str,
         "VpnEcmpSupport": str,
         "DnsSupport": str,
         "MulticastSupport": str,
         "AmazonSideAsn": int,
     },
+    total=False,
 )
 
 AwsEc2TransitGatewayDetailsTypeDef = TypedDict(
     "AwsEc2TransitGatewayDetailsTypeDef",
     {
         "Id": str,
         "Description": str,
@@ -3866,14 +3994,15 @@
     "AwsEc2VolumeAttachmentOutputTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
         "InstanceId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEc2VolumeAttachmentTypeDef = TypedDict(
     "AwsEc2VolumeAttachmentTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
@@ -3886,14 +4015,15 @@
 CidrBlockAssociationOutputTypeDef = TypedDict(
     "CidrBlockAssociationOutputTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": str,
     },
+    total=False,
 )
 
 CidrBlockAssociationTypeDef = TypedDict(
     "CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
@@ -3903,14 +4033,15 @@
 )
 
 AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
     {
         "ServiceType": str,
     },
+    total=False,
 )
 
 AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     {
         "ServiceType": str,
     },
@@ -3919,14 +4050,15 @@
 
 AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
     {
         "Code": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionStatusDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     {
         "Code": str,
         "Message": str,
@@ -3935,30 +4067,33 @@
 )
 
 VpcInfoCidrBlockSetDetailsOutputTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsOutputTypeDef",
     {
         "CidrBlock": str,
     },
+    total=False,
 )
 
 VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef = TypedDict(
     "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
     {
         "Ipv6CidrBlock": str,
     },
+    total=False,
 )
 
 VpcInfoPeeringOptionsDetailsOutputTypeDef = TypedDict(
     "VpcInfoPeeringOptionsDetailsOutputTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
+    total=False,
 )
 
 VpcInfoCidrBlockSetDetailsTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsTypeDef",
     {
         "CidrBlock": str,
     },
@@ -3985,26 +4120,28 @@
 
 AwsEc2VpnConnectionRoutesDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
     {
         "AcceptedRouteCount": int,
         "CertificateArn": str,
         "LastStatusChange": str,
         "OutsideIpAddress": str,
         "Status": str,
         "StatusMessage": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionRoutesDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
@@ -4041,14 +4178,15 @@
         "Phase2LifetimeSeconds": int,
         "PreSharedKey": str,
         "RekeyFuzzPercentage": int,
         "RekeyMarginTimeSeconds": int,
         "ReplayWindowSize": int,
         "TunnelInsideCidr": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     {
         "DpdTimeoutSeconds": int,
         "IkeVersions": Sequence[str],
@@ -4076,14 +4214,15 @@
         "RegistryId": str,
         "RepositoryName": str,
         "Architecture": str,
         "ImageDigest": str,
         "ImageTags": List[str],
         "ImagePublishedAt": str,
     },
+    total=False,
 )
 
 AwsEcrContainerImageDetailsTypeDef = TypedDict(
     "AwsEcrContainerImageDetailsTypeDef",
     {
         "RegistryId": str,
         "RepositoryName": str,
@@ -4096,22 +4235,24 @@
 )
 
 AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
     {
         "ScanOnPush": bool,
     },
+    total=False,
 )
 
 AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef = TypedDict(
     "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
     {
         "LifecyclePolicyText": str,
         "RegistryId": str,
     },
+    total=False,
 )
 
 AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     {
         "ScanOnPush": bool,
     },
@@ -4129,14 +4270,15 @@
 
 AwsEcsClusterClusterSettingsDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsClusterClusterSettingsDetailsTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4150,14 +4292,15 @@
         {
             "CloudWatchEncryptionEnabled": bool,
             "CloudWatchLogGroupName": str,
             "S3BucketName": str,
             "S3EncryptionEnabled": bool,
             "S3KeyPrefix": str,
         },
+        total=False,
     )
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     {
         "CloudWatchEncryptionEnabled": bool,
@@ -4172,14 +4315,15 @@
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
+    total=False,
 )
 
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
@@ -4190,14 +4334,15 @@
 
 AwsMountPointOutputTypeDef = TypedDict(
     "AwsMountPointOutputTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
     },
+    total=False,
 )
 
 AwsMountPointTypeDef = TypedDict(
     "AwsMountPointTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
@@ -4208,14 +4353,15 @@
 AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
+    total=False,
 )
 
 AwsEcsServiceCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
@@ -4226,14 +4372,15 @@
 
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
@@ -4242,14 +4389,15 @@
 )
 
 AwsEcsServiceDeploymentControllerDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentControllerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     {
         "Type": str,
     },
@@ -4260,40 +4408,44 @@
     "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "LoadBalancerName": str,
         "TargetGroupArn": str,
     },
+    total=False,
 )
 
 AwsEcsServicePlacementConstraintsDetailsOutputTypeDef = TypedDict(
     "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
     {
         "Expression": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServicePlacementStrategiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
     {
         "Field": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServiceServiceRegistriesDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "Port": int,
         "RegistryArn": str,
     },
+    total=False,
 )
 
 AwsEcsServiceLoadBalancersDetailsTypeDef = TypedDict(
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
@@ -4335,14 +4487,15 @@
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": List[str],
         "Subnets": List[str],
     },
+    total=False,
 )
 
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
@@ -4353,14 +4506,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
@@ -4370,115 +4524,128 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
     {
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
     {
         "Hostname": str,
         "IpAddress": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
     {
         "Options": Dict[str, str],
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     {
         "Command": List[str],
         "Interval": int,
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "ReadOnly": bool,
         "SourceVolume": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
     {
         "ContainerPort": int,
         "HostPort": int,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
     {
         "CredentialsParameter": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
     {
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
     {
         "Namespace": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
     {
         "HardLimit": int,
         "Name": str,
         "SoftLimit": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4601,14 +4768,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": List[str],
         "Drop": List[str],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": Sequence[str],
         "Drop": Sequence[str],
@@ -4619,23 +4787,25 @@
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
         "Permissions": List[str],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "MountOptions": List[str],
         "Size": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
@@ -4657,14 +4827,15 @@
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef = (
     TypedDict(
         "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
         {
             "Name": str,
             "ValueFrom": str,
         },
+        total=False,
     )
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     {
         "Name": str,
@@ -4675,22 +4846,24 @@
 
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
     {
         "Expression": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
@@ -4709,14 +4882,15 @@
 
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4729,21 +4903,23 @@
     {
         "Autoprovision": bool,
         "Driver": str,
         "DriverOpts": Dict[str, str],
         "Labels": Dict[str, str],
         "Scope": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
     {
         "SourcePath": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     {
         "Autoprovision": bool,
         "Driver": str,
@@ -4765,14 +4941,15 @@
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef = (
     TypedDict(
         "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
         {
             "AccessPointId": str,
             "Iam": str,
         },
+        total=False,
     )
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
@@ -4782,14 +4959,15 @@
 )
 
 AwsEcsTaskVolumeHostDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
     {
         "SourcePath": str,
     },
+    total=False,
 )
 
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
@@ -4799,14 +4977,15 @@
 AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     {
         "Gid": str,
         "SecondaryGids": List[str],
         "Uid": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     {
         "Gid": str,
         "SecondaryGids": Sequence[str],
@@ -4818,14 +4997,15 @@
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
@@ -4837,14 +5017,15 @@
 AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "EndpointPublicAccess": bool,
     },
+    total=False,
 )
 
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
@@ -4855,14 +5036,15 @@
 
 AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "Types": List[str],
     },
+    total=False,
 )
 
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
         "Enabled": bool,
         "Types": Sequence[str],
@@ -4872,33 +5054,36 @@
 
 AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
     {
         "Namespace": str,
         "OptionName": str,
         "ResourceName": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentTierOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
@@ -4929,52 +5114,57 @@
 
 AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     {
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VPCId": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
@@ -5025,14 +5215,15 @@
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
@@ -5041,14 +5232,15 @@
 
 AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
@@ -5058,14 +5250,15 @@
 
 AwsElbAppCookieStickinessPolicyOutputTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyOutputTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsElbAppCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
@@ -5075,14 +5268,15 @@
 
 AwsElbLbCookieStickinessPolicyOutputTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyOutputTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsElbLbCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
@@ -5094,14 +5288,15 @@
     "AwsElbLoadBalancerAccessLogOutputTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
         "S3BucketName": str,
         "S3BucketPrefix": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAccessLogTypeDef = TypedDict(
     "AwsElbLoadBalancerAccessLogTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
@@ -5113,14 +5308,15 @@
 
 AwsElbLoadBalancerAdditionalAttributeOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAdditionalAttributeTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -5130,28 +5326,31 @@
 
 AwsElbLoadBalancerConnectionDrainingOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerConnectionSettingsOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
     {
         "IdleTimeout": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerConnectionDrainingTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
@@ -5177,14 +5376,15 @@
 
 AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
@@ -5197,29 +5397,32 @@
     {
         "HealthyThreshold": int,
         "Interval": int,
         "Target": str,
         "Timeout": int,
         "UnhealthyThreshold": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerInstanceOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerInstanceOutputTypeDef",
     {
         "InstanceId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
     {
         "GroupName": str,
         "OwnerAlias": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerHealthCheckTypeDef = TypedDict(
     "AwsElbLoadBalancerHealthCheckTypeDef",
     {
         "HealthyThreshold": int,
         "Interval": int,
@@ -5252,14 +5455,15 @@
     {
         "InstancePort": int,
         "InstanceProtocol": str,
         "LoadBalancerPort": int,
         "Protocol": str,
         "SslCertificateId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerListenerTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerTypeDef",
     {
         "InstancePort": int,
         "InstanceProtocol": str,
@@ -5272,14 +5476,15 @@
 
 AwsElbv2LoadBalancerAttributeOutputTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElbv2LoadBalancerAttributeTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -5289,14 +5494,15 @@
 
 LoadBalancerStateOutputTypeDef = TypedDict(
     "LoadBalancerStateOutputTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
+    total=False,
 )
 
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": str,
         "Reason": str,
@@ -5307,14 +5513,15 @@
 AwsEventSchemasRegistryDetailsOutputTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsOutputTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
         "RegistryName": str,
     },
+    total=False,
 )
 
 AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
@@ -5324,14 +5531,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5339,28 +5547,31 @@
 )
 
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5384,14 +5595,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5400,14 +5612,15 @@
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
     {
         "Reason": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
     {
         "Reason": str,
         "Status": str,
@@ -5417,14 +5630,15 @@
 
 AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
     {
         "Name": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     {
         "Name": str,
         "Status": str,
@@ -5434,14 +5648,15 @@
 
 AwsIamAccessKeySessionContextAttributesOutputTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
@@ -5454,14 +5669,15 @@
     {
         "Type": str,
         "PrincipalId": str,
         "Arn": str,
         "AccountId": str,
         "UserName": str,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextSessionIssuerTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     {
         "Type": str,
         "PrincipalId": str,
@@ -5474,14 +5690,15 @@
 
 AwsIamAttachedManagedPolicyOutputTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
+    total=False,
 )
 
 AwsIamAttachedManagedPolicyTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
@@ -5490,14 +5707,15 @@
 )
 
 AwsIamGroupPolicyOutputTypeDef = TypedDict(
     "AwsIamGroupPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamGroupPolicyTypeDef = TypedDict(
     "AwsIamGroupPolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5510,14 +5728,15 @@
         "Arn": str,
         "AssumeRolePolicyDocument": str,
         "CreateDate": str,
         "Path": str,
         "RoleId": str,
         "RoleName": str,
     },
+    total=False,
 )
 
 AwsIamInstanceProfileRoleTypeDef = TypedDict(
     "AwsIamInstanceProfileRoleTypeDef",
     {
         "Arn": str,
         "AssumeRolePolicyDocument": str,
@@ -5531,14 +5750,15 @@
 
 AwsIamPermissionsBoundaryOutputTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryOutputTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
     },
+    total=False,
 )
 
 AwsIamPermissionsBoundaryTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
@@ -5549,14 +5769,15 @@
 AwsIamPolicyVersionOutputTypeDef = TypedDict(
     "AwsIamPolicyVersionOutputTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": str,
     },
+    total=False,
 )
 
 AwsIamPolicyVersionTypeDef = TypedDict(
     "AwsIamPolicyVersionTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
@@ -5566,14 +5787,15 @@
 )
 
 AwsIamRolePolicyOutputTypeDef = TypedDict(
     "AwsIamRolePolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamRolePolicyTypeDef = TypedDict(
     "AwsIamRolePolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5581,14 +5803,15 @@
 )
 
 AwsIamUserPolicyOutputTypeDef = TypedDict(
     "AwsIamUserPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamUserPolicyTypeDef = TypedDict(
     "AwsIamUserPolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5597,14 +5820,15 @@
 
 AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
     },
+    total=False,
 )
 
 AwsKinesisStreamStreamEncryptionDetailsTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
@@ -5620,14 +5844,15 @@
         "KeyId": str,
         "KeyManager": str,
         "KeyState": str,
         "Origin": str,
         "Description": str,
         "KeyRotationStatus": bool,
     },
+    total=False,
 )
 
 AwsKmsKeyDetailsTypeDef = TypedDict(
     "AwsKmsKeyDetailsTypeDef",
     {
         "AWSAccountId": str,
         "CreationDate": float,
@@ -5645,14 +5870,15 @@
     "AwsLambdaFunctionCodeOutputTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
         "ZipFile": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionCodeTypeDef = TypedDict(
     "AwsLambdaFunctionCodeTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
@@ -5663,14 +5889,15 @@
 )
 
 AwsLambdaFunctionDeadLetterConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
     {
         "TargetArn": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionDeadLetterConfigTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
@@ -5679,30 +5906,33 @@
 
 AwsLambdaFunctionLayerOutputTypeDef = TypedDict(
     "AwsLambdaFunctionLayerOutputTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
     },
+    total=False,
 )
 
 AwsLambdaFunctionTracingConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionTracingConfigOutputTypeDef",
     {
         "Mode": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionLayerTypeDef = TypedDict(
     "AwsLambdaFunctionLayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
@@ -5730,14 +5960,15 @@
 
 AwsLambdaFunctionEnvironmentErrorOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
@@ -5748,14 +5979,15 @@
 AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsOutputTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": List[str],
         "CreatedDate": str,
     },
+    total=False,
 )
 
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
@@ -5765,14 +5997,15 @@
 )
 
 AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
     {
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     {
         "SubnetId": str,
     },
@@ -5782,14 +6015,15 @@
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
         "MasterUserPassword": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
@@ -5799,14 +6033,15 @@
 )
 
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
@@ -5818,51 +6053,56 @@
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
         "EnforceHTTPS": bool,
         "CustomEndpoint": str,
         "TLSSecurityPolicy": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
@@ -5916,14 +6156,15 @@
 
 AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
@@ -5933,14 +6174,15 @@
 
 AwsRdsDbClusterAssociatedRoleOutputTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
@@ -5952,40 +6194,44 @@
     "AwsRdsDbClusterMemberOutputTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
         "DbInstanceIdentifier": str,
         "DbClusterParameterGroupStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterOptionGroupMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
     {
         "DbClusterOptionGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbDomainMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbDomainMembershipOutputTypeDef",
     {
         "Domain": str,
         "Status": str,
         "Fqdn": str,
         "IamRoleName": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterMemberTypeDef = TypedDict(
     "AwsRdsDbClusterMemberTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
@@ -6026,14 +6272,15 @@
 
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
+    total=False,
 )
 
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": Sequence[str],
@@ -6044,14 +6291,15 @@
 AwsRdsDbInstanceAssociatedRoleOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
@@ -6063,48 +6311,53 @@
 AwsRdsDbInstanceEndpointOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointOutputTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
+    total=False,
 )
 
 AwsRdsDbOptionGroupMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbOptionGroupMembershipOutputTypeDef",
     {
         "OptionGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbParameterGroupOutputTypeDef = TypedDict(
     "AwsRdsDbParameterGroupOutputTypeDef",
     {
         "DbParameterGroupName": str,
         "ParameterApplyStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbProcessorFeatureOutputTypeDef = TypedDict(
     "AwsRdsDbProcessorFeatureOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsRdsDbStatusInfoOutputTypeDef = TypedDict(
     "AwsRdsDbStatusInfoOutputTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceEndpointTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
@@ -6153,14 +6406,15 @@
 
 AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
+    total=False,
 )
 
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
@@ -6172,22 +6426,24 @@
     "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
         "Ec2SecurityGroupOwnerId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupIpRangeOutputTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
     {
         "CidrIp": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
@@ -6207,14 +6463,15 @@
 )
 
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
     {
         "Name": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
@@ -6231,14 +6488,15 @@
         "EventSubscriptionArn": str,
         "SnsTopicArn": str,
         "SourceIdsList": List[str],
         "SourceType": str,
         "Status": str,
         "SubscriptionCreationTime": str,
     },
+    total=False,
 )
 
 AwsRdsEventSubscriptionDetailsTypeDef = TypedDict(
     "AwsRdsEventSubscriptionDetailsTypeDef",
     {
         "CustSubscriptionId": str,
         "CustomerAwsId": str,
@@ -6257,14 +6515,15 @@
 AwsRedshiftClusterClusterNodeOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeOutputTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
         "PublicIpAddress": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterNodeTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
@@ -6276,14 +6535,15 @@
 AwsRedshiftClusterClusterParameterStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterParameterStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
@@ -6294,14 +6554,15 @@
 
 AwsRedshiftClusterClusterSecurityGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterSecurityGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
@@ -6313,14 +6574,15 @@
     "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
@@ -6333,14 +6595,15 @@
 AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
         "DeferMaintenanceStartTime": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterDeferredMaintenanceWindowTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
@@ -6351,51 +6614,56 @@
 
 AwsRedshiftClusterElasticIpStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterEndpointOutputTypeDef = TypedDict(
     "AwsRedshiftClusterEndpointOutputTypeDef",
     {
         "Address": str,
         "Port": int,
     },
+    total=False,
 )
 
 AwsRedshiftClusterHsmStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterHsmStatusOutputTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "HsmConfigurationIdentifier": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterIamRoleOutputTypeDef = TypedDict(
     "AwsRedshiftClusterIamRoleOutputTypeDef",
     {
         "ApplyStatus": str,
         "IamRoleArn": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterLoggingStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterLoggingStatusOutputTypeDef",
     {
         "BucketName": str,
         "LastFailureMessage": str,
         "LastFailureTime": str,
         "LastSuccessfulDeliveryTime": str,
         "LoggingEnabled": bool,
         "S3KeyPrefix": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterPendingModifiedValuesOutputTypeDef = TypedDict(
     "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
     {
         "AutomatedSnapshotRetentionPeriod": int,
         "ClusterIdentifier": str,
@@ -6405,42 +6673,46 @@
         "EnhancedVpcRouting": bool,
         "MaintenanceTrackName": str,
         "MasterUserPassword": str,
         "NodeType": str,
         "NumberOfNodes": int,
         "PubliclyAccessible": bool,
     },
+    total=False,
 )
 
 AwsRedshiftClusterResizeInfoOutputTypeDef = TypedDict(
     "AwsRedshiftClusterResizeInfoOutputTypeDef",
     {
         "AllowCancelResize": bool,
         "ResizeType": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterRestoreStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterRestoreStatusOutputTypeDef",
     {
         "CurrentRestoreRateInMegaBytesPerSecond": float,
         "ElapsedTimeInSeconds": int,
         "EstimatedTimeToCompletionInSeconds": int,
         "ProgressInMegaBytes": int,
         "SnapshotSizeInMegaBytes": int,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterVpcSecurityGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
     {
         "Status": str,
         "VpcSecurityGroupId": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterElasticIpStatusTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
@@ -6542,14 +6814,15 @@
     "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
         "IgnorePublicAcls": bool,
         "RestrictPublicBuckets": bool,
     },
+    total=False,
 )
 
 AwsS3AccountPublicAccessBlockDetailsTypeDef = TypedDict(
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
@@ -6560,14 +6833,15 @@
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
     {
         "DaysAfterInitiation": int,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef = (
     TypedDict(
         "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
         {
             "DaysAfterInitiation": int,
@@ -6578,23 +6852,25 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
     {
         "Days": int,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
     {
         "Date": str,
         "Days": int,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     {
         "Days": int,
         "StorageClass": str,
@@ -6614,14 +6890,15 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -6631,14 +6908,15 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -6648,14 +6926,15 @@
 
 AwsS3BucketBucketVersioningConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketVersioningConfigurationTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
@@ -6665,14 +6944,15 @@
 
 AwsS3BucketLoggingConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationOutputTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
     },
+    total=False,
 )
 
 AwsS3BucketLoggingConfigurationTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
@@ -6682,14 +6962,15 @@
 
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
@@ -6700,14 +6981,15 @@
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
     {
         "Days": int,
         "Mode": str,
         "Years": int,
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     {
         "Days": int,
         "Mode": str,
@@ -6718,14 +7000,15 @@
 
 AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
@@ -6735,14 +7018,15 @@
 
 AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRedirectToTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
@@ -6752,14 +7036,15 @@
 
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
@@ -6772,14 +7057,15 @@
     {
         "Hostname": str,
         "HttpRedirectCode": str,
         "Protocol": str,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     {
         "Hostname": str,
         "HttpRedirectCode": str,
@@ -6796,14 +7082,15 @@
         "LastModified": str,
         "ETag": str,
         "VersionId": str,
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
+    total=False,
 )
 
 AwsS3ObjectDetailsTypeDef = TypedDict(
     "AwsS3ObjectDetailsTypeDef",
     {
         "LastModified": str,
         "ETag": str,
@@ -6816,14 +7103,15 @@
 )
 
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
+    total=False,
 )
 
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
@@ -6831,14 +7119,15 @@
 )
 
 AwsSecretsManagerSecretRotationRulesOutputTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
+    total=False,
 )
 
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
@@ -6846,28 +7135,31 @@
 )
 
 BooleanFilterOutputTypeDef = TypedDict(
     "BooleanFilterOutputTypeDef",
     {
         "Value": bool,
     },
+    total=False,
 )
 
 IpFilterOutputTypeDef = TypedDict(
     "IpFilterOutputTypeDef",
     {
         "Cidr": str,
     },
+    total=False,
 )
 
 KeywordFilterOutputTypeDef = TypedDict(
     "KeywordFilterOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 BooleanFilterTypeDef = TypedDict(
     "BooleanFilterTypeDef",
     {
         "Value": bool,
     },
@@ -6902,89 +7194,117 @@
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
 
-MalwareOutputTypeDef = TypedDict(
-    "MalwareOutputTypeDef",
+_RequiredMalwareOutputTypeDef = TypedDict(
+    "_RequiredMalwareOutputTypeDef",
     {
         "Name": str,
+    },
+)
+_OptionalMalwareOutputTypeDef = TypedDict(
+    "_OptionalMalwareOutputTypeDef",
+    {
         "Type": MalwareTypeType,
         "Path": str,
         "State": MalwareStateType,
     },
+    total=False,
 )
 
+
+class MalwareOutputTypeDef(_RequiredMalwareOutputTypeDef, _OptionalMalwareOutputTypeDef):
+    pass
+
+
 NoteOutputTypeDef = TypedDict(
     "NoteOutputTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
         "UpdatedAt": str,
     },
 )
 
-PatchSummaryOutputTypeDef = TypedDict(
-    "PatchSummaryOutputTypeDef",
+_RequiredPatchSummaryOutputTypeDef = TypedDict(
+    "_RequiredPatchSummaryOutputTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalPatchSummaryOutputTypeDef = TypedDict(
+    "_OptionalPatchSummaryOutputTypeDef",
+    {
         "InstalledCount": int,
         "MissingCount": int,
         "FailedCount": int,
         "InstalledOtherCount": int,
         "InstalledRejectedCount": int,
         "InstalledPendingReboot": int,
         "OperationStartTime": str,
         "OperationEndTime": str,
         "RebootOption": str,
         "Operation": str,
     },
+    total=False,
 )
 
+
+class PatchSummaryOutputTypeDef(
+    _RequiredPatchSummaryOutputTypeDef, _OptionalPatchSummaryOutputTypeDef
+):
+    pass
+
+
 ProcessDetailsOutputTypeDef = TypedDict(
     "ProcessDetailsOutputTypeDef",
     {
         "Name": str,
         "Path": str,
         "Pid": int,
         "ParentPid": int,
         "LaunchedAt": str,
         "TerminatedAt": str,
     },
+    total=False,
 )
 
 SeverityOutputTypeDef = TypedDict(
     "SeverityOutputTypeDef",
     {
         "Product": float,
         "Label": SeverityLabelType,
         "Normalized": int,
         "Original": str,
     },
+    total=False,
 )
 
 ThreatIntelIndicatorOutputTypeDef = TypedDict(
     "ThreatIntelIndicatorOutputTypeDef",
     {
         "Type": ThreatIntelIndicatorTypeType,
         "Value": str,
         "Category": ThreatIntelIndicatorCategoryType,
         "LastObservedAt": str,
         "Source": str,
         "SourceUrl": str,
     },
+    total=False,
 )
 
 WorkflowOutputTypeDef = TypedDict(
     "WorkflowOutputTypeDef",
     {
         "Status": WorkflowStatusType,
     },
+    total=False,
 )
 
 _RequiredMalwareTypeDef = TypedDict(
     "_RequiredMalwareTypeDef",
     {
         "Name": str,
     },
@@ -7088,14 +7408,15 @@
 
 AwsSnsTopicSubscriptionOutputTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionOutputTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsSnsTopicSubscriptionTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
@@ -7107,14 +7428,15 @@
     "AwsSqsQueueDetailsOutputTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
         "QueueName": str,
         "DeadLetterTargetArn": str,
     },
+    total=False,
 )
 
 AwsSqsQueueDetailsTypeDef = TypedDict(
     "AwsSqsQueueDetailsTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
@@ -7142,14 +7464,15 @@
         "ComplianceType": str,
         "PatchBaselineId": str,
         "OverallSeverity": str,
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
+    total=False,
 )
 
 AwsSsmComplianceSummaryTypeDef = TypedDict(
     "AwsSsmComplianceSummaryTypeDef",
     {
         "Status": str,
         "CompliantCriticalCount": int,
@@ -7174,14 +7497,15 @@
 )
 
 AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     {
         "Enabled": bool,
     },
@@ -7189,14 +7513,15 @@
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
     {
         "LogGroupArn": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     {
         "LogGroupArn": str,
     },
@@ -7206,14 +7531,15 @@
 AwsWafRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7225,14 +7551,15 @@
 AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7244,14 +7571,15 @@
 AwsWafRegionalRulePredicateListDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7261,14 +7589,15 @@
 )
 
 AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7276,14 +7605,15 @@
 )
 
 AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7291,14 +7621,15 @@
 )
 
 AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7308,14 +7639,15 @@
 AwsWafRulePredicateListDetailsOutputTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7325,14 +7657,15 @@
 )
 
 AwsWafRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7340,28 +7673,31 @@
 )
 
 WafActionOutputTypeDef = TypedDict(
     "WafActionOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 WafExcludedRuleOutputTypeDef = TypedDict(
     "WafExcludedRuleOutputTypeDef",
     {
         "RuleId": str,
     },
+    total=False,
 )
 
 WafOverrideActionOutputTypeDef = TypedDict(
     "WafOverrideActionOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 WafActionTypeDef = TypedDict(
     "WafActionTypeDef",
     {
         "Type": str,
     },
@@ -7386,14 +7722,15 @@
 
 AwsWafv2CustomHttpHeaderOutputTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -7404,14 +7741,15 @@
 AwsWafv2VisibilityConfigDetailsOutputTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
         "SampledRequestsEnabled": bool,
     },
+    total=False,
 )
 
 AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
@@ -7421,14 +7759,15 @@
 )
 
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
     {
         "ImmunityTime": int,
     },
+    total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     {
         "ImmunityTime": int,
     },
@@ -7438,14 +7777,15 @@
 AwsXrayEncryptionConfigDetailsOutputTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsOutputTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
@@ -7475,14 +7815,15 @@
 UnprocessedAutomationRuleTypeDef = TypedDict(
     "UnprocessedAutomationRuleTypeDef",
     {
         "RuleArn": str,
         "ErrorCode": int,
         "ErrorMessage": str,
     },
+    total=False,
 )
 
 BatchDisableStandardsRequestRequestTypeDef = TypedDict(
     "BatchDisableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
     },
@@ -7532,47 +7873,74 @@
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "SecurityControlStatus": ControlStatusType,
     },
 )
 
-UnprocessedSecurityControlTypeDef = TypedDict(
-    "UnprocessedSecurityControlTypeDef",
+_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
+    "_RequiredUnprocessedSecurityControlTypeDef",
     {
         "SecurityControlId": str,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
+    "_OptionalUnprocessedSecurityControlTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
+
+class UnprocessedSecurityControlTypeDef(
+    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
+):
+    pass
+
+
 StandardsControlAssociationIdTypeDef = TypedDict(
     "StandardsControlAssociationIdTypeDef",
     {
         "SecurityControlId": str,
         "StandardsArn": str,
     },
 )
 
-StandardsControlAssociationDetailTypeDef = TypedDict(
-    "StandardsControlAssociationDetailTypeDef",
+_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationDetailTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationDetailTypeDef",
+    {
         "RelatedRequirements": List[str],
         "UpdatedAt": datetime,
         "UpdatedReason": str,
         "StandardsControlTitle": str,
         "StandardsControlDescription": str,
         "StandardsControlArns": List[str],
     },
+    total=False,
 )
 
+
+class StandardsControlAssociationDetailTypeDef(
+    _RequiredStandardsControlAssociationDetailTypeDef,
+    _OptionalStandardsControlAssociationDetailTypeDef,
+):
+    pass
+
+
 ImportFindingsErrorTypeDef = TypedDict(
     "ImportFindingsErrorTypeDef",
     {
         "Id": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -7606,14 +7974,15 @@
     "CellOutputTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
     },
+    total=False,
 )
 
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
@@ -7625,33 +7994,47 @@
 
 ClassificationStatusOutputTypeDef = TypedDict(
     "ClassificationStatusOutputTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
+    total=False,
 )
 
 ClassificationStatusTypeDef = TypedDict(
     "ClassificationStatusTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-StatusReasonOutputTypeDef = TypedDict(
-    "StatusReasonOutputTypeDef",
+_RequiredStatusReasonOutputTypeDef = TypedDict(
+    "_RequiredStatusReasonOutputTypeDef",
     {
         "ReasonCode": str,
+    },
+)
+_OptionalStatusReasonOutputTypeDef = TypedDict(
+    "_OptionalStatusReasonOutputTypeDef",
+    {
         "Description": str,
     },
+    total=False,
 )
 
+
+class StatusReasonOutputTypeDef(
+    _RequiredStatusReasonOutputTypeDef, _OptionalStatusReasonOutputTypeDef
+):
+    pass
+
+
 _RequiredStatusReasonTypeDef = TypedDict(
     "_RequiredStatusReasonTypeDef",
     {
         "ReasonCode": str,
     },
 )
 _OptionalStatusReasonTypeDef = TypedDict(
@@ -7669,14 +8052,15 @@
 
 VolumeMountOutputTypeDef = TypedDict(
     "VolumeMountOutputTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
+    total=False,
 )
 
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
@@ -7717,22 +8101,24 @@
 
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
+    total=False,
 )
 
 DateRangeOutputTypeDef = TypedDict(
     "DateRangeOutputTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
+    total=False,
 )
 
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
@@ -7816,29 +8202,40 @@
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
     total=False,
 )
 
-ProductTypeDef = TypedDict(
-    "ProductTypeDef",
+_RequiredProductTypeDef = TypedDict(
+    "_RequiredProductTypeDef",
     {
         "ProductArn": str,
+    },
+)
+_OptionalProductTypeDef = TypedDict(
+    "_OptionalProductTypeDef",
+    {
         "ProductName": str,
         "CompanyName": str,
         "Description": str,
         "Categories": List[str],
         "IntegrationTypes": List[IntegrationTypeType],
         "MarketplaceUrl": str,
         "ActivationUrl": str,
         "ProductSubscriptionResourcePolicy": str,
     },
+    total=False,
 )
 
+
+class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
+    pass
+
+
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
 _OptionalDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
@@ -7868,14 +8265,15 @@
         "ControlId": str,
         "Title": str,
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
+    total=False,
 )
 
 DescribeStandardsRequestRequestTypeDef = TypedDict(
     "DescribeStandardsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -7932,14 +8330,15 @@
     "FilePathsOutputTypeDef",
     {
         "FilePath": str,
         "FileName": str,
         "ResourceId": str,
         "Hash": str,
     },
+    total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
         "FilePath": str,
         "FileName": str,
@@ -7950,39 +8349,43 @@
 )
 
 FindingAggregatorTypeDef = TypedDict(
     "FindingAggregatorTypeDef",
     {
         "FindingAggregatorArn": str,
     },
+    total=False,
 )
 
 FindingHistoryUpdateSourceTypeDef = TypedDict(
     "FindingHistoryUpdateSourceTypeDef",
     {
         "Type": FindingHistoryUpdateSourceTypeType,
         "Identity": str,
     },
+    total=False,
 )
 
 FindingHistoryUpdateTypeDef = TypedDict(
     "FindingHistoryUpdateTypeDef",
     {
         "UpdatedField": str,
         "OldValue": str,
         "NewValue": str,
     },
+    total=False,
 )
 
 FindingProviderSeverityOutputTypeDef = TypedDict(
     "FindingProviderSeverityOutputTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
+    total=False,
 )
 
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
@@ -7991,22 +8394,24 @@
 )
 
 FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
     {
         "ResourceArn": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
     {
         "Priority": int,
         "ResourceArn": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     {
         "ResourceArn": str,
     },
@@ -8026,14 +8431,15 @@
     "InvitationTypeDef",
     {
         "AccountId": str,
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
+    total=False,
 )
 
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
@@ -8089,14 +8495,15 @@
         "Email": str,
         "MasterId": str,
         "AdministratorId": str,
         "MemberStatus": str,
         "InvitedAt": datetime,
         "UpdatedAt": datetime,
     },
+    total=False,
 )
 
 InsightResultValueTypeDef = TypedDict(
     "InsightResultValueTypeDef",
     {
         "GroupByAttributeValue": str,
         "Count": int,
@@ -8206,42 +8613,57 @@
 class ListStandardsControlAssociationsRequestRequestTypeDef(
     _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
     _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
 ):
     pass
 
 
-StandardsControlAssociationSummaryTypeDef = TypedDict(
-    "StandardsControlAssociationSummaryTypeDef",
+_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationSummaryTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationSummaryTypeDef",
+    {
         "RelatedRequirements": List[str],
         "UpdatedAt": datetime,
         "UpdatedReason": str,
         "StandardsControlTitle": str,
         "StandardsControlDescription": str,
     },
+    total=False,
 )
 
+
+class StandardsControlAssociationSummaryTypeDef(
+    _RequiredStandardsControlAssociationSummaryTypeDef,
+    _OptionalStandardsControlAssociationSummaryTypeDef,
+):
+    pass
+
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
 PortRangeOutputTypeDef = TypedDict(
     "PortRangeOutputTypeDef",
     {
         "Begin": int,
         "End": int,
     },
+    total=False,
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
@@ -8252,22 +8674,24 @@
 RangeOutputTypeDef = TypedDict(
     "RangeOutputTypeDef",
     {
         "Start": int,
         "End": int,
         "StartColumn": int,
     },
+    total=False,
 )
 
 RecordOutputTypeDef = TypedDict(
     "RecordOutputTypeDef",
     {
         "JsonPath": str,
         "RecordIndex": int,
     },
+    total=False,
 )
 
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Start": int,
         "End": int,
@@ -8287,14 +8711,15 @@
 
 RecommendationOutputTypeDef = TypedDict(
     "RecommendationOutputTypeDef",
     {
         "Text": str,
         "Url": str,
     },
+    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
@@ -8305,14 +8730,15 @@
 RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceListDetailsOutputTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": List[str],
         "Targets": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
@@ -8327,22 +8753,24 @@
         "Destination": str,
         "DestinationPort": str,
         "Direction": str,
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     {
         "Keyword": str,
         "Settings": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     {
         "Destination": str,
         "DestinationPort": str,
@@ -8365,14 +8793,15 @@
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
@@ -8381,14 +8810,15 @@
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
     {
         "AddressDefinition": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     {
         "AddressDefinition": str,
     },
@@ -8397,29 +8827,32 @@
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
     {
         "AddressDefinition": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     {
         "Flags": List[str],
         "Masks": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
@@ -8445,14 +8878,15 @@
 )
 
 RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     {
         "Definition": List[str],
     },
+    total=False,
 )
 
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
@@ -8460,14 +8894,15 @@
 )
 
 RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     {
         "Definition": List[str],
     },
+    total=False,
 )
 
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
@@ -8485,14 +8920,15 @@
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
         "SourceLayerHash": str,
         "SourceLayerArn": str,
     },
+    total=False,
 )
 
 SoftwarePackageTypeDef = TypedDict(
     "SoftwarePackageTypeDef",
     {
         "Name": str,
         "Version": str,
@@ -8511,46 +8947,62 @@
 
 StandardsManagedByTypeDef = TypedDict(
     "StandardsManagedByTypeDef",
     {
         "Company": str,
         "Product": str,
     },
+    total=False,
 )
 
 StandardsControlAssociationIdOutputTypeDef = TypedDict(
     "StandardsControlAssociationIdOutputTypeDef",
     {
         "SecurityControlId": str,
         "StandardsArn": str,
     },
 )
 
-StandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "StandardsControlAssociationUpdateOutputTypeDef",
+_RequiredStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationUpdateOutputTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationUpdateOutputTypeDef",
+    {
         "UpdatedReason": str,
     },
+    total=False,
 )
 
+
+class StandardsControlAssociationUpdateOutputTypeDef(
+    _RequiredStandardsControlAssociationUpdateOutputTypeDef,
+    _OptionalStandardsControlAssociationUpdateOutputTypeDef,
+):
+    pass
+
+
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
         "StatusReasonCode": StatusReasonCodeType,
     },
 )
 
 StatelessCustomPublishMetricActionDimensionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 StatelessCustomPublishMetricActionDimensionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     {
         "Value": str,
     },
@@ -8669,25 +9121,38 @@
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
 
-VulnerabilityVendorOutputTypeDef = TypedDict(
-    "VulnerabilityVendorOutputTypeDef",
+_RequiredVulnerabilityVendorOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityVendorOutputTypeDef",
     {
         "Name": str,
+    },
+)
+_OptionalVulnerabilityVendorOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityVendorOutputTypeDef",
+    {
         "Url": str,
         "VendorSeverity": str,
         "VendorCreatedAt": str,
         "VendorUpdatedAt": str,
     },
+    total=False,
 )
 
+
+class VulnerabilityVendorOutputTypeDef(
+    _RequiredVulnerabilityVendorOutputTypeDef, _OptionalVulnerabilityVendorOutputTypeDef
+):
+    pass
+
+
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -8720,14 +9185,15 @@
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsOutputTypeDef,
         "Country": CountryOutputTypeDef,
         "City": CityOutputTypeDef,
         "GeoLocation": GeoLocationOutputTypeDef,
     },
+    total=False,
 )
 
 ActionRemoteIpDetailsTypeDef = TypedDict(
     "ActionRemoteIpDetailsTypeDef",
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsTypeDef,
@@ -8743,14 +9209,15 @@
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": List[AdjustmentOutputTypeDef],
     },
+    total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
@@ -8767,14 +9234,15 @@
         "AssociationState": AssociationStateDetailsOutputTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
@@ -8795,14 +9263,15 @@
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
         "Workflow": WorkflowUpdateOutputTypeDef,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
     },
+    total=False,
 )
 
 AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateTypeDef",
     {
         "Note": NoteUpdateTypeDef,
         "Severity": SeverityUpdateTypeDef,
@@ -8822,14 +9291,15 @@
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
         "Pending": AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
@@ -8849,14 +9319,15 @@
         "CreatedDate": str,
         "Version": str,
         "BinaryMediaTypes": List[str],
         "MinimumCompressionSize": int,
         "ApiKeySource": str,
         "EndpointConfiguration": AwsApiGatewayEndpointConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
@@ -8887,14 +9358,15 @@
         "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
         "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
         "TracingEnabled": bool,
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
+    total=False,
 )
 
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
     "AwsApiGatewayStageDetailsTypeDef",
     {
         "DeploymentId": str,
         "ClientCertificateId": str,
@@ -8926,14 +9398,15 @@
         "Description": str,
         "Version": str,
         "Name": str,
         "ProtocolType": str,
         "RouteSelectionExpression": str,
         "CorsConfiguration": AwsCorsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": str,
         "ApiId": str,
@@ -8962,14 +9435,15 @@
         "StageName": str,
         "StageVariables": Dict[str, str],
         "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
+    total=False,
 )
 
 AwsApiGatewayV2StageDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
@@ -8992,14 +9466,15 @@
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
@@ -9010,14 +9485,15 @@
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
     {
         "EncryptionConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
@@ -9030,14 +9506,15 @@
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
         "Overrides": List[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
@@ -9051,14 +9528,15 @@
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
         "NoDevice": bool,
         "VirtualName": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
@@ -9070,14 +9548,15 @@
 
 AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
@@ -9090,14 +9569,15 @@
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
         "AccessPolicy": str,
     },
+    total=False,
 )
 
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
@@ -9127,14 +9607,15 @@
         "ResourceArn": str,
         "ResourceType": str,
         "SourceBackupVaultArn": str,
         "Status": str,
         "StatusMessage": str,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointDetailsTypeDef",
     {
         "BackupSizeInBytes": int,
         "BackupVaultArn": str,
@@ -9165,14 +9646,15 @@
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": List[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateDomainValidationOptionTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
@@ -9199,14 +9681,15 @@
         "RoleArn": str,
         "StackId": str,
         "StackName": str,
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
+    total=False,
 )
 
 AwsCloudFormationStackDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsTypeDef",
     {
         "Capabilities": Sequence[str],
         "CreationTime": str,
@@ -9228,14 +9711,15 @@
 )
 
 AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionCacheBehaviorOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
@@ -9248,14 +9732,15 @@
         "HttpPort": int,
         "HttpsPort": int,
         "OriginKeepaliveTimeout": int,
         "OriginProtocolPolicy": str,
         "OriginReadTimeout": int,
         "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": int,
         "HttpsPort": int,
@@ -9268,14 +9753,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     },
@@ -9304,14 +9790,15 @@
         "Period": int,
         "Statistic": str,
         "Threshold": float,
         "ThresholdMetricId": str,
         "TreatMissingData": str,
         "Unit": str,
     },
+    total=False,
 )
 
 AwsCloudWatchAlarmDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDetailsTypeDef",
     {
         "ActionsEnabled": bool,
         "AlarmActions": Sequence[str],
@@ -9347,14 +9834,15 @@
             AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef
         ],
         "PrivilegedMode": bool,
         "ImagePullCredentialsType": str,
         "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": Sequence[
@@ -9370,14 +9858,15 @@
 
 AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
@@ -9394,24 +9883,26 @@
         "IndexSizeBytes": int,
         "IndexStatus": str,
         "ItemCount": int,
         "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
         "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": str,
         "IndexName": str,
         "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": bool,
         "IndexArn": str,
@@ -9439,14 +9930,15 @@
 
 AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
@@ -9467,14 +9959,15 @@
         "SubnetId": str,
         "LaunchedAt": str,
         "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsOutputTypeDef,
         "Monitoring": AwsEc2InstanceMonitoringDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
         "Type": str,
         "ImageId": str,
@@ -9497,14 +9990,15 @@
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
         "NoDevice": str,
         "VirtualName": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
@@ -9516,14 +10010,15 @@
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
@@ -9533,14 +10028,15 @@
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
@@ -9579,14 +10075,15 @@
         "RequireHibernateSupport": bool,
         "SpotMaxPricePercentageOverLowestPrice": int,
         "TotalLocalStorageGB": (
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef
         ),
         "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
         "AcceleratorCount": (
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
@@ -9652,14 +10149,15 @@
         "PrivateIpAddress": str,
         "PrivateIpAddresses": List[
             AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
@@ -9700,14 +10198,15 @@
         "IcmpTypeCode": IcmpTypeCodeOutputTypeDef,
         "Ipv6CidrBlock": str,
         "PortRange": PortRangeFromToOutputTypeDef,
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
+    total=False,
 )
 
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
@@ -9729,14 +10228,15 @@
         "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef],
         "SourceDestCheck": bool,
         "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef],
         "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     {
         "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
@@ -9757,14 +10257,15 @@
         "FromPort": int,
         "ToPort": int,
         "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef],
         "IpRanges": List[AwsEc2SecurityGroupIpRangeOutputTypeDef],
         "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeOutputTypeDef],
         "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
@@ -9790,14 +10291,15 @@
         "OwnerId": str,
         "State": str,
         "SubnetArn": str,
         "SubnetId": str,
         "VpcId": str,
         "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
         "AssignIpv6AddressOnCreation": bool,
         "AvailabilityZone": str,
@@ -9827,14 +10329,15 @@
         "Status": str,
         "KmsKeyId": str,
         "Attachments": List[AwsEc2VolumeAttachmentOutputTypeDef],
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
+    total=False,
 )
 
 AwsEc2VolumeDetailsTypeDef = TypedDict(
     "AwsEc2VolumeDetailsTypeDef",
     {
         "CreateTime": str,
         "DeviceName": str,
@@ -9855,14 +10358,15 @@
     "AwsEc2VpcDetailsOutputTypeDef",
     {
         "CidrBlockAssociationSet": List[CidrBlockAssociationOutputTypeDef],
         "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2VpcDetailsTypeDef = TypedDict(
     "AwsEc2VpcDetailsTypeDef",
     {
         "CidrBlockAssociationSet": Sequence[CidrBlockAssociationTypeDef],
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
@@ -9883,14 +10387,15 @@
         "NetworkLoadBalancerArns": List[str],
         "PrivateDnsName": str,
         "ServiceId": str,
         "ServiceName": str,
         "ServiceState": str,
         "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
         "AcceptanceRequired": bool,
         "AvailabilityZones": Sequence[str],
@@ -9914,14 +10419,15 @@
         "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsOutputTypeDef],
         "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcInfoPeeringOptionsDetailsOutputTypeDef,
         "Region": str,
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     {
         "CidrBlock": str,
         "CidrBlockSet": Sequence[VpcInfoCidrBlockSetDetailsTypeDef],
@@ -9936,14 +10442,15 @@
 
 AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
@@ -9959,14 +10466,15 @@
             AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef
         ),
         "ImageTagMutability": str,
         "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
         "RepositoryName": str,
         "RepositoryPolicyText": str,
     },
+    total=False,
 )
 
 AwsEcrRepositoryDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryDetailsTypeDef",
     {
         "Arn": str,
         "ImageScanningConfiguration": AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
@@ -9981,14 +10489,15 @@
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
         "Logging": str,
     },
+    total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": (
@@ -10003,14 +10512,15 @@
     "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": str,
         "Image": str,
         "MountPoints": List[AwsMountPointOutputTypeDef],
         "Privileged": bool,
     },
+    total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
     {
         "Name": str,
         "Image": str,
@@ -10025,14 +10535,15 @@
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef
         ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
@@ -10046,14 +10557,15 @@
 AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     {
         "AwsVpcConfiguration": (
             AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     },
@@ -10073,14 +10585,15 @@
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
         "Tmpfs": List[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": (
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
@@ -10104,14 +10617,15 @@
     {
         "LogDriver": str,
         "Options": Dict[str, str],
         "SecretOptions": List[
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     {
         "LogDriver": str,
         "Options": Mapping[str, str],
@@ -10127,14 +10641,15 @@
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": List[
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef
         ],
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": Sequence[
@@ -10152,14 +10667,15 @@
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef
         ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
         "AuthorizationConfig": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
@@ -10174,14 +10690,15 @@
 
 AwsEcsTaskVolumeDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsOutputTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEcsTaskVolumeDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsTypeDef,
@@ -10191,14 +10708,15 @@
 
 AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
         "Path": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
@@ -10207,14 +10725,15 @@
 )
 
 AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsOutputTypeDef",
     {
         "ClusterLogging": List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef],
     },
@@ -10237,14 +10756,15 @@
         "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef],
         "PlatformArn": str,
         "SolutionStackName": str,
         "Status": str,
         "Tier": AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
         "VersionLabel": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     {
         "ApplicationName": str,
         "Cname": str,
@@ -10275,14 +10795,15 @@
         "InstanceCount": int,
         "InstanceType": str,
         "ZoneAwarenessConfig": (
             AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
         ),
         "ZoneAwarenessEnabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
@@ -10300,14 +10821,15 @@
 AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
@@ -10319,14 +10841,15 @@
 AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
         "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyOutputTypeDef],
         "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyOutputTypeDef],
         "OtherPolicies": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": Sequence[AwsElbAppCookieStickinessPolicyTypeDef],
         "LbCookieStickinessPolicies": Sequence[AwsElbLbCookieStickinessPolicyTypeDef],
@@ -10340,14 +10863,15 @@
     {
         "AccessLog": AwsElbLoadBalancerAccessLogOutputTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
         "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
         "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
         "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeOutputTypeDef],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
         "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
@@ -10360,14 +10884,15 @@
 
 AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerOutputTypeDef,
         "PolicyNames": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": Sequence[str],
@@ -10386,14 +10911,15 @@
         "Scheme": str,
         "SecurityGroups": List[str],
         "State": LoadBalancerStateOutputTypeDef,
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeOutputTypeDef],
     },
+    total=False,
 )
 
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
@@ -10411,14 +10937,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
     },
@@ -10426,14 +10953,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
     },
@@ -10442,14 +10970,15 @@
 
 AwsIamAccessKeySessionContextOutputTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextOutputTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesOutputTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
@@ -10463,14 +10992,15 @@
         "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
         "GroupPolicyList": List[AwsIamGroupPolicyOutputTypeDef],
         "Path": str,
     },
+    total=False,
 )
 
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
@@ -10488,14 +11018,15 @@
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
         "Roles": List[AwsIamInstanceProfileRoleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
@@ -10518,14 +11049,15 @@
         "Path": str,
         "PermissionsBoundaryUsageCount": int,
         "PolicyId": str,
         "PolicyName": str,
         "PolicyVersionList": List[AwsIamPolicyVersionOutputTypeDef],
         "UpdateDate": str,
     },
+    total=False,
 )
 
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
     {
         "AttachmentCount": int,
         "CreateDate": str,
@@ -10550,14 +11082,15 @@
         "GroupList": List[str],
         "Path": str,
         "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
         "UserId": str,
         "UserName": str,
         "UserPolicyList": List[AwsIamUserPolicyOutputTypeDef],
     },
+    total=False,
 )
 
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
@@ -10576,14 +11109,15 @@
     {
         "Name": str,
         "Arn": str,
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
         "ShardCount": int,
         "RetentionPeriodHours": int,
     },
+    total=False,
 )
 
 AwsKinesisStreamDetailsTypeDef = TypedDict(
     "AwsKinesisStreamDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
@@ -10596,14 +11130,15 @@
 
 AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": Dict[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
     },
+    total=False,
 )
 
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
         "Variables": Mapping[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
@@ -10621,14 +11156,15 @@
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyChangeProtection": bool,
         "SubnetChangeProtection": bool,
         "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     {
         "DeleteProtection": bool,
         "Description": str,
@@ -10647,14 +11183,15 @@
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
         "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
@@ -10675,14 +11212,15 @@
         ),
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
@@ -10703,14 +11241,15 @@
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
@@ -10756,14 +11295,15 @@
         "DbClusterParameterGroup": str,
         "DbSubnetGroup": str,
         "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipOutputTypeDef],
         "DbClusterIdentifier": str,
         "DbClusterMembers": List[AwsRdsDbClusterMemberOutputTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
+    total=False,
 )
 
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
     {
         "AllocatedStorage": int,
         "AvailabilityZones": Sequence[str],
@@ -10827,14 +11367,15 @@
         "DbClusterIdentifier": str,
         "DbClusterSnapshotIdentifier": str,
         "IamDatabaseAuthenticationEnabled": bool,
         "DbClusterSnapshotAttributes": List[
             AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SnapshotCreateTime": str,
@@ -10888,14 +11429,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "Timezone": str,
         "IamDatabaseAuthenticationEnabled": bool,
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
         "DbiResourceId": str,
     },
+    total=False,
 )
 
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
     {
         "DbSnapshotIdentifier": str,
         "DbInstanceIdentifier": str,
@@ -10943,14 +11485,15 @@
         "DbInstanceIdentifier": str,
         "StorageType": str,
         "CaCertificateIdentifier": str,
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
     },
+    total=False,
 )
 
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
         "DbInstanceClass": str,
         "AllocatedStorage": int,
@@ -10978,14 +11521,15 @@
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
         "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef],
         "IpRanges": List[AwsRdsDbSecurityGroupIpRangeOutputTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
@@ -11001,14 +11545,15 @@
 AwsRdsDbSubnetGroupSubnetOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
         "SubnetStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupSubnetTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
@@ -11020,14 +11565,15 @@
 AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
         "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusOutputTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     {
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
@@ -11039,14 +11585,15 @@
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
@@ -11056,14 +11603,15 @@
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
         "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
@@ -11073,14 +11621,15 @@
 AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
     {
         "DefaultRetention": (
             AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     {
         "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     },
@@ -11088,14 +11637,15 @@
 )
 
 AwsS3BucketServerSideEncryptionRuleOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
@@ -11104,14 +11654,15 @@
 
 AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
@@ -11141,14 +11692,15 @@
         "RoleArn": str,
         "RootAccess": str,
         "SecurityGroups": List[str],
         "SubnetId": str,
         "Url": str,
         "VolumeSizeInGB": int,
     },
+    total=False,
 )
 
 AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     {
         "AcceleratorTypes": Sequence[str],
         "AdditionalCodeRepositories": Sequence[str],
@@ -11184,14 +11736,15 @@
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaArn": str,
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
+    total=False,
 )
 
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
@@ -11279,14 +11832,15 @@
         "SqsFailureFeedbackRoleArn": str,
         "ApplicationSuccessFeedbackRoleArn": str,
         "FirehoseSuccessFeedbackRoleArn": str,
         "FirehoseFailureFeedbackRoleArn": str,
         "HttpSuccessFeedbackRoleArn": str,
         "HttpFailureFeedbackRoleArn": str,
     },
+    total=False,
 )
 
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
@@ -11304,14 +11858,15 @@
 )
 
 AwsSsmPatchOutputTypeDef = TypedDict(
     "AwsSsmPatchOutputTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryOutputTypeDef,
     },
+    total=False,
 )
 
 AwsSsmPatchTypeDef = TypedDict(
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
@@ -11319,14 +11874,15 @@
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
@@ -11339,14 +11895,15 @@
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11364,14 +11921,15 @@
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11387,14 +11945,15 @@
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": List[AwsWafRegionalRulePredicateListDetailsOutputTypeDef],
         "RuleId": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11408,14 +11967,15 @@
     "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
@@ -11430,14 +11990,15 @@
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
@@ -11452,14 +12013,15 @@
     "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": List[AwsWafRulePredicateListDetailsOutputTypeDef],
         "RuleId": str,
     },
+    total=False,
 )
 
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11473,14 +12035,15 @@
     "AwsWafRuleGroupRulesDetailsOutputTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
@@ -11496,14 +12059,15 @@
         "Action": WafActionOutputTypeDef,
         "ExcludedRules": List[WafExcludedRuleOutputTypeDef],
         "OverrideAction": WafOverrideActionOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafWebAclRuleTypeDef = TypedDict(
     "AwsWafWebAclRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "ExcludedRules": Sequence[WafExcludedRuleTypeDef],
@@ -11516,23 +12080,25 @@
 )
 
 AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
         "InsertHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
         "ResponseHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
@@ -11550,14 +12116,15 @@
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
@@ -11781,14 +12348,15 @@
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": List[str],
         "StatusReasons": List[StatusReasonOutputTypeDef],
         "SecurityControlId": str,
         "AssociatedStandards": List[AssociatedStandardOutputTypeDef],
     },
+    total=False,
 )
 
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
@@ -11806,14 +12374,15 @@
         "Name": str,
         "ImageId": str,
         "ImageName": str,
         "LaunchedAt": str,
         "VolumeMounts": List[VolumeMountOutputTypeDef],
         "Privileged": bool,
     },
+    total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
@@ -11869,14 +12438,15 @@
 DateFilterOutputTypeDef = TypedDict(
     "DateFilterOutputTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeOutputTypeDef,
     },
+    total=False,
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
@@ -12069,14 +12639,15 @@
     "ThreatOutputTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
         "FilePaths": List[FilePathsOutputTypeDef],
     },
+    total=False,
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
@@ -12101,25 +12672,27 @@
         "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
         "UpdateTime": datetime,
         "FindingCreated": bool,
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
+    total=False,
 )
 
 FindingProviderFieldsOutputTypeDef = TypedDict(
     "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
         "Severity": FindingProviderSeverityOutputTypeDef,
         "Types": List[str],
     },
+    total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
@@ -12212,22 +12785,24 @@
         "SourceDomain": str,
         "SourceMac": str,
         "DestinationIpV4": str,
         "DestinationIpV6": str,
         "DestinationPort": int,
         "DestinationDomain": str,
     },
+    total=False,
 )
 
 NetworkPathComponentDetailsOutputTypeDef = TypedDict(
     "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": List[str],
         "PortRanges": List[PortRangeOutputTypeDef],
     },
+    total=False,
 )
 
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
@@ -12257,14 +12832,15 @@
 PageOutputTypeDef = TypedDict(
     "PageOutputTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeOutputTypeDef,
         "OffsetRange": RangeOutputTypeDef,
     },
+    total=False,
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeTypeDef,
@@ -12274,14 +12850,15 @@
 )
 
 RemediationOutputTypeDef = TypedDict(
     "RemediationOutputTypeDef",
     {
         "Recommendation": RecommendationOutputTypeDef,
     },
+    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
@@ -12291,14 +12868,15 @@
 RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
         "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
@@ -12315,14 +12893,15 @@
         ],
         "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef],
         "Protocols": List[int],
         "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef],
         "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef],
         "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": Sequence[
             RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
@@ -12338,14 +12917,15 @@
 
 RuleGroupVariablesOutputTypeDef = TypedDict(
     "RuleGroupVariablesOutputTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsOutputTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
@@ -12358,50 +12938,93 @@
     {
         "StandardsArn": str,
         "Name": str,
         "Description": str,
         "EnabledByDefault": bool,
         "StandardsManagedBy": StandardsManagedByTypeDef,
     },
+    total=False,
 )
 
-UnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "UnprocessedStandardsControlAssociationTypeDef",
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
     {
         "StandardsControlAssociationId": StandardsControlAssociationIdOutputTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
-UnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
+
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
+
+
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
     {
         "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateOutputTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
-StandardsSubscriptionTypeDef = TypedDict(
-    "StandardsSubscriptionTypeDef",
+
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
+
+_RequiredStandardsSubscriptionTypeDef = TypedDict(
+    "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
+    },
+)
+_OptionalStandardsSubscriptionTypeDef = TypedDict(
+    "_OptionalStandardsSubscriptionTypeDef",
+    {
         "StandardsStatusReason": StandardsStatusReasonTypeDef,
     },
+    total=False,
 )
 
+
+class StandardsSubscriptionTypeDef(
+    _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
+):
+    pass
+
+
 StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionOutputTypeDef",
     {
         "Dimensions": List[StatelessCustomPublishMetricActionDimensionOutputTypeDef],
     },
+    total=False,
 )
 
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
@@ -12416,35 +13039,38 @@
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
         "DomainDetails": AwsApiCallActionDomainDetailsOutputTypeDef,
         "AffectedResources": Dict[str, str],
         "FirstSeen": str,
         "LastSeen": str,
     },
+    total=False,
 )
 
 NetworkConnectionActionOutputTypeDef = TypedDict(
     "NetworkConnectionActionOutputTypeDef",
     {
         "ConnectionDirection": str,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
         "RemotePortDetails": ActionRemotePortDetailsOutputTypeDef,
         "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
         "Protocol": str,
         "Blocked": bool,
     },
+    total=False,
 )
 
 PortProbeDetailOutputTypeDef = TypedDict(
     "PortProbeDetailOutputTypeDef",
     {
         "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsOutputTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
@@ -12477,27 +13103,40 @@
         "LocalPortDetails": ActionLocalPortDetailsTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
     },
     total=False,
 )
 
-VulnerabilityOutputTypeDef = TypedDict(
-    "VulnerabilityOutputTypeDef",
+_RequiredVulnerabilityOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityOutputTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalVulnerabilityOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityOutputTypeDef",
+    {
         "VulnerablePackages": List[SoftwarePackageOutputTypeDef],
         "Cvss": List[CvssOutputTypeDef],
         "RelatedVulnerabilities": List[str],
         "Vendor": VulnerabilityVendorOutputTypeDef,
         "ReferenceUrls": List[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
+    total=False,
 )
 
+
+class VulnerabilityOutputTypeDef(
+    _RequiredVulnerabilityOutputTypeDef, _OptionalVulnerabilityOutputTypeDef
+):
+    pass
+
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -12524,14 +13163,15 @@
         "AssociationSet": List[AssociationSetDetailsOutputTypeDef],
         "OwnerId": str,
         "PropagatingVgwSet": List[PropagatingVgwSetDetailsOutputTypeDef],
         "RouteTableId": str,
         "RouteSet": List[RouteSetDetailsOutputTypeDef],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
     {
         "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
         "OwnerId": str,
@@ -12545,14 +13185,15 @@
 
 AutomationRulesActionOutputTypeDef = TypedDict(
     "AutomationRulesActionOutputTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateOutputTypeDef,
     },
+    total=False,
 )
 
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
@@ -12580,14 +13221,15 @@
         ),
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": str,
         "SubnetIds": List[str],
         "Users": List[AwsAmazonMqBrokerUsersDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
@@ -12625,14 +13267,15 @@
         "AuthenticationType": str,
         "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
         "AdditionalAuthenticationProviders": List[
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef
         ],
         "WafWebAclArn": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     {
         "ApiId": str,
         "Id": str,
@@ -12655,14 +13298,15 @@
 AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
     {
         "ResultConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     },
@@ -12673,14 +13317,15 @@
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     {
         "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
@@ -12715,14 +13360,15 @@
         "PlacementTenancy": str,
         "RamdiskId": str,
         "SecurityGroups": List[str],
         "SpotPrice": str,
         "UserData": str,
         "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": Sequence[
@@ -12758,14 +13404,15 @@
         "RuleName": str,
         "RuleId": str,
         "EnableContinuousBackup": bool,
         "CompletionWindowMinutes": int,
         "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef],
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
@@ -12786,14 +13433,15 @@
         "DomainValidationOptions": List[
             AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
         ],
         "RenewalStatus": str,
         "RenewalStatusReason": str,
         "UpdatedAt": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     {
         "DomainValidationOptions": Sequence[
             AwsCertificateManagerCertificateDomainValidationOptionTypeDef
@@ -12810,14 +13458,15 @@
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
         "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": str,
         "Id": str,
@@ -12829,14 +13478,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     },
@@ -12852,14 +13502,15 @@
         "Name": str,
         "Source": AwsCodeBuildProjectSourceOutputTypeDef,
         "ServiceRole": str,
         "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
         "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": str,
         "Artifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
@@ -12880,14 +13531,15 @@
         "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef],
         "KmsMasterKeyId": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableReplicaTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaTypeDef",
     {
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
@@ -12939,14 +13591,15 @@
         "Placement": AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
         "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
         "RamDiskId": str,
         "SecurityGroupIdSet": List[str],
         "SecurityGroupSet": List[str],
         "UserData": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
     {
         "BlockDeviceMappingSet": Sequence[
             AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
@@ -12996,14 +13649,15 @@
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
         "Associations": List[AwsEc2NetworkAclAssociationOutputTypeDef],
         "Entries": List[AwsEc2NetworkAclEntryOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
@@ -13021,14 +13675,15 @@
         "GroupName": str,
         "GroupId": str,
         "OwnerId": str,
         "VpcId": str,
         "IpPermissions": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
         "IpPermissionsEgress": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
@@ -13045,14 +13700,15 @@
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "Status": AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "ExpirationTime": str,
@@ -13074,14 +13730,15 @@
         "VpnGatewayId": str,
         "Category": str,
         "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef],
         "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
         "Routes": List[AwsEc2VpnConnectionRoutesDetailsOutputTypeDef],
         "TransitGatewayId": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
         "VpnConnectionId": str,
         "State": str,
@@ -13101,14 +13758,15 @@
 AwsEcsClusterConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsOutputTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
@@ -13139,14 +13797,15 @@
         "Role": str,
         "SchedulingStrategy": str,
         "ServiceArn": str,
         "ServiceName": str,
         "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsOutputTypeDef],
         "TaskDefinition": str,
     },
+    total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
         "CapacityProviderStrategy": Sequence[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
@@ -13235,14 +13894,15 @@
         "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef],
         "User": str,
         "VolumesFrom": List[
             AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef
         ],
         "WorkingDirectory": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     {
         "Command": Sequence[str],
         "Cpu": int,
@@ -13307,14 +13967,15 @@
         ),
         "EfsVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef
         ),
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
         "Name": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
@@ -13335,14 +13996,15 @@
         "CreatedAt": str,
         "StartedAt": str,
         "StartedBy": str,
         "Group": str,
         "Volumes": List[AwsEcsTaskVolumeDetailsOutputTypeDef],
         "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": str,
         "TaskDefinitionArn": str,
@@ -13363,14 +14025,15 @@
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
         "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
@@ -13391,14 +14054,15 @@
         "Endpoint": str,
         "Name": str,
         "ResourcesVpcConfig": AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
         "RoleArn": str,
         "Version": str,
         "Logging": AwsEksClusterLoggingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": str,
         "CertificateAuthorityData": str,
@@ -13430,14 +14094,15 @@
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
         "NodeToNodeEncryptionOptions": (
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef
         ),
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
@@ -13475,14 +14140,15 @@
         "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
         "Scheme": str,
         "SecurityGroups": List[str],
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
         "Subnets": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbLoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "BackendServerDescriptions": Sequence[AwsElbLoadBalancerBackendServerDescriptionTypeDef],
@@ -13507,14 +14173,15 @@
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
         "ServiceRole": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
         "ServiceRole": str,
@@ -13531,14 +14198,15 @@
         "PrincipalId": str,
         "PrincipalType": str,
         "PrincipalName": str,
         "AccountId": str,
         "AccessKeyId": str,
         "SessionContext": AwsIamAccessKeySessionContextOutputTypeDef,
     },
+    total=False,
 )
 
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
@@ -13563,14 +14231,15 @@
         "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
         "RoleId": str,
         "RoleName": str,
         "RolePolicyList": List[AwsIamRolePolicyOutputTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
+    total=False,
 )
 
 AwsIamRoleDetailsTypeDef = TypedDict(
     "AwsIamRoleDetailsTypeDef",
     {
         "AssumeRolePolicyDocument": str,
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
@@ -13606,14 +14275,15 @@
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigOutputTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
         "Version": str,
         "Architectures": List[str],
         "PackageType": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
     {
         "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
@@ -13664,14 +14334,15 @@
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
         "DomainEndpoints": Dict[str, str],
         "AdvancedSecurityOptions": (
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
@@ -13700,14 +14371,15 @@
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[AwsRdsDbSubnetGroupSubnetOutputTypeDef],
         "DbSubnetGroupArn": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
@@ -13765,14 +14437,15 @@
         "RestoreStatus": AwsRedshiftClusterRestoreStatusOutputTypeDef,
         "SnapshotScheduleIdentifier": str,
         "SnapshotScheduleState": str,
         "VpcId": str,
         "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupOutputTypeDef],
         "LoggingStatus": AwsRedshiftClusterLoggingStatusOutputTypeDef,
     },
+    total=False,
 )
 
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
@@ -13828,14 +14501,15 @@
         "Operands": List[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef
         ],
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     {
         "Operands": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
@@ -13848,14 +14522,15 @@
 )
 
 AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
@@ -13864,14 +14539,15 @@
 
 AwsS3BucketObjectLockConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
@@ -13880,14 +14556,15 @@
 )
 
 AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
         "Rules": List[AwsS3BucketServerSideEncryptionRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
@@ -13898,14 +14575,15 @@
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
         "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
         "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
@@ -13925,14 +14603,15 @@
 )
 
 AwsSsmPatchComplianceDetailsOutputTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsOutputTypeDef",
     {
         "Patch": AwsSsmPatchOutputTypeDef,
     },
+    total=False,
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
@@ -13944,14 +14623,15 @@
     {
         "Destinations": List[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     {
         "Destinations": Sequence[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
@@ -13966,14 +14646,15 @@
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": List[AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -13988,14 +14669,15 @@
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
         "RulesList": List[AwsWafRegionalWebAclRulesListDetailsOutputTypeDef],
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
@@ -14010,14 +14692,15 @@
     "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": List[AwsWafRuleGroupRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -14031,14 +14714,15 @@
     "AwsWafWebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
         "Rules": List[AwsWafWebAclRuleOutputTypeDef],
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
@@ -14049,35 +14733,39 @@
 )
 
 AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsOutputTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
@@ -14143,14 +14831,15 @@
         "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
         "RelatedFindingsId": List[StringFilterOutputTypeDef],
         "NoteText": List[StringFilterOutputTypeDef],
         "NoteUpdatedAt": List[DateFilterOutputTypeDef],
         "NoteUpdatedBy": List[StringFilterOutputTypeDef],
         "UserDefinedFields": List[MapFilterOutputTypeDef],
     },
+    total=False,
 )
 
 AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
     "AwsSecurityFindingFiltersOutputTypeDef",
     {
         "ProductArn": List[StringFilterOutputTypeDef],
         "AwsAccountId": List[StringFilterOutputTypeDef],
@@ -14246,14 +14935,15 @@
         "FindingProviderFieldsSeverityLabel": List[StringFilterOutputTypeDef],
         "FindingProviderFieldsSeverityOriginal": List[StringFilterOutputTypeDef],
         "FindingProviderFieldsTypes": List[StringFilterOutputTypeDef],
         "Sample": List[BooleanFilterOutputTypeDef],
         "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
         "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
     },
+    total=False,
 )
 
 AutomationRulesFindingFiltersTypeDef = TypedDict(
     "AutomationRulesFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
@@ -14418,14 +15108,15 @@
 NetworkHeaderOutputTypeDef = TypedDict(
     "NetworkHeaderOutputTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsOutputTypeDef,
         "Source": NetworkPathComponentDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsTypeDef,
@@ -14439,14 +15130,15 @@
     {
         "LineRanges": List[RangeOutputTypeDef],
         "OffsetRanges": List[RangeOutputTypeDef],
         "Pages": List[PageOutputTypeDef],
         "Records": List[RecordOutputTypeDef],
         "Cells": List[CellOutputTypeDef],
     },
+    total=False,
 )
 
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
         "LineRanges": Sequence[RangeTypeDef],
         "OffsetRanges": Sequence[RangeTypeDef],
@@ -14459,14 +15151,15 @@
 
 RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     {
         "Actions": List[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
@@ -14526,14 +15219,15 @@
 )
 
 StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
     "StatelessCustomActionDefinitionOutputTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionOutputTypeDef,
     },
+    total=False,
 )
 
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
     },
@@ -14542,14 +15236,15 @@
 
 PortProbeActionOutputTypeDef = TypedDict(
     "PortProbeActionOutputTypeDef",
     {
         "PortProbeDetails": List[PortProbeDetailOutputTypeDef],
         "Blocked": bool,
     },
+    total=False,
 )
 
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
@@ -14561,14 +15256,15 @@
     "AwsAthenaWorkGroupDetailsOutputTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
@@ -14593,14 +15289,15 @@
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef
         ],
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef
         ),
         "CapacityRebalance": bool,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     {
         "LaunchConfigurationName": str,
         "LoadBalancerNames": Sequence[str],
@@ -14624,14 +15321,15 @@
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": List[
             AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef
         ],
         "BackupPlanRule": List[AwsBackupBackupPlanRuleDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef],
@@ -14665,14 +15363,15 @@
         "Serial": str,
         "SignatureAlgorithm": str,
         "Status": str,
         "Subject": str,
         "SubjectAlternativeNames": List[str],
         "Type": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateDetailsTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDetailsTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
@@ -14704,14 +15403,15 @@
 )
 
 AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionOriginItemOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginItemTypeDef],
     },
@@ -14719,14 +15419,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionOriginGroupOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginGroupTypeDef],
     },
@@ -14752,14 +15453,15 @@
         "SseDescription": AwsDynamoDbTableSseDescriptionOutputTypeDef,
         "StreamSpecification": AwsDynamoDbTableStreamSpecificationOutputTypeDef,
         "TableId": str,
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableDetailsTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsTypeDef",
     {
         "AttributeDefinitions": Sequence[AwsDynamoDbTableAttributeDefinitionTypeDef],
         "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
@@ -14789,14 +15491,15 @@
     {
         "LaunchTemplateName": str,
         "Id": str,
         "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": str,
         "Id": str,
@@ -14819,14 +15522,15 @@
             AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef
         ],
         "ClusterName": str,
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
@@ -14860,14 +15564,15 @@
         "PidMode": str,
         "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef],
         "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
         "RequiresCompatibilities": List[str],
         "TaskRoleArn": str,
         "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef],
         "Cpu": str,
@@ -14893,14 +15598,15 @@
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
         "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
         "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
         "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     {
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
@@ -14969,14 +15675,15 @@
         "PerformanceInsightsKmsKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudWatchLogsExports": List[str],
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
         "ListenerEndpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
         "MaxAllocatedStorage": int,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
@@ -15042,14 +15749,15 @@
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     {
         "Predicate": (
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     },
@@ -15060,14 +15768,15 @@
     "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     {
         "Events": List[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
         "Destination": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": Sequence[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
@@ -15085,14 +15794,15 @@
         "Name": str,
         "RoleArn": str,
         "StateMachineArn": str,
         "Status": str,
         "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
@@ -15110,22 +15820,24 @@
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
         "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
         "Captcha": AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
         "Count": AwsWafv2RulesActionCountDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
         "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsTypeDef,
         "Block": AwsWafv2ActionBlockDetailsTypeDef,
@@ -15155,14 +15867,15 @@
         "IsTerminal": bool,
         "Criteria": AutomationRulesFindingFiltersOutputTypeDef,
         "Actions": List[AutomationRulesActionOutputTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
+    total=False,
 )
 
 InsightTypeDef = TypedDict(
     "InsightTypeDef",
     {
         "InsightArn": str,
         "Name": str,
@@ -15306,14 +16019,15 @@
     "NetworkPathComponentOutputTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderOutputTypeDef,
         "Ingress": NetworkHeaderOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
@@ -15327,23 +16041,25 @@
     "CustomDataIdentifiersDetectionsOutputTypeDef",
     {
         "Count": int,
         "Arn": str,
         "Name": str,
         "Occurrences": OccurrencesOutputTypeDef,
     },
+    total=False,
 )
 
 SensitiveDataDetectionsOutputTypeDef = TypedDict(
     "SensitiveDataDetectionsOutputTypeDef",
     {
         "Count": int,
         "Type": str,
         "Occurrences": OccurrencesOutputTypeDef,
     },
+    total=False,
 )
 
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": int,
         "Arn": str,
@@ -15365,14 +16081,15 @@
 
 RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionTypeDef,
@@ -15382,22 +16099,24 @@
 
 FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
         "ActionName": str,
     },
+    total=False,
 )
 
 RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
         "ActionName": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
@@ -15419,14 +16138,15 @@
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionOutputTypeDef,
         "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
         "DnsRequestAction": DnsRequestActionOutputTypeDef,
         "PortProbeAction": PortProbeActionOutputTypeDef,
     },
+    total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
@@ -15441,14 +16161,15 @@
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsTypeDef,
         "BackupPlanArn": str,
@@ -15470,14 +16191,15 @@
         "Logging": AwsCloudFrontDistributionLoggingOutputTypeDef,
         "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
         "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
         "Status": str,
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsTypeDef,
         "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
@@ -15500,14 +16222,15 @@
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
         "Features": List[AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsTypeDef",
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
         "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
@@ -15533,14 +16256,15 @@
         ],
         "Prefix": str,
         "Status": str,
         "Transitions": List[
             AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
         "AbortIncompleteMultipartUpload": (
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
@@ -15564,14 +16288,15 @@
 )
 
 AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationOutputTypeDef",
     {
         "Configurations": List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
@@ -15583,14 +16308,15 @@
     {
         "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsTypeDef,
         "Name": str,
@@ -15628,23 +16354,25 @@
 
 CustomDataIdentifiersResultOutputTypeDef = TypedDict(
     "CustomDataIdentifiersResultOutputTypeDef",
     {
         "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
         "TotalCount": int,
     },
+    total=False,
 )
 
 SensitiveDataResultOutputTypeDef = TypedDict(
     "SensitiveDataResultOutputTypeDef",
     {
         "Category": str,
         "Detections": List[SensitiveDataDetectionsOutputTypeDef],
         "TotalCount": int,
     },
+    total=False,
 )
 
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
         "TotalCount": int,
@@ -15671,22 +16399,24 @@
         "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
         "StatelessRuleGroupReferences": List[
             FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     {
         "CustomActions": List[RuleGroupSourceCustomActionsDetailsOutputTypeDef],
         "StatelessRules": List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": Sequence[
             FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
@@ -15711,14 +16441,15 @@
 )
 
 AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     {
         "Rules": List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
@@ -15733,14 +16464,15 @@
         "Id": str,
         "Name": str,
         "Arn": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "Scope": str,
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "Arn": str,
@@ -15749,14 +16481,15 @@
         "Capacity": int,
         "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
         "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
         "Description": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
@@ -15793,14 +16526,15 @@
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusOutputTypeDef,
         "SensitiveData": List[SensitiveDataResultOutputTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
     },
+    total=False,
 )
 
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
@@ -15817,26 +16551,28 @@
     {
         "FirewallPolicy": FirewallPolicyDetailsOutputTypeDef,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
         "Description": str,
     },
+    total=False,
 )
 
 RuleGroupSourceOutputTypeDef = TypedDict(
     "RuleGroupSourceOutputTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsOutputTypeDef,
         "RulesString": str,
         "StatefulRules": List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef],
         "StatelessRulesAndCustomActions": (
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": FirewallPolicyDetailsTypeDef,
         "FirewallPolicyArn": str,
@@ -15875,14 +16611,15 @@
         "AccessControlList": str,
         "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationOutputTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
         "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
         "OwnerId": str,
         "OwnerName": str,
@@ -15903,14 +16640,15 @@
 
 DataClassificationDetailsOutputTypeDef = TypedDict(
     "DataClassificationDetailsOutputTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultOutputTypeDef,
     },
+    total=False,
 )
 
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultTypeDef,
@@ -15920,14 +16658,15 @@
 
 RuleGroupDetailsOutputTypeDef = TypedDict(
     "RuleGroupDetailsOutputTypeDef",
     {
         "RuleVariables": RuleGroupVariablesOutputTypeDef,
         "RulesSource": RuleGroupSourceOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": RuleGroupVariablesTypeDef,
         "RulesSource": RuleGroupSourceTypeDef,
@@ -15942,14 +16681,15 @@
         "Description": str,
         "RuleGroup": RuleGroupDetailsOutputTypeDef,
         "RuleGroupArn": str,
         "RuleGroupId": str,
         "RuleGroupName": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
@@ -16052,14 +16792,15 @@
         "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
         "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
         "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsOutputTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
         "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsTypeDef,
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsTypeDef,
@@ -16151,28 +16892,39 @@
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
         "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsTypeDef,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+_RequiredResourceOutputTypeDef = TypedDict(
+    "_RequiredResourceOutputTypeDef",
     {
         "Type": str,
         "Id": str,
+    },
+)
+_OptionalResourceOutputTypeDef = TypedDict(
+    "_OptionalResourceOutputTypeDef",
+    {
         "Partition": PartitionType,
         "Region": str,
         "ResourceRole": str,
         "Tags": Dict[str, str],
         "DataClassification": DataClassificationDetailsOutputTypeDef,
         "Details": ResourceDetailsOutputTypeDef,
     },
+    total=False,
 )
 
+
+class ResourceOutputTypeDef(_RequiredResourceOutputTypeDef, _OptionalResourceOutputTypeDef):
+    pass
+
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "Type": str,
         "Id": str,
     },
 )
@@ -16190,61 +16942,74 @@
 )
 
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
 
-AwsSecurityFindingOutputTypeDef = TypedDict(
-    "AwsSecurityFindingOutputTypeDef",
+_RequiredAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_RequiredAwsSecurityFindingOutputTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceOutputTypeDef],
+    },
+)
+_OptionalAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_OptionalAwsSecurityFindingOutputTypeDef",
+    {
         "ProductName": str,
         "CompanyName": str,
         "Region": str,
-        "GeneratorId": str,
-        "AwsAccountId": str,
         "Types": List[str],
         "FirstObservedAt": str,
         "LastObservedAt": str,
-        "CreatedAt": str,
-        "UpdatedAt": str,
         "Severity": SeverityOutputTypeDef,
         "Confidence": int,
         "Criticality": int,
-        "Title": str,
-        "Description": str,
         "Remediation": RemediationOutputTypeDef,
         "SourceUrl": str,
         "ProductFields": Dict[str, str],
         "UserDefinedFields": Dict[str, str],
         "Malware": List[MalwareOutputTypeDef],
         "Network": NetworkOutputTypeDef,
         "NetworkPath": List[NetworkPathComponentOutputTypeDef],
         "Process": ProcessDetailsOutputTypeDef,
         "Threats": List[ThreatOutputTypeDef],
         "ThreatIntelIndicators": List[ThreatIntelIndicatorOutputTypeDef],
-        "Resources": List[ResourceOutputTypeDef],
         "Compliance": ComplianceOutputTypeDef,
         "VerificationState": VerificationStateType,
         "WorkflowState": WorkflowStateType,
         "Workflow": WorkflowOutputTypeDef,
         "RecordState": RecordStateType,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
         "Note": NoteOutputTypeDef,
         "Vulnerabilities": List[VulnerabilityOutputTypeDef],
         "PatchSummary": PatchSummaryOutputTypeDef,
         "Action": ActionOutputTypeDef,
         "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
         "Sample": bool,
     },
+    total=False,
 )
 
+
+class AwsSecurityFindingOutputTypeDef(
+    _RequiredAwsSecurityFindingOutputTypeDef, _OptionalAwsSecurityFindingOutputTypeDef
+):
+    pass
+
+
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1394,14 +1394,15 @@
     pass
 
 ActionLocalIpDetailsOutputTypeDef = TypedDict(
     "ActionLocalIpDetailsOutputTypeDef",
     {
         "IpAddressV4": str,
     },
+    total=False,
 )
 
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
@@ -1410,14 +1411,15 @@
 
 ActionLocalPortDetailsOutputTypeDef = TypedDict(
     "ActionLocalPortDetailsOutputTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
+    total=False,
 )
 
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
@@ -1428,47 +1430,52 @@
 DnsRequestActionOutputTypeDef = TypedDict(
     "DnsRequestActionOutputTypeDef",
     {
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
+    total=False,
 )
 
 CityOutputTypeDef = TypedDict(
     "CityOutputTypeDef",
     {
         "CityName": str,
     },
+    total=False,
 )
 
 CountryOutputTypeDef = TypedDict(
     "CountryOutputTypeDef",
     {
         "CountryCode": str,
         "CountryName": str,
     },
+    total=False,
 )
 
 GeoLocationOutputTypeDef = TypedDict(
     "GeoLocationOutputTypeDef",
     {
         "Lon": float,
         "Lat": float,
     },
+    total=False,
 )
 
 IpOrganizationDetailsOutputTypeDef = TypedDict(
     "IpOrganizationDetailsOutputTypeDef",
     {
         "Asn": int,
         "AsnOrg": str,
         "Isp": str,
         "Org": str,
     },
+    total=False,
 )
 
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
@@ -1506,14 +1513,15 @@
 
 ActionRemotePortDetailsOutputTypeDef = TypedDict(
     "ActionRemotePortDetailsOutputTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
+    total=False,
 )
 
 ActionRemotePortDetailsTypeDef = TypedDict(
     "ActionRemotePortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
@@ -1542,14 +1550,15 @@
 
 AdjustmentOutputTypeDef = TypedDict(
     "AdjustmentOutputTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
+    total=False,
 )
 
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
@@ -1559,21 +1568,23 @@
 
 AdminAccountTypeDef = TypedDict(
     "AdminAccountTypeDef",
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
+    total=False,
 )
 
 AssociatedStandardOutputTypeDef = TypedDict(
     "AssociatedStandardOutputTypeDef",
     {
         "StandardsId": str,
     },
+    total=False,
 )
 
 AssociatedStandardTypeDef = TypedDict(
     "AssociatedStandardTypeDef",
     {
         "StandardsId": str,
     },
@@ -1582,14 +1593,15 @@
 
 AssociationStateDetailsOutputTypeDef = TypedDict(
     "AssociationStateDetailsOutputTypeDef",
     {
         "State": str,
         "StatusMessage": str,
     },
+    total=False,
 )
 
 AssociationStateDetailsTypeDef = TypedDict(
     "AssociationStateDetailsTypeDef",
     {
         "State": str,
         "StatusMessage": str,
@@ -1616,21 +1628,23 @@
 SeverityUpdateOutputTypeDef = TypedDict(
     "SeverityUpdateOutputTypeDef",
     {
         "Normalized": int,
         "Product": float,
         "Label": SeverityLabelType,
     },
+    total=False,
 )
 
 WorkflowUpdateOutputTypeDef = TypedDict(
     "WorkflowUpdateOutputTypeDef",
     {
         "Status": WorkflowStatusType,
     },
+    total=False,
 )
 
 NoteUpdateTypeDef = TypedDict(
     "NoteUpdateTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
@@ -1666,31 +1680,34 @@
 MapFilterOutputTypeDef = TypedDict(
     "MapFilterOutputTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparison": MapFilterComparisonType,
     },
+    total=False,
 )
 
 NumberFilterOutputTypeDef = TypedDict(
     "NumberFilterOutputTypeDef",
     {
         "Gte": float,
         "Lte": float,
         "Eq": float,
     },
+    total=False,
 )
 
 StringFilterOutputTypeDef = TypedDict(
     "StringFilterOutputTypeDef",
     {
         "Value": str,
         "Comparison": StringFilterComparisonType,
     },
+    total=False,
 )
 
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -1727,22 +1744,24 @@
         "RuleName": str,
         "Description": str,
         "IsTerminal": bool,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
+    total=False,
 )
 
 AvailabilityZoneOutputTypeDef = TypedDict(
     "AvailabilityZoneOutputTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
@@ -1752,14 +1771,15 @@
 
 AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
@@ -1768,31 +1788,34 @@
         "RoleSearchSubtree": bool,
         "ServiceAccountUsername": str,
         "UserBase": str,
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
     {
         "DayOfWeek": str,
         "TimeOfDay": str,
         "TimeZone": str,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerUsersDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
     {
         "PendingChange": str,
         "Username": str,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
@@ -1838,14 +1861,15 @@
 
 AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
@@ -1854,14 +1878,15 @@
 )
 
 AwsApiCallActionDomainDetailsOutputTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsOutputTypeDef",
     {
         "Domain": str,
     },
+    total=False,
 )
 
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
@@ -1870,14 +1895,15 @@
 
 AwsApiGatewayAccessLogSettingsOutputTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsOutputTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
     },
+    total=False,
 )
 
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
@@ -1889,14 +1915,15 @@
     "AwsApiGatewayCanarySettingsOutputTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
         "StageVariableOverrides": Dict[str, str],
         "UseStageCache": bool,
     },
+    total=False,
 )
 
 AwsApiGatewayCanarySettingsTypeDef = TypedDict(
     "AwsApiGatewayCanarySettingsTypeDef",
     {
         "PercentTraffic": float,
         "DeploymentId": str,
@@ -1907,14 +1934,15 @@
 )
 
 AwsApiGatewayEndpointConfigurationOutputTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     {
         "Types": List[str],
     },
+    total=False,
 )
 
 AwsApiGatewayEndpointConfigurationTypeDef = TypedDict(
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
@@ -1933,14 +1961,15 @@
         "CacheTtlInSeconds": int,
         "CacheDataEncrypted": bool,
         "RequireAuthorizationForCacheControl": bool,
         "UnauthorizedCacheControlHeaderStrategy": str,
         "HttpMethod": str,
         "ResourcePath": str,
     },
+    total=False,
 )
 
 AwsApiGatewayMethodSettingsTypeDef = TypedDict(
     "AwsApiGatewayMethodSettingsTypeDef",
     {
         "MetricsEnabled": bool,
         "LoggingLevel": str,
@@ -1964,14 +1993,15 @@
         "AllowOrigins": List[str],
         "AllowCredentials": bool,
         "ExposeHeaders": List[str],
         "MaxAge": int,
         "AllowMethods": List[str],
         "AllowHeaders": List[str],
     },
+    total=False,
 )
 
 AwsCorsConfigurationTypeDef = TypedDict(
     "AwsCorsConfigurationTypeDef",
     {
         "AllowOrigins": Sequence[str],
         "AllowCredentials": bool,
@@ -1988,14 +2018,15 @@
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
+    total=False,
 )
 
 AwsApiGatewayV2RouteSettingsTypeDef = TypedDict(
     "AwsApiGatewayV2RouteSettingsTypeDef",
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
@@ -2009,34 +2040,37 @@
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
         "IdentityValidationExpression": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
     {
         "AuthTtL": int,
         "ClientId": str,
         "IatTtL": int,
         "Issuer": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
     {
         "AppIdClientRegex": str,
         "AwsRegion": str,
         "DefaultAction": str,
         "UserPoolId": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
@@ -2070,14 +2104,15 @@
 AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
         "FieldLogLevel": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
@@ -2088,14 +2123,15 @@
 
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
@@ -2104,14 +2140,15 @@
 )
 
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
@@ -2121,14 +2158,15 @@
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -2143,14 +2181,15 @@
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
         "SpotInstancePools": int,
         "SpotMaxPrice": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
@@ -2165,22 +2204,24 @@
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
@@ -2204,14 +2245,15 @@
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -2224,23 +2266,25 @@
 )
 
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
     {
         "HttpEndpoint": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     {
         "Enabled": bool,
     },
@@ -2259,14 +2303,15 @@
 
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     {
         "BackupOptions": Dict[str, str],
         "ResourceType": str,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
@@ -2276,14 +2321,15 @@
 
 AwsBackupBackupPlanLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
@@ -2293,14 +2339,15 @@
 
 AwsBackupBackupVaultNotificationsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     {
         "BackupVaultEvents": List[str],
         "SnsTopicArn": str,
     },
+    total=False,
 )
 
 AwsBackupBackupVaultNotificationsDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
@@ -2310,14 +2357,15 @@
 
 AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
@@ -2329,14 +2377,15 @@
     "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "BackupPlanVersion": str,
         "BackupRuleId": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointCreatedByDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
@@ -2348,14 +2397,15 @@
 
 AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
@@ -2365,28 +2415,31 @@
 
 AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
     {
         "Name": str,
         "OId": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateKeyUsageOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
     {
         "Name": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateOptionsOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateOptionsOutputTypeDef",
     {
         "CertificateTransparencyLoggingPreference": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateExtendedKeyUsageTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     {
         "Name": str,
         "OId": str,
@@ -2413,14 +2466,15 @@
 AwsCertificateManagerCertificateResourceRecordOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateResourceRecordTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -2430,23 +2484,25 @@
 )
 
 AwsCloudFormationStackDriftInformationDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
     {
         "StackDriftStatus": str,
     },
+    total=False,
 )
 
 AwsCloudFormationStackOutputsDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
     {
         "Description": str,
         "OutputKey": str,
         "OutputValue": str,
     },
+    total=False,
 )
 
 AwsCloudFormationStackDriftInformationDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     {
         "StackDriftStatus": str,
     },
@@ -2464,14 +2520,15 @@
 )
 
 AwsCloudFrontDistributionCacheBehaviorOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
@@ -2479,14 +2536,15 @@
 )
 
 AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
@@ -2497,27 +2555,29 @@
     "AwsCloudFrontDistributionLoggingOutputTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
         "IncludeCookies": bool,
         "Prefix": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionViewerCertificateOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
     {
         "AcmCertificateArn": str,
         "Certificate": str,
         "CertificateSource": str,
         "CloudFrontDefaultCertificate": bool,
         "IamCertificateId": str,
         "MinimumProtocolVersion": str,
         "SslSupportMethod": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionLoggingTypeDef = TypedDict(
     "AwsCloudFrontDistributionLoggingTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
@@ -2543,14 +2603,15 @@
 
 AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     {
         "Items": List[str],
         "Quantity": int,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginSslProtocolsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     {
         "Items": Sequence[str],
         "Quantity": int,
@@ -2560,14 +2621,15 @@
 
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     {
         "Items": List[int],
         "Quantity": int,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
     {
         "Items": Sequence[int],
         "Quantity": int,
@@ -2576,14 +2638,15 @@
 )
 
 AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
     {
         "OriginAccessIdentity": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginS3OriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
@@ -2605,14 +2668,15 @@
         "Name": str,
         "S3BucketName": str,
         "S3KeyPrefix": str,
         "SnsTopicArn": str,
         "SnsTopicName": str,
         "TrailArn": str,
     },
+    total=False,
 )
 
 AwsCloudTrailTrailDetailsTypeDef = TypedDict(
     "AwsCloudTrailTrailDetailsTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "CloudWatchLogsRoleArn": str,
@@ -2635,14 +2699,15 @@
 
 AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCloudWatchAlarmDimensionsDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -2659,14 +2724,15 @@
         "Name": str,
         "NamespaceType": str,
         "OverrideArtifactName": bool,
         "Packaging": str,
         "Path": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectArtifactsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     {
         "ArtifactIdentifier": str,
         "EncryptionDisabled": bool,
@@ -2685,23 +2751,25 @@
     "AwsCodeBuildProjectSourceOutputTypeDef",
     {
         "Type": str,
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectVpcConfigOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     {
         "VpcId": str,
         "Subnets": List[str],
         "SecurityGroupIds": List[str],
     },
+    total=False,
 )
 
 AwsCodeBuildProjectSourceTypeDef = TypedDict(
     "AwsCodeBuildProjectSourceTypeDef",
     {
         "Type": str,
         "Location": str,
@@ -2724,14 +2792,15 @@
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -2742,14 +2811,15 @@
 
 AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
@@ -2760,14 +2830,15 @@
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
     {
         "GroupName": str,
         "Status": str,
         "StreamName": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     {
         "GroupName": str,
         "Status": str,
@@ -2779,14 +2850,15 @@
 AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
@@ -2797,14 +2869,15 @@
 
 AwsDynamoDbTableAttributeDefinitionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableAttributeDefinitionTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
@@ -2814,14 +2887,15 @@
 
 AwsDynamoDbTableBillingModeSummaryOutputTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableBillingModeSummaryTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
@@ -2831,53 +2905,58 @@
 
 AwsDynamoDbTableKeySchemaOutputTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaOutputTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProvisionedThroughputOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
     {
         "LastDecreaseDateTime": str,
         "LastIncreaseDateTime": str,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
+    total=False,
 )
 
 AwsDynamoDbTableRestoreSummaryOutputTypeDef = TypedDict(
     "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": str,
         "RestoreInProgress": bool,
     },
+    total=False,
 )
 
 AwsDynamoDbTableSseDescriptionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableSseDescriptionOutputTypeDef",
     {
         "InaccessibleEncryptionDateTime": str,
         "Status": str,
         "SseType": str,
         "KmsMasterKeyArn": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableStreamSpecificationOutputTypeDef = TypedDict(
     "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableKeySchemaTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
@@ -2930,14 +3009,15 @@
 
 AwsDynamoDbTableProjectionOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionOutputTypeDef",
     {
         "NonKeyAttributes": List[str],
         "ProjectionType": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProjectionTypeDef = TypedDict(
     "AwsDynamoDbTableProjectionTypeDef",
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
@@ -2946,14 +3026,15 @@
 )
 
 AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
     {
         "ReadCapacityUnits": int,
     },
+    total=False,
 )
 
 AwsDynamoDbTableProvisionedThroughputOverrideTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
@@ -2970,14 +3051,15 @@
         "Domain": str,
         "PublicIpv4Pool": str,
         "NetworkBorderGroup": str,
         "NetworkInterfaceId": str,
         "NetworkInterfaceOwnerId": str,
         "PrivateIpAddress": str,
     },
+    total=False,
 )
 
 AwsEc2EipDetailsTypeDef = TypedDict(
     "AwsEc2EipDetailsTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
@@ -2998,28 +3080,31 @@
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
         "InstanceMetadataTags": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
     {
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef = TypedDict(
     "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
     {
         "NetworkInterfaceId": str,
     },
+    total=False,
 )
 
 AwsEc2InstanceMetadataOptionsTypeDef = TypedDict(
     "AwsEc2InstanceMetadataOptionsTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
@@ -3054,14 +3139,15 @@
         "Iops": int,
         "KmsKeyId": str,
         "SnapshotId": str,
         "Throughput": int,
         "VolumeSize": int,
         "VolumeType": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
@@ -3077,14 +3163,15 @@
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
@@ -3094,14 +3181,15 @@
 
 AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
@@ -3110,14 +3198,15 @@
 )
 
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
     {
         "CpuCredits": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
     {
         "CpuCredits": str,
     },
@@ -3125,99 +3214,110 @@
 )
 
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
     {
         "Count": int,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
     {
         "Configured": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
     {
         "AutoRecovery": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpTokens": str,
         "HttpPutResponseHopLimit": int,
         "InstanceMetadataTags": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
     {
         "Affinity": str,
         "AvailabilityZone": str,
         "GroupName": str,
         "HostId": str,
         "HostResourceGroupArn": str,
         "PartitionNumber": int,
         "SpreadDomain": str,
         "Tenancy": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
     {
         "EnableResourceNameDnsAAAARecord": bool,
         "EnableResourceNameDnsARecord": bool,
         "HostnameType": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     {
         "Type": str,
     },
@@ -3324,14 +3424,15 @@
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
         "MaxPrice": str,
         "SpotInstanceType": str,
         "ValidUntil": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
@@ -3344,14 +3445,15 @@
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
@@ -3362,14 +3464,15 @@
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef = (
     TypedDict(
         "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
         {
             "Max": int,
             "Min": int,
         },
+        total=False,
     )
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
     {
         "Max": int,
@@ -3381,14 +3484,15 @@
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef = (
     TypedDict(
         "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
         {
             "Max": int,
             "Min": int,
         },
+        total=False,
     )
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
     {
         "Max": int,
@@ -3399,46 +3503,51 @@
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
     {
         "Max": float,
         "Min": float,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
     {
         "Max": float,
         "Min": float,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
     {
         "Max": int,
         "Min": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     {
         "Max": float,
         "Min": float,
@@ -3483,36 +3592,40 @@
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
     {
         "Ipv4Prefix": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
     {
         "Ipv6Address": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
     {
         "Ipv6Prefix": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
     {
         "Primary": bool,
         "PrivateIpAddress": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     {
         "Ipv4Prefix": str,
     },
@@ -3547,14 +3660,15 @@
 AwsEc2NetworkAclAssociationOutputTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationOutputTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
@@ -3565,22 +3679,24 @@
 
 IcmpTypeCodeOutputTypeDef = TypedDict(
     "IcmpTypeCodeOutputTypeDef",
     {
         "Code": int,
         "Type": int,
     },
+    total=False,
 )
 
 PortRangeFromToOutputTypeDef = TypedDict(
     "PortRangeFromToOutputTypeDef",
     {
         "From": int,
         "To": int,
     },
+    total=False,
 )
 
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
@@ -3604,14 +3720,15 @@
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceAttachmentTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": str,
         "AttachmentId": str,
@@ -3625,30 +3742,33 @@
 )
 
 AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
     {
         "IpV6Address": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
     {
         "PrivateIpAddress": str,
         "PrivateDnsName": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     {
         "IpV6Address": str,
     },
@@ -3674,14 +3794,15 @@
 )
 
 PropagatingVgwSetDetailsOutputTypeDef = TypedDict(
     "PropagatingVgwSetDetailsOutputTypeDef",
     {
         "GatewayId": str,
     },
+    total=False,
 )
 
 RouteSetDetailsOutputTypeDef = TypedDict(
     "RouteSetDetailsOutputTypeDef",
     {
         "CarrierGatewayId": str,
         "CoreNetworkArn": str,
@@ -3696,14 +3817,15 @@
         "NatGatewayId": str,
         "NetworkInterfaceId": str,
         "Origin": str,
         "State": str,
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 PropagatingVgwSetDetailsTypeDef = TypedDict(
     "PropagatingVgwSetDetailsTypeDef",
     {
         "GatewayId": str,
     },
@@ -3734,40 +3856,44 @@
 )
 
 AwsEc2SecurityGroupIpRangeOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeOutputTypeDef",
     {
         "CidrIp": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpv6RangeOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
     {
         "CidrIpv6": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupPrefixListIdOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
     {
         "PrefixListId": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
     {
         "GroupId": str,
         "GroupName": str,
         "PeeringStatus": str,
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
@@ -3806,14 +3932,15 @@
 Ipv6CidrBlockAssociationOutputTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationOutputTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
+    total=False,
 )
 
 Ipv6CidrBlockAssociationTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
@@ -3834,14 +3961,15 @@
         "AssociationDefaultRouteTableId": str,
         "PropagationDefaultRouteTableId": str,
         "VpnEcmpSupport": str,
         "DnsSupport": str,
         "MulticastSupport": str,
         "AmazonSideAsn": int,
     },
+    total=False,
 )
 
 AwsEc2TransitGatewayDetailsTypeDef = TypedDict(
     "AwsEc2TransitGatewayDetailsTypeDef",
     {
         "Id": str,
         "Description": str,
@@ -3863,14 +3991,15 @@
     "AwsEc2VolumeAttachmentOutputTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
         "InstanceId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEc2VolumeAttachmentTypeDef = TypedDict(
     "AwsEc2VolumeAttachmentTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
@@ -3883,14 +4012,15 @@
 CidrBlockAssociationOutputTypeDef = TypedDict(
     "CidrBlockAssociationOutputTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": str,
     },
+    total=False,
 )
 
 CidrBlockAssociationTypeDef = TypedDict(
     "CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
@@ -3900,14 +4030,15 @@
 )
 
 AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
     {
         "ServiceType": str,
     },
+    total=False,
 )
 
 AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     {
         "ServiceType": str,
     },
@@ -3916,14 +4047,15 @@
 
 AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
     {
         "Code": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionStatusDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     {
         "Code": str,
         "Message": str,
@@ -3932,30 +4064,33 @@
 )
 
 VpcInfoCidrBlockSetDetailsOutputTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsOutputTypeDef",
     {
         "CidrBlock": str,
     },
+    total=False,
 )
 
 VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef = TypedDict(
     "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
     {
         "Ipv6CidrBlock": str,
     },
+    total=False,
 )
 
 VpcInfoPeeringOptionsDetailsOutputTypeDef = TypedDict(
     "VpcInfoPeeringOptionsDetailsOutputTypeDef",
     {
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
+    total=False,
 )
 
 VpcInfoCidrBlockSetDetailsTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsTypeDef",
     {
         "CidrBlock": str,
     },
@@ -3982,26 +4117,28 @@
 
 AwsEc2VpnConnectionRoutesDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
     {
         "AcceptedRouteCount": int,
         "CertificateArn": str,
         "LastStatusChange": str,
         "OutsideIpAddress": str,
         "Status": str,
         "StatusMessage": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionRoutesDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
@@ -4038,14 +4175,15 @@
         "Phase2LifetimeSeconds": int,
         "PreSharedKey": str,
         "RekeyFuzzPercentage": int,
         "RekeyMarginTimeSeconds": int,
         "ReplayWindowSize": int,
         "TunnelInsideCidr": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     {
         "DpdTimeoutSeconds": int,
         "IkeVersions": Sequence[str],
@@ -4073,14 +4211,15 @@
         "RegistryId": str,
         "RepositoryName": str,
         "Architecture": str,
         "ImageDigest": str,
         "ImageTags": List[str],
         "ImagePublishedAt": str,
     },
+    total=False,
 )
 
 AwsEcrContainerImageDetailsTypeDef = TypedDict(
     "AwsEcrContainerImageDetailsTypeDef",
     {
         "RegistryId": str,
         "RepositoryName": str,
@@ -4093,22 +4232,24 @@
 )
 
 AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
     {
         "ScanOnPush": bool,
     },
+    total=False,
 )
 
 AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef = TypedDict(
     "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
     {
         "LifecyclePolicyText": str,
         "RegistryId": str,
     },
+    total=False,
 )
 
 AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     {
         "ScanOnPush": bool,
     },
@@ -4126,14 +4267,15 @@
 
 AwsEcsClusterClusterSettingsDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsClusterClusterSettingsDetailsTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4147,14 +4289,15 @@
         {
             "CloudWatchEncryptionEnabled": bool,
             "CloudWatchLogGroupName": str,
             "S3BucketName": str,
             "S3EncryptionEnabled": bool,
             "S3KeyPrefix": str,
         },
+        total=False,
     )
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     {
         "CloudWatchEncryptionEnabled": bool,
@@ -4169,14 +4312,15 @@
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
+    total=False,
 )
 
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
@@ -4187,14 +4331,15 @@
 
 AwsMountPointOutputTypeDef = TypedDict(
     "AwsMountPointOutputTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
     },
+    total=False,
 )
 
 AwsMountPointTypeDef = TypedDict(
     "AwsMountPointTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
@@ -4205,14 +4350,15 @@
 AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
+    total=False,
 )
 
 AwsEcsServiceCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
@@ -4223,14 +4369,15 @@
 
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
@@ -4239,14 +4386,15 @@
 )
 
 AwsEcsServiceDeploymentControllerDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentControllerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     {
         "Type": str,
     },
@@ -4257,40 +4405,44 @@
     "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "LoadBalancerName": str,
         "TargetGroupArn": str,
     },
+    total=False,
 )
 
 AwsEcsServicePlacementConstraintsDetailsOutputTypeDef = TypedDict(
     "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
     {
         "Expression": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServicePlacementStrategiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
     {
         "Field": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsServiceServiceRegistriesDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "Port": int,
         "RegistryArn": str,
     },
+    total=False,
 )
 
 AwsEcsServiceLoadBalancersDetailsTypeDef = TypedDict(
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
@@ -4332,14 +4484,15 @@
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": List[str],
         "Subnets": List[str],
     },
+    total=False,
 )
 
 AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
     {
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
@@ -4350,14 +4503,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
@@ -4367,115 +4521,128 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
     {
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
     {
         "Hostname": str,
         "IpAddress": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
     {
         "Options": Dict[str, str],
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     {
         "Command": List[str],
         "Interval": int,
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "ReadOnly": bool,
         "SourceVolume": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
     {
         "ContainerPort": int,
         "HostPort": int,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
     {
         "CredentialsParameter": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
     {
         "Type": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
     {
         "Namespace": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
     {
         "HardLimit": int,
         "Name": str,
         "SoftLimit": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4598,14 +4765,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": List[str],
         "Drop": List[str],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     {
         "Add": Sequence[str],
         "Drop": Sequence[str],
@@ -4616,23 +4784,25 @@
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
         "Permissions": List[str],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     {
         "ContainerPath": str,
         "MountOptions": List[str],
         "Size": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     {
         "ContainerPath": str,
         "HostPath": str,
@@ -4654,14 +4824,15 @@
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef = (
     TypedDict(
         "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
         {
             "Name": str,
             "ValueFrom": str,
         },
+        total=False,
     )
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     {
         "Name": str,
@@ -4672,22 +4843,24 @@
 
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
     {
         "Expression": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
@@ -4706,14 +4879,15 @@
 
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -4726,21 +4900,23 @@
     {
         "Autoprovision": bool,
         "Driver": str,
         "DriverOpts": Dict[str, str],
         "Labels": Dict[str, str],
         "Scope": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
     {
         "SourcePath": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     {
         "Autoprovision": bool,
         "Driver": str,
@@ -4762,14 +4938,15 @@
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef = (
     TypedDict(
         "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
         {
             "AccessPointId": str,
             "Iam": str,
         },
+        total=False,
     )
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
@@ -4779,14 +4956,15 @@
 )
 
 AwsEcsTaskVolumeHostDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
     {
         "SourcePath": str,
     },
+    total=False,
 )
 
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
@@ -4796,14 +4974,15 @@
 AwsEfsAccessPointPosixUserDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     {
         "Gid": str,
         "SecondaryGids": List[str],
         "Uid": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointPosixUserDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
     {
         "Gid": str,
         "SecondaryGids": Sequence[str],
@@ -4815,14 +4994,15 @@
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
@@ -4834,14 +5014,15 @@
 AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "EndpointPublicAccess": bool,
     },
+    total=False,
 )
 
 AwsEksClusterResourcesVpcConfigDetailsTypeDef = TypedDict(
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
@@ -4852,14 +5033,15 @@
 
 AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "Types": List[str],
     },
+    total=False,
 )
 
 AwsEksClusterLoggingClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
     {
         "Enabled": bool,
         "Types": Sequence[str],
@@ -4869,33 +5051,36 @@
 
 AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
     {
         "Namespace": str,
         "OptionName": str,
         "ResourceName": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentTierOutputTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
     {
         "Name": str,
         "Type": str,
         "Version": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
@@ -4926,52 +5111,57 @@
 
 AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainVPCOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     {
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VPCId": str,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
@@ -5022,14 +5212,15 @@
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
@@ -5038,14 +5229,15 @@
 
 AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
@@ -5055,14 +5247,15 @@
 
 AwsElbAppCookieStickinessPolicyOutputTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyOutputTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsElbAppCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
@@ -5072,14 +5265,15 @@
 
 AwsElbLbCookieStickinessPolicyOutputTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyOutputTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsElbLbCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
@@ -5091,14 +5285,15 @@
     "AwsElbLoadBalancerAccessLogOutputTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
         "S3BucketName": str,
         "S3BucketPrefix": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAccessLogTypeDef = TypedDict(
     "AwsElbLoadBalancerAccessLogTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
@@ -5110,14 +5305,15 @@
 
 AwsElbLoadBalancerAdditionalAttributeOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAdditionalAttributeTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -5127,28 +5323,31 @@
 
 AwsElbLoadBalancerConnectionDrainingOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerConnectionSettingsOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
     {
         "IdleTimeout": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerConnectionDrainingTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
@@ -5174,14 +5373,15 @@
 
 AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerBackendServerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
@@ -5194,29 +5394,32 @@
     {
         "HealthyThreshold": int,
         "Interval": int,
         "Target": str,
         "Timeout": int,
         "UnhealthyThreshold": int,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerInstanceOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerInstanceOutputTypeDef",
     {
         "InstanceId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
     {
         "GroupName": str,
         "OwnerAlias": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerHealthCheckTypeDef = TypedDict(
     "AwsElbLoadBalancerHealthCheckTypeDef",
     {
         "HealthyThreshold": int,
         "Interval": int,
@@ -5249,14 +5452,15 @@
     {
         "InstancePort": int,
         "InstanceProtocol": str,
         "LoadBalancerPort": int,
         "Protocol": str,
         "SslCertificateId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerListenerTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerTypeDef",
     {
         "InstancePort": int,
         "InstanceProtocol": str,
@@ -5269,14 +5473,15 @@
 
 AwsElbv2LoadBalancerAttributeOutputTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsElbv2LoadBalancerAttributeTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -5286,14 +5491,15 @@
 
 LoadBalancerStateOutputTypeDef = TypedDict(
     "LoadBalancerStateOutputTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
+    total=False,
 )
 
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": str,
         "Reason": str,
@@ -5304,14 +5510,15 @@
 AwsEventSchemasRegistryDetailsOutputTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsOutputTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
         "RegistryName": str,
     },
+    total=False,
 )
 
 AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
@@ -5321,14 +5528,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5336,28 +5544,31 @@
 )
 
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5381,14 +5592,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
     {
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
     {
         "Status": str,
     },
@@ -5397,14 +5609,15 @@
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
     {
         "Reason": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
     {
         "Reason": str,
         "Status": str,
@@ -5414,14 +5627,15 @@
 
 AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
     {
         "Name": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     {
         "Name": str,
         "Status": str,
@@ -5431,14 +5645,15 @@
 
 AwsIamAccessKeySessionContextAttributesOutputTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
@@ -5451,14 +5666,15 @@
     {
         "Type": str,
         "PrincipalId": str,
         "Arn": str,
         "AccountId": str,
         "UserName": str,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextSessionIssuerTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     {
         "Type": str,
         "PrincipalId": str,
@@ -5471,14 +5687,15 @@
 
 AwsIamAttachedManagedPolicyOutputTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
+    total=False,
 )
 
 AwsIamAttachedManagedPolicyTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
@@ -5487,14 +5704,15 @@
 )
 
 AwsIamGroupPolicyOutputTypeDef = TypedDict(
     "AwsIamGroupPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamGroupPolicyTypeDef = TypedDict(
     "AwsIamGroupPolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5507,14 +5725,15 @@
         "Arn": str,
         "AssumeRolePolicyDocument": str,
         "CreateDate": str,
         "Path": str,
         "RoleId": str,
         "RoleName": str,
     },
+    total=False,
 )
 
 AwsIamInstanceProfileRoleTypeDef = TypedDict(
     "AwsIamInstanceProfileRoleTypeDef",
     {
         "Arn": str,
         "AssumeRolePolicyDocument": str,
@@ -5528,14 +5747,15 @@
 
 AwsIamPermissionsBoundaryOutputTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryOutputTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
     },
+    total=False,
 )
 
 AwsIamPermissionsBoundaryTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
@@ -5546,14 +5766,15 @@
 AwsIamPolicyVersionOutputTypeDef = TypedDict(
     "AwsIamPolicyVersionOutputTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": str,
     },
+    total=False,
 )
 
 AwsIamPolicyVersionTypeDef = TypedDict(
     "AwsIamPolicyVersionTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
@@ -5563,14 +5784,15 @@
 )
 
 AwsIamRolePolicyOutputTypeDef = TypedDict(
     "AwsIamRolePolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamRolePolicyTypeDef = TypedDict(
     "AwsIamRolePolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5578,14 +5800,15 @@
 )
 
 AwsIamUserPolicyOutputTypeDef = TypedDict(
     "AwsIamUserPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
+    total=False,
 )
 
 AwsIamUserPolicyTypeDef = TypedDict(
     "AwsIamUserPolicyTypeDef",
     {
         "PolicyName": str,
     },
@@ -5594,14 +5817,15 @@
 
 AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
     },
+    total=False,
 )
 
 AwsKinesisStreamStreamEncryptionDetailsTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
@@ -5617,14 +5841,15 @@
         "KeyId": str,
         "KeyManager": str,
         "KeyState": str,
         "Origin": str,
         "Description": str,
         "KeyRotationStatus": bool,
     },
+    total=False,
 )
 
 AwsKmsKeyDetailsTypeDef = TypedDict(
     "AwsKmsKeyDetailsTypeDef",
     {
         "AWSAccountId": str,
         "CreationDate": float,
@@ -5642,14 +5867,15 @@
     "AwsLambdaFunctionCodeOutputTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
         "ZipFile": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionCodeTypeDef = TypedDict(
     "AwsLambdaFunctionCodeTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
@@ -5660,14 +5886,15 @@
 )
 
 AwsLambdaFunctionDeadLetterConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
     {
         "TargetArn": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionDeadLetterConfigTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
@@ -5676,30 +5903,33 @@
 
 AwsLambdaFunctionLayerOutputTypeDef = TypedDict(
     "AwsLambdaFunctionLayerOutputTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
     },
+    total=False,
 )
 
 AwsLambdaFunctionTracingConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionTracingConfigOutputTypeDef",
     {
         "Mode": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionLayerTypeDef = TypedDict(
     "AwsLambdaFunctionLayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
@@ -5727,14 +5957,15 @@
 
 AwsLambdaFunctionEnvironmentErrorOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
@@ -5745,14 +5976,15 @@
 AwsLambdaLayerVersionDetailsOutputTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsOutputTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": List[str],
         "CreatedDate": str,
     },
+    total=False,
 )
 
 AwsLambdaLayerVersionDetailsTypeDef = TypedDict(
     "AwsLambdaLayerVersionDetailsTypeDef",
     {
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
@@ -5762,14 +5994,15 @@
 )
 
 AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
     {
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     {
         "SubnetId": str,
     },
@@ -5779,14 +6012,15 @@
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
         "MasterUserPassword": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
@@ -5796,14 +6030,15 @@
 )
 
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
@@ -5815,51 +6050,56 @@
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
         "EnforceHTTPS": bool,
         "CustomEndpoint": str,
         "TLSSecurityPolicy": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
@@ -5913,14 +6153,15 @@
 
 AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
@@ -5930,14 +6171,15 @@
 
 AwsRdsDbClusterAssociatedRoleOutputTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
@@ -5949,40 +6191,44 @@
     "AwsRdsDbClusterMemberOutputTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
         "DbInstanceIdentifier": str,
         "DbClusterParameterGroupStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterOptionGroupMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
     {
         "DbClusterOptionGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbDomainMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbDomainMembershipOutputTypeDef",
     {
         "Domain": str,
         "Status": str,
         "Fqdn": str,
         "IamRoleName": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
     {
         "VpcSecurityGroupId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbClusterMemberTypeDef = TypedDict(
     "AwsRdsDbClusterMemberTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
@@ -6023,14 +6269,15 @@
 
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[str],
     },
+    total=False,
 )
 
 AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": Sequence[str],
@@ -6041,14 +6288,15 @@
 AwsRdsDbInstanceAssociatedRoleOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
@@ -6060,48 +6308,53 @@
 AwsRdsDbInstanceEndpointOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointOutputTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
+    total=False,
 )
 
 AwsRdsDbOptionGroupMembershipOutputTypeDef = TypedDict(
     "AwsRdsDbOptionGroupMembershipOutputTypeDef",
     {
         "OptionGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbParameterGroupOutputTypeDef = TypedDict(
     "AwsRdsDbParameterGroupOutputTypeDef",
     {
         "DbParameterGroupName": str,
         "ParameterApplyStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbProcessorFeatureOutputTypeDef = TypedDict(
     "AwsRdsDbProcessorFeatureOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsRdsDbStatusInfoOutputTypeDef = TypedDict(
     "AwsRdsDbStatusInfoOutputTypeDef",
     {
         "StatusType": str,
         "Normal": bool,
         "Status": str,
         "Message": str,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceEndpointTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
@@ -6150,14 +6403,15 @@
 
 AwsRdsPendingCloudWatchLogsExportsOutputTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
+    total=False,
 )
 
 AwsRdsPendingCloudWatchLogsExportsTypeDef = TypedDict(
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
@@ -6169,22 +6423,24 @@
     "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
         "Ec2SecurityGroupOwnerId": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupIpRangeOutputTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
     {
         "CidrIp": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
@@ -6204,14 +6460,15 @@
 )
 
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
     {
         "Name": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
@@ -6228,14 +6485,15 @@
         "EventSubscriptionArn": str,
         "SnsTopicArn": str,
         "SourceIdsList": List[str],
         "SourceType": str,
         "Status": str,
         "SubscriptionCreationTime": str,
     },
+    total=False,
 )
 
 AwsRdsEventSubscriptionDetailsTypeDef = TypedDict(
     "AwsRdsEventSubscriptionDetailsTypeDef",
     {
         "CustSubscriptionId": str,
         "CustomerAwsId": str,
@@ -6254,14 +6512,15 @@
 AwsRedshiftClusterClusterNodeOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeOutputTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
         "PublicIpAddress": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterNodeTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
@@ -6273,14 +6532,15 @@
 AwsRedshiftClusterClusterParameterStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterParameterStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
@@ -6291,14 +6551,15 @@
 
 AwsRedshiftClusterClusterSecurityGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterSecurityGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
@@ -6310,14 +6571,15 @@
     "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
@@ -6330,14 +6592,15 @@
 AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
         "DeferMaintenanceStartTime": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterDeferredMaintenanceWindowTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
@@ -6348,51 +6611,56 @@
 
 AwsRedshiftClusterElasticIpStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterEndpointOutputTypeDef = TypedDict(
     "AwsRedshiftClusterEndpointOutputTypeDef",
     {
         "Address": str,
         "Port": int,
     },
+    total=False,
 )
 
 AwsRedshiftClusterHsmStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterHsmStatusOutputTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "HsmConfigurationIdentifier": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterIamRoleOutputTypeDef = TypedDict(
     "AwsRedshiftClusterIamRoleOutputTypeDef",
     {
         "ApplyStatus": str,
         "IamRoleArn": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterLoggingStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterLoggingStatusOutputTypeDef",
     {
         "BucketName": str,
         "LastFailureMessage": str,
         "LastFailureTime": str,
         "LastSuccessfulDeliveryTime": str,
         "LoggingEnabled": bool,
         "S3KeyPrefix": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterPendingModifiedValuesOutputTypeDef = TypedDict(
     "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
     {
         "AutomatedSnapshotRetentionPeriod": int,
         "ClusterIdentifier": str,
@@ -6402,42 +6670,46 @@
         "EnhancedVpcRouting": bool,
         "MaintenanceTrackName": str,
         "MasterUserPassword": str,
         "NodeType": str,
         "NumberOfNodes": int,
         "PubliclyAccessible": bool,
     },
+    total=False,
 )
 
 AwsRedshiftClusterResizeInfoOutputTypeDef = TypedDict(
     "AwsRedshiftClusterResizeInfoOutputTypeDef",
     {
         "AllowCancelResize": bool,
         "ResizeType": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterRestoreStatusOutputTypeDef = TypedDict(
     "AwsRedshiftClusterRestoreStatusOutputTypeDef",
     {
         "CurrentRestoreRateInMegaBytesPerSecond": float,
         "ElapsedTimeInSeconds": int,
         "EstimatedTimeToCompletionInSeconds": int,
         "ProgressInMegaBytes": int,
         "SnapshotSizeInMegaBytes": int,
         "Status": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterVpcSecurityGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
     {
         "Status": str,
         "VpcSecurityGroupId": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterElasticIpStatusTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
@@ -6539,14 +6811,15 @@
     "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
         "IgnorePublicAcls": bool,
         "RestrictPublicBuckets": bool,
     },
+    total=False,
 )
 
 AwsS3AccountPublicAccessBlockDetailsTypeDef = TypedDict(
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
@@ -6557,14 +6830,15 @@
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
     {
         "DaysAfterInitiation": int,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef = (
     TypedDict(
         "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
         {
             "DaysAfterInitiation": int,
@@ -6575,23 +6849,25 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
     {
         "Days": int,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
     {
         "Date": str,
         "Days": int,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     {
         "Days": int,
         "StorageClass": str,
@@ -6611,14 +6887,15 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -6628,14 +6905,15 @@
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
     {
         "Key": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -6645,14 +6923,15 @@
 
 AwsS3BucketBucketVersioningConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketVersioningConfigurationTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
@@ -6662,14 +6941,15 @@
 
 AwsS3BucketLoggingConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationOutputTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
     },
+    total=False,
 )
 
 AwsS3BucketLoggingConfigurationTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
@@ -6679,14 +6959,15 @@
 
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
@@ -6697,14 +6978,15 @@
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
     {
         "Days": int,
         "Mode": str,
         "Years": int,
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     {
         "Days": int,
         "Mode": str,
@@ -6715,14 +6997,15 @@
 
 AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
@@ -6732,14 +7015,15 @@
 
 AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRedirectToTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
@@ -6749,14 +7033,15 @@
 
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
@@ -6769,14 +7054,15 @@
     {
         "Hostname": str,
         "HttpRedirectCode": str,
         "Protocol": str,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     {
         "Hostname": str,
         "HttpRedirectCode": str,
@@ -6793,14 +7079,15 @@
         "LastModified": str,
         "ETag": str,
         "VersionId": str,
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
+    total=False,
 )
 
 AwsS3ObjectDetailsTypeDef = TypedDict(
     "AwsS3ObjectDetailsTypeDef",
     {
         "LastModified": str,
         "ETag": str,
@@ -6813,14 +7100,15 @@
 )
 
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
+    total=False,
 )
 
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
@@ -6828,14 +7116,15 @@
 )
 
 AwsSecretsManagerSecretRotationRulesOutputTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
+    total=False,
 )
 
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
@@ -6843,28 +7132,31 @@
 )
 
 BooleanFilterOutputTypeDef = TypedDict(
     "BooleanFilterOutputTypeDef",
     {
         "Value": bool,
     },
+    total=False,
 )
 
 IpFilterOutputTypeDef = TypedDict(
     "IpFilterOutputTypeDef",
     {
         "Cidr": str,
     },
+    total=False,
 )
 
 KeywordFilterOutputTypeDef = TypedDict(
     "KeywordFilterOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 BooleanFilterTypeDef = TypedDict(
     "BooleanFilterTypeDef",
     {
         "Value": bool,
     },
@@ -6899,89 +7191,113 @@
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
 
-MalwareOutputTypeDef = TypedDict(
-    "MalwareOutputTypeDef",
+_RequiredMalwareOutputTypeDef = TypedDict(
+    "_RequiredMalwareOutputTypeDef",
     {
         "Name": str,
+    },
+)
+_OptionalMalwareOutputTypeDef = TypedDict(
+    "_OptionalMalwareOutputTypeDef",
+    {
         "Type": MalwareTypeType,
         "Path": str,
         "State": MalwareStateType,
     },
+    total=False,
 )
 
+class MalwareOutputTypeDef(_RequiredMalwareOutputTypeDef, _OptionalMalwareOutputTypeDef):
+    pass
+
 NoteOutputTypeDef = TypedDict(
     "NoteOutputTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
         "UpdatedAt": str,
     },
 )
 
-PatchSummaryOutputTypeDef = TypedDict(
-    "PatchSummaryOutputTypeDef",
+_RequiredPatchSummaryOutputTypeDef = TypedDict(
+    "_RequiredPatchSummaryOutputTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalPatchSummaryOutputTypeDef = TypedDict(
+    "_OptionalPatchSummaryOutputTypeDef",
+    {
         "InstalledCount": int,
         "MissingCount": int,
         "FailedCount": int,
         "InstalledOtherCount": int,
         "InstalledRejectedCount": int,
         "InstalledPendingReboot": int,
         "OperationStartTime": str,
         "OperationEndTime": str,
         "RebootOption": str,
         "Operation": str,
     },
+    total=False,
 )
 
+class PatchSummaryOutputTypeDef(
+    _RequiredPatchSummaryOutputTypeDef, _OptionalPatchSummaryOutputTypeDef
+):
+    pass
+
 ProcessDetailsOutputTypeDef = TypedDict(
     "ProcessDetailsOutputTypeDef",
     {
         "Name": str,
         "Path": str,
         "Pid": int,
         "ParentPid": int,
         "LaunchedAt": str,
         "TerminatedAt": str,
     },
+    total=False,
 )
 
 SeverityOutputTypeDef = TypedDict(
     "SeverityOutputTypeDef",
     {
         "Product": float,
         "Label": SeverityLabelType,
         "Normalized": int,
         "Original": str,
     },
+    total=False,
 )
 
 ThreatIntelIndicatorOutputTypeDef = TypedDict(
     "ThreatIntelIndicatorOutputTypeDef",
     {
         "Type": ThreatIntelIndicatorTypeType,
         "Value": str,
         "Category": ThreatIntelIndicatorCategoryType,
         "LastObservedAt": str,
         "Source": str,
         "SourceUrl": str,
     },
+    total=False,
 )
 
 WorkflowOutputTypeDef = TypedDict(
     "WorkflowOutputTypeDef",
     {
         "Status": WorkflowStatusType,
     },
+    total=False,
 )
 
 _RequiredMalwareTypeDef = TypedDict(
     "_RequiredMalwareTypeDef",
     {
         "Name": str,
     },
@@ -7081,14 +7397,15 @@
 
 AwsSnsTopicSubscriptionOutputTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionOutputTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
     },
+    total=False,
 )
 
 AwsSnsTopicSubscriptionTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
@@ -7100,14 +7417,15 @@
     "AwsSqsQueueDetailsOutputTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
         "QueueName": str,
         "DeadLetterTargetArn": str,
     },
+    total=False,
 )
 
 AwsSqsQueueDetailsTypeDef = TypedDict(
     "AwsSqsQueueDetailsTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
@@ -7135,14 +7453,15 @@
         "ComplianceType": str,
         "PatchBaselineId": str,
         "OverallSeverity": str,
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
+    total=False,
 )
 
 AwsSsmComplianceSummaryTypeDef = TypedDict(
     "AwsSsmComplianceSummaryTypeDef",
     {
         "Status": str,
         "CompliantCriticalCount": int,
@@ -7167,14 +7486,15 @@
 )
 
 AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
     {
         "Enabled": bool,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     {
         "Enabled": bool,
     },
@@ -7182,14 +7502,15 @@
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
     {
         "LogGroupArn": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     {
         "LogGroupArn": str,
     },
@@ -7199,14 +7520,15 @@
 AwsWafRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7218,14 +7540,15 @@
 AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7237,14 +7560,15 @@
 AwsWafRegionalRulePredicateListDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7254,14 +7578,15 @@
 )
 
 AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7269,14 +7594,15 @@
 )
 
 AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7284,14 +7610,15 @@
 )
 
 AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7301,14 +7628,15 @@
 AwsWafRulePredicateListDetailsOutputTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsOutputTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
@@ -7318,14 +7646,15 @@
 )
 
 AwsWafRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
@@ -7333,28 +7662,31 @@
 )
 
 WafActionOutputTypeDef = TypedDict(
     "WafActionOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 WafExcludedRuleOutputTypeDef = TypedDict(
     "WafExcludedRuleOutputTypeDef",
     {
         "RuleId": str,
     },
+    total=False,
 )
 
 WafOverrideActionOutputTypeDef = TypedDict(
     "WafOverrideActionOutputTypeDef",
     {
         "Type": str,
     },
+    total=False,
 )
 
 WafActionTypeDef = TypedDict(
     "WafActionTypeDef",
     {
         "Type": str,
     },
@@ -7379,14 +7711,15 @@
 
 AwsWafv2CustomHttpHeaderOutputTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderOutputTypeDef",
     {
         "Name": str,
         "Value": str,
     },
+    total=False,
 )
 
 AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -7397,14 +7730,15 @@
 AwsWafv2VisibilityConfigDetailsOutputTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
         "SampledRequestsEnabled": bool,
     },
+    total=False,
 )
 
 AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
@@ -7414,14 +7748,15 @@
 )
 
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
     {
         "ImmunityTime": int,
     },
+    total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     {
         "ImmunityTime": int,
     },
@@ -7431,14 +7766,15 @@
 AwsXrayEncryptionConfigDetailsOutputTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsOutputTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
@@ -7468,14 +7804,15 @@
 UnprocessedAutomationRuleTypeDef = TypedDict(
     "UnprocessedAutomationRuleTypeDef",
     {
         "RuleArn": str,
         "ErrorCode": int,
         "ErrorMessage": str,
     },
+    total=False,
 )
 
 BatchDisableStandardsRequestRequestTypeDef = TypedDict(
     "BatchDisableStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
     },
@@ -7523,47 +7860,70 @@
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "SecurityControlStatus": ControlStatusType,
     },
 )
 
-UnprocessedSecurityControlTypeDef = TypedDict(
-    "UnprocessedSecurityControlTypeDef",
+_RequiredUnprocessedSecurityControlTypeDef = TypedDict(
+    "_RequiredUnprocessedSecurityControlTypeDef",
     {
         "SecurityControlId": str,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedSecurityControlTypeDef = TypedDict(
+    "_OptionalUnprocessedSecurityControlTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
+class UnprocessedSecurityControlTypeDef(
+    _RequiredUnprocessedSecurityControlTypeDef, _OptionalUnprocessedSecurityControlTypeDef
+):
+    pass
+
 StandardsControlAssociationIdTypeDef = TypedDict(
     "StandardsControlAssociationIdTypeDef",
     {
         "SecurityControlId": str,
         "StandardsArn": str,
     },
 )
 
-StandardsControlAssociationDetailTypeDef = TypedDict(
-    "StandardsControlAssociationDetailTypeDef",
+_RequiredStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationDetailTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationDetailTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationDetailTypeDef",
+    {
         "RelatedRequirements": List[str],
         "UpdatedAt": datetime,
         "UpdatedReason": str,
         "StandardsControlTitle": str,
         "StandardsControlDescription": str,
         "StandardsControlArns": List[str],
     },
+    total=False,
 )
 
+class StandardsControlAssociationDetailTypeDef(
+    _RequiredStandardsControlAssociationDetailTypeDef,
+    _OptionalStandardsControlAssociationDetailTypeDef,
+):
+    pass
+
 ImportFindingsErrorTypeDef = TypedDict(
     "ImportFindingsErrorTypeDef",
     {
         "Id": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -7595,14 +7955,15 @@
     "CellOutputTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
     },
+    total=False,
 )
 
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
@@ -7614,33 +7975,45 @@
 
 ClassificationStatusOutputTypeDef = TypedDict(
     "ClassificationStatusOutputTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
+    total=False,
 )
 
 ClassificationStatusTypeDef = TypedDict(
     "ClassificationStatusTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-StatusReasonOutputTypeDef = TypedDict(
-    "StatusReasonOutputTypeDef",
+_RequiredStatusReasonOutputTypeDef = TypedDict(
+    "_RequiredStatusReasonOutputTypeDef",
     {
         "ReasonCode": str,
+    },
+)
+_OptionalStatusReasonOutputTypeDef = TypedDict(
+    "_OptionalStatusReasonOutputTypeDef",
+    {
         "Description": str,
     },
+    total=False,
 )
 
+class StatusReasonOutputTypeDef(
+    _RequiredStatusReasonOutputTypeDef, _OptionalStatusReasonOutputTypeDef
+):
+    pass
+
 _RequiredStatusReasonTypeDef = TypedDict(
     "_RequiredStatusReasonTypeDef",
     {
         "ReasonCode": str,
     },
 )
 _OptionalStatusReasonTypeDef = TypedDict(
@@ -7656,14 +8029,15 @@
 
 VolumeMountOutputTypeDef = TypedDict(
     "VolumeMountOutputTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
+    total=False,
 )
 
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
@@ -7702,22 +8076,24 @@
 
 ResultTypeDef = TypedDict(
     "ResultTypeDef",
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
+    total=False,
 )
 
 DateRangeOutputTypeDef = TypedDict(
     "DateRangeOutputTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
+    total=False,
 )
 
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
@@ -7801,29 +8177,38 @@
         "NextToken": str,
         "MaxResults": int,
         "ProductArn": str,
     },
     total=False,
 )
 
-ProductTypeDef = TypedDict(
-    "ProductTypeDef",
+_RequiredProductTypeDef = TypedDict(
+    "_RequiredProductTypeDef",
     {
         "ProductArn": str,
+    },
+)
+_OptionalProductTypeDef = TypedDict(
+    "_OptionalProductTypeDef",
+    {
         "ProductName": str,
         "CompanyName": str,
         "Description": str,
         "Categories": List[str],
         "IntegrationTypes": List[IntegrationTypeType],
         "MarketplaceUrl": str,
         "ActivationUrl": str,
         "ProductSubscriptionResourcePolicy": str,
     },
+    total=False,
 )
 
+class ProductTypeDef(_RequiredProductTypeDef, _OptionalProductTypeDef):
+    pass
+
 _RequiredDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeStandardsControlsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArn": str,
     },
 )
 _OptionalDescribeStandardsControlsRequestRequestTypeDef = TypedDict(
@@ -7851,14 +8236,15 @@
         "ControlId": str,
         "Title": str,
         "Description": str,
         "RemediationUrl": str,
         "SeverityRating": SeverityRatingType,
         "RelatedRequirements": List[str],
     },
+    total=False,
 )
 
 DescribeStandardsRequestRequestTypeDef = TypedDict(
     "DescribeStandardsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -7915,14 +8301,15 @@
     "FilePathsOutputTypeDef",
     {
         "FilePath": str,
         "FileName": str,
         "ResourceId": str,
         "Hash": str,
     },
+    total=False,
 )
 
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
         "FilePath": str,
         "FileName": str,
@@ -7933,39 +8320,43 @@
 )
 
 FindingAggregatorTypeDef = TypedDict(
     "FindingAggregatorTypeDef",
     {
         "FindingAggregatorArn": str,
     },
+    total=False,
 )
 
 FindingHistoryUpdateSourceTypeDef = TypedDict(
     "FindingHistoryUpdateSourceTypeDef",
     {
         "Type": FindingHistoryUpdateSourceTypeType,
         "Identity": str,
     },
+    total=False,
 )
 
 FindingHistoryUpdateTypeDef = TypedDict(
     "FindingHistoryUpdateTypeDef",
     {
         "UpdatedField": str,
         "OldValue": str,
         "NewValue": str,
     },
+    total=False,
 )
 
 FindingProviderSeverityOutputTypeDef = TypedDict(
     "FindingProviderSeverityOutputTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
+    total=False,
 )
 
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
@@ -7974,22 +8365,24 @@
 )
 
 FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
     {
         "ResourceArn": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
     {
         "Priority": int,
         "ResourceArn": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     {
         "ResourceArn": str,
     },
@@ -8009,14 +8402,15 @@
     "InvitationTypeDef",
     {
         "AccountId": str,
         "InvitationId": str,
         "InvitedAt": datetime,
         "MemberStatus": str,
     },
+    total=False,
 )
 
 GetEnabledStandardsRequestRequestTypeDef = TypedDict(
     "GetEnabledStandardsRequestRequestTypeDef",
     {
         "StandardsSubscriptionArns": Sequence[str],
         "NextToken": str,
@@ -8072,14 +8466,15 @@
         "Email": str,
         "MasterId": str,
         "AdministratorId": str,
         "MemberStatus": str,
         "InvitedAt": datetime,
         "UpdatedAt": datetime,
     },
+    total=False,
 )
 
 InsightResultValueTypeDef = TypedDict(
     "InsightResultValueTypeDef",
     {
         "GroupByAttributeValue": str,
         "Count": int,
@@ -8187,42 +8582,55 @@
 
 class ListStandardsControlAssociationsRequestRequestTypeDef(
     _RequiredListStandardsControlAssociationsRequestRequestTypeDef,
     _OptionalListStandardsControlAssociationsRequestRequestTypeDef,
 ):
     pass
 
-StandardsControlAssociationSummaryTypeDef = TypedDict(
-    "StandardsControlAssociationSummaryTypeDef",
+_RequiredStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationSummaryTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "SecurityControlArn": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationSummaryTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationSummaryTypeDef",
+    {
         "RelatedRequirements": List[str],
         "UpdatedAt": datetime,
         "UpdatedReason": str,
         "StandardsControlTitle": str,
         "StandardsControlDescription": str,
     },
+    total=False,
 )
 
+class StandardsControlAssociationSummaryTypeDef(
+    _RequiredStandardsControlAssociationSummaryTypeDef,
+    _OptionalStandardsControlAssociationSummaryTypeDef,
+):
+    pass
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
 PortRangeOutputTypeDef = TypedDict(
     "PortRangeOutputTypeDef",
     {
         "Begin": int,
         "End": int,
     },
+    total=False,
 )
 
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
@@ -8233,22 +8641,24 @@
 RangeOutputTypeDef = TypedDict(
     "RangeOutputTypeDef",
     {
         "Start": int,
         "End": int,
         "StartColumn": int,
     },
+    total=False,
 )
 
 RecordOutputTypeDef = TypedDict(
     "RecordOutputTypeDef",
     {
         "JsonPath": str,
         "RecordIndex": int,
     },
+    total=False,
 )
 
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Start": int,
         "End": int,
@@ -8268,14 +8678,15 @@
 
 RecommendationOutputTypeDef = TypedDict(
     "RecommendationOutputTypeDef",
     {
         "Text": str,
         "Url": str,
     },
+    total=False,
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
@@ -8286,14 +8697,15 @@
 RuleGroupSourceListDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceListDetailsOutputTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": List[str],
         "Targets": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceListDetailsTypeDef = TypedDict(
     "RuleGroupSourceListDetailsTypeDef",
     {
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
@@ -8308,22 +8720,24 @@
         "Destination": str,
         "DestinationPort": str,
         "Direction": str,
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     {
         "Keyword": str,
         "Settings": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     {
         "Destination": str,
         "DestinationPort": str,
@@ -8346,14 +8760,15 @@
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
@@ -8362,14 +8777,15 @@
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
     {
         "AddressDefinition": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     {
         "AddressDefinition": str,
     },
@@ -8378,29 +8794,32 @@
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
     {
         "AddressDefinition": str,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     {
         "Flags": List[str],
         "Masks": List[str],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
@@ -8426,14 +8845,15 @@
 )
 
 RuleGroupVariablesIpSetsDetailsOutputTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     {
         "Definition": List[str],
     },
+    total=False,
 )
 
 RuleGroupVariablesIpSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
@@ -8441,14 +8861,15 @@
 )
 
 RuleGroupVariablesPortSetsDetailsOutputTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     {
         "Definition": List[str],
     },
+    total=False,
 )
 
 RuleGroupVariablesPortSetsDetailsTypeDef = TypedDict(
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
@@ -8466,14 +8887,15 @@
         "PackageManager": str,
         "FilePath": str,
         "FixedInVersion": str,
         "Remediation": str,
         "SourceLayerHash": str,
         "SourceLayerArn": str,
     },
+    total=False,
 )
 
 SoftwarePackageTypeDef = TypedDict(
     "SoftwarePackageTypeDef",
     {
         "Name": str,
         "Version": str,
@@ -8492,46 +8914,60 @@
 
 StandardsManagedByTypeDef = TypedDict(
     "StandardsManagedByTypeDef",
     {
         "Company": str,
         "Product": str,
     },
+    total=False,
 )
 
 StandardsControlAssociationIdOutputTypeDef = TypedDict(
     "StandardsControlAssociationIdOutputTypeDef",
     {
         "SecurityControlId": str,
         "StandardsArn": str,
     },
 )
 
-StandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "StandardsControlAssociationUpdateOutputTypeDef",
+_RequiredStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
+    "_RequiredStandardsControlAssociationUpdateOutputTypeDef",
     {
         "StandardsArn": str,
         "SecurityControlId": str,
         "AssociationStatus": AssociationStatusType,
+    },
+)
+_OptionalStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
+    "_OptionalStandardsControlAssociationUpdateOutputTypeDef",
+    {
         "UpdatedReason": str,
     },
+    total=False,
 )
 
+class StandardsControlAssociationUpdateOutputTypeDef(
+    _RequiredStandardsControlAssociationUpdateOutputTypeDef,
+    _OptionalStandardsControlAssociationUpdateOutputTypeDef,
+):
+    pass
+
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
         "StatusReasonCode": StatusReasonCodeType,
     },
 )
 
 StatelessCustomPublishMetricActionDimensionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
     {
         "Value": str,
     },
+    total=False,
 )
 
 StatelessCustomPublishMetricActionDimensionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     {
         "Value": str,
     },
@@ -8642,25 +9078,36 @@
 
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
-VulnerabilityVendorOutputTypeDef = TypedDict(
-    "VulnerabilityVendorOutputTypeDef",
+_RequiredVulnerabilityVendorOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityVendorOutputTypeDef",
     {
         "Name": str,
+    },
+)
+_OptionalVulnerabilityVendorOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityVendorOutputTypeDef",
+    {
         "Url": str,
         "VendorSeverity": str,
         "VendorCreatedAt": str,
         "VendorUpdatedAt": str,
     },
+    total=False,
 )
 
+class VulnerabilityVendorOutputTypeDef(
+    _RequiredVulnerabilityVendorOutputTypeDef, _OptionalVulnerabilityVendorOutputTypeDef
+):
+    pass
+
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -8691,14 +9138,15 @@
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsOutputTypeDef,
         "Country": CountryOutputTypeDef,
         "City": CityOutputTypeDef,
         "GeoLocation": GeoLocationOutputTypeDef,
     },
+    total=False,
 )
 
 ActionRemoteIpDetailsTypeDef = TypedDict(
     "ActionRemoteIpDetailsTypeDef",
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsTypeDef,
@@ -8714,14 +9162,15 @@
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
         "Adjustments": List[AdjustmentOutputTypeDef],
     },
+    total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
         "Version": str,
         "BaseScore": float,
@@ -8738,14 +9187,15 @@
         "AssociationState": AssociationStateDetailsOutputTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
         "RouteTableId": str,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
@@ -8766,14 +9216,15 @@
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
         "Workflow": WorkflowUpdateOutputTypeDef,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
     },
+    total=False,
 )
 
 AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateTypeDef",
     {
         "Note": NoteUpdateTypeDef,
         "Severity": SeverityUpdateTypeDef,
@@ -8793,14 +9244,15 @@
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
         "Pending": AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
@@ -8820,14 +9272,15 @@
         "CreatedDate": str,
         "Version": str,
         "BinaryMediaTypes": List[str],
         "MinimumCompressionSize": int,
         "ApiKeySource": str,
         "EndpointConfiguration": AwsApiGatewayEndpointConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiGatewayRestApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayRestApiDetailsTypeDef",
     {
         "Id": str,
         "Name": str,
@@ -8858,14 +9311,15 @@
         "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
         "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
         "TracingEnabled": bool,
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
+    total=False,
 )
 
 AwsApiGatewayStageDetailsTypeDef = TypedDict(
     "AwsApiGatewayStageDetailsTypeDef",
     {
         "DeploymentId": str,
         "ClientCertificateId": str,
@@ -8897,14 +9351,15 @@
         "Description": str,
         "Version": str,
         "Name": str,
         "ProtocolType": str,
         "RouteSelectionExpression": str,
         "CorsConfiguration": AwsCorsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiGatewayV2ApiDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2ApiDetailsTypeDef",
     {
         "ApiEndpoint": str,
         "ApiId": str,
@@ -8933,14 +9388,15 @@
         "StageName": str,
         "StageVariables": Dict[str, str],
         "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
+    total=False,
 )
 
 AwsApiGatewayV2StageDetailsTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
@@ -8963,14 +9419,15 @@
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
@@ -8981,14 +9438,15 @@
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
     {
         "EncryptionConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
@@ -9001,14 +9459,15 @@
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
         "Overrides": List[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[
@@ -9022,14 +9481,15 @@
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
         "NoDevice": bool,
         "VirtualName": str,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
@@ -9041,14 +9501,15 @@
 
 AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
@@ -9061,14 +9522,15 @@
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
         "AccessPolicy": str,
     },
+    total=False,
 )
 
 AwsBackupBackupVaultDetailsTypeDef = TypedDict(
     "AwsBackupBackupVaultDetailsTypeDef",
     {
         "BackupVaultArn": str,
         "BackupVaultName": str,
@@ -9098,14 +9560,15 @@
         "ResourceArn": str,
         "ResourceType": str,
         "SourceBackupVaultArn": str,
         "Status": str,
         "StatusMessage": str,
         "StorageClass": str,
     },
+    total=False,
 )
 
 AwsBackupRecoveryPointDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointDetailsTypeDef",
     {
         "BackupSizeInBytes": int,
         "BackupVaultArn": str,
@@ -9136,14 +9599,15 @@
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": List[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateDomainValidationOptionTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     {
         "DomainName": str,
         "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
@@ -9170,14 +9634,15 @@
         "RoleArn": str,
         "StackId": str,
         "StackName": str,
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
+    total=False,
 )
 
 AwsCloudFormationStackDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsTypeDef",
     {
         "Capabilities": Sequence[str],
         "CreationTime": str,
@@ -9199,14 +9664,15 @@
 )
 
 AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionCacheBehaviorOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
@@ -9219,14 +9685,15 @@
         "HttpPort": int,
         "HttpsPort": int,
         "OriginKeepaliveTimeout": int,
         "OriginProtocolPolicy": str,
         "OriginReadTimeout": int,
         "OriginSslProtocols": AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     {
         "HttpPort": int,
         "HttpsPort": int,
@@ -9239,14 +9706,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupFailoverTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     {
         "StatusCodes": AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
     },
@@ -9275,14 +9743,15 @@
         "Period": int,
         "Statistic": str,
         "Threshold": float,
         "ThresholdMetricId": str,
         "TreatMissingData": str,
         "Unit": str,
     },
+    total=False,
 )
 
 AwsCloudWatchAlarmDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDetailsTypeDef",
     {
         "ActionsEnabled": bool,
         "AlarmActions": Sequence[str],
@@ -9318,14 +9787,15 @@
             AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef
         ],
         "PrivilegedMode": bool,
         "ImagePullCredentialsType": str,
         "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": Sequence[
@@ -9341,14 +9811,15 @@
 
 AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
@@ -9365,24 +9836,26 @@
         "IndexSizeBytes": int,
         "IndexStatus": str,
         "ItemCount": int,
         "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
         "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": str,
         "IndexName": str,
         "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     {
         "Backfilling": bool,
         "IndexArn": str,
@@ -9410,14 +9883,15 @@
 
 AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
     },
+    total=False,
 )
 
 AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
@@ -9438,14 +9912,15 @@
         "SubnetId": str,
         "LaunchedAt": str,
         "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef],
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsOutputTypeDef,
         "Monitoring": AwsEc2InstanceMonitoringDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
         "Type": str,
         "ImageId": str,
@@ -9468,14 +9943,15 @@
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
         "NoDevice": str,
         "VirtualName": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
@@ -9487,14 +9963,15 @@
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
@@ -9504,14 +9981,15 @@
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
@@ -9550,14 +10028,15 @@
         "RequireHibernateSupport": bool,
         "SpotMaxPricePercentageOverLowestPrice": int,
         "TotalLocalStorageGB": (
             AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef
         ),
         "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
         "AcceleratorCount": (
             AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
@@ -9623,14 +10102,15 @@
         "PrivateIpAddress": str,
         "PrivateIpAddresses": List[
             AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
     {
         "AssociateCarrierIpAddress": bool,
         "AssociatePublicIpAddress": bool,
@@ -9671,14 +10151,15 @@
         "IcmpTypeCode": IcmpTypeCodeOutputTypeDef,
         "Ipv6CidrBlock": str,
         "PortRange": PortRangeFromToOutputTypeDef,
         "Protocol": str,
         "RuleAction": str,
         "RuleNumber": int,
     },
+    total=False,
 )
 
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
@@ -9700,14 +10181,15 @@
         "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef],
         "SourceDestCheck": bool,
         "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef],
         "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
+    total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     {
         "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
@@ -9728,14 +10210,15 @@
         "FromPort": int,
         "ToPort": int,
         "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef],
         "IpRanges": List[AwsEc2SecurityGroupIpRangeOutputTypeDef],
         "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeOutputTypeDef],
         "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
@@ -9761,14 +10244,15 @@
         "OwnerId": str,
         "State": str,
         "SubnetArn": str,
         "SubnetId": str,
         "VpcId": str,
         "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
         "AssignIpv6AddressOnCreation": bool,
         "AvailabilityZone": str,
@@ -9798,14 +10282,15 @@
         "Status": str,
         "KmsKeyId": str,
         "Attachments": List[AwsEc2VolumeAttachmentOutputTypeDef],
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
+    total=False,
 )
 
 AwsEc2VolumeDetailsTypeDef = TypedDict(
     "AwsEc2VolumeDetailsTypeDef",
     {
         "CreateTime": str,
         "DeviceName": str,
@@ -9826,14 +10311,15 @@
     "AwsEc2VpcDetailsOutputTypeDef",
     {
         "CidrBlockAssociationSet": List[CidrBlockAssociationOutputTypeDef],
         "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
+    total=False,
 )
 
 AwsEc2VpcDetailsTypeDef = TypedDict(
     "AwsEc2VpcDetailsTypeDef",
     {
         "CidrBlockAssociationSet": Sequence[CidrBlockAssociationTypeDef],
         "Ipv6CidrBlockAssociationSet": Sequence[Ipv6CidrBlockAssociationTypeDef],
@@ -9854,14 +10340,15 @@
         "NetworkLoadBalancerArns": List[str],
         "PrivateDnsName": str,
         "ServiceId": str,
         "ServiceName": str,
         "ServiceState": str,
         "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
         "AcceptanceRequired": bool,
         "AvailabilityZones": Sequence[str],
@@ -9885,14 +10372,15 @@
         "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsOutputTypeDef],
         "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef],
         "OwnerId": str,
         "PeeringOptions": VpcInfoPeeringOptionsDetailsOutputTypeDef,
         "Region": str,
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     {
         "CidrBlock": str,
         "CidrBlockSet": Sequence[VpcInfoCidrBlockSetDetailsTypeDef],
@@ -9907,14 +10395,15 @@
 
 AwsEc2VpnConnectionOptionsDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": List[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionOptionsDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
@@ -9930,14 +10419,15 @@
             AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef
         ),
         "ImageTagMutability": str,
         "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
         "RepositoryName": str,
         "RepositoryPolicyText": str,
     },
+    total=False,
 )
 
 AwsEcrRepositoryDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryDetailsTypeDef",
     {
         "Arn": str,
         "ImageScanningConfiguration": AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
@@ -9952,14 +10442,15 @@
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
         "Logging": str,
     },
+    total=False,
 )
 
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": (
@@ -9974,14 +10465,15 @@
     "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": str,
         "Image": str,
         "MountPoints": List[AwsMountPointOutputTypeDef],
         "Privileged": bool,
     },
+    total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
     {
         "Name": str,
         "Image": str,
@@ -9996,14 +10488,15 @@
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef
         ),
         "MaximumPercent": int,
         "MinimumHealthyPercent": int,
     },
+    total=False,
 )
 
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
@@ -10017,14 +10510,15 @@
 AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     {
         "AwsVpcConfiguration": (
             AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsEcsServiceNetworkConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     {
         "AwsVpcConfiguration": AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
     },
@@ -10044,14 +10538,15 @@
         "MaxSwap": int,
         "SharedMemorySize": int,
         "Swappiness": int,
         "Tmpfs": List[
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     {
         "Capabilities": (
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef
@@ -10075,14 +10570,15 @@
     {
         "LogDriver": str,
         "Options": Dict[str, str],
         "SecretOptions": List[
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     {
         "LogDriver": str,
         "Options": Mapping[str, str],
@@ -10098,14 +10594,15 @@
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": List[
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef
         ],
         "Type": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": Sequence[
@@ -10123,14 +10620,15 @@
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef
         ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
         "AuthorizationConfig": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
@@ -10145,14 +10643,15 @@
 
 AwsEcsTaskVolumeDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsOutputTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEcsTaskVolumeDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsTypeDef,
@@ -10162,14 +10661,15 @@
 
 AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
         "Path": str,
     },
+    total=False,
 )
 
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
@@ -10178,14 +10678,15 @@
 )
 
 AwsEksClusterLoggingDetailsOutputTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsOutputTypeDef",
     {
         "ClusterLogging": List[AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEksClusterLoggingDetailsTypeDef = TypedDict(
     "AwsEksClusterLoggingDetailsTypeDef",
     {
         "ClusterLogging": Sequence[AwsEksClusterLoggingClusterLoggingDetailsTypeDef],
     },
@@ -10208,14 +10709,15 @@
         "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef],
         "PlatformArn": str,
         "SolutionStackName": str,
         "Status": str,
         "Tier": AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
         "VersionLabel": str,
     },
+    total=False,
 )
 
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
     {
         "ApplicationName": str,
         "Cname": str,
@@ -10246,14 +10748,15 @@
         "InstanceCount": int,
         "InstanceType": str,
         "ZoneAwarenessConfig": (
             AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
         ),
         "ZoneAwarenessEnabled": bool,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
@@ -10271,14 +10774,15 @@
 AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
@@ -10290,14 +10794,15 @@
 AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
         "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyOutputTypeDef],
         "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyOutputTypeDef],
         "OtherPolicies": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
     {
         "AppCookieStickinessPolicies": Sequence[AwsElbAppCookieStickinessPolicyTypeDef],
         "LbCookieStickinessPolicies": Sequence[AwsElbLbCookieStickinessPolicyTypeDef],
@@ -10311,14 +10816,15 @@
     {
         "AccessLog": AwsElbLoadBalancerAccessLogOutputTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
         "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
         "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
         "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeOutputTypeDef],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
         "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
         "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
@@ -10331,14 +10837,15 @@
 
 AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerOutputTypeDef,
         "PolicyNames": List[str],
     },
+    total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     {
         "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": Sequence[str],
@@ -10357,14 +10864,15 @@
         "Scheme": str,
         "SecurityGroups": List[str],
         "State": LoadBalancerStateOutputTypeDef,
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeOutputTypeDef],
     },
+    total=False,
 )
 
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
@@ -10382,14 +10890,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
     },
@@ -10397,14 +10906,15 @@
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
     },
@@ -10413,14 +10923,15 @@
 
 AwsIamAccessKeySessionContextOutputTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextOutputTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesOutputTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
     },
+    total=False,
 )
 
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
@@ -10434,14 +10945,15 @@
         "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
         "GroupPolicyList": List[AwsIamGroupPolicyOutputTypeDef],
         "Path": str,
     },
+    total=False,
 )
 
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
@@ -10459,14 +10971,15 @@
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
         "Roles": List[AwsIamInstanceProfileRoleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
@@ -10489,14 +11002,15 @@
         "Path": str,
         "PermissionsBoundaryUsageCount": int,
         "PolicyId": str,
         "PolicyName": str,
         "PolicyVersionList": List[AwsIamPolicyVersionOutputTypeDef],
         "UpdateDate": str,
     },
+    total=False,
 )
 
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
     {
         "AttachmentCount": int,
         "CreateDate": str,
@@ -10521,14 +11035,15 @@
         "GroupList": List[str],
         "Path": str,
         "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
         "UserId": str,
         "UserName": str,
         "UserPolicyList": List[AwsIamUserPolicyOutputTypeDef],
     },
+    total=False,
 )
 
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
@@ -10547,14 +11062,15 @@
     {
         "Name": str,
         "Arn": str,
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
         "ShardCount": int,
         "RetentionPeriodHours": int,
     },
+    total=False,
 )
 
 AwsKinesisStreamDetailsTypeDef = TypedDict(
     "AwsKinesisStreamDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
@@ -10567,14 +11083,15 @@
 
 AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": Dict[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
     },
+    total=False,
 )
 
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
         "Variables": Mapping[str, str],
         "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
@@ -10592,14 +11109,15 @@
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyChangeProtection": bool,
         "SubnetChangeProtection": bool,
         "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
     {
         "DeleteProtection": bool,
         "Description": str,
@@ -10618,14 +11136,15 @@
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
         "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
@@ -10646,14 +11165,15 @@
         ),
         "DedicatedMasterCount": int,
         "InstanceType": str,
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
@@ -10674,14 +11194,15 @@
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
@@ -10727,14 +11248,15 @@
         "DbClusterParameterGroup": str,
         "DbSubnetGroup": str,
         "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipOutputTypeDef],
         "DbClusterIdentifier": str,
         "DbClusterMembers": List[AwsRdsDbClusterMemberOutputTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
+    total=False,
 )
 
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
     {
         "AllocatedStorage": int,
         "AvailabilityZones": Sequence[str],
@@ -10798,14 +11320,15 @@
         "DbClusterIdentifier": str,
         "DbClusterSnapshotIdentifier": str,
         "IamDatabaseAuthenticationEnabled": bool,
         "DbClusterSnapshotAttributes": List[
             AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsRdsDbClusterSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SnapshotCreateTime": str,
@@ -10859,14 +11382,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "Timezone": str,
         "IamDatabaseAuthenticationEnabled": bool,
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
         "DbiResourceId": str,
     },
+    total=False,
 )
 
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
     {
         "DbSnapshotIdentifier": str,
         "DbInstanceIdentifier": str,
@@ -10914,14 +11438,15 @@
         "DbInstanceIdentifier": str,
         "StorageType": str,
         "CaCertificateIdentifier": str,
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
     },
+    total=False,
 )
 
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
         "DbInstanceClass": str,
         "AllocatedStorage": int,
@@ -10949,14 +11474,15 @@
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
         "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef],
         "IpRanges": List[AwsRdsDbSecurityGroupIpRangeOutputTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
@@ -10972,14 +11498,15 @@
 AwsRdsDbSubnetGroupSubnetOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
         "SubnetStatus": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupSubnetTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
@@ -10991,14 +11518,15 @@
 AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
         "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusOutputTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
+    total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
     {
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
@@ -11010,14 +11538,15 @@
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
@@ -11027,14 +11556,15 @@
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
         "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
@@ -11044,14 +11574,15 @@
 AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
     {
         "DefaultRetention": (
             AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     {
         "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     },
@@ -11059,14 +11590,15 @@
 )
 
 AwsS3BucketServerSideEncryptionRuleOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
@@ -11075,14 +11607,15 @@
 
 AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
@@ -11112,14 +11645,15 @@
         "RoleArn": str,
         "RootAccess": str,
         "SecurityGroups": List[str],
         "SubnetId": str,
         "Url": str,
         "VolumeSizeInGB": int,
     },
+    total=False,
 )
 
 AwsSageMakerNotebookInstanceDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
     {
         "AcceleratorTypes": Sequence[str],
         "AdditionalCodeRepositories": Sequence[str],
@@ -11155,14 +11689,15 @@
         "KmsKeyId": str,
         "RotationEnabled": bool,
         "RotationLambdaArn": str,
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
+    total=False,
 )
 
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
@@ -11246,14 +11781,15 @@
         "SqsFailureFeedbackRoleArn": str,
         "ApplicationSuccessFeedbackRoleArn": str,
         "FirehoseSuccessFeedbackRoleArn": str,
         "FirehoseFailureFeedbackRoleArn": str,
         "HttpSuccessFeedbackRoleArn": str,
         "HttpFailureFeedbackRoleArn": str,
     },
+    total=False,
 )
 
 AwsSnsTopicDetailsTypeDef = TypedDict(
     "AwsSnsTopicDetailsTypeDef",
     {
         "KmsMasterKeyId": str,
         "Subscription": Sequence[AwsSnsTopicSubscriptionTypeDef],
@@ -11271,14 +11807,15 @@
 )
 
 AwsSsmPatchOutputTypeDef = TypedDict(
     "AwsSsmPatchOutputTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryOutputTypeDef,
     },
+    total=False,
 )
 
 AwsSsmPatchTypeDef = TypedDict(
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
@@ -11286,14 +11823,15 @@
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
@@ -11306,14 +11844,15 @@
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11331,14 +11870,15 @@
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
         "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11354,14 +11894,15 @@
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": List[AwsWafRegionalRulePredicateListDetailsOutputTypeDef],
         "RuleId": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11375,14 +11916,15 @@
     "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
@@ -11397,14 +11939,15 @@
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclRulesListDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
@@ -11419,14 +11962,15 @@
     "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "PredicateList": List[AwsWafRulePredicateListDetailsOutputTypeDef],
         "RuleId": str,
     },
+    total=False,
 )
 
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -11440,14 +11984,15 @@
     "AwsWafRuleGroupRulesDetailsOutputTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
@@ -11463,14 +12008,15 @@
         "Action": WafActionOutputTypeDef,
         "ExcludedRules": List[WafExcludedRuleOutputTypeDef],
         "OverrideAction": WafOverrideActionOutputTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsWafWebAclRuleTypeDef = TypedDict(
     "AwsWafWebAclRuleTypeDef",
     {
         "Action": WafActionTypeDef,
         "ExcludedRules": Sequence[WafExcludedRuleTypeDef],
@@ -11483,23 +12029,25 @@
 )
 
 AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
         "InsertHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
         "ResponseHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
@@ -11517,14 +12065,15 @@
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
         "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
     },
@@ -11748,14 +12297,15 @@
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": List[str],
         "StatusReasons": List[StatusReasonOutputTypeDef],
         "SecurityControlId": str,
         "AssociatedStandards": List[AssociatedStandardOutputTypeDef],
     },
+    total=False,
 )
 
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": Sequence[str],
@@ -11773,14 +12323,15 @@
         "Name": str,
         "ImageId": str,
         "ImageName": str,
         "LaunchedAt": str,
         "VolumeMounts": List[VolumeMountOutputTypeDef],
         "Privileged": bool,
     },
+    total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
@@ -11836,14 +12387,15 @@
 DateFilterOutputTypeDef = TypedDict(
     "DateFilterOutputTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeOutputTypeDef,
     },
+    total=False,
 )
 
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
@@ -12030,14 +12582,15 @@
     "ThreatOutputTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
         "FilePaths": List[FilePathsOutputTypeDef],
     },
+    total=False,
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
         "Name": str,
         "Severity": str,
@@ -12062,25 +12615,27 @@
         "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
         "UpdateTime": datetime,
         "FindingCreated": bool,
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
+    total=False,
 )
 
 FindingProviderFieldsOutputTypeDef = TypedDict(
     "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
         "Severity": FindingProviderSeverityOutputTypeDef,
         "Types": List[str],
     },
+    total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
@@ -12173,22 +12728,24 @@
         "SourceDomain": str,
         "SourceMac": str,
         "DestinationIpV4": str,
         "DestinationIpV6": str,
         "DestinationPort": int,
         "DestinationDomain": str,
     },
+    total=False,
 )
 
 NetworkPathComponentDetailsOutputTypeDef = TypedDict(
     "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": List[str],
         "PortRanges": List[PortRangeOutputTypeDef],
     },
+    total=False,
 )
 
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
         "Address": Sequence[str],
         "PortRanges": Sequence[PortRangeTypeDef],
@@ -12218,14 +12775,15 @@
 PageOutputTypeDef = TypedDict(
     "PageOutputTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeOutputTypeDef,
         "OffsetRange": RangeOutputTypeDef,
     },
+    total=False,
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeTypeDef,
@@ -12235,14 +12793,15 @@
 )
 
 RemediationOutputTypeDef = TypedDict(
     "RemediationOutputTypeDef",
     {
         "Recommendation": RecommendationOutputTypeDef,
     },
+    total=False,
 )
 
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
@@ -12252,14 +12811,15 @@
 RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
         "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     {
         "Action": str,
         "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
@@ -12276,14 +12836,15 @@
         ],
         "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef],
         "Protocols": List[int],
         "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef],
         "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef],
         "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     {
         "DestinationPorts": Sequence[
             RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
@@ -12299,14 +12860,15 @@
 
 RuleGroupVariablesOutputTypeDef = TypedDict(
     "RuleGroupVariablesOutputTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsOutputTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupVariablesTypeDef = TypedDict(
     "RuleGroupVariablesTypeDef",
     {
         "IpSets": RuleGroupVariablesIpSetsDetailsTypeDef,
         "PortSets": RuleGroupVariablesPortSetsDetailsTypeDef,
@@ -12319,50 +12881,87 @@
     {
         "StandardsArn": str,
         "Name": str,
         "Description": str,
         "EnabledByDefault": bool,
         "StandardsManagedBy": StandardsManagedByTypeDef,
     },
+    total=False,
 )
 
-UnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "UnprocessedStandardsControlAssociationTypeDef",
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
     {
         "StandardsControlAssociationId": StandardsControlAssociationIdOutputTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
-UnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
+
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
     {
         "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateOutputTypeDef,
         "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
         "ErrorReason": str,
     },
+    total=False,
 )
 
-StandardsSubscriptionTypeDef = TypedDict(
-    "StandardsSubscriptionTypeDef",
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
+_RequiredStandardsSubscriptionTypeDef = TypedDict(
+    "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
+    },
+)
+_OptionalStandardsSubscriptionTypeDef = TypedDict(
+    "_OptionalStandardsSubscriptionTypeDef",
+    {
         "StandardsStatusReason": StandardsStatusReasonTypeDef,
     },
+    total=False,
 )
 
+class StandardsSubscriptionTypeDef(
+    _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
+):
+    pass
+
 StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionOutputTypeDef",
     {
         "Dimensions": List[StatelessCustomPublishMetricActionDimensionOutputTypeDef],
     },
+    total=False,
 )
 
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
         "Dimensions": Sequence[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
@@ -12377,35 +12976,38 @@
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
         "DomainDetails": AwsApiCallActionDomainDetailsOutputTypeDef,
         "AffectedResources": Dict[str, str],
         "FirstSeen": str,
         "LastSeen": str,
     },
+    total=False,
 )
 
 NetworkConnectionActionOutputTypeDef = TypedDict(
     "NetworkConnectionActionOutputTypeDef",
     {
         "ConnectionDirection": str,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
         "RemotePortDetails": ActionRemotePortDetailsOutputTypeDef,
         "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
         "Protocol": str,
         "Blocked": bool,
     },
+    total=False,
 )
 
 PortProbeDetailOutputTypeDef = TypedDict(
     "PortProbeDetailOutputTypeDef",
     {
         "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsOutputTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
@@ -12438,27 +13040,38 @@
         "LocalPortDetails": ActionLocalPortDetailsTypeDef,
         "LocalIpDetails": ActionLocalIpDetailsTypeDef,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
     },
     total=False,
 )
 
-VulnerabilityOutputTypeDef = TypedDict(
-    "VulnerabilityOutputTypeDef",
+_RequiredVulnerabilityOutputTypeDef = TypedDict(
+    "_RequiredVulnerabilityOutputTypeDef",
     {
         "Id": str,
+    },
+)
+_OptionalVulnerabilityOutputTypeDef = TypedDict(
+    "_OptionalVulnerabilityOutputTypeDef",
+    {
         "VulnerablePackages": List[SoftwarePackageOutputTypeDef],
         "Cvss": List[CvssOutputTypeDef],
         "RelatedVulnerabilities": List[str],
         "Vendor": VulnerabilityVendorOutputTypeDef,
         "ReferenceUrls": List[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
+    total=False,
 )
 
+class VulnerabilityOutputTypeDef(
+    _RequiredVulnerabilityOutputTypeDef, _OptionalVulnerabilityOutputTypeDef
+):
+    pass
+
 _RequiredVulnerabilityTypeDef = TypedDict(
     "_RequiredVulnerabilityTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityTypeDef = TypedDict(
@@ -12483,14 +13096,15 @@
         "AssociationSet": List[AssociationSetDetailsOutputTypeDef],
         "OwnerId": str,
         "PropagatingVgwSet": List[PropagatingVgwSetDetailsOutputTypeDef],
         "RouteTableId": str,
         "RouteSet": List[RouteSetDetailsOutputTypeDef],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
     {
         "AssociationSet": Sequence[AssociationSetDetailsTypeDef],
         "OwnerId": str,
@@ -12504,14 +13118,15 @@
 
 AutomationRulesActionOutputTypeDef = TypedDict(
     "AutomationRulesActionOutputTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateOutputTypeDef,
     },
+    total=False,
 )
 
 AutomationRulesActionTypeDef = TypedDict(
     "AutomationRulesActionTypeDef",
     {
         "Type": Literal["FINDING_FIELDS_UPDATE"],
         "FindingFieldsUpdate": AutomationRulesFindingFieldsUpdateTypeDef,
@@ -12539,14 +13154,15 @@
         ),
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": str,
         "SubnetIds": List[str],
         "Users": List[AwsAmazonMqBrokerUsersDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
@@ -12584,14 +13200,15 @@
         "AuthenticationType": str,
         "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
         "AdditionalAuthenticationProviders": List[
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef
         ],
         "WafWebAclArn": str,
     },
+    total=False,
 )
 
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsTypeDef",
     {
         "ApiId": str,
         "Id": str,
@@ -12614,14 +13231,15 @@
 AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
     {
         "ResultConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     },
@@ -12632,14 +13250,15 @@
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     {
         "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     {
         "InstancesDistribution": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
@@ -12674,14 +13293,15 @@
         "PlacementTenancy": str,
         "RamdiskId": str,
         "SecurityGroups": List[str],
         "SpotPrice": str,
         "UserData": str,
         "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": Sequence[
@@ -12717,14 +13337,15 @@
         "RuleName": str,
         "RuleId": str,
         "EnableContinuousBackup": bool,
         "CompletionWindowMinutes": int,
         "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef],
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
@@ -12745,14 +13366,15 @@
         "DomainValidationOptions": List[
             AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
         ],
         "RenewalStatus": str,
         "RenewalStatusReason": str,
         "UpdatedAt": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateRenewalSummaryTypeDef = TypedDict(
     "AwsCertificateManagerCertificateRenewalSummaryTypeDef",
     {
         "DomainValidationOptions": Sequence[
             AwsCertificateManagerCertificateDomainValidationOptionTypeDef
@@ -12769,14 +13391,15 @@
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
         "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
     {
         "DomainName": str,
         "Id": str,
@@ -12788,14 +13411,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupOutputTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupTypeDef",
     {
         "FailoverCriteria": AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     },
@@ -12811,14 +13435,15 @@
         "Name": str,
         "Source": AwsCodeBuildProjectSourceOutputTypeDef,
         "ServiceRole": str,
         "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
         "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
         "EncryptionKey": str,
         "Artifacts": Sequence[AwsCodeBuildProjectArtifactsDetailsTypeDef],
@@ -12839,14 +13464,15 @@
         "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef],
         "KmsMasterKeyId": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableReplicaTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaTypeDef",
     {
         "GlobalSecondaryIndexes": Sequence[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
@@ -12898,14 +13524,15 @@
         "Placement": AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
         "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
         "RamDiskId": str,
         "SecurityGroupIdSet": List[str],
         "SecurityGroupSet": List[str],
         "UserData": str,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDataDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsTypeDef",
     {
         "BlockDeviceMappingSet": Sequence[
             AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef
@@ -12955,14 +13582,15 @@
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
         "Associations": List[AwsEc2NetworkAclAssociationOutputTypeDef],
         "Entries": List[AwsEc2NetworkAclEntryOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
@@ -12980,14 +13608,15 @@
         "GroupName": str,
         "GroupId": str,
         "OwnerId": str,
         "VpcId": str,
         "IpPermissions": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
         "IpPermissionsEgress": List[AwsEc2SecurityGroupIpPermissionOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEc2SecurityGroupDetailsTypeDef = TypedDict(
     "AwsEc2SecurityGroupDetailsTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
@@ -13004,14 +13633,15 @@
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "Status": AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
         "VpcPeeringConnectionId": str,
     },
+    total=False,
 )
 
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
         "ExpirationTime": str,
@@ -13033,14 +13663,15 @@
         "VpnGatewayId": str,
         "Category": str,
         "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef],
         "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
         "Routes": List[AwsEc2VpnConnectionRoutesDetailsOutputTypeDef],
         "TransitGatewayId": str,
     },
+    total=False,
 )
 
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
     {
         "VpnConnectionId": str,
         "State": str,
@@ -13060,14 +13691,15 @@
 AwsEcsClusterConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsOutputTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
@@ -13098,14 +13730,15 @@
         "Role": str,
         "SchedulingStrategy": str,
         "ServiceArn": str,
         "ServiceName": str,
         "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsOutputTypeDef],
         "TaskDefinition": str,
     },
+    total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
     {
         "CapacityProviderStrategy": Sequence[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
@@ -13194,14 +13827,15 @@
         "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef],
         "User": str,
         "VolumesFrom": List[
             AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef
         ],
         "WorkingDirectory": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     {
         "Command": Sequence[str],
         "Cpu": int,
@@ -13266,14 +13900,15 @@
         ),
         "EfsVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef
         ),
         "Host": AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
         "Name": str,
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef
@@ -13294,14 +13929,15 @@
         "CreatedAt": str,
         "StartedAt": str,
         "StartedBy": str,
         "Group": str,
         "Volumes": List[AwsEcsTaskVolumeDetailsOutputTypeDef],
         "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
     {
         "ClusterArn": str,
         "TaskDefinitionArn": str,
@@ -13322,14 +13958,15 @@
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
         "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
@@ -13350,14 +13987,15 @@
         "Endpoint": str,
         "Name": str,
         "ResourcesVpcConfig": AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
         "RoleArn": str,
         "Version": str,
         "Logging": AwsEksClusterLoggingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsEksClusterDetailsTypeDef = TypedDict(
     "AwsEksClusterDetailsTypeDef",
     {
         "Arn": str,
         "CertificateAuthorityData": str,
@@ -13389,14 +14027,15 @@
         "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
         "NodeToNodeEncryptionOptions": (
             AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef
         ),
         "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
     {
         "AccessPolicies": str,
         "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
@@ -13434,14 +14073,15 @@
         "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
         "Scheme": str,
         "SecurityGroups": List[str],
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
         "Subnets": List[str],
         "VpcId": str,
     },
+    total=False,
 )
 
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbLoadBalancerDetailsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "BackendServerDescriptions": Sequence[AwsElbLoadBalancerBackendServerDescriptionTypeDef],
@@ -13466,14 +14106,15 @@
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
         "ServiceRole": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
         "ServiceRole": str,
@@ -13490,14 +14131,15 @@
         "PrincipalId": str,
         "PrincipalType": str,
         "PrincipalName": str,
         "AccountId": str,
         "AccessKeyId": str,
         "SessionContext": AwsIamAccessKeySessionContextOutputTypeDef,
     },
+    total=False,
 )
 
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
@@ -13522,14 +14164,15 @@
         "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
         "RoleId": str,
         "RoleName": str,
         "RolePolicyList": List[AwsIamRolePolicyOutputTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
+    total=False,
 )
 
 AwsIamRoleDetailsTypeDef = TypedDict(
     "AwsIamRoleDetailsTypeDef",
     {
         "AssumeRolePolicyDocument": str,
         "AttachedManagedPolicies": Sequence[AwsIamAttachedManagedPolicyTypeDef],
@@ -13565,14 +14208,15 @@
         "Timeout": int,
         "TracingConfig": AwsLambdaFunctionTracingConfigOutputTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
         "Version": str,
         "Architectures": List[str],
         "PackageType": str,
     },
+    total=False,
 )
 
 AwsLambdaFunctionDetailsTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsTypeDef",
     {
         "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
@@ -13623,14 +14267,15 @@
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
         "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
         "DomainEndpoints": Dict[str, str],
         "AdvancedSecurityOptions": (
             AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
         "Arn": str,
         "AccessPolicies": str,
@@ -13659,14 +14304,15 @@
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[AwsRdsDbSubnetGroupSubnetOutputTypeDef],
         "DbSubnetGroupArn": str,
     },
+    total=False,
 )
 
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
@@ -13724,14 +14370,15 @@
         "RestoreStatus": AwsRedshiftClusterRestoreStatusOutputTypeDef,
         "SnapshotScheduleIdentifier": str,
         "SnapshotScheduleState": str,
         "VpcId": str,
         "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupOutputTypeDef],
         "LoggingStatus": AwsRedshiftClusterLoggingStatusOutputTypeDef,
     },
+    total=False,
 )
 
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
@@ -13787,14 +14434,15 @@
         "Operands": List[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef
         ],
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     {
         "Operands": Sequence[
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
@@ -13807,14 +14455,15 @@
 )
 
 AwsS3BucketNotificationConfigurationFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
@@ -13823,14 +14472,15 @@
 
 AwsS3BucketObjectLockConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationOutputTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
@@ -13839,14 +14489,15 @@
 )
 
 AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
         "Rules": List[AwsS3BucketServerSideEncryptionRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
         "Rules": Sequence[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
@@ -13857,14 +14508,15 @@
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
         "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
         "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
@@ -13884,14 +14536,15 @@
 )
 
 AwsSsmPatchComplianceDetailsOutputTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsOutputTypeDef",
     {
         "Patch": AwsSsmPatchOutputTypeDef,
     },
+    total=False,
 )
 
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
@@ -13903,14 +14556,15 @@
     {
         "Destinations": List[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     {
         "Destinations": Sequence[
             AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
@@ -13925,14 +14579,15 @@
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": List[AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -13947,14 +14602,15 @@
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
         "RulesList": List[AwsWafRegionalWebAclRulesListDetailsOutputTypeDef],
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
@@ -13969,14 +14625,15 @@
     "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
         "Rules": List[AwsWafRuleGroupRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
         "MetricName": str,
         "Name": str,
@@ -13990,14 +14647,15 @@
     "AwsWafWebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
         "Rules": List[AwsWafWebAclRuleOutputTypeDef],
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsWafWebAclDetailsTypeDef = TypedDict(
     "AwsWafWebAclDetailsTypeDef",
     {
         "Name": str,
         "DefaultAction": str,
@@ -14008,35 +14666,39 @@
 )
 
 AwsWafv2ActionAllowDetailsOutputTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionCaptchaDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionCountDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsOutputTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
@@ -14102,14 +14764,15 @@
         "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
         "RelatedFindingsId": List[StringFilterOutputTypeDef],
         "NoteText": List[StringFilterOutputTypeDef],
         "NoteUpdatedAt": List[DateFilterOutputTypeDef],
         "NoteUpdatedBy": List[StringFilterOutputTypeDef],
         "UserDefinedFields": List[MapFilterOutputTypeDef],
     },
+    total=False,
 )
 
 AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
     "AwsSecurityFindingFiltersOutputTypeDef",
     {
         "ProductArn": List[StringFilterOutputTypeDef],
         "AwsAccountId": List[StringFilterOutputTypeDef],
@@ -14205,14 +14868,15 @@
         "FindingProviderFieldsSeverityLabel": List[StringFilterOutputTypeDef],
         "FindingProviderFieldsSeverityOriginal": List[StringFilterOutputTypeDef],
         "FindingProviderFieldsTypes": List[StringFilterOutputTypeDef],
         "Sample": List[BooleanFilterOutputTypeDef],
         "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
         "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
     },
+    total=False,
 )
 
 AutomationRulesFindingFiltersTypeDef = TypedDict(
     "AutomationRulesFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
@@ -14377,14 +15041,15 @@
 NetworkHeaderOutputTypeDef = TypedDict(
     "NetworkHeaderOutputTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsOutputTypeDef,
         "Source": NetworkPathComponentDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkHeaderTypeDef = TypedDict(
     "NetworkHeaderTypeDef",
     {
         "Protocol": str,
         "Destination": NetworkPathComponentDetailsTypeDef,
@@ -14398,14 +15063,15 @@
     {
         "LineRanges": List[RangeOutputTypeDef],
         "OffsetRanges": List[RangeOutputTypeDef],
         "Pages": List[PageOutputTypeDef],
         "Records": List[RecordOutputTypeDef],
         "Cells": List[CellOutputTypeDef],
     },
+    total=False,
 )
 
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
         "LineRanges": Sequence[RangeTypeDef],
         "OffsetRanges": Sequence[RangeTypeDef],
@@ -14418,14 +15084,15 @@
 
 RuleGroupSourceStatelessRuleDefinitionOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     {
         "Actions": List[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRuleDefinitionTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     {
         "Actions": Sequence[str],
         "MatchAttributes": RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
@@ -14485,14 +15152,15 @@
 )
 
 StatelessCustomActionDefinitionOutputTypeDef = TypedDict(
     "StatelessCustomActionDefinitionOutputTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionOutputTypeDef,
     },
+    total=False,
 )
 
 StatelessCustomActionDefinitionTypeDef = TypedDict(
     "StatelessCustomActionDefinitionTypeDef",
     {
         "PublishMetricAction": StatelessCustomPublishMetricActionTypeDef,
     },
@@ -14501,14 +15169,15 @@
 
 PortProbeActionOutputTypeDef = TypedDict(
     "PortProbeActionOutputTypeDef",
     {
         "PortProbeDetails": List[PortProbeDetailOutputTypeDef],
         "Blocked": bool,
     },
+    total=False,
 )
 
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
@@ -14520,14 +15189,15 @@
     "AwsAthenaWorkGroupDetailsOutputTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
@@ -14552,14 +15222,15 @@
             AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef
         ],
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef
         ),
         "CapacityRebalance": bool,
     },
+    total=False,
 )
 
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     {
         "LaunchConfigurationName": str,
         "LoadBalancerNames": Sequence[str],
@@ -14583,14 +15254,15 @@
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": List[
             AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef
         ],
         "BackupPlanRule": List[AwsBackupBackupPlanRuleDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsBackupBackupPlanBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     {
         "BackupPlanName": str,
         "AdvancedBackupSettings": Sequence[AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef],
@@ -14624,14 +15296,15 @@
         "Serial": str,
         "SignatureAlgorithm": str,
         "Status": str,
         "Subject": str,
         "SubjectAlternativeNames": List[str],
         "Type": str,
     },
+    total=False,
 )
 
 AwsCertificateManagerCertificateDetailsTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDetailsTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
@@ -14663,14 +15336,15 @@
 )
 
 AwsCloudFrontDistributionOriginsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionOriginItemOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginItemTypeDef],
     },
@@ -14678,14 +15352,15 @@
 )
 
 AwsCloudFrontDistributionOriginGroupsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsOutputTypeDef",
     {
         "Items": List[AwsCloudFrontDistributionOriginGroupOutputTypeDef],
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionOriginGroupsTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginGroupsTypeDef",
     {
         "Items": Sequence[AwsCloudFrontDistributionOriginGroupTypeDef],
     },
@@ -14711,14 +15386,15 @@
         "SseDescription": AwsDynamoDbTableSseDescriptionOutputTypeDef,
         "StreamSpecification": AwsDynamoDbTableStreamSpecificationOutputTypeDef,
         "TableId": str,
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
+    total=False,
 )
 
 AwsDynamoDbTableDetailsTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsTypeDef",
     {
         "AttributeDefinitions": Sequence[AwsDynamoDbTableAttributeDefinitionTypeDef],
         "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
@@ -14748,14 +15424,15 @@
     {
         "LaunchTemplateName": str,
         "Id": str,
         "LaunchTemplateData": AwsEc2LaunchTemplateDataDetailsOutputTypeDef,
         "DefaultVersionNumber": int,
         "LatestVersionNumber": int,
     },
+    total=False,
 )
 
 AwsEc2LaunchTemplateDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDetailsTypeDef",
     {
         "LaunchTemplateName": str,
         "Id": str,
@@ -14778,14 +15455,15 @@
             AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef
         ],
         "ClusterName": str,
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
+    total=False,
 )
 
 AwsEcsClusterDetailsTypeDef = TypedDict(
     "AwsEcsClusterDetailsTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
@@ -14819,14 +15497,15 @@
         "PidMode": str,
         "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef],
         "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
         "RequiresCompatibilities": List[str],
         "TaskRoleArn": str,
         "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsEcsTaskDefinitionDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsTypeDef",
     {
         "ContainerDefinitions": Sequence[AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef],
         "Cpu": str,
@@ -14852,14 +15531,15 @@
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
         "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
         "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
         "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     {
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
@@ -14928,14 +15608,15 @@
         "PerformanceInsightsKmsKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudWatchLogsExports": List[str],
         "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
         "ListenerEndpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
         "MaxAllocatedStorage": int,
     },
+    total=False,
 )
 
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
     {
         "AssociatedRoles": Sequence[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
@@ -15001,14 +15682,15 @@
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     {
         "Predicate": (
             AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     {
         "Predicate": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     },
@@ -15019,14 +15701,15 @@
     "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     {
         "Events": List[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
         "Destination": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationDetailTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     {
         "Events": Sequence[str],
         "Filter": AwsS3BucketNotificationConfigurationFilterTypeDef,
@@ -15044,14 +15727,15 @@
         "Name": str,
         "RoleArn": str,
         "StateMachineArn": str,
         "Status": str,
         "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
         "Type": str,
     },
+    total=False,
 )
 
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
@@ -15069,22 +15753,24 @@
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
         "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
         "Captcha": AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
         "Count": AwsWafv2RulesActionCountDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclActionDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsOutputTypeDef,
         "Block": AwsWafv2ActionBlockDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesActionDetailsTypeDef = TypedDict(
     "AwsWafv2RulesActionDetailsTypeDef",
     {
         "Allow": AwsWafv2ActionAllowDetailsTypeDef,
         "Block": AwsWafv2ActionBlockDetailsTypeDef,
@@ -15114,14 +15800,15 @@
         "IsTerminal": bool,
         "Criteria": AutomationRulesFindingFiltersOutputTypeDef,
         "Actions": List[AutomationRulesActionOutputTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
+    total=False,
 )
 
 InsightTypeDef = TypedDict(
     "InsightTypeDef",
     {
         "InsightArn": str,
         "Name": str,
@@ -15257,14 +15944,15 @@
     "NetworkPathComponentOutputTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
         "Egress": NetworkHeaderOutputTypeDef,
         "Ingress": NetworkHeaderOutputTypeDef,
     },
+    total=False,
 )
 
 NetworkPathComponentTypeDef = TypedDict(
     "NetworkPathComponentTypeDef",
     {
         "ComponentId": str,
         "ComponentType": str,
@@ -15278,23 +15966,25 @@
     "CustomDataIdentifiersDetectionsOutputTypeDef",
     {
         "Count": int,
         "Arn": str,
         "Name": str,
         "Occurrences": OccurrencesOutputTypeDef,
     },
+    total=False,
 )
 
 SensitiveDataDetectionsOutputTypeDef = TypedDict(
     "SensitiveDataDetectionsOutputTypeDef",
     {
         "Count": int,
         "Type": str,
         "Occurrences": OccurrencesOutputTypeDef,
     },
+    total=False,
 )
 
 CustomDataIdentifiersDetectionsTypeDef = TypedDict(
     "CustomDataIdentifiersDetectionsTypeDef",
     {
         "Count": int,
         "Arn": str,
@@ -15316,14 +16006,15 @@
 
 RuleGroupSourceStatelessRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsOutputTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesDetailsTypeDef",
     {
         "Priority": int,
         "RuleDefinition": RuleGroupSourceStatelessRuleDefinitionTypeDef,
@@ -15333,22 +16024,24 @@
 
 FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
         "ActionName": str,
     },
+    total=False,
 )
 
 RuleGroupSourceCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceCustomActionsDetailsOutputTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionOutputTypeDef,
         "ActionName": str,
     },
+    total=False,
 )
 
 FirewallPolicyStatelessCustomActionsDetailsTypeDef = TypedDict(
     "FirewallPolicyStatelessCustomActionsDetailsTypeDef",
     {
         "ActionDefinition": StatelessCustomActionDefinitionTypeDef,
         "ActionName": str,
@@ -15370,14 +16063,15 @@
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionOutputTypeDef,
         "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
         "DnsRequestAction": DnsRequestActionOutputTypeDef,
         "PortProbeAction": PortProbeActionOutputTypeDef,
     },
+    total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionType": str,
         "NetworkConnectionAction": NetworkConnectionActionTypeDef,
@@ -15392,14 +16086,15 @@
     "AwsBackupBackupPlanDetailsOutputTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "VersionId": str,
     },
+    total=False,
 )
 
 AwsBackupBackupPlanDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanDetailsTypeDef",
     {
         "BackupPlan": AwsBackupBackupPlanBackupPlanDetailsTypeDef,
         "BackupPlanArn": str,
@@ -15421,14 +16116,15 @@
         "Logging": AwsCloudFrontDistributionLoggingOutputTypeDef,
         "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
         "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
         "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
         "Status": str,
         "WebAclId": str,
     },
+    total=False,
 )
 
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsTypeDef,
         "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
@@ -15451,14 +16147,15 @@
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
         "Features": List[AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
+    total=False,
 )
 
 AwsGuardDutyDetectorDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsTypeDef",
     {
         "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
         "Features": Sequence[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
@@ -15484,14 +16181,15 @@
         ],
         "Prefix": str,
         "Status": str,
         "Transitions": List[
             AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
         "AbortIncompleteMultipartUpload": (
             AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
@@ -15515,14 +16213,15 @@
 )
 
 AwsS3BucketNotificationConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationOutputTypeDef",
     {
         "Configurations": List[AwsS3BucketNotificationConfigurationDetailOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketNotificationConfigurationTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationTypeDef",
     {
         "Configurations": Sequence[AwsS3BucketNotificationConfigurationDetailTypeDef],
     },
@@ -15534,14 +16233,15 @@
     {
         "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsTypeDef,
         "Name": str,
@@ -15579,23 +16279,25 @@
 
 CustomDataIdentifiersResultOutputTypeDef = TypedDict(
     "CustomDataIdentifiersResultOutputTypeDef",
     {
         "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
         "TotalCount": int,
     },
+    total=False,
 )
 
 SensitiveDataResultOutputTypeDef = TypedDict(
     "SensitiveDataResultOutputTypeDef",
     {
         "Category": str,
         "Detections": List[SensitiveDataDetectionsOutputTypeDef],
         "TotalCount": int,
     },
+    total=False,
 )
 
 CustomDataIdentifiersResultTypeDef = TypedDict(
     "CustomDataIdentifiersResultTypeDef",
     {
         "Detections": Sequence[CustomDataIdentifiersDetectionsTypeDef],
         "TotalCount": int,
@@ -15622,22 +16324,24 @@
         "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
         "StatelessRuleGroupReferences": List[
             FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef
         ],
     },
+    total=False,
 )
 
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     {
         "CustomActions": List[RuleGroupSourceCustomActionsDetailsOutputTypeDef],
         "StatelessRules": List[RuleGroupSourceStatelessRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 FirewallPolicyDetailsTypeDef = TypedDict(
     "FirewallPolicyDetailsTypeDef",
     {
         "StatefulRuleGroupReferences": Sequence[
             FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
@@ -15662,14 +16366,15 @@
 )
 
 AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef",
     {
         "Rules": List[AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef],
     },
+    total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationDetailsTypeDef",
     {
         "Rules": Sequence[AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef],
     },
@@ -15684,14 +16389,15 @@
         "Id": str,
         "Name": str,
         "Arn": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "Scope": str,
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "Arn": str,
@@ -15700,14 +16406,15 @@
         "Capacity": int,
         "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
         "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
         "Description": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
@@ -15744,14 +16451,15 @@
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
         "Status": ClassificationStatusOutputTypeDef,
         "SensitiveData": List[SensitiveDataResultOutputTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
     },
+    total=False,
 )
 
 ClassificationResultTypeDef = TypedDict(
     "ClassificationResultTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
@@ -15768,26 +16476,28 @@
     {
         "FirewallPolicy": FirewallPolicyDetailsOutputTypeDef,
         "FirewallPolicyArn": str,
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
         "Description": str,
     },
+    total=False,
 )
 
 RuleGroupSourceOutputTypeDef = TypedDict(
     "RuleGroupSourceOutputTypeDef",
     {
         "RulesSourceList": RuleGroupSourceListDetailsOutputTypeDef,
         "RulesString": str,
         "StatefulRules": List[RuleGroupSourceStatefulRulesDetailsOutputTypeDef],
         "StatelessRulesAndCustomActions": (
             RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef
         ),
     },
+    total=False,
 )
 
 AwsNetworkFirewallFirewallPolicyDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallPolicyDetailsTypeDef",
     {
         "FirewallPolicy": FirewallPolicyDetailsTypeDef,
         "FirewallPolicyArn": str,
@@ -15826,14 +16536,15 @@
         "AccessControlList": str,
         "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationOutputTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
         "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
         "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
         "OwnerId": str,
         "OwnerName": str,
@@ -15854,14 +16565,15 @@
 
 DataClassificationDetailsOutputTypeDef = TypedDict(
     "DataClassificationDetailsOutputTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultOutputTypeDef,
     },
+    total=False,
 )
 
 DataClassificationDetailsTypeDef = TypedDict(
     "DataClassificationDetailsTypeDef",
     {
         "DetailedResultsLocation": str,
         "Result": ClassificationResultTypeDef,
@@ -15871,14 +16583,15 @@
 
 RuleGroupDetailsOutputTypeDef = TypedDict(
     "RuleGroupDetailsOutputTypeDef",
     {
         "RuleVariables": RuleGroupVariablesOutputTypeDef,
         "RulesSource": RuleGroupSourceOutputTypeDef,
     },
+    total=False,
 )
 
 RuleGroupDetailsTypeDef = TypedDict(
     "RuleGroupDetailsTypeDef",
     {
         "RuleVariables": RuleGroupVariablesTypeDef,
         "RulesSource": RuleGroupSourceTypeDef,
@@ -15893,14 +16606,15 @@
         "Description": str,
         "RuleGroup": RuleGroupDetailsOutputTypeDef,
         "RuleGroupArn": str,
         "RuleGroupId": str,
         "RuleGroupName": str,
         "Type": str,
     },
+    total=False,
 )
 
 AwsNetworkFirewallRuleGroupDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallRuleGroupDetailsTypeDef",
     {
         "Capacity": int,
         "Description": str,
@@ -16003,14 +16717,15 @@
         "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
         "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
         "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsOutputTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
         "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsOutputTypeDef,
     },
+    total=False,
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "AwsAutoScalingAutoScalingGroup": AwsAutoScalingAutoScalingGroupDetailsTypeDef,
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsTypeDef,
@@ -16102,28 +16817,37 @@
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsTypeDef,
         "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsTypeDef,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+_RequiredResourceOutputTypeDef = TypedDict(
+    "_RequiredResourceOutputTypeDef",
     {
         "Type": str,
         "Id": str,
+    },
+)
+_OptionalResourceOutputTypeDef = TypedDict(
+    "_OptionalResourceOutputTypeDef",
+    {
         "Partition": PartitionType,
         "Region": str,
         "ResourceRole": str,
         "Tags": Dict[str, str],
         "DataClassification": DataClassificationDetailsOutputTypeDef,
         "Details": ResourceDetailsOutputTypeDef,
     },
+    total=False,
 )
 
+class ResourceOutputTypeDef(_RequiredResourceOutputTypeDef, _OptionalResourceOutputTypeDef):
+    pass
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "Type": str,
         "Id": str,
     },
 )
@@ -16139,61 +16863,72 @@
     },
     total=False,
 )
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-AwsSecurityFindingOutputTypeDef = TypedDict(
-    "AwsSecurityFindingOutputTypeDef",
+_RequiredAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_RequiredAwsSecurityFindingOutputTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
+        "GeneratorId": str,
+        "AwsAccountId": str,
+        "CreatedAt": str,
+        "UpdatedAt": str,
+        "Title": str,
+        "Description": str,
+        "Resources": List[ResourceOutputTypeDef],
+    },
+)
+_OptionalAwsSecurityFindingOutputTypeDef = TypedDict(
+    "_OptionalAwsSecurityFindingOutputTypeDef",
+    {
         "ProductName": str,
         "CompanyName": str,
         "Region": str,
-        "GeneratorId": str,
-        "AwsAccountId": str,
         "Types": List[str],
         "FirstObservedAt": str,
         "LastObservedAt": str,
-        "CreatedAt": str,
-        "UpdatedAt": str,
         "Severity": SeverityOutputTypeDef,
         "Confidence": int,
         "Criticality": int,
-        "Title": str,
-        "Description": str,
         "Remediation": RemediationOutputTypeDef,
         "SourceUrl": str,
         "ProductFields": Dict[str, str],
         "UserDefinedFields": Dict[str, str],
         "Malware": List[MalwareOutputTypeDef],
         "Network": NetworkOutputTypeDef,
         "NetworkPath": List[NetworkPathComponentOutputTypeDef],
         "Process": ProcessDetailsOutputTypeDef,
         "Threats": List[ThreatOutputTypeDef],
         "ThreatIntelIndicators": List[ThreatIntelIndicatorOutputTypeDef],
-        "Resources": List[ResourceOutputTypeDef],
         "Compliance": ComplianceOutputTypeDef,
         "VerificationState": VerificationStateType,
         "WorkflowState": WorkflowStateType,
         "Workflow": WorkflowOutputTypeDef,
         "RecordState": RecordStateType,
         "RelatedFindings": List[RelatedFindingOutputTypeDef],
         "Note": NoteOutputTypeDef,
         "Vulnerabilities": List[VulnerabilityOutputTypeDef],
         "PatchSummary": PatchSummaryOutputTypeDef,
         "Action": ActionOutputTypeDef,
         "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
         "Sample": bool,
     },
+    total=False,
 )
 
+class AwsSecurityFindingOutputTypeDef(
+    _RequiredAwsSecurityFindingOutputTypeDef, _OptionalAwsSecurityFindingOutputTypeDef
+):
+    pass
+
 _RequiredAwsSecurityFindingTypeDef = TypedDict(
     "_RequiredAwsSecurityFindingTypeDef",
     {
         "SchemaVersion": str,
         "Id": str,
         "ProductArn": str,
         "GeneratorId": str,
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.11
-Summary: Type annotations for boto3.SecurityHub 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securityhub?color=blue)](https://pypistats.org/packages/mypy-boto3-securityhub)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-securityhub-1.28.11/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.11/setup.py` & `mypy-boto3-securityhub-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.28.11 service generated with mypy-boto3-builder"
-        " 7.15.1"
+        "Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

