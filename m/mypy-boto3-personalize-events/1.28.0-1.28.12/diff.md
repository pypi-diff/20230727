# Comparing `tmp/mypy-boto3-personalize-events-1.28.0.tar.gz` & `tmp/mypy-boto3-personalize-events-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-personalize-events-1.28.0.tar", last modified: Thu Jul  6 21:00:18 2023, max compression
+gzip compressed data, was "mypy-boto3-personalize-events-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
```

## Comparing `mypy-boto3-personalize-events-1.28.0.tar` & `mypy-boto3-personalize-events-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.306392 mypy-boto3-personalize-events-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-06 21:00:18.302392 mypy-boto3-personalize-events-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.298392 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:18.302392 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-06 21:00:17.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-06 21:00:18.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:17.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:17.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:17.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 21:00:17.000000 mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:18.306392 mypy-boto3-personalize-events-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-06 20:49:12.000000 mypy-boto3-personalize-events-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.789132 mypy-boto3-personalize-events-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-27 11:49:21.789132 mypy-boto3-personalize-events-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11049 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.785132 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.789132 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 11:49:21.000000 mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.789132 mypy-boto3-personalize-events-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 11:41:19.000000 mypy-boto3-personalize-events-1.28.12/setup.py
```

### Comparing `mypy-boto3-personalize-events-1.28.0/LICENSE` & `mypy-boto3-personalize-events-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.0/PKG-INFO` & `mypy-boto3-personalize-events-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.28.0
-Summary: Type annotations for boto3.PersonalizeEvents 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PersonalizeEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,27 +296,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.0/README.md` & `mypy-boto3-personalize-events-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,27 +264,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/__main__.py` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.PersonalizeEvents 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.PersonalizeEvents 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents\nOther"
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

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/client.py` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/client.pyi` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/literals.py` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/literals.py`

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

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/literals.pyi` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/type_defs.py` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,48 @@
 Type annotations for personalize-events service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize_events.type_defs import EmptyResponseMetadataTypeDef
+    from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
 
-    data: EmptyResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
@@ -57,46 +60,38 @@
     "_OptionalItemTypeDef",
     {
         "properties": str,
     },
     total=False,
 )
 
-
 class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
     pass
 
-
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "properties": str,
     },
     total=False,
 )
 
-
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
@@ -113,19 +108,17 @@
         "recommendationId": str,
         "impression": Sequence[str],
         "metricAttribution": MetricAttributionTypeDef,
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
 PutItemsRequestRequestTypeDef = TypedDict(
     "PutItemsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "items": Sequence[ItemTypeDef],
     },
 )
@@ -150,12 +143,11 @@
     "_OptionalPutEventsRequestRequestTypeDef",
     {
         "userId": str,
     },
     total=False,
 )
 
-
 class PutEventsRequestRequestTypeDef(
     _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events/type_defs.pyi` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,44 +2,49 @@
 Type annotations for personalize-events service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_personalize_events.type_defs import EmptyResponseMetadataTypeDef
+    from mypy_boto3_personalize_events.type_defs import ResponseMetadataTypeDef
 
-    data: EmptyResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricAttributionTypeDef",
     "ItemTypeDef",
     "UserTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "PutItemsRequestRequestTypeDef",
     "PutUsersRequestRequestTypeDef",
     "PutEventsRequestRequestTypeDef",
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricAttributionTypeDef = TypedDict(
     "MetricAttributionTypeDef",
     {
         "eventAttributionSource": str,
@@ -56,42 +61,42 @@
     "_OptionalItemTypeDef",
     {
         "properties": str,
     },
     total=False,
 )
 
+
 class ItemTypeDef(_RequiredItemTypeDef, _OptionalItemTypeDef):
     pass
 
+
 _RequiredUserTypeDef = TypedDict(
     "_RequiredUserTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUserTypeDef = TypedDict(
     "_OptionalUserTypeDef",
     {
         "properties": str,
     },
     total=False,
 )
 
+
 class UserTypeDef(_RequiredUserTypeDef, _OptionalUserTypeDef):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventType": str,
@@ -108,17 +113,19 @@
         "recommendationId": str,
         "impression": Sequence[str],
         "metricAttribution": MetricAttributionTypeDef,
     },
     total=False,
 )
 
+
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
+
 PutItemsRequestRequestTypeDef = TypedDict(
     "PutItemsRequestRequestTypeDef",
     {
         "datasetArn": str,
         "items": Sequence[ItemTypeDef],
     },
 )
@@ -143,11 +150,12 @@
     "_OptionalPutEventsRequestRequestTypeDef",
     {
         "userId": str,
     },
     total=False,
 )
 
+
 class PutEventsRequestRequestTypeDef(
     _RequiredPutEventsRequestRequestTypeDef, _OptionalPutEventsRequestRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/PKG-INFO` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-personalize-events
-Version: 1.28.0
-Summary: Type annotations for boto3.PersonalizeEvents 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.PersonalizeEvents 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-personalize-events"></a>
 
 # mypy-boto3-personalize-events
 
 [![PyPI - mypy-boto3-personalize-events](https://img.shields.io/pypi/v/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-personalize-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-personalize-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-personalize-events?color=blue)](https://pypistats.org/packages/mypy-boto3-personalize-events)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-personalize-events)](https://pepy.tech/project/mypy-boto3-personalize-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.PersonalizeEvents 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
+[boto3.PersonalizeEvents 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
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
 [mypy-boto3-personalize-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_personalize_events/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,27 +296,27 @@
 ### Typed dictionaries
 
 `mypy_boto3_personalize_events.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_personalize_events.type_defs import (
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     MetricAttributionTypeDef,
     ItemTypeDef,
     UserTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     PutItemsRequestRequestTypeDef,
     PutUsersRequestRequestTypeDef,
     PutEventsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-personalize-events-1.28.0/mypy_boto3_personalize_events.egg-info/SOURCES.txt` & `mypy-boto3-personalize-events-1.28.12/mypy_boto3_personalize_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-personalize-events-1.28.0/setup.py` & `mypy-boto3-personalize-events-1.28.12/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-personalize-events",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_personalize_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.PersonalizeEvents 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.PersonalizeEvents 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

