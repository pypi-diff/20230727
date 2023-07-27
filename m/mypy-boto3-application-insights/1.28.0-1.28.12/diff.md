# Comparing `tmp/mypy-boto3-application-insights-1.28.0.tar.gz` & `tmp/mypy-boto3-application-insights-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-application-insights-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-application-insights-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-application-insights-1.28.0.tar` & `mypy-boto3-application-insights-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.682221 mypy-boto3-application-insights-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-06 20:58:58.682221 mypy-boto3-application-insights-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.662220 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-06 20:33:24.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-07-06 20:33:24.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.662220 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14982 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:58:58.000000 mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.682221 mypy-boto3-application-insights-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 20:33:23.000000 mypy-boto3-application-insights-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.472577 mypy-boto3-application-insights-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20900 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9681 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19938 2023-07-27 05:17:26.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19923 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.464577 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:34:18.000000 mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.472577 mypy-boto3-application-insights-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-27 05:17:25.000000 mypy-boto3-application-insights-1.28.12/setup.py
```

### Comparing `mypy-boto3-application-insights-1.28.0/LICENSE` & `mypy-boto3-application-insights-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.0/PKG-INFO` & `mypy-boto3-application-insights-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.0
-Summary: Type annotations for boto3.ApplicationInsights 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ApplicationInsights 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,38 +339,39 @@
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
 def get_structure() -> ApplicationComponentTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-application-insights-1.28.0/README.md` & `mypy-boto3-application-insights-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,38 +307,39 @@
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
 def get_structure() -> ApplicationComponentTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/__main__.py` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationInsights 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ApplicationInsights 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/client.py` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/client.pyi` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/literals.py` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,15 @@
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
@@ -274,26 +275,28 @@
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
@@ -440,24 +443,28 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/literals.pyi` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
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
@@ -272,26 +273,28 @@
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
@@ -438,24 +441,28 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ca-central-1",
     "eu-central-1",
+    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
+    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/type_defs.py` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,38 +65,39 @@
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
     "DescribeComponentResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
@@ -468,14 +469,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -660,22 +669,14 @@
         "AutoConfigEnabled": bool,
         "AutoCreate": bool,
         "GroupingType": Literal["ACCOUNT_BASED"],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -747,14 +748,22 @@
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights/type_defs.pyi` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,38 +64,39 @@
     "ListComponentsRequestRequestTypeDef",
     "ListConfigurationHistoryRequestRequestTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
     "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
     "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
     "DescribeComponentResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
@@ -461,14 +462,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -645,22 +654,14 @@
         "AutoConfigEnabled": bool,
         "AutoCreate": bool,
         "GroupingType": Literal["ACCOUNT_BASED"],
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -732,14 +733,22 @@
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/PKG-INFO` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-application-insights
-Version: 1.28.0
-Summary: Type annotations for boto3.ApplicationInsights 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ApplicationInsights 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-application-insights"></a>
 
 # mypy-boto3-application-insights
 
 [![PyPI - mypy-boto3-application-insights](https://img.shields.io/pypi/v/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-application-insights.svg?color=blue)](https://pypi.org/project/mypy-boto3-application-insights)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-application-insights?color=blue)](https://pypistats.org/packages/mypy-boto3-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-application-insights)](https://pepy.tech/project/mypy-boto3-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationInsights 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
+[boto3.ApplicationInsights 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [mypy-boto3-application-insights docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_application_insights/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,38 +339,39 @@
     ListComponentsRequestRequestTypeDef,
     ListConfigurationHistoryRequestRequestTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
     ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
     DescribeComponentResponseTypeDef,
     ListComponentsResponseTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
 def get_structure() -> ApplicationComponentTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-application-insights-1.28.0/mypy_boto3_application_insights.egg-info/SOURCES.txt` & `mypy-boto3-application-insights-1.28.12/mypy_boto3_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-application-insights-1.28.0/setup.py` & `mypy-boto3-application-insights-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-application-insights",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationInsights 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ApplicationInsights 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

