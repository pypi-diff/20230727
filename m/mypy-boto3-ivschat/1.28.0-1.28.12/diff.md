# Comparing `tmp/mypy-boto3-ivschat-1.28.0.tar.gz` & `tmp/mypy-boto3-ivschat-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivschat-1.28.0.tar", last modified: Thu Jul  6 20:59:51 2023, max compression
+gzip compressed data, was "mypy-boto3-ivschat-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
```

## Comparing `mypy-boto3-ivschat-1.28.0.tar` & `mypy-boto3-ivschat-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.602337 mypy-boto3-ivschat-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-06 20:59:51.602337 mypy-boto3-ivschat-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.598337 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8277 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-07-06 20:44:22.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:51.602337 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:51.000000 mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:51.602337 mypy-boto3-ivschat-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:44:21.000000 mypy-boto3-ivschat-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.752474 mypy-boto3-ivschat-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-27 05:34:51.744475 mypy-boto3-ivschat-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.736474 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-27 05:24:26.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-27 05:24:26.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.744475 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.752474 mypy-boto3-ivschat-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/setup.py
```

### Comparing `mypy-boto3-ivschat-1.28.0/LICENSE` & `mypy-boto3-ivschat-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.0/PKG-INFO` & `mypy-boto3-ivschat-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.28.0
-Summary: Type annotations for boto3.ivschat 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,22 +300,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
+    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
     CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
+    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
+    FirehoseDestinationConfigurationOutputTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -324,32 +328,33 @@
     ListTagsForResourceResponseTypeDef,
     ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
     SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.0/README.md` & `mypy-boto3-ivschat-1.28.12/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,22 +268,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
+    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
     CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
+    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
+    FirehoseDestinationConfigurationOutputTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -292,32 +296,33 @@
     ListTagsForResourceResponseTypeDef,
     ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
     SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/__main__.py` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivschat 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.ivschat 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
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

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/client.py` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/client.pyi` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/literals.py` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
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
@@ -241,26 +242,28 @@
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

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/literals.pyi` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -153,14 +153,15 @@
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
@@ -239,26 +240,28 @@
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

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/type_defs.py` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ivschat service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
+    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationOutputTypeDef
 
-    data: CloudWatchLogsDestinationConfigurationTypeDef = {...}
+    data: CloudWatchLogsDestinationConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ChatTokenCapabilityType, FallbackResultType, LoggingConfigurationStateType
@@ -24,22 +24,26 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
     "CreateChatTokenResponseTypeDef",
     "MessageReviewHandlerTypeDef",
+    "MessageReviewHandlerOutputTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
+    "FirehoseDestinationConfigurationOutputTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
@@ -48,30 +52,38 @@
     "ListTagsForResourceResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
     "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
+    "UpdateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
-    "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "ListRoomsResponseTypeDef",
-    "CreateLoggingConfigurationRequestRequestTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationSummaryTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "CreateLoggingConfigurationRequestRequestTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
 )
 
+CloudWatchLogsDestinationConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+
 CloudWatchLogsDestinationConfigurationTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 
@@ -114,14 +126,23 @@
     {
         "fallbackResult": FallbackResultType,
         "uri": str,
     },
     total=False,
 )
 
+MessageReviewHandlerOutputTypeDef = TypedDict(
+    "MessageReviewHandlerOutputTypeDef",
+    {
+        "fallbackResult": FallbackResultType,
+        "uri": str,
+    },
+    total=False,
+)
+
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -158,14 +179,28 @@
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
+FirehoseDestinationConfigurationOutputTypeDef = TypedDict(
+    "FirehoseDestinationConfigurationOutputTypeDef",
+    {
+        "deliveryStreamName": str,
+    },
+)
+
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 FirehoseDestinationConfigurationTypeDef = TypedDict(
     "FirehoseDestinationConfigurationTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 
@@ -321,24 +356,49 @@
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRoomRequestRequestTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRoomRequestRequestTypeDef",
+    {
+        "loggingConfigurationIdentifiers": Sequence[str],
+        "maximumMessageLength": int,
+        "maximumMessageRatePerSecond": int,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "name": str,
+    },
+    total=False,
+)
+
+
+class UpdateRoomRequestRequestTypeDef(
+    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
+):
+    pass
+
+
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -347,79 +407,64 @@
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRoomRequestRequestTypeDef",
-    {
-        "identifier": str,
-    },
-)
-_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRoomRequestRequestTypeDef",
-    {
-        "loggingConfigurationIdentifiers": Sequence[str],
-        "maximumMessageLength": int,
-        "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
-        "name": str,
-    },
-    total=False,
-)
-
-
-class UpdateRoomRequestRequestTypeDef(
-    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
-):
-    pass
-
-
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "cloudWatchLogs": CloudWatchLogsDestinationConfigurationOutputTypeDef,
+        "firehose": FirehoseDestinationConfigurationOutputTypeDef,
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
         "firehose": FirehoseDestinationConfigurationTypeDef,
         "s3": S3DestinationConfigurationTypeDef,
     },
@@ -431,82 +476,97 @@
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateLoggingConfigurationRequestRequestTypeDef(
-    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
-    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 CreateLoggingConfigurationResponseTypeDef = TypedDict(
     "CreateLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "id": str,
+        "name": str,
+        "state": Literal["ACTIVE"],
+        "tags": Dict[str, str],
+        "updateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateLoggingConfigurationRequestRequestTypeDef(
+    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
+    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
@@ -522,29 +582,14 @@
 class UpdateLoggingConfigurationRequestRequestTypeDef(
     _RequiredUpdateLoggingConfigurationRequestRequestTypeDef,
     _OptionalUpdateLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "arn": str,
-        "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "id": str,
-        "name": str,
-        "state": Literal["ACTIVE"],
-        "tags": Dict[str, str],
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat/type_defs.pyi` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ivschat service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
+    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationOutputTypeDef
 
-    data: CloudWatchLogsDestinationConfigurationTypeDef = {...}
+    data: CloudWatchLogsDestinationConfigurationOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ChatTokenCapabilityType, FallbackResultType, LoggingConfigurationStateType
@@ -23,22 +23,26 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
     "CreateChatTokenResponseTypeDef",
     "MessageReviewHandlerTypeDef",
+    "MessageReviewHandlerOutputTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
+    "FirehoseDestinationConfigurationOutputTypeDef",
+    "S3DestinationConfigurationOutputTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
@@ -47,30 +51,38 @@
     "ListTagsForResourceResponseTypeDef",
     "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
     "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
+    "UpdateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
-    "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
+    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "ListRoomsResponseTypeDef",
-    "CreateLoggingConfigurationRequestRequestTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationSummaryTypeDef",
-    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationResponseTypeDef",
+    "CreateLoggingConfigurationRequestRequestTypeDef",
+    "UpdateLoggingConfigurationRequestRequestTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
 )
 
+CloudWatchLogsDestinationConfigurationOutputTypeDef = TypedDict(
+    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
+    {
+        "logGroupName": str,
+    },
+)
+
 CloudWatchLogsDestinationConfigurationTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 
@@ -111,14 +123,23 @@
     {
         "fallbackResult": FallbackResultType,
         "uri": str,
     },
     total=False,
 )
 
+MessageReviewHandlerOutputTypeDef = TypedDict(
+    "MessageReviewHandlerOutputTypeDef",
+    {
+        "fallbackResult": FallbackResultType,
+        "uri": str,
+    },
+    total=False,
+)
+
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -153,14 +174,28 @@
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
+FirehoseDestinationConfigurationOutputTypeDef = TypedDict(
+    "FirehoseDestinationConfigurationOutputTypeDef",
+    {
+        "deliveryStreamName": str,
+    },
+)
+
+S3DestinationConfigurationOutputTypeDef = TypedDict(
+    "S3DestinationConfigurationOutputTypeDef",
+    {
+        "bucketName": str,
+    },
+)
+
 FirehoseDestinationConfigurationTypeDef = TypedDict(
     "FirehoseDestinationConfigurationTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 
@@ -312,24 +347,47 @@
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRoomRequestRequestTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRoomRequestRequestTypeDef",
+    {
+        "loggingConfigurationIdentifiers": Sequence[str],
+        "maximumMessageLength": int,
+        "maximumMessageRatePerSecond": int,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "name": str,
+    },
+    total=False,
+)
+
+class UpdateRoomRequestRequestTypeDef(
+    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
+):
+    pass
+
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -338,77 +396,64 @@
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRoomRequestRequestTypeDef",
-    {
-        "identifier": str,
-    },
-)
-_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRoomRequestRequestTypeDef",
-    {
-        "loggingConfigurationIdentifiers": Sequence[str],
-        "maximumMessageLength": int,
-        "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
-        "name": str,
-    },
-    total=False,
-)
-
-class UpdateRoomRequestRequestTypeDef(
-    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
-):
-    pass
-
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+DestinationConfigurationOutputTypeDef = TypedDict(
+    "DestinationConfigurationOutputTypeDef",
+    {
+        "cloudWatchLogs": CloudWatchLogsDestinationConfigurationOutputTypeDef,
+        "firehose": FirehoseDestinationConfigurationOutputTypeDef,
+        "s3": S3DestinationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
         "firehose": FirehoseDestinationConfigurationTypeDef,
         "s3": S3DestinationConfigurationTypeDef,
     },
@@ -420,80 +465,95 @@
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateLoggingConfigurationRequestRequestTypeDef(
-    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
-    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
 CreateLoggingConfigurationResponseTypeDef = TypedDict(
     "CreateLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "id": str,
+        "name": str,
+        "state": Literal["ACTIVE"],
+        "tags": Dict[str, str],
+        "updateTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateLoggingConfigurationRequestRequestTypeDef(
+    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
+    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
@@ -507,29 +567,14 @@
 
 class UpdateLoggingConfigurationRequestRequestTypeDef(
     _RequiredUpdateLoggingConfigurationRequestRequestTypeDef,
     _OptionalUpdateLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "arn": str,
-        "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-        "id": str,
-        "name": str,
-        "state": Literal["ACTIVE"],
-        "tags": Dict[str, str],
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/PKG-INFO` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.28.0
-Summary: Type annotations for boto3.ivschat 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ivschat"></a>
 
 # mypy-boto3-ivschat
 
 [![PyPI - mypy-boto3-ivschat](https://img.shields.io/pypi/v/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ivschat?color=blue)](https://pypistats.org/packages/mypy-boto3-ivschat)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,22 +300,26 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
+    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
     CreateChatTokenResponseTypeDef,
     MessageReviewHandlerTypeDef,
+    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
+    FirehoseDestinationConfigurationOutputTypeDef,
+    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
     EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
@@ -324,32 +328,33 @@
     ListTagsForResourceResponseTypeDef,
     ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
     SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
+    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationRequestRequestTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.0/mypy_boto3_ivschat.egg-info/SOURCES.txt` & `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.0/setup.py` & `mypy-boto3-ivschat-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivschat",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ivschat 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

