# Comparing `tmp/mypy-boto3-wisdom-1.28.11.tar.gz` & `tmp/mypy-boto3-wisdom-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.28.11.tar", last modified: Tue Jul 25 19:49:16 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.28.11.tar` & `mypy-boto3-wisdom-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33923 2023-07-25 19:49:03.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33886 2023-07-25 19:49:02.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17881 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 19:49:16.000000 mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:16.501064 mypy-boto3-wisdom-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-25 19:49:01.000000 mypy-boto3-wisdom-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37471 2023-07-27 11:48:48.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/setup.py
```

### Comparing `mypy-boto3-wisdom-1.28.11/LICENSE` & `mypy-boto3-wisdom-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/PKG-INFO` & `mypy-boto3-wisdom-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.11
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.11/README.md` & `mypy-boto3-wisdom-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.28.11\nVersion:         1.28.11\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,15 @@
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
@@ -290,14 +291,15 @@
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

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
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
@@ -288,14 +289,15 @@
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

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,22 +132,36 @@
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
-AppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "AppIntegrationsConfigurationOutputTypeDef",
+_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
     {
         "appIntegrationArn": str,
+    },
+)
+_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
+    {
         "objectFields": List[str],
     },
+    total=False,
 )
 
+
+class AppIntegrationsConfigurationOutputTypeDef(
+    _RequiredAppIntegrationsConfigurationOutputTypeDef,
+    _OptionalAppIntegrationsConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -175,76 +189,102 @@
 
 KnowledgeBaseAssociationDataTypeDef = TypedDict(
     "KnowledgeBaseAssociationDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
+    total=False,
 )
 
 AssistantIntegrationConfigurationTypeDef = TypedDict(
     "AssistantIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
+    total=False,
 )
 
 ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
+    total=False,
 )
 
-ContentDataTypeDef = TypedDict(
-    "ContentDataTypeDef",
+_RequiredContentDataTypeDef = TypedDict(
+    "_RequiredContentDataTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
-        "linkOutUri": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
-        "tags": Dict[str, str],
         "title": str,
         "url": str,
         "urlExpiry": datetime,
     },
 )
+_OptionalContentDataTypeDef = TypedDict(
+    "_OptionalContentDataTypeDef",
+    {
+        "linkOutUri": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class ContentDataTypeDef(_RequiredContentDataTypeDef, _OptionalContentDataTypeDef):
+    pass
+
 
 ContentReferenceTypeDef = TypedDict(
     "ContentReferenceTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
+    total=False,
 )
 
-ContentSummaryTypeDef = TypedDict(
-    "ContentSummaryTypeDef",
+_RequiredContentSummaryTypeDef = TypedDict(
+    "_RequiredContentSummaryTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
-        "tags": Dict[str, str],
         "title": str,
     },
 )
+_OptionalContentSummaryTypeDef = TypedDict(
+    "_OptionalContentSummaryTypeDef",
+    {
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
+    pass
+
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -352,14 +392,15 @@
 
 HighlightTypeDef = TypedDict(
     "HighlightTypeDef",
     {
         "beginOffsetInclusive": int,
         "endOffsetExclusive": int,
     },
+    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "field": Literal["NAME"],
         "operator": Literal["EQUALS"],
@@ -438,14 +479,15 @@
 )
 
 RenderingConfigurationOutputTypeDef = TypedDict(
     "RenderingConfigurationOutputTypeDef",
     {
         "templateUri": str,
     },
+    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -526,14 +568,15 @@
 
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
+    total=False,
 )
 
 NotifyRecommendationsReceivedRequestRequestTypeDef = TypedDict(
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
@@ -565,14 +608,15 @@
 
 
 QueryRecommendationTriggerDataTypeDef = TypedDict(
     "QueryRecommendationTriggerDataTypeDef",
     {
         "text": str,
     },
+    total=False,
 )
 
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
@@ -589,14 +633,15 @@
 )
 
 SessionIntegrationConfigurationTypeDef = TypedDict(
     "SessionIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
+    total=False,
 )
 
 StartContentUploadRequestRequestTypeDef = TypedDict(
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
@@ -655,14 +700,15 @@
 )
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
@@ -695,46 +741,69 @@
 
 
 AssistantAssociationOutputDataTypeDef = TypedDict(
     "AssistantAssociationOutputDataTypeDef",
     {
         "knowledgeBaseAssociation": KnowledgeBaseAssociationDataTypeDef,
     },
+    total=False,
 )
 
-AssistantDataTypeDef = TypedDict(
-    "AssistantDataTypeDef",
+_RequiredAssistantDataTypeDef = TypedDict(
+    "_RequiredAssistantDataTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "name": str,
+        "status": AssistantStatusType,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalAssistantDataTypeDef = TypedDict(
+    "_OptionalAssistantDataTypeDef",
+    {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "name": str,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "status": AssistantStatusType,
         "tags": Dict[str, str],
-        "type": Literal["AGENT"],
     },
+    total=False,
 )
 
-AssistantSummaryTypeDef = TypedDict(
-    "AssistantSummaryTypeDef",
+
+class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
+    pass
+
+
+_RequiredAssistantSummaryTypeDef = TypedDict(
+    "_RequiredAssistantSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "name": str,
+        "status": AssistantStatusType,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalAssistantSummaryTypeDef = TypedDict(
+    "_OptionalAssistantSummaryTypeDef",
+    {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "name": str,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "status": AssistantStatusType,
         "tags": Dict[str, str],
-        "type": Literal["AGENT"],
     },
+    total=False,
 )
 
+
+class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
+    pass
+
+
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -827,14 +896,15 @@
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
+    total=False,
 )
 
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
@@ -933,70 +1003,108 @@
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
     },
+    total=False,
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SessionDataTypeDef = TypedDict(
-    "SessionDataTypeDef",
+_RequiredSessionDataTypeDef = TypedDict(
+    "_RequiredSessionDataTypeDef",
     {
-        "description": str,
-        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
         "name": str,
         "sessionArn": str,
         "sessionId": str,
+    },
+)
+_OptionalSessionDataTypeDef = TypedDict(
+    "_OptionalSessionDataTypeDef",
+    {
+        "description": str,
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-KnowledgeBaseDataTypeDef = TypedDict(
-    "KnowledgeBaseDataTypeDef",
+
+class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
+    pass
+
+
+_RequiredKnowledgeBaseDataTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseDataTypeDef",
     {
-        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
-        "lastContentModificationTime": datetime,
         "name": str,
+        "status": KnowledgeBaseStatusType,
+    },
+)
+_OptionalKnowledgeBaseDataTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseDataTypeDef",
+    {
+        "description": str,
+        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationOutputTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-KnowledgeBaseSummaryTypeDef = TypedDict(
-    "KnowledgeBaseSummaryTypeDef",
+
+class KnowledgeBaseDataTypeDef(
+    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
+):
+    pass
+
+
+_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseSummaryTypeDef",
     {
-        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
+        "status": KnowledgeBaseStatusType,
+    },
+)
+_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseSummaryTypeDef",
+    {
+        "description": str,
         "renderingConfiguration": RenderingConfigurationOutputTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
+
+class KnowledgeBaseSummaryTypeDef(
+    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+):
+    pass
+
+
 _RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
     },
 )
@@ -1017,40 +1125,66 @@
 class CreateKnowledgeBaseRequestRequestTypeDef(
     _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
     _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
 
-AssistantAssociationDataTypeDef = TypedDict(
-    "AssistantAssociationDataTypeDef",
+_RequiredAssistantAssociationDataTypeDef = TypedDict(
+    "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
+    },
+)
+_OptionalAssistantAssociationDataTypeDef = TypedDict(
+    "_OptionalAssistantAssociationDataTypeDef",
+    {
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-AssistantAssociationSummaryTypeDef = TypedDict(
-    "AssistantAssociationSummaryTypeDef",
+
+class AssistantAssociationDataTypeDef(
+    _RequiredAssistantAssociationDataTypeDef, _OptionalAssistantAssociationDataTypeDef
+):
+    pass
+
+
+_RequiredAssistantAssociationSummaryTypeDef = TypedDict(
+    "_RequiredAssistantAssociationSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
+    },
+)
+_OptionalAssistantAssociationSummaryTypeDef = TypedDict(
+    "_OptionalAssistantAssociationSummaryTypeDef",
+    {
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
+
+class AssistantAssociationSummaryTypeDef(
+    _RequiredAssistantAssociationSummaryTypeDef, _OptionalAssistantAssociationSummaryTypeDef
+):
+    pass
+
+
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1068,23 +1202,34 @@
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
+_RequiredDocumentTypeDef = TypedDict(
+    "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
+    },
+)
+_OptionalDocumentTypeDef = TypedDict(
+    "_OptionalDocumentTypeDef",
+    {
         "excerpt": DocumentTextTypeDef,
         "title": DocumentTextTypeDef,
     },
+    total=False,
 )
 
+
+class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
+    pass
+
+
 _RequiredSearchContentRequestRequestTypeDef = TypedDict(
     "_RequiredSearchContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
@@ -1254,33 +1399,57 @@
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecommendationDataTypeDef = TypedDict(
-    "RecommendationDataTypeDef",
+_RequiredRecommendationDataTypeDef = TypedDict(
+    "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
         "recommendationId": str,
+    },
+)
+_OptionalRecommendationDataTypeDef = TypedDict(
+    "_OptionalRecommendationDataTypeDef",
+    {
         "relevanceLevel": RelevanceLevelType,
         "relevanceScore": float,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
+    total=False,
 )
 
-ResultDataTypeDef = TypedDict(
-    "ResultDataTypeDef",
+
+class RecommendationDataTypeDef(
+    _RequiredRecommendationDataTypeDef, _OptionalRecommendationDataTypeDef
+):
+    pass
+
+
+_RequiredResultDataTypeDef = TypedDict(
+    "_RequiredResultDataTypeDef",
     {
         "document": DocumentTypeDef,
-        "relevanceScore": float,
         "resultId": str,
     },
 )
+_OptionalResultDataTypeDef = TypedDict(
+    "_OptionalResultDataTypeDef",
+    {
+        "relevanceScore": float,
+    },
+    total=False,
+)
+
+
+class ResultDataTypeDef(_RequiredResultDataTypeDef, _OptionalResultDataTypeDef):
+    pass
+
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -131,22 +131,34 @@
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
-AppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "AppIntegrationsConfigurationOutputTypeDef",
+_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
     {
         "appIntegrationArn": str,
+    },
+)
+_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
+    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
+    {
         "objectFields": List[str],
     },
+    total=False,
 )
 
+class AppIntegrationsConfigurationOutputTypeDef(
+    _RequiredAppIntegrationsConfigurationOutputTypeDef,
+    _OptionalAppIntegrationsConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -172,76 +184,98 @@
 
 KnowledgeBaseAssociationDataTypeDef = TypedDict(
     "KnowledgeBaseAssociationDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
+    total=False,
 )
 
 AssistantIntegrationConfigurationTypeDef = TypedDict(
     "AssistantIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
+    total=False,
 )
 
 ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationOutputTypeDef",
     {
         "kmsKeyId": str,
     },
+    total=False,
 )
 
-ContentDataTypeDef = TypedDict(
-    "ContentDataTypeDef",
+_RequiredContentDataTypeDef = TypedDict(
+    "_RequiredContentDataTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
-        "linkOutUri": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
-        "tags": Dict[str, str],
         "title": str,
         "url": str,
         "urlExpiry": datetime,
     },
 )
+_OptionalContentDataTypeDef = TypedDict(
+    "_OptionalContentDataTypeDef",
+    {
+        "linkOutUri": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class ContentDataTypeDef(_RequiredContentDataTypeDef, _OptionalContentDataTypeDef):
+    pass
 
 ContentReferenceTypeDef = TypedDict(
     "ContentReferenceTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
+    total=False,
 )
 
-ContentSummaryTypeDef = TypedDict(
-    "ContentSummaryTypeDef",
+_RequiredContentSummaryTypeDef = TypedDict(
+    "_RequiredContentSummaryTypeDef",
     {
         "contentArn": str,
         "contentId": str,
         "contentType": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "metadata": Dict[str, str],
         "name": str,
         "revisionId": str,
         "status": ContentStatusType,
-        "tags": Dict[str, str],
         "title": str,
     },
 )
+_OptionalContentSummaryTypeDef = TypedDict(
+    "_OptionalContentSummaryTypeDef",
+    {
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class ContentSummaryTypeDef(_RequiredContentSummaryTypeDef, _OptionalContentSummaryTypeDef):
+    pass
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -345,14 +379,15 @@
 
 HighlightTypeDef = TypedDict(
     "HighlightTypeDef",
     {
         "beginOffsetInclusive": int,
         "endOffsetExclusive": int,
     },
+    total=False,
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "field": Literal["NAME"],
         "operator": Literal["EQUALS"],
@@ -429,14 +464,15 @@
 )
 
 RenderingConfigurationOutputTypeDef = TypedDict(
     "RenderingConfigurationOutputTypeDef",
     {
         "templateUri": str,
     },
+    total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
@@ -513,14 +549,15 @@
 
 NotifyRecommendationsReceivedErrorTypeDef = TypedDict(
     "NotifyRecommendationsReceivedErrorTypeDef",
     {
         "message": str,
         "recommendationId": str,
     },
+    total=False,
 )
 
 NotifyRecommendationsReceivedRequestRequestTypeDef = TypedDict(
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     {
         "assistantId": str,
         "recommendationIds": Sequence[str],
@@ -550,14 +587,15 @@
     pass
 
 QueryRecommendationTriggerDataTypeDef = TypedDict(
     "QueryRecommendationTriggerDataTypeDef",
     {
         "text": str,
     },
+    total=False,
 )
 
 RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = TypedDict(
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
     },
@@ -574,14 +612,15 @@
 )
 
 SessionIntegrationConfigurationTypeDef = TypedDict(
     "SessionIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
+    total=False,
 )
 
 StartContentUploadRequestRequestTypeDef = TypedDict(
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
@@ -638,14 +677,15 @@
 )
 
 SourceConfigurationOutputTypeDef = TypedDict(
     "SourceConfigurationOutputTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
@@ -676,46 +716,65 @@
     pass
 
 AssistantAssociationOutputDataTypeDef = TypedDict(
     "AssistantAssociationOutputDataTypeDef",
     {
         "knowledgeBaseAssociation": KnowledgeBaseAssociationDataTypeDef,
     },
+    total=False,
 )
 
-AssistantDataTypeDef = TypedDict(
-    "AssistantDataTypeDef",
+_RequiredAssistantDataTypeDef = TypedDict(
+    "_RequiredAssistantDataTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "name": str,
+        "status": AssistantStatusType,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalAssistantDataTypeDef = TypedDict(
+    "_OptionalAssistantDataTypeDef",
+    {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "name": str,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "status": AssistantStatusType,
         "tags": Dict[str, str],
-        "type": Literal["AGENT"],
     },
+    total=False,
 )
 
-AssistantSummaryTypeDef = TypedDict(
-    "AssistantSummaryTypeDef",
+class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
+    pass
+
+_RequiredAssistantSummaryTypeDef = TypedDict(
+    "_RequiredAssistantSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantId": str,
+        "name": str,
+        "status": AssistantStatusType,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalAssistantSummaryTypeDef = TypedDict(
+    "_OptionalAssistantSummaryTypeDef",
+    {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "name": str,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
-        "status": AssistantStatusType,
         "tags": Dict[str, str],
-        "type": Literal["AGENT"],
     },
+    total=False,
 )
 
+class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
+    pass
+
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -806,14 +865,15 @@
 
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
+    total=False,
 )
 
 SearchExpressionTypeDef = TypedDict(
     "SearchExpressionTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
     },
@@ -906,70 +966,102 @@
 )
 
 RecommendationTriggerDataTypeDef = TypedDict(
     "RecommendationTriggerDataTypeDef",
     {
         "query": QueryRecommendationTriggerDataTypeDef,
     },
+    total=False,
 )
 
 SearchSessionsResponseTypeDef = TypedDict(
     "SearchSessionsResponseTypeDef",
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SessionDataTypeDef = TypedDict(
-    "SessionDataTypeDef",
+_RequiredSessionDataTypeDef = TypedDict(
+    "_RequiredSessionDataTypeDef",
     {
-        "description": str,
-        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
         "name": str,
         "sessionArn": str,
         "sessionId": str,
+    },
+)
+_OptionalSessionDataTypeDef = TypedDict(
+    "_OptionalSessionDataTypeDef",
+    {
+        "description": str,
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-KnowledgeBaseDataTypeDef = TypedDict(
-    "KnowledgeBaseDataTypeDef",
+class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
+    pass
+
+_RequiredKnowledgeBaseDataTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseDataTypeDef",
     {
-        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
-        "lastContentModificationTime": datetime,
         "name": str,
+        "status": KnowledgeBaseStatusType,
+    },
+)
+_OptionalKnowledgeBaseDataTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseDataTypeDef",
+    {
+        "description": str,
+        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationOutputTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-KnowledgeBaseSummaryTypeDef = TypedDict(
-    "KnowledgeBaseSummaryTypeDef",
+class KnowledgeBaseDataTypeDef(
+    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
+):
+    pass
+
+_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseSummaryTypeDef",
     {
-        "description": str,
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
+        "status": KnowledgeBaseStatusType,
+    },
+)
+_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseSummaryTypeDef",
+    {
+        "description": str,
         "renderingConfiguration": RenderingConfigurationOutputTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "status": KnowledgeBaseStatusType,
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
+class KnowledgeBaseSummaryTypeDef(
+    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+):
+    pass
+
 _RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
     },
 )
@@ -988,40 +1080,62 @@
 
 class CreateKnowledgeBaseRequestRequestTypeDef(
     _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
     _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
-AssistantAssociationDataTypeDef = TypedDict(
-    "AssistantAssociationDataTypeDef",
+_RequiredAssistantAssociationDataTypeDef = TypedDict(
+    "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
+    },
+)
+_OptionalAssistantAssociationDataTypeDef = TypedDict(
+    "_OptionalAssistantAssociationDataTypeDef",
+    {
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
-AssistantAssociationSummaryTypeDef = TypedDict(
-    "AssistantAssociationSummaryTypeDef",
+class AssistantAssociationDataTypeDef(
+    _RequiredAssistantAssociationDataTypeDef, _OptionalAssistantAssociationDataTypeDef
+):
+    pass
+
+_RequiredAssistantAssociationSummaryTypeDef = TypedDict(
+    "_RequiredAssistantAssociationSummaryTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
         "associationData": AssistantAssociationOutputDataTypeDef,
         "associationType": Literal["KNOWLEDGE_BASE"],
+    },
+)
+_OptionalAssistantAssociationSummaryTypeDef = TypedDict(
+    "_OptionalAssistantAssociationSummaryTypeDef",
+    {
         "tags": Dict[str, str],
     },
+    total=False,
 )
 
+class AssistantAssociationSummaryTypeDef(
+    _RequiredAssistantAssociationSummaryTypeDef, _OptionalAssistantAssociationSummaryTypeDef
+):
+    pass
+
 CreateAssistantResponseTypeDef = TypedDict(
     "CreateAssistantResponseTypeDef",
     {
         "assistant": AssistantDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1039,23 +1153,32 @@
     {
         "assistantSummaries": List[AssistantSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DocumentTypeDef = TypedDict(
-    "DocumentTypeDef",
+_RequiredDocumentTypeDef = TypedDict(
+    "_RequiredDocumentTypeDef",
     {
         "contentReference": ContentReferenceTypeDef,
+    },
+)
+_OptionalDocumentTypeDef = TypedDict(
+    "_OptionalDocumentTypeDef",
+    {
         "excerpt": DocumentTextTypeDef,
         "title": DocumentTextTypeDef,
     },
+    total=False,
 )
 
+class DocumentTypeDef(_RequiredDocumentTypeDef, _OptionalDocumentTypeDef):
+    pass
+
 _RequiredSearchContentRequestRequestTypeDef = TypedDict(
     "_RequiredSearchContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "searchExpression": SearchExpressionTypeDef,
     },
 )
@@ -1217,33 +1340,53 @@
     {
         "assistantAssociationSummaries": List[AssistantAssociationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RecommendationDataTypeDef = TypedDict(
-    "RecommendationDataTypeDef",
+_RequiredRecommendationDataTypeDef = TypedDict(
+    "_RequiredRecommendationDataTypeDef",
     {
         "document": DocumentTypeDef,
         "recommendationId": str,
+    },
+)
+_OptionalRecommendationDataTypeDef = TypedDict(
+    "_OptionalRecommendationDataTypeDef",
+    {
         "relevanceLevel": RelevanceLevelType,
         "relevanceScore": float,
         "type": Literal["KNOWLEDGE_CONTENT"],
     },
+    total=False,
 )
 
-ResultDataTypeDef = TypedDict(
-    "ResultDataTypeDef",
+class RecommendationDataTypeDef(
+    _RequiredRecommendationDataTypeDef, _OptionalRecommendationDataTypeDef
+):
+    pass
+
+_RequiredResultDataTypeDef = TypedDict(
+    "_RequiredResultDataTypeDef",
     {
         "document": DocumentTypeDef,
-        "relevanceScore": float,
         "resultId": str,
     },
 )
+_OptionalResultDataTypeDef = TypedDict(
+    "_OptionalResultDataTypeDef",
+    {
+        "relevanceScore": float,
+    },
+    total=False,
+)
+
+class ResultDataTypeDef(_RequiredResultDataTypeDef, _OptionalResultDataTypeDef):
+    pass
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "recommendations": List[RecommendationDataTypeDef],
         "triggers": List[RecommendationTriggerTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.11
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-wisdom"></a>
 
 # mypy-boto3-wisdom
 
 [![PyPI - mypy-boto3-wisdom](https://img.shields.io/pypi/v/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-wisdom?color=blue)](https://pypistats.org/packages/mypy-boto3-wisdom)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-wisdom-1.28.11/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.11/setup.py` & `mypy-boto3-wisdom-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectWisdomService 1.28.11 service generated with"
-        " mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

