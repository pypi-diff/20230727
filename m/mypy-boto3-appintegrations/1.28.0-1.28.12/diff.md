# Comparing `tmp/mypy-boto3-appintegrations-1.28.0.tar.gz` & `tmp/mypy-boto3-appintegrations-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appintegrations-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-appintegrations-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-appintegrations-1.28.0.tar` & `mypy-boto3-appintegrations-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.610220 mypy-boto3-appintegrations-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-06 20:58:58.606220 mypy-boto3-appintegrations-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.602220 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-07-06 20:33:19.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-07-06 20:33:19.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-06 20:33:19.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-07-06 20:33:19.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.606220 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:58:58.000000 mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.610220 mypy-boto3-appintegrations-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 20:33:18.000000 mypy-boto3-appintegrations-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.424577 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-07-27 05:17:23.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:18.000000 mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.428577 mypy-boto3-appintegrations-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:17:22.000000 mypy-boto3-appintegrations-1.28.12/setup.py
```

### Comparing `mypy-boto3-appintegrations-1.28.0/LICENSE` & `mypy-boto3-appintegrations-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.0/PKG-INFO` & `mypy-boto3-appintegrations-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.0
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,20 +299,23 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     EventFilterTypeDef,
     CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
+    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
@@ -323,18 +326,18 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    EventIntegrationTypeDef,
-    GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
+    EventIntegrationTypeDef,
+    GetEventIntegrationResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.0/README.md` & `mypy-boto3-appintegrations-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,20 +267,23 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     EventFilterTypeDef,
     CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
+    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
@@ -291,18 +294,18 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    EventIntegrationTypeDef,
-    GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
+    EventIntegrationTypeDef,
+    GetEventIntegrationResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/__main__.py` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppIntegrationsService 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppIntegrationsService 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/client.py` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/client.pyi` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/literals.py` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,15 @@
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
@@ -224,26 +225,28 @@
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

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/literals.pyi` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
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
@@ -222,26 +223,28 @@
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

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/type_defs.py` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
+    "FileConfigurationOutputTypeDef",
+    "ScheduleConfigurationOutputTypeDef",
     "EventFilterTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
+    "EventFilterOutputTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
@@ -43,18 +45,18 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
-    "EventIntegrationTypeDef",
-    "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
+    "EventIntegrationTypeDef",
+    "GetEventIntegrationResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
 )
 
 _RequiredFileConfigurationTypeDef = TypedDict(
     "_RequiredFileConfigurationTypeDef",
     {
@@ -65,21 +67,19 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -87,20 +87,57 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
-
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
+_RequiredFileConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFileConfigurationOutputTypeDef",
+    {
+        "Folders": List[str],
+    },
+)
+_OptionalFileConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFileConfigurationOutputTypeDef",
+    {
+        "Filters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+class FileConfigurationOutputTypeDef(
+    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
+):
+    pass
+
+_RequiredScheduleConfigurationOutputTypeDef = TypedDict(
+    "_RequiredScheduleConfigurationOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+_OptionalScheduleConfigurationOutputTypeDef = TypedDict(
+    "_OptionalScheduleConfigurationOutputTypeDef",
+    {
+        "FirstExecutionFrom": str,
+        "Object": str,
+    },
+    total=False,
+)
+
+class ScheduleConfigurationOutputTypeDef(
+    _RequiredScheduleConfigurationOutputTypeDef, _OptionalScheduleConfigurationOutputTypeDef
+):
+    pass
 
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "Source": str,
     },
 )
@@ -143,14 +180,21 @@
 DeleteEventIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+EventFilterOutputTypeDef = TypedDict(
+    "EventFilterOutputTypeDef",
+    {
+        "Source": str,
+    },
+)
+
 EventIntegrationAssociationTypeDef = TypedDict(
     "EventIntegrationAssociationTypeDef",
     {
         "EventIntegrationAssociationArn": str,
         "EventIntegrationAssociationId": str,
         "EventIntegrationName": str,
         "ClientId": str,
@@ -185,22 +229,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -217,22 +259,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -291,44 +331,40 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -342,52 +378,50 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
-
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
@@ -403,66 +437,64 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    {
+        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataIntegrationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationsResponseTypeDef",
+    {
+        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
 
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
-        "EventFilter": EventFilterTypeDef,
+        "EventFilter": EventFilterOutputTypeDef,
         "EventBridgeBus": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 GetEventIntegrationResponseTypeDef = TypedDict(
     "GetEventIntegrationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
-        "EventFilter": EventFilterTypeDef,
+        "EventFilter": EventFilterOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    {
-        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDataIntegrationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationsResponseTypeDef",
-    {
-        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations/type_defs.pyi` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
+    "FileConfigurationOutputTypeDef",
+    "ScheduleConfigurationOutputTypeDef",
     "EventFilterTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
+    "EventFilterOutputTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
@@ -42,18 +46,18 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
-    "EventIntegrationTypeDef",
-    "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
+    "EventIntegrationTypeDef",
+    "GetEventIntegrationResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
 )
 
 _RequiredFileConfigurationTypeDef = TypedDict(
     "_RequiredFileConfigurationTypeDef",
     {
@@ -64,19 +68,21 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -84,19 +90,64 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
+
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
+
+_RequiredFileConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFileConfigurationOutputTypeDef",
+    {
+        "Folders": List[str],
+    },
+)
+_OptionalFileConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFileConfigurationOutputTypeDef",
+    {
+        "Filters": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+
+class FileConfigurationOutputTypeDef(
+    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
+):
+    pass
+
+
+_RequiredScheduleConfigurationOutputTypeDef = TypedDict(
+    "_RequiredScheduleConfigurationOutputTypeDef",
+    {
+        "ScheduleExpression": str,
+    },
+)
+_OptionalScheduleConfigurationOutputTypeDef = TypedDict(
+    "_OptionalScheduleConfigurationOutputTypeDef",
+    {
+        "FirstExecutionFrom": str,
+        "Object": str,
+    },
+    total=False,
+)
+
+
+class ScheduleConfigurationOutputTypeDef(
+    _RequiredScheduleConfigurationOutputTypeDef, _OptionalScheduleConfigurationOutputTypeDef
+):
+    pass
+
+
 EventFilterTypeDef = TypedDict(
     "EventFilterTypeDef",
     {
         "Source": str,
     },
 )
 
@@ -138,14 +189,21 @@
 DeleteEventIntegrationRequestRequestTypeDef = TypedDict(
     "DeleteEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+EventFilterOutputTypeDef = TypedDict(
+    "EventFilterOutputTypeDef",
+    {
+        "Source": str,
+    },
+)
+
 EventIntegrationAssociationTypeDef = TypedDict(
     "EventIntegrationAssociationTypeDef",
     {
         "EventIntegrationAssociationArn": str,
         "EventIntegrationAssociationId": str,
         "EventIntegrationName": str,
         "ClientId": str,
@@ -180,20 +238,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -210,20 +270,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -282,40 +344,44 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -329,50 +395,52 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
+
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
@@ -388,64 +456,66 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
+ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationAssociationsResponseTypeDef",
+    {
+        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListDataIntegrationsResponseTypeDef = TypedDict(
+    "ListDataIntegrationsResponseTypeDef",
+    {
+        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
-        "EventFilter": EventFilterTypeDef,
+        "EventFilter": EventFilterOutputTypeDef,
         "EventBridgeBus": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
 GetEventIntegrationResponseTypeDef = TypedDict(
     "GetEventIntegrationResponseTypeDef",
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
-        "EventFilter": EventFilterTypeDef,
+        "EventFilter": EventFilterOutputTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationAssociationsResponseTypeDef",
-    {
-        "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDataIntegrationsResponseTypeDef = TypedDict(
-    "ListDataIntegrationsResponseTypeDef",
-    {
-        "DataIntegrations": List[DataIntegrationSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/PKG-INFO` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appintegrations
-Version: 1.28.0
-Summary: Type annotations for boto3.AppIntegrationsService 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appintegrations"></a>
 
 # mypy-boto3-appintegrations
 
 [![PyPI - mypy-boto3-appintegrations](https://img.shields.io/pypi/v/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appintegrations.svg?color=blue)](https://pypi.org/project/mypy-boto3-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appintegrations?color=blue)](https://pypistats.org/packages/mypy-boto3-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appintegrations)](https://pepy.tech/project/mypy-boto3-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppIntegrationsService 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
+[boto3.AppIntegrationsService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [mypy-boto3-appintegrations docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,20 +299,23 @@
 `mypy_boto3_appintegrations.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ScheduleConfigurationOutputTypeDef,
     EventFilterTypeDef,
     CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
+    EventFilterOutputTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
@@ -323,18 +326,18 @@
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
     CreateDataIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
-    EventIntegrationTypeDef,
-    GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
+    EventIntegrationTypeDef,
+    GetEventIntegrationResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
 def get_structure() -> FileConfigurationTypeDef:
     return {...}
```

### Comparing `mypy-boto3-appintegrations-1.28.0/mypy_boto3_appintegrations.egg-info/SOURCES.txt` & `mypy-boto3-appintegrations-1.28.12/mypy_boto3_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appintegrations-1.28.0/setup.py` & `mypy-boto3-appintegrations-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appintegrations",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppIntegrationsService 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AppIntegrationsService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

