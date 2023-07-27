# Comparing `tmp/mypy-boto3-synthetics-1.28.0.tar.gz` & `tmp/mypy-boto3-synthetics-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-synthetics-1.28.0.tar", last modified: Thu Jul  6 21:00:46 2023, max compression
+gzip compressed data, was "mypy-boto3-synthetics-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
```

## Comparing `mypy-boto3-synthetics-1.28.0.tar` & `mypy-boto3-synthetics-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.490449 mypy-boto3-synthetics-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-06 21:00:46.490449 mypy-boto3-synthetics-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.490449 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18358 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18335 2023-07-06 20:57:05.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:46.490449 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 21:00:46.000000 mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:46.490449 mypy-boto3-synthetics-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:57:04.000000 mypy-boto3-synthetics-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.377431 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14159 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:46.000000 mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.381431 mypy-boto3-synthetics-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:47:55.000000 mypy-boto3-synthetics-1.28.12/setup.py
```

### Comparing `mypy-boto3-synthetics-1.28.0/LICENSE` & `mypy-boto3-synthetics-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.0/PKG-INFO` & `mypy-boto3-synthetics-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-synthetics
-Version: 1.28.0
-Summary: Type annotations for boto3.Synthetics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-synthetics"></a>
 
 # mypy-boto3-synthetics
 
 [![PyPI - mypy-boto3-synthetics](https://img.shields.io/pypi/v/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-synthetics?color=blue)](https://pypistats.org/packages/mypy-boto3-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,28 +301,31 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
+    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -330,36 +333,35 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateCanaryRequestRequestTypeDef,
-    UpdateCanaryRequestRequestTypeDef,
     CanaryTypeDef,
+    UpdateCanaryRequestRequestTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-synthetics-1.28.0/README.md` & `mypy-boto3-synthetics-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-synthetics"></a>
 
 # mypy-boto3-synthetics
 
 [![PyPI - mypy-boto3-synthetics](https://img.shields.io/pypi/v/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-synthetics?color=blue)](https://pypistats.org/packages/mypy-boto3-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,28 +269,31 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
+    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -298,36 +301,35 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateCanaryRequestRequestTypeDef,
-    UpdateCanaryRequestRequestTypeDef,
     CanaryTypeDef,
+    UpdateCanaryRequestRequestTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/__main__.py` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Synthetics 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Synthetics 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics\nOther"
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

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/client.py` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/client.pyi` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/literals.py` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
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
@@ -262,26 +263,28 @@
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

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/literals.pyi` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
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
@@ -260,26 +261,28 @@
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

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/type_defs.py` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
+    "S3EncryptionConfigOutputTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
     "CanaryScheduleInputTypeDef",
     "CanaryScheduleOutputTypeDef",
     "CanaryStatusTypeDef",
     "CanaryTimelineTypeDef",
     "VpcConfigOutputTypeDef",
     "VpcConfigInputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "DeleteCanaryRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DescribeCanariesLastRunRequestRequestTypeDef",
     "DescribeCanariesRequestRequestTypeDef",
     "DescribeRuntimeVersionsRequestRequestTypeDef",
@@ -58,36 +61,35 @@
     "DisassociateResourceRequestRequestTypeDef",
     "GetCanaryRequestRequestTypeDef",
     "GetCanaryRunsRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GroupSummaryTypeDef",
     "ListAssociatedGroupsRequestRequestTypeDef",
     "ListGroupResourcesRequestRequestTypeDef",
-    "ListGroupResourcesResponseTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceInputTypeDef",
     "VisualReferenceOutputTypeDef",
+    "VisualReferenceInputTypeDef",
     "CanaryRunTypeDef",
+    "ListGroupResourcesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
     "ListAssociatedGroupsResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "CreateCanaryRequestRequestTypeDef",
-    "UpdateCanaryRequestRequestTypeDef",
     "CanaryTypeDef",
+    "UpdateCanaryRequestRequestTypeDef",
     "CanaryLastRunTypeDef",
     "GetCanaryRunsResponseTypeDef",
     "CreateCanaryResponseTypeDef",
     "DescribeCanariesResponseTypeDef",
     "GetCanaryResponseTypeDef",
     "DescribeCanariesLastRunResponseTypeDef",
 )
@@ -97,32 +99,62 @@
     {
         "EncryptionMode": EncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+S3EncryptionConfigOutputTypeDef = TypedDict(
+    "S3EncryptionConfigOutputTypeDef",
+    {
+        "EncryptionMode": EncryptionModeType,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
+_RequiredBaseScreenshotOutputTypeDef = TypedDict(
+    "_RequiredBaseScreenshotOutputTypeDef",
+    {
+        "ScreenshotName": str,
+    },
+)
+_OptionalBaseScreenshotOutputTypeDef = TypedDict(
+    "_OptionalBaseScreenshotOutputTypeDef",
+    {
+        "IgnoreCoordinates": List[str],
+    },
+    total=False,
+)
+
+
+class BaseScreenshotOutputTypeDef(
+    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
+):
+    pass
+
+
 _RequiredBaseScreenshotTypeDef = TypedDict(
     "_RequiredBaseScreenshotTypeDef",
     {
         "ScreenshotName": str,
     },
 )
 _OptionalBaseScreenshotTypeDef = TypedDict(
     "_OptionalBaseScreenshotTypeDef",
     {
-        "IgnoreCoordinates": List[str],
+        "IgnoreCoordinates": Sequence[str],
     },
     total=False,
 )
 
 
 class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
@@ -265,14 +297,25 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
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
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupRequestRequestTypeDef = TypedDict(
@@ -467,23 +510,14 @@
 class ListGroupResourcesRequestRequestTypeDef(
     _RequiredListGroupResourcesRequestRequestTypeDef,
     _OptionalListGroupResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-ListGroupResourcesResponseTypeDef = TypedDict(
-    "ListGroupResourcesResponseTypeDef",
-    {
-        "Resources": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -492,33 +526,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 StartCanaryRequestRequestTypeDef = TypedDict(
     "StartCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -552,15 +567,24 @@
     },
     total=False,
 )
 
 ArtifactConfigOutputTypeDef = TypedDict(
     "ArtifactConfigOutputTypeDef",
     {
-        "S3Encryption": S3EncryptionConfigTypeDef,
+        "S3Encryption": S3EncryptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
+        "BaseCanaryRunId": str,
     },
     total=False,
 )
 
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
@@ -578,75 +602,83 @@
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
-    {
-        "BaseScreenshots": List[BaseScreenshotTypeDef],
-        "BaseCanaryRunId": str,
-    },
-    total=False,
-)
-
 CanaryRunTypeDef = TypedDict(
     "CanaryRunTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": CanaryRunStatusTypeDef,
         "Timeline": CanaryRunTimelineTypeDef,
         "ArtifactS3Location": str,
     },
     total=False,
 )
 
+ListGroupResourcesResponseTypeDef = TypedDict(
+    "ListGroupResourcesResponseTypeDef",
+    {
+        "Resources": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRuntimeVersionsResponseTypeDef = TypedDict(
     "DescribeRuntimeVersionsResponseTypeDef",
     {
         "RuntimeVersions": List[RuntimeVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedGroupsResponseTypeDef = TypedDict(
     "ListAssociatedGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCanaryRequestRequestTypeDef",
     {
         "Name": str,
@@ -673,14 +705,38 @@
 
 class CreateCanaryRequestRequestTypeDef(
     _RequiredCreateCanaryRequestRequestTypeDef, _OptionalCreateCanaryRequestRequestTypeDef
 ):
     pass
 
 
+CanaryTypeDef = TypedDict(
+    "CanaryTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Code": CanaryCodeOutputTypeDef,
+        "ExecutionRoleArn": str,
+        "Schedule": CanaryScheduleOutputTypeDef,
+        "RunConfig": CanaryRunConfigOutputTypeDef,
+        "SuccessRetentionPeriodInDays": int,
+        "FailureRetentionPeriodInDays": int,
+        "Status": CanaryStatusTypeDef,
+        "Timeline": CanaryTimelineTypeDef,
+        "ArtifactS3Location": str,
+        "EngineArn": str,
+        "RuntimeVersion": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "VisualReference": VisualReferenceOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ArtifactConfig": ArtifactConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCanaryRequestRequestTypeDef = TypedDict(
@@ -704,82 +760,58 @@
 
 class UpdateCanaryRequestRequestTypeDef(
     _RequiredUpdateCanaryRequestRequestTypeDef, _OptionalUpdateCanaryRequestRequestTypeDef
 ):
     pass
 
 
-CanaryTypeDef = TypedDict(
-    "CanaryTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Code": CanaryCodeOutputTypeDef,
-        "ExecutionRoleArn": str,
-        "Schedule": CanaryScheduleOutputTypeDef,
-        "RunConfig": CanaryRunConfigOutputTypeDef,
-        "SuccessRetentionPeriodInDays": int,
-        "FailureRetentionPeriodInDays": int,
-        "Status": CanaryStatusTypeDef,
-        "Timeline": CanaryTimelineTypeDef,
-        "ArtifactS3Location": str,
-        "EngineArn": str,
-        "RuntimeVersion": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "VisualReference": VisualReferenceOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ArtifactConfig": ArtifactConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 CanaryLastRunTypeDef = TypedDict(
     "CanaryLastRunTypeDef",
     {
         "CanaryName": str,
         "LastRun": CanaryRunTypeDef,
     },
     total=False,
 )
 
 GetCanaryRunsResponseTypeDef = TypedDict(
     "GetCanaryRunsResponseTypeDef",
     {
         "CanaryRuns": List[CanaryRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCanaryResponseTypeDef = TypedDict(
     "CreateCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesResponseTypeDef = TypedDict(
     "DescribeCanariesResponseTypeDef",
     {
         "Canaries": List[CanaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCanaryResponseTypeDef = TypedDict(
     "GetCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesLastRunResponseTypeDef = TypedDict(
     "DescribeCanariesLastRunResponseTypeDef",
     {
         "CanariesLastRun": List[CanaryLastRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics/type_defs.pyi` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "S3EncryptionConfigTypeDef",
+    "S3EncryptionConfigOutputTypeDef",
     "AssociateResourceRequestRequestTypeDef",
+    "BaseScreenshotOutputTypeDef",
     "BaseScreenshotTypeDef",
     "CanaryCodeInputTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
     "CanaryRunConfigOutputTypeDef",
     "CanaryRunStatusTypeDef",
     "CanaryRunTimelineTypeDef",
     "CanaryScheduleInputTypeDef",
     "CanaryScheduleOutputTypeDef",
     "CanaryStatusTypeDef",
     "CanaryTimelineTypeDef",
     "VpcConfigOutputTypeDef",
     "VpcConfigInputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
     "DeleteCanaryRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DescribeCanariesLastRunRequestRequestTypeDef",
     "DescribeCanariesRequestRequestTypeDef",
     "DescribeRuntimeVersionsRequestRequestTypeDef",
@@ -57,36 +60,35 @@
     "DisassociateResourceRequestRequestTypeDef",
     "GetCanaryRequestRequestTypeDef",
     "GetCanaryRunsRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GroupSummaryTypeDef",
     "ListAssociatedGroupsRequestRequestTypeDef",
     "ListGroupResourcesRequestRequestTypeDef",
-    "ListGroupResourcesResponseTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartCanaryRequestRequestTypeDef",
     "StopCanaryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ArtifactConfigInputTypeDef",
     "ArtifactConfigOutputTypeDef",
-    "VisualReferenceInputTypeDef",
     "VisualReferenceOutputTypeDef",
+    "VisualReferenceInputTypeDef",
     "CanaryRunTypeDef",
+    "ListGroupResourcesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "DescribeRuntimeVersionsResponseTypeDef",
     "ListAssociatedGroupsResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "CreateCanaryRequestRequestTypeDef",
-    "UpdateCanaryRequestRequestTypeDef",
     "CanaryTypeDef",
+    "UpdateCanaryRequestRequestTypeDef",
     "CanaryLastRunTypeDef",
     "GetCanaryRunsResponseTypeDef",
     "CreateCanaryResponseTypeDef",
     "DescribeCanariesResponseTypeDef",
     "GetCanaryResponseTypeDef",
     "DescribeCanariesLastRunResponseTypeDef",
 )
@@ -96,32 +98,60 @@
     {
         "EncryptionMode": EncryptionModeType,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+S3EncryptionConfigOutputTypeDef = TypedDict(
+    "S3EncryptionConfigOutputTypeDef",
+    {
+        "EncryptionMode": EncryptionModeType,
+        "KmsKeyArn": str,
+    },
+    total=False,
+)
+
 AssociateResourceRequestRequestTypeDef = TypedDict(
     "AssociateResourceRequestRequestTypeDef",
     {
         "GroupIdentifier": str,
         "ResourceArn": str,
     },
 )
 
+_RequiredBaseScreenshotOutputTypeDef = TypedDict(
+    "_RequiredBaseScreenshotOutputTypeDef",
+    {
+        "ScreenshotName": str,
+    },
+)
+_OptionalBaseScreenshotOutputTypeDef = TypedDict(
+    "_OptionalBaseScreenshotOutputTypeDef",
+    {
+        "IgnoreCoordinates": List[str],
+    },
+    total=False,
+)
+
+class BaseScreenshotOutputTypeDef(
+    _RequiredBaseScreenshotOutputTypeDef, _OptionalBaseScreenshotOutputTypeDef
+):
+    pass
+
 _RequiredBaseScreenshotTypeDef = TypedDict(
     "_RequiredBaseScreenshotTypeDef",
     {
         "ScreenshotName": str,
     },
 )
 _OptionalBaseScreenshotTypeDef = TypedDict(
     "_OptionalBaseScreenshotTypeDef",
     {
-        "IgnoreCoordinates": List[str],
+        "IgnoreCoordinates": Sequence[str],
     },
     total=False,
 )
 
 class BaseScreenshotTypeDef(_RequiredBaseScreenshotTypeDef, _OptionalBaseScreenshotTypeDef):
     pass
 
@@ -258,14 +288,25 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
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
 _RequiredCreateGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateGroupRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateGroupRequestRequestTypeDef = TypedDict(
@@ -450,23 +491,14 @@
 
 class ListGroupResourcesRequestRequestTypeDef(
     _RequiredListGroupResourcesRequestRequestTypeDef,
     _OptionalListGroupResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListGroupResourcesResponseTypeDef = TypedDict(
-    "ListGroupResourcesResponseTypeDef",
-    {
-        "Resources": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListGroupsRequestRequestTypeDef = TypedDict(
     "ListGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -475,33 +507,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 StartCanaryRequestRequestTypeDef = TypedDict(
     "StartCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -535,15 +548,24 @@
     },
     total=False,
 )
 
 ArtifactConfigOutputTypeDef = TypedDict(
     "ArtifactConfigOutputTypeDef",
     {
-        "S3Encryption": S3EncryptionConfigTypeDef,
+        "S3Encryption": S3EncryptionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+VisualReferenceOutputTypeDef = TypedDict(
+    "VisualReferenceOutputTypeDef",
+    {
+        "BaseScreenshots": List[BaseScreenshotOutputTypeDef],
+        "BaseCanaryRunId": str,
     },
     total=False,
 )
 
 _RequiredVisualReferenceInputTypeDef = TypedDict(
     "_RequiredVisualReferenceInputTypeDef",
     {
@@ -559,75 +581,83 @@
 )
 
 class VisualReferenceInputTypeDef(
     _RequiredVisualReferenceInputTypeDef, _OptionalVisualReferenceInputTypeDef
 ):
     pass
 
-VisualReferenceOutputTypeDef = TypedDict(
-    "VisualReferenceOutputTypeDef",
-    {
-        "BaseScreenshots": List[BaseScreenshotTypeDef],
-        "BaseCanaryRunId": str,
-    },
-    total=False,
-)
-
 CanaryRunTypeDef = TypedDict(
     "CanaryRunTypeDef",
     {
         "Id": str,
         "Name": str,
         "Status": CanaryRunStatusTypeDef,
         "Timeline": CanaryRunTimelineTypeDef,
         "ArtifactS3Location": str,
     },
     total=False,
 )
 
+ListGroupResourcesResponseTypeDef = TypedDict(
+    "ListGroupResourcesResponseTypeDef",
+    {
+        "Resources": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRuntimeVersionsResponseTypeDef = TypedDict(
     "DescribeRuntimeVersionsResponseTypeDef",
     {
         "RuntimeVersions": List[RuntimeVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssociatedGroupsResponseTypeDef = TypedDict(
     "ListAssociatedGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCanaryRequestRequestTypeDef",
     {
         "Name": str,
@@ -652,14 +682,38 @@
 )
 
 class CreateCanaryRequestRequestTypeDef(
     _RequiredCreateCanaryRequestRequestTypeDef, _OptionalCreateCanaryRequestRequestTypeDef
 ):
     pass
 
+CanaryTypeDef = TypedDict(
+    "CanaryTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "Code": CanaryCodeOutputTypeDef,
+        "ExecutionRoleArn": str,
+        "Schedule": CanaryScheduleOutputTypeDef,
+        "RunConfig": CanaryRunConfigOutputTypeDef,
+        "SuccessRetentionPeriodInDays": int,
+        "FailureRetentionPeriodInDays": int,
+        "Status": CanaryStatusTypeDef,
+        "Timeline": CanaryTimelineTypeDef,
+        "ArtifactS3Location": str,
+        "EngineArn": str,
+        "RuntimeVersion": str,
+        "VpcConfig": VpcConfigOutputTypeDef,
+        "VisualReference": VisualReferenceOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ArtifactConfig": ArtifactConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateCanaryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCanaryRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateCanaryRequestRequestTypeDef = TypedDict(
@@ -681,82 +735,58 @@
 )
 
 class UpdateCanaryRequestRequestTypeDef(
     _RequiredUpdateCanaryRequestRequestTypeDef, _OptionalUpdateCanaryRequestRequestTypeDef
 ):
     pass
 
-CanaryTypeDef = TypedDict(
-    "CanaryTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "Code": CanaryCodeOutputTypeDef,
-        "ExecutionRoleArn": str,
-        "Schedule": CanaryScheduleOutputTypeDef,
-        "RunConfig": CanaryRunConfigOutputTypeDef,
-        "SuccessRetentionPeriodInDays": int,
-        "FailureRetentionPeriodInDays": int,
-        "Status": CanaryStatusTypeDef,
-        "Timeline": CanaryTimelineTypeDef,
-        "ArtifactS3Location": str,
-        "EngineArn": str,
-        "RuntimeVersion": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "VisualReference": VisualReferenceOutputTypeDef,
-        "Tags": Dict[str, str],
-        "ArtifactConfig": ArtifactConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 CanaryLastRunTypeDef = TypedDict(
     "CanaryLastRunTypeDef",
     {
         "CanaryName": str,
         "LastRun": CanaryRunTypeDef,
     },
     total=False,
 )
 
 GetCanaryRunsResponseTypeDef = TypedDict(
     "GetCanaryRunsResponseTypeDef",
     {
         "CanaryRuns": List[CanaryRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCanaryResponseTypeDef = TypedDict(
     "CreateCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesResponseTypeDef = TypedDict(
     "DescribeCanariesResponseTypeDef",
     {
         "Canaries": List[CanaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCanaryResponseTypeDef = TypedDict(
     "GetCanaryResponseTypeDef",
     {
         "Canary": CanaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCanariesLastRunResponseTypeDef = TypedDict(
     "DescribeCanariesLastRunResponseTypeDef",
     {
         "CanariesLastRun": List[CanaryLastRunTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/PKG-INFO` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-synthetics
-Version: 1.28.0
-Summary: Type annotations for boto3.Synthetics 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-synthetics"></a>
 
 # mypy-boto3-synthetics
 
 [![PyPI - mypy-boto3-synthetics](https://img.shields.io/pypi/v/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-synthetics.svg?color=blue)](https://pypi.org/project/mypy-boto3-synthetics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-synthetics?color=blue)](https://pypistats.org/packages/mypy-boto3-synthetics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-synthetics)](https://pepy.tech/project/mypy-boto3-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Synthetics 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[boto3.Synthetics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [mypy-boto3-synthetics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_synthetics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,28 +301,31 @@
 
 `mypy_boto3_synthetics.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_synthetics.type_defs import (
     S3EncryptionConfigTypeDef,
+    S3EncryptionConfigOutputTypeDef,
     AssociateResourceRequestRequestTypeDef,
+    BaseScreenshotOutputTypeDef,
     BaseScreenshotTypeDef,
     CanaryCodeInputTypeDef,
     CanaryCodeOutputTypeDef,
     CanaryRunConfigInputTypeDef,
     CanaryRunConfigOutputTypeDef,
     CanaryRunStatusTypeDef,
     CanaryRunTimelineTypeDef,
     CanaryScheduleInputTypeDef,
     CanaryScheduleOutputTypeDef,
     CanaryStatusTypeDef,
     CanaryTimelineTypeDef,
     VpcConfigOutputTypeDef,
     VpcConfigInputTypeDef,
+    ResponseMetadataTypeDef,
     CreateGroupRequestRequestTypeDef,
     GroupTypeDef,
     DeleteCanaryRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DescribeCanariesLastRunRequestRequestTypeDef,
     DescribeCanariesRequestRequestTypeDef,
     DescribeRuntimeVersionsRequestRequestTypeDef,
@@ -330,36 +333,35 @@
     DisassociateResourceRequestRequestTypeDef,
     GetCanaryRequestRequestTypeDef,
     GetCanaryRunsRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GroupSummaryTypeDef,
     ListAssociatedGroupsRequestRequestTypeDef,
     ListGroupResourcesRequestRequestTypeDef,
-    ListGroupResourcesResponseTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartCanaryRequestRequestTypeDef,
     StopCanaryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ArtifactConfigInputTypeDef,
     ArtifactConfigOutputTypeDef,
-    VisualReferenceInputTypeDef,
     VisualReferenceOutputTypeDef,
+    VisualReferenceInputTypeDef,
     CanaryRunTypeDef,
+    ListGroupResourcesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     DescribeRuntimeVersionsResponseTypeDef,
     ListAssociatedGroupsResponseTypeDef,
     ListGroupsResponseTypeDef,
     CreateCanaryRequestRequestTypeDef,
-    UpdateCanaryRequestRequestTypeDef,
     CanaryTypeDef,
+    UpdateCanaryRequestRequestTypeDef,
     CanaryLastRunTypeDef,
     GetCanaryRunsResponseTypeDef,
     CreateCanaryResponseTypeDef,
     DescribeCanariesResponseTypeDef,
     GetCanaryResponseTypeDef,
     DescribeCanariesLastRunResponseTypeDef,
 )
```

### Comparing `mypy-boto3-synthetics-1.28.0/mypy_boto3_synthetics.egg-info/SOURCES.txt` & `mypy-boto3-synthetics-1.28.12/mypy_boto3_synthetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-synthetics-1.28.0/setup.py` & `mypy-boto3-synthetics-1.28.12/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-synthetics",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_synthetics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Synthetics 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.Synthetics 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

