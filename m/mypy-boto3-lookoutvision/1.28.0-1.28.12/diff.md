# Comparing `tmp/mypy-boto3-lookoutvision-1.28.0.tar.gz` & `tmp/mypy-boto3-lookoutvision-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lookoutvision-1.28.0.tar", last modified: Thu Jul  6 21:00:01 2023, max compression
+gzip compressed data, was "mypy-boto3-lookoutvision-1.28.12.tar", last modified: Thu Jul 27 05:34:58 2023, max compression
```

## Comparing `mypy-boto3-lookoutvision-1.28.0.tar` & `mypy-boto3-lookoutvision-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.606358 mypy-boto3-lookoutvision-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-07-06 21:00:01.602358 mypy-boto3-lookoutvision-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.598358 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26200 2023-07-06 20:46:16.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-06 20:46:15.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:01.602358 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16235 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 21:00:01.000000 mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:01.606358 mypy-boto3-lookoutvision-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-06 20:46:14.000000 mypy-boto3-lookoutvision-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.016452 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28476 2023-07-27 05:25:40.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28429 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16425 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:57.000000 mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:58.020452 mypy-boto3-lookoutvision-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 05:25:39.000000 mypy-boto3-lookoutvision-1.28.12/setup.py
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/LICENSE` & `mypy-boto3-lookoutvision-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutforVision 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutforVision 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,14 +361,17 @@
     DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
+    S3LocationOutputTypeDef,
+    TagOutputTypeDef,
+    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
@@ -390,31 +393,34 @@
     StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
     CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
+    OutputConfigOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
+    ModelPackagingConfigurationOutputTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/README.md` & `mypy-boto3-lookoutvision-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,14 +329,17 @@
     DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
+    S3LocationOutputTypeDef,
+    TagOutputTypeDef,
+    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
@@ -358,31 +361,34 @@
     StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
     CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
+    OutputConfigOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
+    ModelPackagingConfigurationOutputTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__init__.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__init__.pyi` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/__main__.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LookoutforVision 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LookoutforVision 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision\nOther"
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

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/client.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/client.pyi` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/literals.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/literals.pyi` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/literals.pyi`

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

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/paginator.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/paginator.pyi` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/type_defs.py` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
@@ -50,14 +49,17 @@
     "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
+    "S3LocationOutputTypeDef",
+    "TagOutputTypeDef",
+    "TargetPlatformOutputTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
     "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
     "ListDatasetEntriesResponseTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
@@ -79,31 +81,34 @@
     "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
     "CreateDatasetResponseTypeDef",
     "ProjectDescriptionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
+    "OutputConfigOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GreengrassConfigurationOutputTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
+    "ModelPackagingConfigurationOutputTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
@@ -149,21 +154,19 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -192,19 +195,17 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
-
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
-
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -212,21 +213,19 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -234,21 +233,19 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
-
 DeleteModelResponseTypeDef = TypedDict(
     "DeleteModelResponseTypeDef",
     {
         "ModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -263,21 +260,19 @@
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProjectResponseTypeDef = TypedDict(
     "DeleteProjectResponseTypeDef",
     {
         "ProjectArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -327,33 +322,76 @@
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+_RequiredTargetPlatformOutputTypeDef = TypedDict(
+    "_RequiredTargetPlatformOutputTypeDef",
+    {
+        "Os": Literal["LINUX"],
+        "Arch": TargetPlatformArchType,
+    },
+)
+_OptionalTargetPlatformOutputTypeDef = TypedDict(
+    "_OptionalTargetPlatformOutputTypeDef",
+    {
+        "Accelerator": Literal["NVIDIA"],
+    },
+    total=False,
+)
+
+class TargetPlatformOutputTypeDef(
+    _RequiredTargetPlatformOutputTypeDef, _OptionalTargetPlatformOutputTypeDef
+):
+    pass
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3LocationTypeDef = TypedDict(
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
-
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
-
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -361,19 +399,17 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
-
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
-
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
@@ -396,22 +432,20 @@
         "AfterCreationDate": Union[datetime, str],
         "SourceRefContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -425,22 +459,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 ListDatasetEntriesResponseTypeDef = TypedDict(
     "ListDatasetEntriesResponseTypeDef",
     {
         "DatasetEntries": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -456,22 +488,20 @@
     "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
     _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -479,22 +509,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
-
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -517,22 +545,20 @@
     "_OptionalListModelsRequestListModelsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class ListModelsRequestListModelsPaginateTypeDef(
     _RequiredListModelsRequestListModelsPaginateTypeDef,
     _OptionalListModelsRequestListModelsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -540,21 +566,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
-
 ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -635,21 +659,19 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
-
 StartModelResponseTypeDef = TypedDict(
     "StartModelResponseTypeDef",
     {
         "Status": ModelHostingStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -665,21 +687,19 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
-
 StopModelResponseTypeDef = TypedDict(
     "StopModelResponseTypeDef",
     {
         "Status": ModelHostingStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -704,22 +724,20 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateDatasetEntriesResponseTypeDef = TypedDict(
     "UpdateDatasetEntriesResponseTypeDef",
     {
         "Status": DatasetStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -748,22 +766,14 @@
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -803,14 +813,54 @@
     "DatasetGroundTruthManifestTypeDef",
     {
         "S3Object": InputS3ObjectTypeDef,
     },
     total=False,
 )
 
+OutputConfigOutputTypeDef = TypedDict(
+    "OutputConfigOutputTypeDef",
+    {
+        "S3Location": S3LocationOutputTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGreengrassConfigurationOutputTypeDef",
+    {
+        "S3OutputLocation": S3LocationOutputTypeDef,
+        "ComponentName": str,
+    },
+)
+_OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGreengrassConfigurationOutputTypeDef",
+    {
+        "CompilerOptions": str,
+        "TargetDevice": Literal["jetson_xavier"],
+        "TargetPlatform": TargetPlatformOutputTypeDef,
+        "ComponentVersion": str,
+        "ComponentDescription": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+class GreengrassConfigurationOutputTypeDef(
+    _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
+):
+    pass
+
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
@@ -825,26 +875,24 @@
     "_OptionalGreengrassConfigurationTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
         "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
-
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
@@ -904,14 +952,42 @@
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
     },
     total=False,
 )
 
+ModelDescriptionTypeDef = TypedDict(
+    "ModelDescriptionTypeDef",
+    {
+        "ModelVersion": str,
+        "ModelArn": str,
+        "CreationTimestamp": datetime,
+        "Description": str,
+        "Status": ModelStatusType,
+        "StatusMessage": str,
+        "Performance": ModelPerformanceTypeDef,
+        "OutputConfig": OutputConfigOutputTypeDef,
+        "EvaluationManifest": OutputS3ObjectTypeDef,
+        "EvaluationResult": OutputS3ObjectTypeDef,
+        "EvaluationEndTimestamp": datetime,
+        "KmsKeyId": str,
+        "MinInferenceUnits": int,
+        "MaxInferenceUnits": int,
+    },
+    total=False,
+)
+
+ModelPackagingConfigurationOutputTypeDef = TypedDict(
+    "ModelPackagingConfigurationOutputTypeDef",
+    {
+        "Greengrass": GreengrassConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
 )
@@ -922,42 +998,19 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-
-ModelDescriptionTypeDef = TypedDict(
-    "ModelDescriptionTypeDef",
-    {
-        "ModelVersion": str,
-        "ModelArn": str,
-        "CreationTimestamp": datetime,
-        "Description": str,
-        "Status": ModelStatusType,
-        "StatusMessage": str,
-        "Performance": ModelPerformanceTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "EvaluationManifest": OutputS3ObjectTypeDef,
-        "EvaluationResult": OutputS3ObjectTypeDef,
-        "EvaluationEndTimestamp": datetime,
-        "KmsKeyId": str,
-        "MinInferenceUnits": int,
-        "MaxInferenceUnits": int,
-    },
-    total=False,
-)
-
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
 
@@ -998,36 +1051,34 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
-        "ModelPackagingConfiguration": ModelPackagingConfigurationTypeDef,
+        "ModelPackagingConfiguration": ModelPackagingConfigurationOutputTypeDef,
         "ModelPackagingJobDescription": str,
         "ModelPackagingMethod": str,
         "ModelPackagingOutputDetails": ModelPackagingOutputDetailsTypeDef,
         "Status": ModelPackagingJobStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
@@ -1049,22 +1100,20 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision/type_defs.pyi` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "PixelAnomalyTypeDef",
     "DatasetMetadataTypeDef",
     "TagTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectMetadataTypeDef",
     "DatasetImageStatsTypeDef",
@@ -49,14 +50,17 @@
     "DeleteProjectResponseTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeModelPackagingJobRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DetectAnomaliesRequestRequestTypeDef",
     "ImageSourceTypeDef",
+    "S3LocationOutputTypeDef",
+    "TagOutputTypeDef",
+    "TargetPlatformOutputTypeDef",
     "S3LocationTypeDef",
     "TargetPlatformTypeDef",
     "GreengrassOutputDetailsTypeDef",
     "ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef",
     "ListDatasetEntriesRequestRequestTypeDef",
     "ListDatasetEntriesResponseTypeDef",
     "ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
@@ -78,31 +82,34 @@
     "StopModelResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetEntriesRequestRequestTypeDef",
     "UpdateDatasetEntriesResponseTypeDef",
     "AnomalyTypeDef",
     "CreateDatasetResponseTypeDef",
     "ProjectDescriptionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateProjectResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "DatasetDescriptionTypeDef",
     "DatasetGroundTruthManifestTypeDef",
+    "OutputConfigOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GreengrassConfigurationOutputTypeDef",
     "OutputConfigTypeDef",
     "GreengrassConfigurationTypeDef",
     "ModelPackagingOutputDetailsTypeDef",
     "ListModelPackagingJobsResponseTypeDef",
     "ModelMetadataTypeDef",
     "DetectAnomalyResultTypeDef",
     "DescribeProjectResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DatasetSourceTypeDef",
-    "CreateModelRequestRequestTypeDef",
     "ModelDescriptionTypeDef",
+    "ModelPackagingConfigurationOutputTypeDef",
+    "CreateModelRequestRequestTypeDef",
     "ModelPackagingConfigurationTypeDef",
     "CreateModelResponseTypeDef",
     "ListModelsResponseTypeDef",
     "DetectAnomaliesResponseTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
     "ModelPackagingDescriptionTypeDef",
@@ -148,19 +155,21 @@
     "_OptionalCreateProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateProjectRequestRequestTypeDef(
     _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
+
 ProjectMetadataTypeDef = TypedDict(
     "ProjectMetadataTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "CreationTimestamp": datetime,
     },
@@ -189,17 +198,19 @@
     "_OptionalInputS3ObjectTypeDef",
     {
         "VersionId": str,
     },
     total=False,
 )
 
+
 class InputS3ObjectTypeDef(_RequiredInputS3ObjectTypeDef, _OptionalInputS3ObjectTypeDef):
     pass
 
+
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -207,19 +218,21 @@
     "_OptionalDeleteDatasetRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteModelRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "ModelVersion": str,
     },
 )
@@ -227,19 +240,21 @@
     "_OptionalDeleteModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteModelRequestRequestTypeDef(
     _RequiredDeleteModelRequestRequestTypeDef, _OptionalDeleteModelRequestRequestTypeDef
 ):
     pass
 
+
 DeleteModelResponseTypeDef = TypedDict(
     "DeleteModelResponseTypeDef",
     {
         "ModelArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -254,19 +269,21 @@
     "_OptionalDeleteProjectRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class DeleteProjectRequestRequestTypeDef(
     _RequiredDeleteProjectRequestRequestTypeDef, _OptionalDeleteProjectRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProjectResponseTypeDef = TypedDict(
     "DeleteProjectResponseTypeDef",
     {
         "ProjectArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -316,31 +333,82 @@
     "ImageSourceTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
+_RequiredS3LocationOutputTypeDef = TypedDict(
+    "_RequiredS3LocationOutputTypeDef",
+    {
+        "Bucket": str,
+    },
+)
+_OptionalS3LocationOutputTypeDef = TypedDict(
+    "_OptionalS3LocationOutputTypeDef",
+    {
+        "Prefix": str,
+    },
+    total=False,
+)
+
+
+class S3LocationOutputTypeDef(_RequiredS3LocationOutputTypeDef, _OptionalS3LocationOutputTypeDef):
+    pass
+
+
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
+_RequiredTargetPlatformOutputTypeDef = TypedDict(
+    "_RequiredTargetPlatformOutputTypeDef",
+    {
+        "Os": Literal["LINUX"],
+        "Arch": TargetPlatformArchType,
+    },
+)
+_OptionalTargetPlatformOutputTypeDef = TypedDict(
+    "_OptionalTargetPlatformOutputTypeDef",
+    {
+        "Accelerator": Literal["NVIDIA"],
+    },
+    total=False,
+)
+
+
+class TargetPlatformOutputTypeDef(
+    _RequiredTargetPlatformOutputTypeDef, _OptionalTargetPlatformOutputTypeDef
+):
+    pass
+
+
 _RequiredS3LocationTypeDef = TypedDict(
     "_RequiredS3LocationTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3LocationTypeDef = TypedDict(
     "_OptionalS3LocationTypeDef",
     {
         "Prefix": str,
     },
     total=False,
 )
 
+
 class S3LocationTypeDef(_RequiredS3LocationTypeDef, _OptionalS3LocationTypeDef):
     pass
 
+
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": Literal["LINUX"],
         "Arch": TargetPlatformArchType,
     },
 )
@@ -348,17 +416,19 @@
     "_OptionalTargetPlatformTypeDef",
     {
         "Accelerator": Literal["NVIDIA"],
     },
     total=False,
 )
 
+
 class TargetPlatformTypeDef(_RequiredTargetPlatformTypeDef, _OptionalTargetPlatformTypeDef):
     pass
 
+
 GreengrassOutputDetailsTypeDef = TypedDict(
     "GreengrassOutputDetailsTypeDef",
     {
         "ComponentVersionArn": str,
         "ComponentName": str,
         "ComponentVersion": str,
     },
@@ -381,20 +451,22 @@
         "AfterCreationDate": Union[datetime, str],
         "SourceRefContains": str,
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDatasetEntriesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetEntriesRequestRequestTypeDef",
     {
         "ProjectName": str,
         "DatasetType": str,
     },
 )
@@ -408,20 +480,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SourceRefContains": str,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 ListDatasetEntriesResponseTypeDef = TypedDict(
     "ListDatasetEntriesResponseTypeDef",
     {
         "DatasetEntries": List[str],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -437,20 +511,22 @@
     "_OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef(
     _RequiredListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
     _OptionalListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListModelPackagingJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelPackagingJobsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelPackagingJobsRequestRequestTypeDef = TypedDict(
@@ -458,20 +534,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelPackagingJobsRequestRequestTypeDef(
     _RequiredListModelPackagingJobsRequestRequestTypeDef,
     _OptionalListModelPackagingJobsRequestRequestTypeDef,
 ):
     pass
 
+
 ModelPackagingJobMetadataTypeDef = TypedDict(
     "ModelPackagingJobMetadataTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
         "ModelPackagingJobDescription": str,
@@ -494,20 +572,22 @@
     "_OptionalListModelsRequestListModelsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class ListModelsRequestListModelsPaginateTypeDef(
     _RequiredListModelsRequestListModelsPaginateTypeDef,
     _OptionalListModelsRequestListModelsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListModelsRequestRequestTypeDef = TypedDict(
     "_RequiredListModelsRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalListModelsRequestRequestTypeDef = TypedDict(
@@ -515,19 +595,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListModelsRequestRequestTypeDef(
     _RequiredListModelsRequestRequestTypeDef, _OptionalListModelsRequestRequestTypeDef
 ):
     pass
 
+
 ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
     "ListProjectsRequestListProjectsPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
@@ -608,19 +690,21 @@
     {
         "ClientToken": str,
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
+
 class StartModelRequestRequestTypeDef(
     _RequiredStartModelRequestRequestTypeDef, _OptionalStartModelRequestRequestTypeDef
 ):
     pass
 
+
 StartModelResponseTypeDef = TypedDict(
     "StartModelResponseTypeDef",
     {
         "Status": ModelHostingStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -636,19 +720,21 @@
     "_OptionalStopModelRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StopModelRequestRequestTypeDef(
     _RequiredStopModelRequestRequestTypeDef, _OptionalStopModelRequestRequestTypeDef
 ):
     pass
 
+
 StopModelResponseTypeDef = TypedDict(
     "StopModelResponseTypeDef",
     {
         "Status": ModelHostingStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -673,20 +759,22 @@
     "_OptionalUpdateDatasetEntriesRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class UpdateDatasetEntriesRequestRequestTypeDef(
     _RequiredUpdateDatasetEntriesRequestRequestTypeDef,
     _OptionalUpdateDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateDatasetEntriesResponseTypeDef = TypedDict(
     "UpdateDatasetEntriesResponseTypeDef",
     {
         "Status": DatasetStatusType,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -715,22 +803,14 @@
         "ProjectName": str,
         "CreationTimestamp": datetime,
         "Datasets": List[DatasetMetadataTypeDef],
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
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -770,14 +850,56 @@
     "DatasetGroundTruthManifestTypeDef",
     {
         "S3Object": InputS3ObjectTypeDef,
     },
     total=False,
 )
 
+OutputConfigOutputTypeDef = TypedDict(
+    "OutputConfigOutputTypeDef",
+    {
+        "S3Location": S3LocationOutputTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredGreengrassConfigurationOutputTypeDef = TypedDict(
+    "_RequiredGreengrassConfigurationOutputTypeDef",
+    {
+        "S3OutputLocation": S3LocationOutputTypeDef,
+        "ComponentName": str,
+    },
+)
+_OptionalGreengrassConfigurationOutputTypeDef = TypedDict(
+    "_OptionalGreengrassConfigurationOutputTypeDef",
+    {
+        "CompilerOptions": str,
+        "TargetDevice": Literal["jetson_xavier"],
+        "TargetPlatform": TargetPlatformOutputTypeDef,
+        "ComponentVersion": str,
+        "ComponentDescription": str,
+        "Tags": List[TagOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class GreengrassConfigurationOutputTypeDef(
+    _RequiredGreengrassConfigurationOutputTypeDef, _OptionalGreengrassConfigurationOutputTypeDef
+):
+    pass
+
+
 OutputConfigTypeDef = TypedDict(
     "OutputConfigTypeDef",
     {
         "S3Location": S3LocationTypeDef,
     },
 )
 
@@ -792,24 +914,26 @@
     "_OptionalGreengrassConfigurationTypeDef",
     {
         "CompilerOptions": str,
         "TargetDevice": Literal["jetson_xavier"],
         "TargetPlatform": TargetPlatformTypeDef,
         "ComponentVersion": str,
         "ComponentDescription": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class GreengrassConfigurationTypeDef(
     _RequiredGreengrassConfigurationTypeDef, _OptionalGreengrassConfigurationTypeDef
 ):
     pass
 
+
 ModelPackagingOutputDetailsTypeDef = TypedDict(
     "ModelPackagingOutputDetailsTypeDef",
     {
         "Greengrass": GreengrassOutputDetailsTypeDef,
     },
     total=False,
 )
@@ -869,14 +993,42 @@
     "DatasetSourceTypeDef",
     {
         "GroundTruthManifest": DatasetGroundTruthManifestTypeDef,
     },
     total=False,
 )
 
+ModelDescriptionTypeDef = TypedDict(
+    "ModelDescriptionTypeDef",
+    {
+        "ModelVersion": str,
+        "ModelArn": str,
+        "CreationTimestamp": datetime,
+        "Description": str,
+        "Status": ModelStatusType,
+        "StatusMessage": str,
+        "Performance": ModelPerformanceTypeDef,
+        "OutputConfig": OutputConfigOutputTypeDef,
+        "EvaluationManifest": OutputS3ObjectTypeDef,
+        "EvaluationResult": OutputS3ObjectTypeDef,
+        "EvaluationEndTimestamp": datetime,
+        "KmsKeyId": str,
+        "MinInferenceUnits": int,
+        "MaxInferenceUnits": int,
+    },
+    total=False,
+)
+
+ModelPackagingConfigurationOutputTypeDef = TypedDict(
+    "ModelPackagingConfigurationOutputTypeDef",
+    {
+        "Greengrass": GreengrassConfigurationOutputTypeDef,
+    },
+)
+
 _RequiredCreateModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelRequestRequestTypeDef",
     {
         "ProjectName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
 )
@@ -887,39 +1039,20 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-ModelDescriptionTypeDef = TypedDict(
-    "ModelDescriptionTypeDef",
-    {
-        "ModelVersion": str,
-        "ModelArn": str,
-        "CreationTimestamp": datetime,
-        "Description": str,
-        "Status": ModelStatusType,
-        "StatusMessage": str,
-        "Performance": ModelPerformanceTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "EvaluationManifest": OutputS3ObjectTypeDef,
-        "EvaluationResult": OutputS3ObjectTypeDef,
-        "EvaluationEndTimestamp": datetime,
-        "KmsKeyId": str,
-        "MinInferenceUnits": int,
-        "MaxInferenceUnits": int,
-    },
-    total=False,
-)
 
 ModelPackagingConfigurationTypeDef = TypedDict(
     "ModelPackagingConfigurationTypeDef",
     {
         "Greengrass": GreengrassConfigurationTypeDef,
     },
 )
@@ -961,34 +1094,36 @@
     {
         "DatasetSource": DatasetSourceTypeDef,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 DescribeModelResponseTypeDef = TypedDict(
     "DescribeModelResponseTypeDef",
     {
         "ModelDescription": ModelDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModelPackagingDescriptionTypeDef = TypedDict(
     "ModelPackagingDescriptionTypeDef",
     {
         "JobName": str,
         "ProjectName": str,
         "ModelVersion": str,
-        "ModelPackagingConfiguration": ModelPackagingConfigurationTypeDef,
+        "ModelPackagingConfiguration": ModelPackagingConfigurationOutputTypeDef,
         "ModelPackagingJobDescription": str,
         "ModelPackagingMethod": str,
         "ModelPackagingOutputDetails": ModelPackagingOutputDetailsTypeDef,
         "Status": ModelPackagingJobStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
@@ -1010,20 +1145,22 @@
         "JobName": str,
         "Description": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartModelPackagingJobRequestRequestTypeDef(
     _RequiredStartModelPackagingJobRequestRequestTypeDef,
     _OptionalStartModelPackagingJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeModelPackagingJobResponseTypeDef = TypedDict(
     "DescribeModelPackagingJobResponseTypeDef",
     {
         "ModelPackagingDescription": ModelPackagingDescriptionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/PKG-INFO` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lookoutvision
-Version: 1.28.0
-Summary: Type annotations for boto3.LookoutforVision 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LookoutforVision 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lookoutvision"></a>
 
 # mypy-boto3-lookoutvision
 
 [![PyPI - mypy-boto3-lookoutvision](https://img.shields.io/pypi/v/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lookoutvision.svg?color=blue)](https://pypi.org/project/mypy-boto3-lookoutvision)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lookoutvision?color=blue)](https://pypistats.org/packages/mypy-boto3-lookoutvision)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lookoutvision)](https://pepy.tech/project/mypy-boto3-lookoutvision)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LookoutforVision 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
+[boto3.LookoutforVision 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
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
 [mypy-boto3-lookoutvision docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lookoutvision/).
 
 See how it helps to find and fix potential bugs:
 
@@ -361,14 +361,17 @@
     DeleteProjectResponseTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeModelPackagingJobRequestRequestTypeDef,
     DescribeModelRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DetectAnomaliesRequestRequestTypeDef,
     ImageSourceTypeDef,
+    S3LocationOutputTypeDef,
+    TagOutputTypeDef,
+    TargetPlatformOutputTypeDef,
     S3LocationTypeDef,
     TargetPlatformTypeDef,
     GreengrassOutputDetailsTypeDef,
     ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     ListDatasetEntriesRequestRequestTypeDef,
     ListDatasetEntriesResponseTypeDef,
     ListModelPackagingJobsRequestListModelPackagingJobsPaginateTypeDef,
@@ -390,31 +393,34 @@
     StopModelResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetEntriesRequestRequestTypeDef,
     UpdateDatasetEntriesResponseTypeDef,
     AnomalyTypeDef,
     CreateDatasetResponseTypeDef,
     ProjectDescriptionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateProjectResponseTypeDef,
     ListProjectsResponseTypeDef,
     DatasetDescriptionTypeDef,
     DatasetGroundTruthManifestTypeDef,
+    OutputConfigOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GreengrassConfigurationOutputTypeDef,
     OutputConfigTypeDef,
     GreengrassConfigurationTypeDef,
     ModelPackagingOutputDetailsTypeDef,
     ListModelPackagingJobsResponseTypeDef,
     ModelMetadataTypeDef,
     DetectAnomalyResultTypeDef,
     DescribeProjectResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DatasetSourceTypeDef,
-    CreateModelRequestRequestTypeDef,
     ModelDescriptionTypeDef,
+    ModelPackagingConfigurationOutputTypeDef,
+    CreateModelRequestRequestTypeDef,
     ModelPackagingConfigurationTypeDef,
     CreateModelResponseTypeDef,
     ListModelsResponseTypeDef,
     DetectAnomaliesResponseTypeDef,
     CreateDatasetRequestRequestTypeDef,
     DescribeModelResponseTypeDef,
     ModelPackagingDescriptionTypeDef,
```

### Comparing `mypy-boto3-lookoutvision-1.28.0/mypy_boto3_lookoutvision.egg-info/SOURCES.txt` & `mypy-boto3-lookoutvision-1.28.12/mypy_boto3_lookoutvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lookoutvision-1.28.0/setup.py` & `mypy-boto3-lookoutvision-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lookoutvision",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_lookoutvision"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LookoutforVision 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.LookoutforVision 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

