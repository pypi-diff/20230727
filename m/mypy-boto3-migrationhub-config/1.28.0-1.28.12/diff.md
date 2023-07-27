# Comparing `tmp/mypy-boto3-migrationhub-config-1.28.0.tar.gz` & `tmp/mypy-boto3-migrationhub-config-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.0.tar", last modified: Thu Jul  6 21:00:09 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhub-config-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
```

## Comparing `mypy-boto3-migrationhub-config-1.28.0.tar` & `mypy-boto3-migrationhub-config-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.534374 mypy-boto3-migrationhub-config-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-06 21:00:09.526374 mypy-boto3-migrationhub-config-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.526374 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-06 20:47:47.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:09.526374 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 21:00:09.000000 mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:09.534374 mypy-boto3-migrationhub-config-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 20:47:46.000000 mypy-boto3-migrationhub-config-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.848431 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-27 05:26:41.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:35:03.000000 mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.852431 mypy-boto3-migrationhub-config-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 05:26:40.000000 mypy-boto3-migrationhub-config-1.28.12/setup.py
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/LICENSE` & `mypy-boto3-migrationhub-config-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.0/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhub-config"></a>
 
 # mypy-boto3-migrationhub-config
 
 [![PyPI - mypy-boto3-migrationhub-config](https://img.shields.io/pypi/v/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhub-config?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhub-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,14 +299,15 @@
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     GetHomeRegionResultTypeDef,
+    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/README.md` & `mypy-boto3-migrationhub-config-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-migrationhub-config"></a>
 
 # mypy-boto3-migrationhub-config
 
 [![PyPI - mypy-boto3-migrationhub-config](https://img.shields.io/pypi/v/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhub-config?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhub-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,14 +267,15 @@
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     GetHomeRegionResultTypeDef,
+    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/__main__.py` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubConfig 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.MigrationHubConfig 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig\nOther"
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

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/client.py` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/client.pyi` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/literals.py` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TargetTypeType", "MigrationHubConfigServiceName", "ServiceName", "ResourceServiceName")
 
-
 TargetTypeType = Literal["ACCOUNT"]
 MigrationHubConfigServiceName = Literal["migrationhub-config"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -139,14 +137,15 @@
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
@@ -225,26 +224,28 @@
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

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/literals.pyi` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("TargetTypeType", "MigrationHubConfigServiceName", "ServiceName", "ResourceServiceName")
 
+
 TargetTypeType = Literal["ACCOUNT"]
 MigrationHubConfigServiceName = Literal["migrationhub-config"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -137,14 +139,15 @@
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
@@ -223,26 +226,28 @@
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

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/type_defs.py` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TargetTypeDef",
     "GetHomeRegionResultTypeDef",
+    "TargetOutputTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
     "CreateHomeRegionControlResultTypeDef",
     "DescribeHomeRegionControlsResultTypeDef",
 )
@@ -59,14 +60,33 @@
     "GetHomeRegionResultTypeDef",
     {
         "HomeRegion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Type": Literal["ACCOUNT"],
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
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
@@ -110,15 +130,15 @@
 )
 
 HomeRegionControlTypeDef = TypedDict(
     "HomeRegionControlTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
-        "Target": TargetTypeDef,
+        "Target": TargetOutputTypeDef,
         "RequestedTime": datetime,
     },
     total=False,
 )
 
 CreateHomeRegionControlResultTypeDef = TypedDict(
     "CreateHomeRegionControlResultTypeDef",
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config/type_defs.pyi` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TargetTypeDef",
     "GetHomeRegionResultTypeDef",
+    "TargetOutputTypeDef",
     "ResponseMetadataTypeDef",
     "CreateHomeRegionControlRequestRequestTypeDef",
     "DescribeHomeRegionControlsRequestRequestTypeDef",
     "HomeRegionControlTypeDef",
     "CreateHomeRegionControlResultTypeDef",
     "DescribeHomeRegionControlsResultTypeDef",
 )
@@ -56,14 +57,31 @@
     "GetHomeRegionResultTypeDef",
     {
         "HomeRegion": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredTargetOutputTypeDef = TypedDict(
+    "_RequiredTargetOutputTypeDef",
+    {
+        "Type": Literal["ACCOUNT"],
+    },
+)
+_OptionalTargetOutputTypeDef = TypedDict(
+    "_OptionalTargetOutputTypeDef",
+    {
+        "Id": str,
+    },
+    total=False,
+)
+
+class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
+    pass
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -105,15 +123,15 @@
 )
 
 HomeRegionControlTypeDef = TypedDict(
     "HomeRegionControlTypeDef",
     {
         "ControlId": str,
         "HomeRegion": str,
-        "Target": TargetTypeDef,
+        "Target": TargetOutputTypeDef,
         "RequestedTime": datetime,
     },
     total=False,
 )
 
 CreateHomeRegionControlResultTypeDef = TypedDict(
     "CreateHomeRegionControlResultTypeDef",
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/PKG-INFO` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhub-config
-Version: 1.28.0
-Summary: Type annotations for boto3.MigrationHubConfig 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-migrationhub-config"></a>
 
 # mypy-boto3-migrationhub-config
 
 [![PyPI - mypy-boto3-migrationhub-config](https://img.shields.io/pypi/v/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhub-config.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-migrationhub-config?color=blue)](https://pypistats.org/packages/mypy-boto3-migrationhub-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhub-config)](https://pepy.tech/project/mypy-boto3-migrationhub-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
+[boto3.MigrationHubConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
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
 [mypy-boto3-migrationhub-config docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,14 +299,15 @@
 `mypy_boto3_migrationhub_config.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migrationhub_config.type_defs import (
     TargetTypeDef,
     GetHomeRegionResultTypeDef,
+    TargetOutputTypeDef,
     ResponseMetadataTypeDef,
     CreateHomeRegionControlRequestRequestTypeDef,
     DescribeHomeRegionControlsRequestRequestTypeDef,
     HomeRegionControlTypeDef,
     CreateHomeRegionControlResultTypeDef,
     DescribeHomeRegionControlsResultTypeDef,
 )
```

### Comparing `mypy-boto3-migrationhub-config-1.28.0/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt` & `mypy-boto3-migrationhub-config-1.28.12/mypy_boto3_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhub-config-1.28.0/setup.py` & `mypy-boto3-migrationhub-config-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhub-config",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubConfig 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MigrationHubConfig 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

