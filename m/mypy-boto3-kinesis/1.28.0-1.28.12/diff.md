# Comparing `tmp/mypy-boto3-kinesis-1.28.0.tar.gz` & `tmp/mypy-boto3-kinesis-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-1.28.0.tar", last modified: Thu Jul  6 20:59:54 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
```

## Comparing `mypy-boto3-kinesis-1.28.0.tar` & `mypy-boto3-kinesis-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.298343 mypy-boto3-kinesis-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-07-06 20:59:54.298343 mypy-boto3-kinesis-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.294343 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-07-06 20:44:43.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9808 2023-07-06 20:44:43.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-07-06 20:44:44.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-07-06 20:44:43.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:54.298343 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:54.000000 mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:54.298343 mypy-boto3-kinesis-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:44:42.000000 mypy-boto3-kinesis-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24849 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24807 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32120 2023-07-27 05:24:40.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32059 2023-07-27 05:24:40.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16915 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.432469 mypy-boto3-kinesis-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:24:38.000000 mypy-boto3-kinesis-1.28.12/setup.py
```

### Comparing `mypy-boto3-kinesis-1.28.0/LICENSE` & `mypy-boto3-kinesis-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/PKG-INFO` & `mypy-boto3-kinesis-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.0
-Summary: Type annotations for boto3.Kinesis 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,39 +417,40 @@
     ResourceNotFoundExceptionTypeDef,
     ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
+    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
     UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
-    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
+    StreamDescriptionSummaryTypeDef,
+    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
-    ListStreamsOutputTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
+    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.0/README.md` & `mypy-boto3-kinesis-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -385,39 +385,40 @@
     ResourceNotFoundExceptionTypeDef,
     ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
+    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
     UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
-    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
+    StreamDescriptionSummaryTypeDef,
+    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
-    ListStreamsOutputTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
+    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__init__.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__init__.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/__main__.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kinesis 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Kinesis 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis\nOther"
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

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/client.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/client.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/literals.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
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
@@ -277,26 +278,28 @@
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

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/literals.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,15 @@
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
@@ -275,26 +276,28 @@
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

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/paginator.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/paginator.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/type_defs.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     data: AddTagsToStreamInputRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
+from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
 from .literals import (
     ConsumerStatusType,
     EncryptionTypeType,
     MetricsNameType,
     ShardFilterTypeType,
@@ -88,39 +89,40 @@
     "ResourceNotFoundExceptionTypeDef",
     "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
+    "StreamModeDetailsOutputTypeDef",
     "UpdateShardCountInputRequestTypeDef",
     "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "StreamSummaryTypeDef",
     "UpdateStreamModeInputRequestTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
-    "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
     "SubscribeToShardInputRequestTypeDef",
+    "StreamDescriptionSummaryTypeDef",
+    "StreamSummaryTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
-    "ListStreamsOutputTypeDef",
-    "DescribeStreamSummaryOutputTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
+    "DescribeStreamSummaryOutputTypeDef",
+    "ListStreamsOutputTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
 _RequiredAddTagsToStreamInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToStreamInputRequestTypeDef",
@@ -893,14 +895,21 @@
 class StopStreamEncryptionInputRequestTypeDef(
     _RequiredStopStreamEncryptionInputRequestTypeDef,
     _OptionalStopStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
 
+StreamModeDetailsOutputTypeDef = TypedDict(
+    "StreamModeDetailsOutputTypeDef",
+    {
+        "StreamMode": StreamModeType,
+    },
+)
+
 _RequiredUpdateShardCountInputRequestTypeDef = TypedDict(
     "_RequiredUpdateShardCountInputRequestTypeDef",
     {
         "TargetShardCount": int,
         "ScalingType": Literal["UNIFORM_SCALING"],
     },
 )
@@ -983,36 +992,14 @@
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
 
-_RequiredStreamSummaryTypeDef = TypedDict(
-    "_RequiredStreamSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-    },
-)
-_OptionalStreamSummaryTypeDef = TypedDict(
-    "_OptionalStreamSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
-        "StreamCreationTimestamp": datetime,
-    },
-    total=False,
-)
-
-
-class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
-    pass
-
-
 UpdateStreamModeInputRequestTypeDef = TypedDict(
     "UpdateStreamModeInputRequestTypeDef",
     {
         "StreamARN": str,
         "StreamModeDetails": StreamModeDetailsTypeDef,
     },
 )
@@ -1037,44 +1024,14 @@
         "ExclusiveStartShardId": str,
         "StreamARN": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
-    "_RequiredStreamDescriptionSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-        "RetentionPeriodHours": int,
-        "StreamCreationTimestamp": datetime,
-        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
-        "OpenShardCount": int,
-    },
-)
-_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
-    "_OptionalStreamDescriptionSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
-        "EncryptionType": EncryptionTypeType,
-        "KeyId": str,
-        "ConsumerCount": int,
-    },
-    total=False,
-)
-
-
-class StreamDescriptionSummaryTypeDef(
-    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
-):
-    pass
-
-
 ListShardsInputListShardsPaginateTypeDef = TypedDict(
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
@@ -1166,14 +1123,66 @@
     {
         "ConsumerARN": str,
         "ShardId": str,
         "StartingPosition": StartingPositionTypeDef,
     },
 )
 
+_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
+    "_RequiredStreamDescriptionSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+        "RetentionPeriodHours": int,
+        "StreamCreationTimestamp": datetime,
+        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
+        "OpenShardCount": int,
+    },
+)
+_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
+    "_OptionalStreamDescriptionSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "EncryptionType": EncryptionTypeType,
+        "KeyId": str,
+        "ConsumerCount": int,
+    },
+    total=False,
+)
+
+
+class StreamDescriptionSummaryTypeDef(
+    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
+):
+    pass
+
+
+_RequiredStreamSummaryTypeDef = TypedDict(
+    "_RequiredStreamSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+    },
+)
+_OptionalStreamSummaryTypeDef = TypedDict(
+    "_OptionalStreamSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "StreamCreationTimestamp": datetime,
+    },
+    total=False,
+)
+
+
+class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
+    pass
+
+
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
@@ -1200,33 +1209,14 @@
 
 class SubscribeToShardEventTypeDef(
     _RequiredSubscribeToShardEventTypeDef, _OptionalSubscribeToShardEventTypeDef
 ):
     pass
 
 
-ListStreamsOutputTypeDef = TypedDict(
-    "ListStreamsOutputTypeDef",
-    {
-        "StreamNames": List[str],
-        "HasMoreStreams": bool,
-        "NextToken": str,
-        "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStreamSummaryOutputTypeDef = TypedDict(
-    "DescribeStreamSummaryOutputTypeDef",
-    {
-        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1244,28 +1234,47 @@
         "StreamCreationTimestamp": datetime,
         "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
     },
 )
 _OptionalStreamDescriptionTypeDef = TypedDict(
     "_OptionalStreamDescriptionTypeDef",
     {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
     total=False,
 )
 
 
 class StreamDescriptionTypeDef(
     _RequiredStreamDescriptionTypeDef, _OptionalStreamDescriptionTypeDef
 ):
     pass
 
 
+DescribeStreamSummaryOutputTypeDef = TypedDict(
+    "DescribeStreamSummaryOutputTypeDef",
+    {
+        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStreamsOutputTypeDef = TypedDict(
+    "ListStreamsOutputTypeDef",
+    {
+        "StreamNames": List[str],
+        "HasMoreStreams": bool,
+        "NextToken": str,
+        "StreamSummaries": List[StreamSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSubscribeToShardEventStreamTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventStreamTypeDef",
     {
         "SubscribeToShardEvent": SubscribeToShardEventTypeDef,
     },
 )
 _OptionalSubscribeToShardEventStreamTypeDef = TypedDict(
@@ -1298,11 +1307,11 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
-        "EventStream": SubscribeToShardEventStreamTypeDef,
+        "EventStream": "EventStream[SubscribeToShardEventStreamTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/type_defs.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     data: AddTagsToStreamInputRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
+from botocore.eventstream import EventStream
 from botocore.response import StreamingBody
 
 from .literals import (
     ConsumerStatusType,
     EncryptionTypeType,
     MetricsNameType,
     ShardFilterTypeType,
@@ -87,39 +88,40 @@
     "ResourceNotFoundExceptionTypeDef",
     "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
     "SplitShardInputRequestTypeDef",
     "StartStreamEncryptionInputRequestTypeDef",
     "StartingPositionTypeDef",
     "StopStreamEncryptionInputRequestTypeDef",
+    "StreamModeDetailsOutputTypeDef",
     "UpdateShardCountInputRequestTypeDef",
     "UpdateShardCountOutputTypeDef",
     "ChildShardTypeDef",
     "DescribeStreamConsumerOutputTypeDef",
     "ListStreamConsumersOutputTypeDef",
     "RegisterStreamConsumerOutputTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "StreamSummaryTypeDef",
     "UpdateStreamModeInputRequestTypeDef",
     "DescribeStreamInputStreamExistsWaitTypeDef",
     "DescribeStreamInputStreamNotExistsWaitTypeDef",
-    "StreamDescriptionSummaryTypeDef",
     "ListShardsInputListShardsPaginateTypeDef",
     "ListShardsInputRequestTypeDef",
     "ListTagsForStreamOutputTypeDef",
     "PutRecordsInputRequestTypeDef",
     "PutRecordsOutputTypeDef",
     "ShardTypeDef",
     "SubscribeToShardInputRequestTypeDef",
+    "StreamDescriptionSummaryTypeDef",
+    "StreamSummaryTypeDef",
     "GetRecordsOutputTypeDef",
     "SubscribeToShardEventTypeDef",
-    "ListStreamsOutputTypeDef",
-    "DescribeStreamSummaryOutputTypeDef",
     "ListShardsOutputTypeDef",
     "StreamDescriptionTypeDef",
+    "DescribeStreamSummaryOutputTypeDef",
+    "ListStreamsOutputTypeDef",
     "SubscribeToShardEventStreamTypeDef",
     "DescribeStreamOutputTypeDef",
     "SubscribeToShardOutputTypeDef",
 )
 
 _RequiredAddTagsToStreamInputRequestTypeDef = TypedDict(
     "_RequiredAddTagsToStreamInputRequestTypeDef",
@@ -850,14 +852,21 @@
 
 class StopStreamEncryptionInputRequestTypeDef(
     _RequiredStopStreamEncryptionInputRequestTypeDef,
     _OptionalStopStreamEncryptionInputRequestTypeDef,
 ):
     pass
 
+StreamModeDetailsOutputTypeDef = TypedDict(
+    "StreamModeDetailsOutputTypeDef",
+    {
+        "StreamMode": StreamModeType,
+    },
+)
+
 _RequiredUpdateShardCountInputRequestTypeDef = TypedDict(
     "_RequiredUpdateShardCountInputRequestTypeDef",
     {
         "TargetShardCount": int,
         "ScalingType": Literal["UNIFORM_SCALING"],
     },
 )
@@ -936,34 +945,14 @@
 )
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
-_RequiredStreamSummaryTypeDef = TypedDict(
-    "_RequiredStreamSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-    },
-)
-_OptionalStreamSummaryTypeDef = TypedDict(
-    "_OptionalStreamSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
-        "StreamCreationTimestamp": datetime,
-    },
-    total=False,
-)
-
-class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
-    pass
-
 UpdateStreamModeInputRequestTypeDef = TypedDict(
     "UpdateStreamModeInputRequestTypeDef",
     {
         "StreamARN": str,
         "StreamModeDetails": StreamModeDetailsTypeDef,
     },
 )
@@ -988,42 +977,14 @@
         "ExclusiveStartShardId": str,
         "StreamARN": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
-    "_RequiredStreamDescriptionSummaryTypeDef",
-    {
-        "StreamName": str,
-        "StreamARN": str,
-        "StreamStatus": StreamStatusType,
-        "RetentionPeriodHours": int,
-        "StreamCreationTimestamp": datetime,
-        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
-        "OpenShardCount": int,
-    },
-)
-_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
-    "_OptionalStreamDescriptionSummaryTypeDef",
-    {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
-        "EncryptionType": EncryptionTypeType,
-        "KeyId": str,
-        "ConsumerCount": int,
-    },
-    total=False,
-)
-
-class StreamDescriptionSummaryTypeDef(
-    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
-):
-    pass
-
 ListShardsInputListShardsPaginateTypeDef = TypedDict(
     "ListShardsInputListShardsPaginateTypeDef",
     {
         "StreamName": str,
         "ExclusiveStartShardId": str,
         "StreamCreationTimestamp": Union[datetime, str],
         "ShardFilter": ShardFilterTypeDef,
@@ -1111,14 +1072,62 @@
     {
         "ConsumerARN": str,
         "ShardId": str,
         "StartingPosition": StartingPositionTypeDef,
     },
 )
 
+_RequiredStreamDescriptionSummaryTypeDef = TypedDict(
+    "_RequiredStreamDescriptionSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+        "RetentionPeriodHours": int,
+        "StreamCreationTimestamp": datetime,
+        "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
+        "OpenShardCount": int,
+    },
+)
+_OptionalStreamDescriptionSummaryTypeDef = TypedDict(
+    "_OptionalStreamDescriptionSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "EncryptionType": EncryptionTypeType,
+        "KeyId": str,
+        "ConsumerCount": int,
+    },
+    total=False,
+)
+
+class StreamDescriptionSummaryTypeDef(
+    _RequiredStreamDescriptionSummaryTypeDef, _OptionalStreamDescriptionSummaryTypeDef
+):
+    pass
+
+_RequiredStreamSummaryTypeDef = TypedDict(
+    "_RequiredStreamSummaryTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "StreamStatus": StreamStatusType,
+    },
+)
+_OptionalStreamSummaryTypeDef = TypedDict(
+    "_OptionalStreamSummaryTypeDef",
+    {
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
+        "StreamCreationTimestamp": datetime,
+    },
+    total=False,
+)
+
+class StreamSummaryTypeDef(_RequiredStreamSummaryTypeDef, _OptionalStreamSummaryTypeDef):
+    pass
+
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
         "MillisBehindLatest": int,
         "ChildShards": List[ChildShardTypeDef],
@@ -1143,33 +1152,14 @@
 )
 
 class SubscribeToShardEventTypeDef(
     _RequiredSubscribeToShardEventTypeDef, _OptionalSubscribeToShardEventTypeDef
 ):
     pass
 
-ListStreamsOutputTypeDef = TypedDict(
-    "ListStreamsOutputTypeDef",
-    {
-        "StreamNames": List[str],
-        "HasMoreStreams": bool,
-        "NextToken": str,
-        "StreamSummaries": List[StreamSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStreamSummaryOutputTypeDef = TypedDict(
-    "DescribeStreamSummaryOutputTypeDef",
-    {
-        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListShardsOutputTypeDef = TypedDict(
     "ListShardsOutputTypeDef",
     {
         "Shards": List[ShardTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1187,26 +1177,45 @@
         "StreamCreationTimestamp": datetime,
         "EnhancedMonitoring": List[EnhancedMetricsTypeDef],
     },
 )
 _OptionalStreamDescriptionTypeDef = TypedDict(
     "_OptionalStreamDescriptionTypeDef",
     {
-        "StreamModeDetails": StreamModeDetailsTypeDef,
+        "StreamModeDetails": StreamModeDetailsOutputTypeDef,
         "EncryptionType": EncryptionTypeType,
         "KeyId": str,
     },
     total=False,
 )
 
 class StreamDescriptionTypeDef(
     _RequiredStreamDescriptionTypeDef, _OptionalStreamDescriptionTypeDef
 ):
     pass
 
+DescribeStreamSummaryOutputTypeDef = TypedDict(
+    "DescribeStreamSummaryOutputTypeDef",
+    {
+        "StreamDescriptionSummary": StreamDescriptionSummaryTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListStreamsOutputTypeDef = TypedDict(
+    "ListStreamsOutputTypeDef",
+    {
+        "StreamNames": List[str],
+        "HasMoreStreams": bool,
+        "NextToken": str,
+        "StreamSummaries": List[StreamSummaryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredSubscribeToShardEventStreamTypeDef = TypedDict(
     "_RequiredSubscribeToShardEventStreamTypeDef",
     {
         "SubscribeToShardEvent": SubscribeToShardEventTypeDef,
     },
 )
 _OptionalSubscribeToShardEventStreamTypeDef = TypedDict(
@@ -1237,11 +1246,11 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SubscribeToShardOutputTypeDef = TypedDict(
     "SubscribeToShardOutputTypeDef",
     {
-        "EventStream": SubscribeToShardEventStreamTypeDef,
+        "EventStream": "EventStream[SubscribeToShardEventStreamTypeDef]",
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/waiter.py` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis/waiter.pyi` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/PKG-INFO` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis
-Version: 1.28.0
-Summary: Type annotations for boto3.Kinesis 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-kinesis"></a>
 
 # mypy-boto3-kinesis
 
 [![PyPI - mypy-boto3-kinesis](https://img.shields.io/pypi/v/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-kinesis?color=blue)](https://pypistats.org/packages/mypy-boto3-kinesis)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis)](https://pepy.tech/project/mypy-boto3-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kinesis 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[boto3.Kinesis 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [mypy-boto3-kinesis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -417,39 +417,40 @@
     ResourceNotFoundExceptionTypeDef,
     ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
     SplitShardInputRequestTypeDef,
     StartStreamEncryptionInputRequestTypeDef,
     StartingPositionTypeDef,
     StopStreamEncryptionInputRequestTypeDef,
+    StreamModeDetailsOutputTypeDef,
     UpdateShardCountInputRequestTypeDef,
     UpdateShardCountOutputTypeDef,
     ChildShardTypeDef,
     DescribeStreamConsumerOutputTypeDef,
     ListStreamConsumersOutputTypeDef,
     RegisterStreamConsumerOutputTypeDef,
     CreateStreamInputRequestTypeDef,
-    StreamSummaryTypeDef,
     UpdateStreamModeInputRequestTypeDef,
     DescribeStreamInputStreamExistsWaitTypeDef,
     DescribeStreamInputStreamNotExistsWaitTypeDef,
-    StreamDescriptionSummaryTypeDef,
     ListShardsInputListShardsPaginateTypeDef,
     ListShardsInputRequestTypeDef,
     ListTagsForStreamOutputTypeDef,
     PutRecordsInputRequestTypeDef,
     PutRecordsOutputTypeDef,
     ShardTypeDef,
     SubscribeToShardInputRequestTypeDef,
+    StreamDescriptionSummaryTypeDef,
+    StreamSummaryTypeDef,
     GetRecordsOutputTypeDef,
     SubscribeToShardEventTypeDef,
-    ListStreamsOutputTypeDef,
-    DescribeStreamSummaryOutputTypeDef,
     ListShardsOutputTypeDef,
     StreamDescriptionTypeDef,
+    DescribeStreamSummaryOutputTypeDef,
+    ListStreamsOutputTypeDef,
     SubscribeToShardEventStreamTypeDef,
     DescribeStreamOutputTypeDef,
     SubscribeToShardOutputTypeDef,
 )
 
 
 def get_structure() -> AddTagsToStreamInputRequestTypeDef:
```

### Comparing `mypy-boto3-kinesis-1.28.0/mypy_boto3_kinesis.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-1.28.12/mypy_boto3_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-1.28.0/setup.py` & `mypy-boto3-kinesis-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Kinesis 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Kinesis 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

