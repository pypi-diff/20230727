# Comparing `tmp/mypy-boto3-osis-1.28.0.tar.gz` & `tmp/mypy-boto3-osis-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.28.0.tar", last modified: Thu Jul  6 21:00:15 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-osis-1.28.0.tar` & `mypy-boto3-osis-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.846387 mypy-boto3-osis-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-06 21:00:15.834387 mypy-boto3-osis-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.826387 mypy-boto3-osis-1.28.0/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:48:57.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:15.834387 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 21:00:15.000000 mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:15.846387 mypy-boto3-osis-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 20:48:56.000000 mypy-boto3-osis-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.785132 mypy-boto3-osis-1.28.12/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-27 11:41:08.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/setup.py
```

### Comparing `mypy-boto3-osis-1.28.0/LICENSE` & `mypy-boto3-osis-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.0/PKG-INFO` & `mypy-boto3-osis-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-osis"></a>
 
 # mypy-boto3-osis
 
 [![PyPI - mypy-boto3-osis](https://img.shields.io/pypi/v/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,46 +299,50 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
+    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
+    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
```

### Comparing `mypy-boto3-osis-1.28.0/README.md` & `mypy-boto3-osis-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-osis"></a>
 
 # mypy-boto3-osis
 
 [![PyPI - mypy-boto3-osis](https://img.shields.io/pypi/v/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,46 +267,50 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
+    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
+    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
```

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
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
@@ -246,26 +247,28 @@
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

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
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
@@ -244,26 +245,28 @@
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

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,46 +25,50 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChangeProgressStageTypeDef",
+    "CloudWatchLogDestinationOutputTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PipelineStatusReasonTypeDef",
-    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
+    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
+    "LogPublishingOptionsOutputTypeDef",
     "LogPublishingOptionsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "VpcEndpointTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
+    "VpcEndpointTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PipelineTypeDef",
     "ListPipelinesResponseTypeDef",
+    "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -75,14 +79,21 @@
         "Status": ChangeProgressStageStatusesType,
         "Description": str,
         "LastUpdatedAt": datetime,
     },
     total=False,
 )
 
+CloudWatchLogDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogDestinationOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+)
+
 CloudWatchLogDestinationTypeDef = TypedDict(
     "CloudWatchLogDestinationTypeDef",
     {
         "LogGroup": str,
     },
 )
 
@@ -109,14 +120,25 @@
 )
 
 
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
 
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
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -170,31 +192,28 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-PipelineStatusReasonTypeDef = TypedDict(
-    "PipelineStatusReasonTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Description": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+PipelineStatusReasonTypeDef = TypedDict(
+    "PipelineStatusReasonTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Description": str,
     },
+    total=False,
 )
 
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
@@ -226,73 +245,91 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredVpcOptionsOutputTypeDef = TypedDict(
+    "_RequiredVpcOptionsOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcOptionsOutputTypeDef = TypedDict(
+    "_OptionalVpcOptionsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+
+class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
+    pass
+
+
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-LogPublishingOptionsTypeDef = TypedDict(
-    "LogPublishingOptionsTypeDef",
+LogPublishingOptionsOutputTypeDef = TypedDict(
+    "LogPublishingOptionsOutputTypeDef",
     {
         "IsLoggingEnabled": bool,
-        "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
+        "CloudWatchLogDestination": CloudWatchLogDestinationOutputTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+LogPublishingOptionsTypeDef = TypedDict(
+    "LogPublishingOptionsTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IsLoggingEnabled": bool,
+        "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
-    {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsTypeDef,
-    },
-    total=False,
-)
-
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -308,23 +345,33 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -370,74 +417,74 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineConfigurationBody": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "IngestEndpointUrls": List[str],
-        "LogPublishingOptions": LogPublishingOptionsTypeDef,
+        "LogPublishingOptions": LogPublishingOptionsOutputTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -24,46 +24,50 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChangeProgressStageTypeDef",
+    "CloudWatchLogDestinationOutputTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
+    "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "PipelineStatusReasonTypeDef",
-    "ResponseMetadataTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
+    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
+    "LogPublishingOptionsOutputTypeDef",
     "LogPublishingOptionsTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "VpcEndpointTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
+    "VpcEndpointTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "PipelineTypeDef",
     "ListPipelinesResponseTypeDef",
+    "PipelineTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -74,14 +78,21 @@
         "Status": ChangeProgressStageStatusesType,
         "Description": str,
         "LastUpdatedAt": datetime,
     },
     total=False,
 )
 
+CloudWatchLogDestinationOutputTypeDef = TypedDict(
+    "CloudWatchLogDestinationOutputTypeDef",
+    {
+        "LogGroup": str,
+    },
+)
+
 CloudWatchLogDestinationTypeDef = TypedDict(
     "CloudWatchLogDestinationTypeDef",
     {
         "LogGroup": str,
     },
 )
 
@@ -106,14 +117,25 @@
     },
     total=False,
 )
 
 class VpcOptionsTypeDef(_RequiredVpcOptionsTypeDef, _OptionalVpcOptionsTypeDef):
     pass
 
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
 DeletePipelineRequestRequestTypeDef = TypedDict(
     "DeletePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
 )
 
@@ -167,31 +189,28 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-PipelineStatusReasonTypeDef = TypedDict(
-    "PipelineStatusReasonTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Description": str,
+        "Key": str,
+        "Value": str,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+PipelineStatusReasonTypeDef = TypedDict(
+    "PipelineStatusReasonTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Description": str,
     },
+    total=False,
 )
 
 StartPipelineRequestRequestTypeDef = TypedDict(
     "StartPipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
     },
@@ -223,73 +242,89 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
+_RequiredVpcOptionsOutputTypeDef = TypedDict(
+    "_RequiredVpcOptionsOutputTypeDef",
+    {
+        "SubnetIds": List[str],
+    },
+)
+_OptionalVpcOptionsOutputTypeDef = TypedDict(
+    "_OptionalVpcOptionsOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+    },
+    total=False,
+)
+
+class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
+    pass
+
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-LogPublishingOptionsTypeDef = TypedDict(
-    "LogPublishingOptionsTypeDef",
+LogPublishingOptionsOutputTypeDef = TypedDict(
+    "LogPublishingOptionsOutputTypeDef",
     {
         "IsLoggingEnabled": bool,
-        "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
+        "CloudWatchLogDestination": CloudWatchLogDestinationOutputTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+LogPublishingOptionsTypeDef = TypedDict(
+    "LogPublishingOptionsTypeDef",
     {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IsLoggingEnabled": bool,
+        "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
+    total=False,
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
-    {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsTypeDef,
-    },
-    total=False,
-)
-
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelineBlueprintsResponseTypeDef = TypedDict(
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
@@ -305,23 +340,33 @@
 )
 
 ValidatePipelineResponseTypeDef = TypedDict(
     "ValidatePipelineResponseTypeDef",
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsOutputTypeDef,
+    },
+    total=False,
+)
+
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "PipelineName": str,
@@ -363,74 +408,74 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineConfigurationBody": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "IngestEndpointUrls": List[str],
-        "LogPublishingOptions": LogPublishingOptionsTypeDef,
+        "LogPublishingOptions": LogPublishingOptionsOutputTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPipelineResponseTypeDef = TypedDict(
     "GetPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartPipelineResponseTypeDef = TypedDict(
     "StartPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopPipelineResponseTypeDef = TypedDict(
     "StopPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.0
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-osis"></a>
 
 # mypy-boto3-osis
 
 [![PyPI - mypy-boto3-osis](https://img.shields.io/pypi/v/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-osis?color=blue)](https://pypistats.org/packages/mypy-boto3-osis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,46 +299,50 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
+    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
+    ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
-    ResponseMetadataTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
+    VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
+    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    VpcEndpointTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
+    VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    PipelineTypeDef,
     ListPipelinesResponseTypeDef,
+    PipelineTypeDef,
     CreatePipelineResponseTypeDef,
     GetPipelineResponseTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     UpdatePipelineResponseTypeDef,
 )
```

### Comparing `mypy-boto3-osis-1.28.0/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.0/setup.py` & `mypy-boto3-osis-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

