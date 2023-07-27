# Comparing `tmp/mypy-boto3-mq-1.28.0.tar.gz` & `tmp/mypy-boto3-mq-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mq-1.28.0.tar", last modified: Thu Jul  6 21:00:11 2023, max compression
+gzip compressed data, was "mypy-boto3-mq-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
```

## Comparing `mypy-boto3-mq-1.28.0.tar` & `mypy-boto3-mq-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.414378 mypy-boto3-mq-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-06 21:00:11.414378 mypy-boto3-mq-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.410378 mypy-boto3-mq-1.28.0/mypy_boto3_mq/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28057 2023-07-06 20:47:57.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28010 2023-07-06 20:47:56.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:11.414378 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14854 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 21:00:11.000000 mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:11.418378 mypy-boto3-mq-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-06 20:47:55.000000 mypy-boto3-mq-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/mypy_boto3_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29695 2023-07-27 05:26:47.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-07-27 05:26:47.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/setup.py
```

### Comparing `mypy-boto3-mq-1.28.0/LICENSE` & `mypy-boto3-mq-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/PKG-INFO` & `mypy-boto3-mq-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.0
-Summary: Type annotations for boto3.MQ 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
+    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
@@ -351,29 +352,32 @@
     DeleteBrokerRequestRequestTypeDef,
     DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
+    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
+    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
+    LogsOutputTypeDef,
     PendingLogsTypeDef,
     PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
     PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.0/README.md` & `mypy-boto3-mq-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,14 +300,15 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
+    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
@@ -319,29 +320,32 @@
     DeleteBrokerRequestRequestTypeDef,
     DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
+    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
+    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
+    LogsOutputTypeDef,
     PendingLogsTypeDef,
     PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
     PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/__init__.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/__init__.pyi` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/__main__.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MQ 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MQ 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
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

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/client.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/client.pyi` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/literals.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,14 +178,15 @@
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
@@ -264,26 +265,28 @@
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

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/literals.pyi` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.pyi`

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

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/paginator.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/paginator.pyi` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/type_defs.py` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 __all__ = (
     "ActionRequiredTypeDef",
     "AvailabilityZoneTypeDef",
     "EngineVersionTypeDef",
     "BrokerInstanceTypeDef",
     "BrokerSummaryTypeDef",
+    "ConfigurationIdOutputTypeDef",
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
@@ -55,29 +56,32 @@
     "DeleteBrokerRequestRequestTypeDef",
     "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
+    "EncryptionOptionsOutputTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
+    "WeeklyStartTimeOutputTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBrokersRequestListBrokersPaginateTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "LogsOutputTypeDef",
     "PendingLogsTypeDef",
     "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
     "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
@@ -161,14 +165,35 @@
 )
 
 
 class BrokerSummaryTypeDef(_RequiredBrokerSummaryTypeDef, _OptionalBrokerSummaryTypeDef):
     pass
 
 
+_RequiredConfigurationIdOutputTypeDef = TypedDict(
+    "_RequiredConfigurationIdOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalConfigurationIdOutputTypeDef = TypedDict(
+    "_OptionalConfigurationIdOutputTypeDef",
+    {
+        "Revision": int,
+    },
+    total=False,
+)
+
+
+class ConfigurationIdOutputTypeDef(
+    _RequiredConfigurationIdOutputTypeDef, _OptionalConfigurationIdOutputTypeDef
+):
+    pass
+
+
 _RequiredConfigurationIdTypeDef = TypedDict(
     "_RequiredConfigurationIdTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigurationIdTypeDef = TypedDict(
@@ -452,14 +477,35 @@
 DescribeBrokerRequestRequestTypeDef = TypedDict(
     "DescribeBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
+_RequiredEncryptionOptionsOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOptionsOutputTypeDef",
+    {
+        "UseAwsOwnedKey": bool,
+    },
+)
+_OptionalEncryptionOptionsOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOptionsOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class EncryptionOptionsOutputTypeDef(
+    _RequiredEncryptionOptionsOutputTypeDef, _OptionalEncryptionOptionsOutputTypeDef
+):
+    pass
+
+
 _RequiredLdapServerMetadataOutputTypeDef = TypedDict(
     "_RequiredLdapServerMetadataOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
         "RoleSearchMatching": str,
         "ServiceAccountUsername": str,
@@ -500,14 +546,36 @@
 )
 
 
 class UserSummaryTypeDef(_RequiredUserSummaryTypeDef, _OptionalUserSummaryTypeDef):
     pass
 
 
+_RequiredWeeklyStartTimeOutputTypeDef = TypedDict(
+    "_RequiredWeeklyStartTimeOutputTypeDef",
+    {
+        "DayOfWeek": DayOfWeekType,
+        "TimeOfDay": str,
+    },
+)
+_OptionalWeeklyStartTimeOutputTypeDef = TypedDict(
+    "_OptionalWeeklyStartTimeOutputTypeDef",
+    {
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+
+class WeeklyStartTimeOutputTypeDef(
+    _RequiredWeeklyStartTimeOutputTypeDef, _OptionalWeeklyStartTimeOutputTypeDef
+):
+    pass
+
+
 DescribeConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationRequestRequestTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 
@@ -649,14 +717,23 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
+LogsOutputTypeDef = TypedDict(
+    "LogsOutputTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+    },
+    total=False,
+)
+
 PendingLogsTypeDef = TypedDict(
     "PendingLogsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
@@ -806,17 +883,17 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
-        "Current": ConfigurationIdTypeDef,
-        "History": List[ConfigurationIdTypeDef],
-        "Pending": ConfigurationIdTypeDef,
+        "Current": ConfigurationIdOutputTypeDef,
+        "History": List[ConfigurationIdOutputTypeDef],
+        "Pending": ConfigurationIdOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
@@ -1067,20 +1144,20 @@
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdTypeDef,
+        "Configuration": ConfigurationIdOutputTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "Logs": LogsOutputTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1096,21 +1173,21 @@
         "BrokerId": str,
         "BrokerInstances": List[BrokerInstanceTypeDef],
         "BrokerName": str,
         "BrokerState": BrokerStateType,
         "Configurations": ConfigurationsTypeDef,
         "Created": datetime,
         "DeploymentMode": DeploymentModeType,
-        "EncryptionOptions": EncryptionOptionsTypeDef,
+        "EncryptionOptions": EncryptionOptionsOutputTypeDef,
         "EngineType": EngineTypeType,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "Logs": LogsSummaryTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
         "PendingAuthenticationStrategy": AuthenticationStrategyType,
         "PendingEngineVersion": str,
         "PendingHostInstanceType": str,
         "PendingLdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
```

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq/type_defs.pyi` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 __all__ = (
     "ActionRequiredTypeDef",
     "AvailabilityZoneTypeDef",
     "EngineVersionTypeDef",
     "BrokerInstanceTypeDef",
     "BrokerSummaryTypeDef",
+    "ConfigurationIdOutputTypeDef",
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
@@ -54,29 +55,32 @@
     "DeleteBrokerRequestRequestTypeDef",
     "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
+    "EncryptionOptionsOutputTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
+    "WeeklyStartTimeOutputTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListBrokersRequestListBrokersPaginateTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
+    "LogsOutputTypeDef",
     "PendingLogsTypeDef",
     "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
     "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
@@ -158,14 +162,33 @@
     },
     total=False,
 )
 
 class BrokerSummaryTypeDef(_RequiredBrokerSummaryTypeDef, _OptionalBrokerSummaryTypeDef):
     pass
 
+_RequiredConfigurationIdOutputTypeDef = TypedDict(
+    "_RequiredConfigurationIdOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalConfigurationIdOutputTypeDef = TypedDict(
+    "_OptionalConfigurationIdOutputTypeDef",
+    {
+        "Revision": int,
+    },
+    total=False,
+)
+
+class ConfigurationIdOutputTypeDef(
+    _RequiredConfigurationIdOutputTypeDef, _OptionalConfigurationIdOutputTypeDef
+):
+    pass
+
 _RequiredConfigurationIdTypeDef = TypedDict(
     "_RequiredConfigurationIdTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigurationIdTypeDef = TypedDict(
@@ -431,14 +454,33 @@
 DescribeBrokerRequestRequestTypeDef = TypedDict(
     "DescribeBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
+_RequiredEncryptionOptionsOutputTypeDef = TypedDict(
+    "_RequiredEncryptionOptionsOutputTypeDef",
+    {
+        "UseAwsOwnedKey": bool,
+    },
+)
+_OptionalEncryptionOptionsOutputTypeDef = TypedDict(
+    "_OptionalEncryptionOptionsOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class EncryptionOptionsOutputTypeDef(
+    _RequiredEncryptionOptionsOutputTypeDef, _OptionalEncryptionOptionsOutputTypeDef
+):
+    pass
+
 _RequiredLdapServerMetadataOutputTypeDef = TypedDict(
     "_RequiredLdapServerMetadataOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
         "RoleSearchMatching": str,
         "ServiceAccountUsername": str,
@@ -475,14 +517,34 @@
     },
     total=False,
 )
 
 class UserSummaryTypeDef(_RequiredUserSummaryTypeDef, _OptionalUserSummaryTypeDef):
     pass
 
+_RequiredWeeklyStartTimeOutputTypeDef = TypedDict(
+    "_RequiredWeeklyStartTimeOutputTypeDef",
+    {
+        "DayOfWeek": DayOfWeekType,
+        "TimeOfDay": str,
+    },
+)
+_OptionalWeeklyStartTimeOutputTypeDef = TypedDict(
+    "_OptionalWeeklyStartTimeOutputTypeDef",
+    {
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+class WeeklyStartTimeOutputTypeDef(
+    _RequiredWeeklyStartTimeOutputTypeDef, _OptionalWeeklyStartTimeOutputTypeDef
+):
+    pass
+
 DescribeConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationRequestRequestTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 
@@ -618,14 +680,23 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+LogsOutputTypeDef = TypedDict(
+    "LogsOutputTypeDef",
+    {
+        "Audit": bool,
+        "General": bool,
+    },
+    total=False,
+)
+
 PendingLogsTypeDef = TypedDict(
     "PendingLogsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
@@ -769,17 +840,17 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
-        "Current": ConfigurationIdTypeDef,
-        "History": List[ConfigurationIdTypeDef],
-        "Pending": ConfigurationIdTypeDef,
+        "Current": ConfigurationIdOutputTypeDef,
+        "History": List[ConfigurationIdOutputTypeDef],
+        "Pending": ConfigurationIdOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
@@ -1020,20 +1091,20 @@
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdTypeDef,
+        "Configuration": ConfigurationIdOutputTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "Logs": LogsOutputTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1049,21 +1120,21 @@
         "BrokerId": str,
         "BrokerInstances": List[BrokerInstanceTypeDef],
         "BrokerName": str,
         "BrokerState": BrokerStateType,
         "Configurations": ConfigurationsTypeDef,
         "Created": datetime,
         "DeploymentMode": DeploymentModeType,
-        "EncryptionOptions": EncryptionOptionsTypeDef,
+        "EncryptionOptions": EncryptionOptionsOutputTypeDef,
         "EngineType": EngineTypeType,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "Logs": LogsSummaryTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
         "PendingAuthenticationStrategy": AuthenticationStrategyType,
         "PendingEngineVersion": str,
         "PendingHostInstanceType": str,
         "PendingLdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
```

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/PKG-INFO` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.0
-Summary: Type annotations for boto3.MQ 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-mq"></a>
 
 # mypy-boto3-mq
 
 [![PyPI - mypy-boto3-mq](https://img.shields.io/pypi/v/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mq?color=blue)](https://pypistats.org/packages/mypy-boto3-mq)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,14 +332,15 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
+    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
@@ -351,29 +352,32 @@
     DeleteBrokerRequestRequestTypeDef,
     DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
+    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
+    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
     DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBrokersRequestListBrokersPaginateTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
     ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
+    LogsOutputTypeDef,
     PendingLogsTypeDef,
     PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
     PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.0/mypy_boto3_mq.egg-info/SOURCES.txt` & `mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.0/setup.py` & `mypy-boto3-mq-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mq",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MQ 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

