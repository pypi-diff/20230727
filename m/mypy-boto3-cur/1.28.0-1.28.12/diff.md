# Comparing `tmp/mypy-boto3-cur-1.28.0.tar.gz` & `tmp/mypy-boto3-cur-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.28.0.tar", last modified: Thu Jul  6 20:59:21 2023, max compression
+gzip compressed data, was "mypy-boto3-cur-1.28.12.tar", last modified: Thu Jul 27 05:34:32 2023, max compression
```

## Comparing `mypy-boto3-cur-1.28.0.tar` & `mypy-boto3-cur-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.054270 mypy-boto3-cur-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-06 20:59:21.046270 mypy-boto3-cur-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.046270 mypy-boto3-cur-1.28.0/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-07-06 20:37:15.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-06 20:37:15.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-06 20:37:15.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-06 20:37:15.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:21.046270 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 20:59:20.000000 mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:21.054270 mypy-boto3-cur-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 20:37:14.000000 mypy-boto3-cur-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.492540 mypy-boto3-cur-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:32.492540 mypy-boto3-cur-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/setup.py
```

### Comparing `mypy-boto3-cur-1.28.0/LICENSE` & `mypy-boto3-cur-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/PKG-INFO` & `mypy-boto3-cur-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.0
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,14 +331,15 @@
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-cur-1.28.0/README.md` & `mypy-boto3-cur-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,14 +299,15 @@
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostandUsageReportService 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CostandUsageReportService 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -31,15 +30,14 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -189,14 +187,15 @@
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
@@ -275,26 +274,28 @@
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

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.py`

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
     "AWSRegionType",
     "AdditionalArtifactType",
     "CompressionFormatType",
     "DescribeReportDefinitionsPaginatorName",
     "ReportFormatType",
     "ReportVersioningType",
@@ -30,14 +31,15 @@
     "CostandUsageReportServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 AWSRegionType = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
@@ -187,14 +189,15 @@
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
@@ -273,26 +276,28 @@
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

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
     data: DeleteReportDefinitionRequestRequestTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List
+from typing import Dict, List, Sequence
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -31,14 +31,15 @@
 
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
+    "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
@@ -72,31 +73,62 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredReportDefinitionOutputTypeDef = TypedDict(
+    "_RequiredReportDefinitionOutputTypeDef",
+    {
+        "ReportName": str,
+        "TimeUnit": TimeUnitType,
+        "Format": ReportFormatType,
+        "Compression": CompressionFormatType,
+        "AdditionalSchemaElements": List[SchemaElementType],
+        "S3Bucket": str,
+        "S3Prefix": str,
+        "S3Region": AWSRegionType,
+    },
+)
+_OptionalReportDefinitionOutputTypeDef = TypedDict(
+    "_OptionalReportDefinitionOutputTypeDef",
+    {
+        "AdditionalArtifacts": List[AdditionalArtifactType],
+        "RefreshClosedReports": bool,
+        "ReportVersioning": ReportVersioningType,
+        "BillingViewArn": str,
+    },
+    total=False,
+)
+
+
+class ReportDefinitionOutputTypeDef(
+    _RequiredReportDefinitionOutputTypeDef, _OptionalReportDefinitionOutputTypeDef
+):
+    pass
+
+
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[SchemaElementType],
+        "AdditionalSchemaElements": Sequence[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
     {
-        "AdditionalArtifacts": List[AdditionalArtifactType],
+        "AdditionalArtifacts": Sequence[AdditionalArtifactType],
         "RefreshClosedReports": bool,
         "ReportVersioning": ReportVersioningType,
         "BillingViewArn": str,
     },
     total=False,
 )
 
@@ -125,15 +157,15 @@
         "RetryAttempts": int,
     },
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
-        "ReportDefinitions": List[ReportDefinitionTypeDef],
+        "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
```

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from mypy_boto3_cur.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
     data: DeleteReportDefinitionRequestRequestTypeDef = {...}
     ```
 """
 import sys
-from typing import Dict, List
+from typing import Dict, List, Sequence
 
 from .literals import (
     AdditionalArtifactType,
     AWSRegionType,
     CompressionFormatType,
     ReportFormatType,
     ReportVersioningType,
@@ -30,14 +30,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
     "DeleteReportDefinitionResponseTypeDef",
     "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
+    "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
@@ -71,31 +72,60 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredReportDefinitionOutputTypeDef = TypedDict(
+    "_RequiredReportDefinitionOutputTypeDef",
+    {
+        "ReportName": str,
+        "TimeUnit": TimeUnitType,
+        "Format": ReportFormatType,
+        "Compression": CompressionFormatType,
+        "AdditionalSchemaElements": List[SchemaElementType],
+        "S3Bucket": str,
+        "S3Prefix": str,
+        "S3Region": AWSRegionType,
+    },
+)
+_OptionalReportDefinitionOutputTypeDef = TypedDict(
+    "_OptionalReportDefinitionOutputTypeDef",
+    {
+        "AdditionalArtifacts": List[AdditionalArtifactType],
+        "RefreshClosedReports": bool,
+        "ReportVersioning": ReportVersioningType,
+        "BillingViewArn": str,
+    },
+    total=False,
+)
+
+class ReportDefinitionOutputTypeDef(
+    _RequiredReportDefinitionOutputTypeDef, _OptionalReportDefinitionOutputTypeDef
+):
+    pass
+
 _RequiredReportDefinitionTypeDef = TypedDict(
     "_RequiredReportDefinitionTypeDef",
     {
         "ReportName": str,
         "TimeUnit": TimeUnitType,
         "Format": ReportFormatType,
         "Compression": CompressionFormatType,
-        "AdditionalSchemaElements": List[SchemaElementType],
+        "AdditionalSchemaElements": Sequence[SchemaElementType],
         "S3Bucket": str,
         "S3Prefix": str,
         "S3Region": AWSRegionType,
     },
 )
 _OptionalReportDefinitionTypeDef = TypedDict(
     "_OptionalReportDefinitionTypeDef",
     {
-        "AdditionalArtifacts": List[AdditionalArtifactType],
+        "AdditionalArtifacts": Sequence[AdditionalArtifactType],
         "RefreshClosedReports": bool,
         "ReportVersioning": ReportVersioningType,
         "BillingViewArn": str,
     },
     total=False,
 )
 
@@ -122,15 +152,15 @@
         "RetryAttempts": int,
     },
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
-        "ReportDefinitions": List[ReportDefinitionTypeDef],
+        "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
```

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.0
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-cur"></a>
 
 # mypy-boto3-cur
 
 [![PyPI - mypy-boto3-cur](https://img.shields.io/pypi/v/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cur?color=blue)](https://pypistats.org/packages/mypy-boto3-cur)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,14 +331,15 @@
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
     DeleteReportDefinitionResponseTypeDef,
     DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
+    ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-cur-1.28.0/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.0/setup.py` & `mypy-boto3-cur-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostandUsageReportService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

