# Comparing `tmp/mypy-boto3-sagemaker-geospatial-1.28.0.tar.gz` & `tmp/mypy-boto3-sagemaker-geospatial-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.0.tar", last modified: Thu Jul  6 21:00:32 2023, max compression
+gzip compressed data, was "mypy-boto3-sagemaker-geospatial-1.28.12.tar", last modified: Thu Jul 27 11:49:35 2023, max compression
```

## Comparing `mypy-boto3-sagemaker-geospatial-1.28.0.tar` & `mypy-boto3-sagemaker-geospatial-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.498421 mypy-boto3-sagemaker-geospatial-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-06 21:00:32.494421 mypy-boto3-sagemaker-geospatial-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.486420 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34431 2023-07-06 20:54:53.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-07-06 20:54:52.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:32.494421 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18205 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 21:00:32.000000 mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:32.498421 mypy-boto3-sagemaker-geospatial-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-06 20:54:51.000000 mypy-boto3-sagemaker-geospatial-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.721264 mypy-boto3-sagemaker-geospatial-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18580 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-27 11:45:58.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-07-27 11:45:59.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-07-27 11:45:58.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:35.709264 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19587 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 11:49:35.000000 mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:35.721264 mypy-boto3-sagemaker-geospatial-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-27 11:45:57.000000 mypy-boto3-sagemaker-geospatial-1.28.12/setup.py
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/LICENSE` & `mypy-boto3-sagemaker-geospatial-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.12/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,111 +326,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
+    MultiPolygonGeometryInputOutputTypeDef,
+    PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
+    CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
+    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
+    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
+    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
+    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
+    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
+    GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
-    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
+    TemporalStatisticsConfigInputOutputTypeDef,
+    ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
+    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
+    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
+    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PaginatorConfigTypeDef,
+    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
+    ViewOffNadirInputOutputTypeDef,
+    ViewSunAzimuthInputOutputTypeDef,
+    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
+    CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
+    GetTileOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
+    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
+    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
+    OutputResolutionResamplingInputOutputTypeDef,
+    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
+    PropertyOutputTypeDef,
     PropertyTypeDef,
+    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
+    BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
-    ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportEarthObservationJobInputRequestTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
+    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
+    ResamplingConfigInputOutputTypeDef,
+    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
     StackConfigInputTypeDef,
+    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
+    StartVectorEnrichmentJobInputRequestTypeDef,
+    JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
+    PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
-    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
+    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
-    InputConfigInputTypeDef,
     InputConfigOutputTypeDef,
+    InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
-    StartEarthObservationJobInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
+    StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputTypeDef:
+def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/README.md` & `mypy-boto3-sagemaker-geospatial-1.28.12/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-sagemaker-geospatial
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 sagemaker-geospatial type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,111 +358,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
+    MultiPolygonGeometryInputOutputTypeDef,
+    PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
+    CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
+    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
+    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
+    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
+    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
+    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
+    GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
-    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
+    TemporalStatisticsConfigInputOutputTypeDef,
+    ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
+    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
+    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
+    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PaginatorConfigTypeDef,
+    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
+    ViewOffNadirInputOutputTypeDef,
+    ViewSunAzimuthInputOutputTypeDef,
+    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
+    CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
+    GetTileOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
+    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
+    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
+    OutputResolutionResamplingInputOutputTypeDef,
+    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
+    PropertyOutputTypeDef,
     PropertyTypeDef,
+    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
+    BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
-    ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportEarthObservationJobInputRequestTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
+    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
+    ResamplingConfigInputOutputTypeDef,
+    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
     StackConfigInputTypeDef,
+    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
+    StartVectorEnrichmentJobInputRequestTypeDef,
+    JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
+    PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
-    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
+    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
-    InputConfigInputTypeDef,
     InputConfigOutputTypeDef,
+    InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
-    StartEarthObservationJobInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
+    StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputTypeDef:
+def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__init__.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__init__.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/__main__.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12\nVersion:        "
+        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities\nOther"
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/client.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/client.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/literals.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,15 @@
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
@@ -332,26 +333,28 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/literals.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -244,14 +244,15 @@
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
@@ -330,26 +331,28 @@
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

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/paginator.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,30 +60,30 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
 
 class ListRasterDataCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRasterDataCollectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
         """
 
 
@@ -95,13 +95,13 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/paginator.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -57,29 +57,29 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: EarthObservationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEarthObservationJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listearthobservationjobspaginator)
         """
 
 class ListRasterDataCollectionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRasterDataCollectionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listrasterdatacollectionspaginator)
         """
 
 class ListVectorEnrichmentJobsPaginator(Paginator):
@@ -90,13 +90,13 @@
 
     def paginate(
         self,
         *,
         SortBy: str = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVectorEnrichmentJobOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/paginators/#listvectorenrichmentjobspaginator)
         """
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/type_defs.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sagemaker-geospatial service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
+    from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
 
-    data: MultiPolygonGeometryInputTypeDef = {...}
+    data: MultiPolygonGeometryInputOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -45,143 +45,219 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "MultiPolygonGeometryInputOutputTypeDef",
+    "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
+    "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
+    "OperationOutputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
+    "EoCloudCoverInputOutputTypeDef",
     "EoCloudCoverInputTypeDef",
+    "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
+    "ExportS3DataInputOutputTypeDef",
     "ExportS3DataInputTypeDef",
+    "VectorEnrichmentJobS3DataOutputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
+    "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
-    "GetTileOutputTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
+    "TemporalStatisticsConfigInputOutputTypeDef",
+    "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
+    "LandsatCloudCoverLandInputOutputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
+    "MapMatchingConfigOutputTypeDef",
     "MapMatchingConfigTypeDef",
+    "UserDefinedOutputTypeDef",
     "UserDefinedTypeDef",
-    "PaginatorConfigTypeDef",
+    "PlatformInputOutputTypeDef",
     "PlatformInputTypeDef",
+    "ViewOffNadirInputOutputTypeDef",
+    "ViewSunAzimuthInputOutputTypeDef",
+    "ViewSunElevationInputOutputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "ReverseGeocodingConfigOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
+    "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
+    "GetTileOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
+    "OutputConfigInputOutputTypeDef",
     "OutputConfigInputTypeDef",
+    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
+    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
+    "OutputResolutionResamplingInputOutputTypeDef",
+    "OutputResolutionStackInputOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
+    "PropertyOutputTypeDef",
     "PropertyTypeDef",
+    "VectorEnrichmentJobConfigOutputTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
+    "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
+    "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
-    "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
-    "ExportVectorEnrichmentJobInputRequestTypeDef",
+    "ExportEarthObservationJobInputRequestTypeDef",
     "ExportVectorEnrichmentJobOutputTypeDef",
+    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    "ExportVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
+    "ResamplingConfigInputOutputTypeDef",
+    "StackConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
     "StackConfigInputTypeDef",
+    "PropertyFilterOutputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
-    "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
+    "StartVectorEnrichmentJobInputRequestTypeDef",
+    "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
+    "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
-    "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
+    "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
-    "InputConfigInputTypeDef",
     "InputConfigOutputTypeDef",
+    "InputConfigInputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
-    "StartEarthObservationJobInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
     "StartEarthObservationJobOutputTypeDef",
+    "StartEarthObservationJobInputRequestTypeDef",
+)
+
+MultiPolygonGeometryInputOutputTypeDef = TypedDict(
+    "MultiPolygonGeometryInputOutputTypeDef",
+    {
+        "Coordinates": List[List[List[List[float]]]],
+    },
+)
+
+PolygonGeometryInputOutputTypeDef = TypedDict(
+    "PolygonGeometryInputOutputTypeDef",
+    {
+        "Coordinates": List[List[List[float]]],
+    },
 )
 
 MultiPolygonGeometryInputTypeDef = TypedDict(
     "MultiPolygonGeometryInputTypeDef",
     {
-        "Coordinates": List[List[List[List[float]]]],
+        "Coordinates": Sequence[Sequence[Sequence[Sequence[float]]]],
     },
 )
 
 PolygonGeometryInputTypeDef = TypedDict(
     "PolygonGeometryInputTypeDef",
     {
-        "Coordinates": List[List[List[float]]],
+        "Coordinates": Sequence[Sequence[Sequence[float]]],
     },
 )
 
 AssetValueTypeDef = TypedDict(
     "AssetValueTypeDef",
     {
         "Href": str,
     },
     total=False,
 )
 
+CloudRemovalConfigInputOutputTypeDef = TypedDict(
+    "CloudRemovalConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": Literal["INTERPOLATION"],
+        "InterpolationValue": str,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
 CloudRemovalConfigInputTypeDef = TypedDict(
     "CloudRemovalConfigInputTypeDef",
     {
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
+    },
+    total=False,
+)
+
+_RequiredOperationOutputTypeDef = TypedDict(
+    "_RequiredOperationOutputTypeDef",
+    {
+        "Equation": str,
+        "Name": str,
+    },
+)
+_OptionalOperationOutputTypeDef = TypedDict(
+    "_OptionalOperationOutputTypeDef",
+    {
+        "OutputType": OutputTypeType,
     },
     total=False,
 )
 
+class OperationOutputTypeDef(_RequiredOperationOutputTypeDef, _OptionalOperationOutputTypeDef):
+    pass
+
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
         "Equation": str,
         "Name": str,
     },
 )
@@ -189,19 +265,17 @@
     "_OptionalOperationTypeDef",
     {
         "OutputType": OutputTypeType,
     },
     total=False,
 )
 
-
 class OperationTypeDef(_RequiredOperationTypeDef, _OptionalOperationTypeDef):
     pass
 
-
 DeleteEarthObservationJobInputRequestTypeDef = TypedDict(
     "DeleteEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -217,51 +291,106 @@
     {
         "Message": str,
         "Type": EarthObservationJobErrorTypeType,
     },
     total=False,
 )
 
+EoCloudCoverInputOutputTypeDef = TypedDict(
+    "EoCloudCoverInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
 EoCloudCoverInputTypeDef = TypedDict(
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
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
 ExportErrorDetailsOutputTypeDef = TypedDict(
     "ExportErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
 )
 
+_RequiredExportS3DataInputOutputTypeDef = TypedDict(
+    "_RequiredExportS3DataInputOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalExportS3DataInputOutputTypeDef = TypedDict(
+    "_OptionalExportS3DataInputOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class ExportS3DataInputOutputTypeDef(
+    _RequiredExportS3DataInputOutputTypeDef, _OptionalExportS3DataInputOutputTypeDef
+):
+    pass
+
 _RequiredExportS3DataInputTypeDef = TypedDict(
     "_RequiredExportS3DataInputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalExportS3DataInputTypeDef = TypedDict(
     "_OptionalExportS3DataInputTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class ExportS3DataInputTypeDef(
     _RequiredExportS3DataInputTypeDef, _OptionalExportS3DataInputTypeDef
 ):
     pass
 
+_RequiredVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
+    "_RequiredVectorEnrichmentJobS3DataOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
+    "_OptionalVectorEnrichmentJobS3DataOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class VectorEnrichmentJobS3DataOutputTypeDef(
+    _RequiredVectorEnrichmentJobS3DataOutputTypeDef, _OptionalVectorEnrichmentJobS3DataOutputTypeDef
+):
+    pass
 
 _RequiredVectorEnrichmentJobS3DataTypeDef = TypedDict(
     "_RequiredVectorEnrichmentJobS3DataTypeDef",
     {
         "S3Uri": str,
     },
 )
@@ -269,21 +398,19 @@
     "_OptionalVectorEnrichmentJobS3DataTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class VectorEnrichmentJobS3DataTypeDef(
     _RequiredVectorEnrichmentJobS3DataTypeDef, _OptionalVectorEnrichmentJobS3DataTypeDef
 ):
     pass
 
-
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -292,24 +419,31 @@
     {
         "Maximum": float,
         "Minimum": float,
     },
     total=False,
 )
 
-
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
+GeoMosaicConfigInputOutputTypeDef = TypedDict(
+    "GeoMosaicConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": AlgorithmNameGeoMosaicType,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
 
 GeoMosaicConfigInputTypeDef = TypedDict(
     "GeoMosaicConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
@@ -360,29 +494,19 @@
         "OutputFormat": str,
         "PropertyFilters": str,
         "TimeRangeFilter": str,
     },
     total=False,
 )
 
-
 class GetTileInputRequestTypeDef(
     _RequiredGetTileInputRequestTypeDef, _OptionalGetTileInputRequestTypeDef
 ):
     pass
 
-
-GetTileOutputTypeDef = TypedDict(
-    "GetTileOutputTypeDef",
-    {
-        "BinaryFile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "GetVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -413,74 +537,120 @@
         "ViewOffNadir": float,
         "ViewSunAzimuth": float,
         "ViewSunElevation": float,
     },
     total=False,
 )
 
+_RequiredTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_RequiredTemporalStatisticsConfigInputOutputTypeDef",
+    {
+        "Statistics": List[TemporalStatisticsType],
+    },
+)
+_OptionalTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_OptionalTemporalStatisticsConfigInputOutputTypeDef",
+    {
+        "GroupBy": GroupByType,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
+class TemporalStatisticsConfigInputOutputTypeDef(
+    _RequiredTemporalStatisticsConfigInputOutputTypeDef,
+    _OptionalTemporalStatisticsConfigInputOutputTypeDef,
+):
+    pass
+
+_RequiredZonalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_RequiredZonalStatisticsConfigInputOutputTypeDef",
+    {
+        "Statistics": List[ZonalStatisticsType],
+        "ZoneS3Path": str,
+    },
+)
+_OptionalZonalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_OptionalZonalStatisticsConfigInputOutputTypeDef",
+    {
+        "TargetBands": List[str],
+        "ZoneS3PathKmsKeyId": str,
+    },
+    total=False,
+)
+
+class ZonalStatisticsConfigInputOutputTypeDef(
+    _RequiredZonalStatisticsConfigInputOutputTypeDef,
+    _OptionalZonalStatisticsConfigInputOutputTypeDef,
+):
+    pass
+
 _RequiredTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredTemporalStatisticsConfigInputTypeDef",
     {
-        "Statistics": List[TemporalStatisticsType],
+        "Statistics": Sequence[TemporalStatisticsType],
     },
 )
 _OptionalTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalTemporalStatisticsConfigInputTypeDef",
     {
         "GroupBy": GroupByType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
-
 class TemporalStatisticsConfigInputTypeDef(
     _RequiredTemporalStatisticsConfigInputTypeDef, _OptionalTemporalStatisticsConfigInputTypeDef
 ):
     pass
 
-
 _RequiredZonalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredZonalStatisticsConfigInputTypeDef",
     {
-        "Statistics": List[ZonalStatisticsType],
+        "Statistics": Sequence[ZonalStatisticsType],
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
         "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
-
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
 ):
     pass
 
+LandsatCloudCoverLandInputOutputTypeDef = TypedDict(
+    "LandsatCloudCoverLandInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
 
 LandsatCloudCoverLandInputTypeDef = TypedDict(
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": EarthObservationJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEarthObservationJobInputRequestTypeDef = TypedDict(
     "ListEarthObservationJobInputRequestTypeDef",
     {
@@ -508,30 +678,20 @@
     "_OptionalListEarthObservationJobOutputConfigTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ListEarthObservationJobOutputConfigTypeDef(
     _RequiredListEarthObservationJobOutputConfigTypeDef,
     _OptionalListEarthObservationJobOutputConfigTypeDef,
 ):
     pass
 
-
-ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRasterDataCollectionsInputRequestTypeDef = TypedDict(
     "ListRasterDataCollectionsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -540,33 +700,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "ListVectorEnrichmentJobInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -590,68 +731,115 @@
     "_OptionalListVectorEnrichmentJobOutputConfigTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ListVectorEnrichmentJobOutputConfigTypeDef(
     _RequiredListVectorEnrichmentJobOutputConfigTypeDef,
     _OptionalListVectorEnrichmentJobOutputConfigTypeDef,
 ):
     pass
 
+MapMatchingConfigOutputTypeDef = TypedDict(
+    "MapMatchingConfigOutputTypeDef",
+    {
+        "IdAttributeName": str,
+        "TimestampAttributeName": str,
+        "XAttributeName": str,
+        "YAttributeName": str,
+    },
+)
 
 MapMatchingConfigTypeDef = TypedDict(
     "MapMatchingConfigTypeDef",
     {
         "IdAttributeName": str,
         "TimestampAttributeName": str,
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
 
+UserDefinedOutputTypeDef = TypedDict(
+    "UserDefinedOutputTypeDef",
+    {
+        "Unit": Literal["METERS"],
+        "Value": float,
+    },
+)
+
 UserDefinedTypeDef = TypedDict(
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredPlatformInputOutputTypeDef = TypedDict(
+    "_RequiredPlatformInputOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Value": str,
+    },
+)
+_OptionalPlatformInputOutputTypeDef = TypedDict(
+    "_OptionalPlatformInputOutputTypeDef",
+    {
+        "ComparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
+class PlatformInputOutputTypeDef(
+    _RequiredPlatformInputOutputTypeDef, _OptionalPlatformInputOutputTypeDef
+):
+    pass
+
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
     "_OptionalPlatformInputTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
-
 class PlatformInputTypeDef(_RequiredPlatformInputTypeDef, _OptionalPlatformInputTypeDef):
     pass
 
+ViewOffNadirInputOutputTypeDef = TypedDict(
+    "ViewOffNadirInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
+ViewSunAzimuthInputOutputTypeDef = TypedDict(
+    "ViewSunAzimuthInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
+ViewSunElevationInputOutputTypeDef = TypedDict(
+    "ViewSunElevationInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
 
 ViewOffNadirInputTypeDef = TypedDict(
     "ViewOffNadirInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
@@ -685,22 +873,19 @@
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ReverseGeocodingConfigOutputTypeDef = TypedDict(
+    "ReverseGeocodingConfigOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "XAttributeName": str,
+        "YAttributeName": str,
     },
 )
 
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
@@ -734,47 +919,102 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AreaOfInterestGeometryOutputTypeDef = TypedDict(
+    "AreaOfInterestGeometryOutputTypeDef",
+    {
+        "MultiPolygonGeometry": MultiPolygonGeometryInputOutputTypeDef,
+        "PolygonGeometry": PolygonGeometryInputOutputTypeDef,
+    },
+    total=False,
+)
+
 AreaOfInterestGeometryTypeDef = TypedDict(
     "AreaOfInterestGeometryTypeDef",
     {
         "MultiPolygonGeometry": MultiPolygonGeometryInputTypeDef,
         "PolygonGeometry": PolygonGeometryInputTypeDef,
     },
     total=False,
 )
 
+CustomIndicesInputOutputTypeDef = TypedDict(
+    "CustomIndicesInputOutputTypeDef",
+    {
+        "Operations": List[OperationOutputTypeDef],
+    },
+    total=False,
+)
+
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
-        "Operations": List[OperationTypeDef],
+        "Operations": Sequence[OperationTypeDef],
     },
     total=False,
 )
 
+GetTileOutputTypeDef = TypedDict(
+    "GetTileOutputTypeDef",
+    {
+        "BinaryFile": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ExportErrorDetailsTypeDef = TypedDict(
     "ExportErrorDetailsTypeDef",
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
 )
 
+OutputConfigInputOutputTypeDef = TypedDict(
+    "OutputConfigInputOutputTypeDef",
+    {
+        "S3Data": ExportS3DataInputOutputTypeDef,
+    },
+)
+
 OutputConfigInputTypeDef = TypedDict(
     "OutputConfigInputTypeDef",
     {
         "S3Data": ExportS3DataInputTypeDef,
     },
 )
 
+ExportVectorEnrichmentJobOutputConfigOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
+    {
+        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
+    },
+)
+
+VectorEnrichmentJobDataSourceConfigInputOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
+    {
+        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
+    },
+    total=False,
+)
+
 ExportVectorEnrichmentJobOutputConfigTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     {
         "S3Data": VectorEnrichmentJobS3DataTypeDef,
     },
 )
 
@@ -793,15 +1033,15 @@
         "Description": str,
         "DescriptionPageUrl": str,
         "ImageSourceBands": List[str],
         "Name": str,
         "SupportedFilters": List[FilterTypeDef],
         "Tags": Dict[str, str],
         "Type": DataCollectionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRasterDataCollectionMetadataTypeDef = TypedDict(
     "_RequiredRasterDataCollectionMetadataTypeDef",
     {
         "Arn": str,
@@ -816,21 +1056,19 @@
     {
         "DescriptionPageUrl": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class RasterDataCollectionMetadataTypeDef(
     _RequiredRasterDataCollectionMetadataTypeDef, _OptionalRasterDataCollectionMetadataTypeDef
 ):
     pass
 
-
 _RequiredItemSourceTypeDef = TypedDict(
     "_RequiredItemSourceTypeDef",
     {
         "DateTime": datetime,
         "Geometry": GeometryTypeDef,
         "Id": str,
     },
@@ -840,35 +1078,79 @@
     {
         "Assets": Dict[str, AssetValueTypeDef],
         "Properties": PropertiesTypeDef,
     },
     total=False,
 )
 
-
 class ItemSourceTypeDef(_RequiredItemSourceTypeDef, _OptionalItemSourceTypeDef):
     pass
 
+ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": EarthObservationJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 ListEarthObservationJobOutputTypeDef = TypedDict(
     "ListEarthObservationJobOutputTypeDef",
     {
         "EarthObservationJobSummaries": List[ListEarthObservationJobOutputConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ListVectorEnrichmentJobOutputTypeDef",
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OutputResolutionResamplingInputOutputTypeDef = TypedDict(
+    "OutputResolutionResamplingInputOutputTypeDef",
+    {
+        "UserDefined": UserDefinedOutputTypeDef,
+    },
+)
+
+OutputResolutionStackInputOutputTypeDef = TypedDict(
+    "OutputResolutionStackInputOutputTypeDef",
+    {
+        "Predefined": PredefinedResolutionType,
+        "UserDefined": UserDefinedOutputTypeDef,
     },
+    total=False,
 )
 
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
     },
@@ -879,53 +1161,105 @@
     {
         "Predefined": PredefinedResolutionType,
         "UserDefined": UserDefinedTypeDef,
     },
     total=False,
 )
 
+PropertyOutputTypeDef = TypedDict(
+    "PropertyOutputTypeDef",
+    {
+        "EoCloudCover": EoCloudCoverInputOutputTypeDef,
+        "LandsatCloudCoverLand": LandsatCloudCoverLandInputOutputTypeDef,
+        "Platform": PlatformInputOutputTypeDef,
+        "ViewOffNadir": ViewOffNadirInputOutputTypeDef,
+        "ViewSunAzimuth": ViewSunAzimuthInputOutputTypeDef,
+        "ViewSunElevation": ViewSunElevationInputOutputTypeDef,
+    },
+    total=False,
+)
+
 PropertyTypeDef = TypedDict(
     "PropertyTypeDef",
     {
         "EoCloudCover": EoCloudCoverInputTypeDef,
         "LandsatCloudCoverLand": LandsatCloudCoverLandInputTypeDef,
         "Platform": PlatformInputTypeDef,
         "ViewOffNadir": ViewOffNadirInputTypeDef,
         "ViewSunAzimuth": ViewSunAzimuthInputTypeDef,
         "ViewSunElevation": ViewSunElevationInputTypeDef,
     },
     total=False,
 )
 
+VectorEnrichmentJobConfigOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobConfigOutputTypeDef",
+    {
+        "MapMatchingConfig": MapMatchingConfigOutputTypeDef,
+        "ReverseGeocodingConfig": ReverseGeocodingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 VectorEnrichmentJobConfigTypeDef = TypedDict(
     "VectorEnrichmentJobConfigTypeDef",
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
 )
 
+AreaOfInterestOutputTypeDef = TypedDict(
+    "AreaOfInterestOutputTypeDef",
+    {
+        "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
+    },
+    total=False,
+)
+
 AreaOfInterestTypeDef = TypedDict(
     "AreaOfInterestTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryTypeDef,
     },
     total=False,
 )
 
+BandMathConfigInputOutputTypeDef = TypedDict(
+    "BandMathConfigInputOutputTypeDef",
+    {
+        "CustomIndices": CustomIndicesInputOutputTypeDef,
+        "PredefinedIndices": List[str],
+    },
+    total=False,
+)
+
 BandMathConfigInputTypeDef = TypedDict(
     "BandMathConfigInputTypeDef",
     {
         "CustomIndices": CustomIndicesInputTypeDef,
-        "PredefinedIndices": List[str],
+        "PredefinedIndices": Sequence[str],
     },
     total=False,
 )
 
+ExportEarthObservationJobOutputTypeDef = TypedDict(
+    "ExportEarthObservationJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionRoleArn": str,
+        "ExportSourceImages": bool,
+        "ExportStatus": EarthObservationJobExportStatusType,
+        "OutputConfig": OutputConfigInputOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
@@ -935,32 +1269,37 @@
     {
         "ClientToken": str,
         "ExportSourceImages": bool,
     },
     total=False,
 )
 
-
 class ExportEarthObservationJobInputRequestTypeDef(
     _RequiredExportEarthObservationJobInputRequestTypeDef,
     _OptionalExportEarthObservationJobInputRequestTypeDef,
 ):
     pass
 
-
-ExportEarthObservationJobOutputTypeDef = TypedDict(
-    "ExportEarthObservationJobOutputTypeDef",
+ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
-        "ExportSourceImages": bool,
-        "ExportStatus": EarthObservationJobExportStatusType,
-        "OutputConfig": OutputConfigInputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ExportStatus": VectorEnrichmentJobExportStatusType,
+        "OutputConfig": ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VectorEnrichmentJobInputConfigOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    {
+        "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
+        "DocumentType": Literal["CSV"],
     },
 )
 
 _RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
@@ -972,92 +1311,112 @@
     "_OptionalExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ExportVectorEnrichmentJobInputRequestTypeDef(
     _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
     _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
-
-ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionRoleArn": str,
-        "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
         "DocumentType": Literal["CSV"],
     },
 )
 
 ListRasterDataCollectionsOutputTypeDef = TypedDict(
     "ListRasterDataCollectionsOutputTypeDef",
     {
         "NextToken": str,
         "RasterDataCollectionSummaries": List[RasterDataCollectionMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchRasterDataCollectionOutputTypeDef = TypedDict(
     "SearchRasterDataCollectionOutputTypeDef",
     {
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredResamplingConfigInputOutputTypeDef = TypedDict(
+    "_RequiredResamplingConfigInputOutputTypeDef",
+    {
+        "OutputResolution": OutputResolutionResamplingInputOutputTypeDef,
+    },
+)
+_OptionalResamplingConfigInputOutputTypeDef = TypedDict(
+    "_OptionalResamplingConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": AlgorithmNameResamplingType,
+        "TargetBands": List[str],
     },
+    total=False,
+)
+
+class ResamplingConfigInputOutputTypeDef(
+    _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
+):
+    pass
+
+StackConfigInputOutputTypeDef = TypedDict(
+    "StackConfigInputOutputTypeDef",
+    {
+        "OutputResolution": OutputResolutionStackInputOutputTypeDef,
+        "TargetBands": List[str],
+    },
+    total=False,
 )
 
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
-
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
-
 StackConfigInputTypeDef = TypedDict(
     "StackConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
+PropertyFilterOutputTypeDef = TypedDict(
+    "PropertyFilterOutputTypeDef",
+    {
+        "Property": PropertyOutputTypeDef,
+    },
+)
+
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
         "Property": PropertyTypeDef,
     },
 )
 
@@ -1067,22 +1426,40 @@
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": VectorEnrichmentJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": VectorEnrichmentJobExportErrorDetailsTypeDef,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigTypeDef,
+        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
+        "KmsKeyId": str,
+        "Name": str,
+        "Status": VectorEnrichmentJobStatusType,
+        "Tags": Dict[str, str],
+        "Type": VectorEnrichmentJobTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "StartVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "DurationInSeconds": int,
+        "ExecutionRoleArn": str,
+        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredStartVectorEnrichmentJobInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
@@ -1097,112 +1474,113 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartVectorEnrichmentJobInputRequestTypeDef(
     _RequiredStartVectorEnrichmentJobInputRequestTypeDef,
     _OptionalStartVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
-
-StartVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "StartVectorEnrichmentJobOutputTypeDef",
+JobConfigInputOutputTypeDef = TypedDict(
+    "JobConfigInputOutputTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "DurationInSeconds": int,
-        "ExecutionRoleArn": str,
-        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigTypeDef,
-        "KmsKeyId": str,
-        "Name": str,
-        "Status": VectorEnrichmentJobStatusType,
-        "Tags": Dict[str, str],
-        "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BandMathConfig": BandMathConfigInputOutputTypeDef,
+        "CloudMaskingConfig": Dict[str, Any],
+        "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
+        "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
+        "LandCoverSegmentationConfig": Dict[str, Any],
+        "ResamplingConfig": ResamplingConfigInputOutputTypeDef,
+        "StackConfig": StackConfigInputOutputTypeDef,
+        "TemporalStatisticsConfig": TemporalStatisticsConfigInputOutputTypeDef,
+        "ZonalStatisticsConfig": ZonalStatisticsConfigInputOutputTypeDef,
     },
+    total=False,
 )
 
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
-        "CloudMaskingConfig": Dict[str, Any],
+        "CloudMaskingConfig": Mapping[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputTypeDef,
-        "LandCoverSegmentationConfig": Dict[str, Any],
+        "LandCoverSegmentationConfig": Mapping[str, Any],
         "ResamplingConfig": ResamplingConfigInputTypeDef,
         "StackConfig": StackConfigInputTypeDef,
         "TemporalStatisticsConfig": TemporalStatisticsConfigInputTypeDef,
         "ZonalStatisticsConfig": ZonalStatisticsConfigInputTypeDef,
     },
     total=False,
 )
 
+PropertyFiltersOutputTypeDef = TypedDict(
+    "PropertyFiltersOutputTypeDef",
+    {
+        "LogicalOperator": Literal["AND"],
+        "Properties": List[PropertyFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterTypeDef],
+        "Properties": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryInputTypeDef",
+_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "RasterDataCollectionName": str,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryInputTypeDef",
+_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
-        "AreaOfInterest": AreaOfInterestTypeDef,
-        "PropertyFilters": PropertyFiltersTypeDef,
+        "AreaOfInterest": AreaOfInterestOutputTypeDef,
+        "PropertyFilters": PropertyFiltersOutputTypeDef,
     },
     total=False,
 )
 
-
-class RasterDataCollectionQueryInputTypeDef(
-    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
+class RasterDataCollectionQueryOutputTypeDef(
+    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
 ):
     pass
 
-
-_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryOutputTypeDef",
+_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryInputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryOutputTypeDef",
+_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryInputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
-
-class RasterDataCollectionQueryOutputTypeDef(
-    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
+class RasterDataCollectionQueryInputTypeDef(
+    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
 ):
     pass
 
-
 _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef",
     {
         "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
 _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
@@ -1211,36 +1589,34 @@
         "AreaOfInterest": AreaOfInterestTypeDef,
         "BandFilter": Sequence[str],
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
-
 class RasterDataCollectionQueryWithBandFilterInputTypeDef(
     _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef,
     _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef,
 ):
     pass
 
-
-InputConfigInputTypeDef = TypedDict(
-    "InputConfigInputTypeDef",
+InputConfigOutputTypeDef = TypedDict(
+    "InputConfigOutputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
-InputConfigOutputTypeDef = TypedDict(
-    "InputConfigOutputTypeDef",
+InputConfigInputTypeDef = TypedDict(
+    "InputConfigInputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
     "_RequiredSearchRasterDataCollectionInputRequestTypeDef",
     {
@@ -1252,79 +1628,75 @@
     "_OptionalSearchRasterDataCollectionInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class SearchRasterDataCollectionInputRequestTypeDef(
     _RequiredSearchRasterDataCollectionInputRequestTypeDef,
     _OptionalSearchRasterDataCollectionInputRequestTypeDef,
 ):
     pass
 
-
-_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_RequiredStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-        "InputConfig": InputConfigInputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
-        "Name": str,
-    },
-)
-_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_OptionalStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartEarthObservationJobInputRequestTypeDef(
-    _RequiredStartEarthObservationJobInputRequestTypeDef,
-    _OptionalStartEarthObservationJobInputRequestTypeDef,
-):
-    pass
-
-
 GetEarthObservationJobOutputTypeDef = TypedDict(
     "GetEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": EarthObservationJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": ExportErrorDetailsTypeDef,
         "ExportStatus": EarthObservationJobExportStatusType,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
+        "JobConfig": JobConfigInputOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartEarthObservationJobOutputTypeDef = TypedDict(
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
+        "JobConfig": JobConfigInputOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_RequiredStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+        "InputConfig": InputConfigInputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
+        "Name": str,
+    },
+)
+_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_OptionalStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartEarthObservationJobInputRequestTypeDef(
+    _RequiredStartEarthObservationJobInputRequestTypeDef,
+    _OptionalStartEarthObservationJobInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial/type_defs.pyi` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial/type_defs.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for sagemaker-geospatial service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputTypeDef
+    from mypy_boto3_sagemaker_geospatial.type_defs import MultiPolygonGeometryInputOutputTypeDef
 
-    data: MultiPolygonGeometryInputTypeDef = {...}
+    data: MultiPolygonGeometryInputOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -45,142 +45,222 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "MultiPolygonGeometryInputOutputTypeDef",
+    "PolygonGeometryInputOutputTypeDef",
     "MultiPolygonGeometryInputTypeDef",
     "PolygonGeometryInputTypeDef",
     "AssetValueTypeDef",
+    "CloudRemovalConfigInputOutputTypeDef",
     "CloudRemovalConfigInputTypeDef",
+    "OperationOutputTypeDef",
     "OperationTypeDef",
     "DeleteEarthObservationJobInputRequestTypeDef",
     "DeleteVectorEnrichmentJobInputRequestTypeDef",
     "EarthObservationJobErrorDetailsTypeDef",
+    "EoCloudCoverInputOutputTypeDef",
     "EoCloudCoverInputTypeDef",
+    "ResponseMetadataTypeDef",
     "ExportErrorDetailsOutputTypeDef",
+    "ExportS3DataInputOutputTypeDef",
     "ExportS3DataInputTypeDef",
+    "VectorEnrichmentJobS3DataOutputTypeDef",
     "VectorEnrichmentJobS3DataTypeDef",
     "FilterTypeDef",
+    "GeoMosaicConfigInputOutputTypeDef",
     "GeoMosaicConfigInputTypeDef",
     "GeometryTypeDef",
     "GetEarthObservationJobInputRequestTypeDef",
     "OutputBandTypeDef",
     "GetRasterDataCollectionInputRequestTypeDef",
     "GetTileInputRequestTypeDef",
-    "GetTileOutputTypeDef",
     "GetVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobErrorDetailsTypeDef",
     "VectorEnrichmentJobExportErrorDetailsTypeDef",
     "PropertiesTypeDef",
+    "TemporalStatisticsConfigInputOutputTypeDef",
+    "ZonalStatisticsConfigInputOutputTypeDef",
     "TemporalStatisticsConfigInputTypeDef",
     "ZonalStatisticsConfigInputTypeDef",
+    "LandsatCloudCoverLandInputOutputTypeDef",
     "LandsatCloudCoverLandInputTypeDef",
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEarthObservationJobInputRequestTypeDef",
     "ListEarthObservationJobOutputConfigTypeDef",
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
     "ListRasterDataCollectionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListVectorEnrichmentJobInputRequestTypeDef",
     "ListVectorEnrichmentJobOutputConfigTypeDef",
+    "MapMatchingConfigOutputTypeDef",
     "MapMatchingConfigTypeDef",
+    "UserDefinedOutputTypeDef",
     "UserDefinedTypeDef",
-    "PaginatorConfigTypeDef",
+    "PlatformInputOutputTypeDef",
     "PlatformInputTypeDef",
+    "ViewOffNadirInputOutputTypeDef",
+    "ViewSunAzimuthInputOutputTypeDef",
+    "ViewSunElevationInputOutputTypeDef",
     "ViewOffNadirInputTypeDef",
     "ViewSunAzimuthInputTypeDef",
     "ViewSunElevationInputTypeDef",
     "TimeRangeFilterInputTypeDef",
     "TimeRangeFilterOutputTypeDef",
-    "ResponseMetadataTypeDef",
+    "ReverseGeocodingConfigOutputTypeDef",
     "ReverseGeocodingConfigTypeDef",
     "StopEarthObservationJobInputRequestTypeDef",
     "StopVectorEnrichmentJobInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AreaOfInterestGeometryOutputTypeDef",
     "AreaOfInterestGeometryTypeDef",
+    "CustomIndicesInputOutputTypeDef",
     "CustomIndicesInputTypeDef",
+    "GetTileOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ExportErrorDetailsTypeDef",
+    "OutputConfigInputOutputTypeDef",
     "OutputConfigInputTypeDef",
+    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
+    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     "VectorEnrichmentJobDataSourceConfigInputTypeDef",
     "GetRasterDataCollectionOutputTypeDef",
     "RasterDataCollectionMetadataTypeDef",
     "ItemSourceTypeDef",
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
     "ListEarthObservationJobOutputTypeDef",
     "ListVectorEnrichmentJobOutputTypeDef",
+    "OutputResolutionResamplingInputOutputTypeDef",
+    "OutputResolutionStackInputOutputTypeDef",
     "OutputResolutionResamplingInputTypeDef",
     "OutputResolutionStackInputTypeDef",
+    "PropertyOutputTypeDef",
     "PropertyTypeDef",
+    "VectorEnrichmentJobConfigOutputTypeDef",
     "VectorEnrichmentJobConfigTypeDef",
+    "AreaOfInterestOutputTypeDef",
     "AreaOfInterestTypeDef",
+    "BandMathConfigInputOutputTypeDef",
     "BandMathConfigInputTypeDef",
-    "ExportEarthObservationJobInputRequestTypeDef",
     "ExportEarthObservationJobOutputTypeDef",
-    "ExportVectorEnrichmentJobInputRequestTypeDef",
+    "ExportEarthObservationJobInputRequestTypeDef",
     "ExportVectorEnrichmentJobOutputTypeDef",
+    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    "ExportVectorEnrichmentJobInputRequestTypeDef",
     "VectorEnrichmentJobInputConfigTypeDef",
     "ListRasterDataCollectionsOutputTypeDef",
     "SearchRasterDataCollectionOutputTypeDef",
+    "ResamplingConfigInputOutputTypeDef",
+    "StackConfigInputOutputTypeDef",
     "ResamplingConfigInputTypeDef",
     "StackConfigInputTypeDef",
+    "PropertyFilterOutputTypeDef",
     "PropertyFilterTypeDef",
     "GetVectorEnrichmentJobOutputTypeDef",
-    "StartVectorEnrichmentJobInputRequestTypeDef",
     "StartVectorEnrichmentJobOutputTypeDef",
+    "StartVectorEnrichmentJobInputRequestTypeDef",
+    "JobConfigInputOutputTypeDef",
     "JobConfigInputTypeDef",
+    "PropertyFiltersOutputTypeDef",
     "PropertyFiltersTypeDef",
-    "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryOutputTypeDef",
+    "RasterDataCollectionQueryInputTypeDef",
     "RasterDataCollectionQueryWithBandFilterInputTypeDef",
-    "InputConfigInputTypeDef",
     "InputConfigOutputTypeDef",
+    "InputConfigInputTypeDef",
     "SearchRasterDataCollectionInputRequestTypeDef",
-    "StartEarthObservationJobInputRequestTypeDef",
     "GetEarthObservationJobOutputTypeDef",
     "StartEarthObservationJobOutputTypeDef",
+    "StartEarthObservationJobInputRequestTypeDef",
+)
+
+MultiPolygonGeometryInputOutputTypeDef = TypedDict(
+    "MultiPolygonGeometryInputOutputTypeDef",
+    {
+        "Coordinates": List[List[List[List[float]]]],
+    },
+)
+
+PolygonGeometryInputOutputTypeDef = TypedDict(
+    "PolygonGeometryInputOutputTypeDef",
+    {
+        "Coordinates": List[List[List[float]]],
+    },
 )
 
 MultiPolygonGeometryInputTypeDef = TypedDict(
     "MultiPolygonGeometryInputTypeDef",
     {
-        "Coordinates": List[List[List[List[float]]]],
+        "Coordinates": Sequence[Sequence[Sequence[Sequence[float]]]],
     },
 )
 
 PolygonGeometryInputTypeDef = TypedDict(
     "PolygonGeometryInputTypeDef",
     {
-        "Coordinates": List[List[List[float]]],
+        "Coordinates": Sequence[Sequence[Sequence[float]]],
     },
 )
 
 AssetValueTypeDef = TypedDict(
     "AssetValueTypeDef",
     {
         "Href": str,
     },
     total=False,
 )
 
+CloudRemovalConfigInputOutputTypeDef = TypedDict(
+    "CloudRemovalConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": Literal["INTERPOLATION"],
+        "InterpolationValue": str,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
 CloudRemovalConfigInputTypeDef = TypedDict(
     "CloudRemovalConfigInputTypeDef",
     {
         "AlgorithmName": Literal["INTERPOLATION"],
         "InterpolationValue": str,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
+_RequiredOperationOutputTypeDef = TypedDict(
+    "_RequiredOperationOutputTypeDef",
+    {
+        "Equation": str,
+        "Name": str,
+    },
+)
+_OptionalOperationOutputTypeDef = TypedDict(
+    "_OptionalOperationOutputTypeDef",
+    {
+        "OutputType": OutputTypeType,
+    },
+    total=False,
+)
+
+
+class OperationOutputTypeDef(_RequiredOperationOutputTypeDef, _OptionalOperationOutputTypeDef):
+    pass
+
+
 _RequiredOperationTypeDef = TypedDict(
     "_RequiredOperationTypeDef",
     {
         "Equation": str,
         "Name": str,
     },
 )
@@ -188,17 +268,19 @@
     "_OptionalOperationTypeDef",
     {
         "OutputType": OutputTypeType,
     },
     total=False,
 )
 
+
 class OperationTypeDef(_RequiredOperationTypeDef, _OptionalOperationTypeDef):
     pass
 
+
 DeleteEarthObservationJobInputRequestTypeDef = TypedDict(
     "DeleteEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
@@ -214,69 +296,134 @@
     {
         "Message": str,
         "Type": EarthObservationJobErrorTypeType,
     },
     total=False,
 )
 
+EoCloudCoverInputOutputTypeDef = TypedDict(
+    "EoCloudCoverInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
 EoCloudCoverInputTypeDef = TypedDict(
     "EoCloudCoverInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
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
 ExportErrorDetailsOutputTypeDef = TypedDict(
     "ExportErrorDetailsOutputTypeDef",
     {
         "Message": str,
         "Type": ExportErrorTypeType,
     },
     total=False,
 )
 
+_RequiredExportS3DataInputOutputTypeDef = TypedDict(
+    "_RequiredExportS3DataInputOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalExportS3DataInputOutputTypeDef = TypedDict(
+    "_OptionalExportS3DataInputOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class ExportS3DataInputOutputTypeDef(
+    _RequiredExportS3DataInputOutputTypeDef, _OptionalExportS3DataInputOutputTypeDef
+):
+    pass
+
+
 _RequiredExportS3DataInputTypeDef = TypedDict(
     "_RequiredExportS3DataInputTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalExportS3DataInputTypeDef = TypedDict(
     "_OptionalExportS3DataInputTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class ExportS3DataInputTypeDef(
     _RequiredExportS3DataInputTypeDef, _OptionalExportS3DataInputTypeDef
 ):
     pass
 
+
+_RequiredVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
+    "_RequiredVectorEnrichmentJobS3DataOutputTypeDef",
+    {
+        "S3Uri": str,
+    },
+)
+_OptionalVectorEnrichmentJobS3DataOutputTypeDef = TypedDict(
+    "_OptionalVectorEnrichmentJobS3DataOutputTypeDef",
+    {
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class VectorEnrichmentJobS3DataOutputTypeDef(
+    _RequiredVectorEnrichmentJobS3DataOutputTypeDef, _OptionalVectorEnrichmentJobS3DataOutputTypeDef
+):
+    pass
+
+
 _RequiredVectorEnrichmentJobS3DataTypeDef = TypedDict(
     "_RequiredVectorEnrichmentJobS3DataTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalVectorEnrichmentJobS3DataTypeDef = TypedDict(
     "_OptionalVectorEnrichmentJobS3DataTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class VectorEnrichmentJobS3DataTypeDef(
     _RequiredVectorEnrichmentJobS3DataTypeDef, _OptionalVectorEnrichmentJobS3DataTypeDef
 ):
     pass
 
+
 _RequiredFilterTypeDef = TypedDict(
     "_RequiredFilterTypeDef",
     {
         "Name": str,
         "Type": str,
     },
 )
@@ -285,22 +432,33 @@
     {
         "Maximum": float,
         "Minimum": float,
     },
     total=False,
 )
 
+
 class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
     pass
 
+
+GeoMosaicConfigInputOutputTypeDef = TypedDict(
+    "GeoMosaicConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": AlgorithmNameGeoMosaicType,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
 GeoMosaicConfigInputTypeDef = TypedDict(
     "GeoMosaicConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameGeoMosaicType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
 GeometryTypeDef = TypedDict(
     "GeometryTypeDef",
     {
@@ -351,26 +509,20 @@
         "OutputFormat": str,
         "PropertyFilters": str,
         "TimeRangeFilter": str,
     },
     total=False,
 )
 
+
 class GetTileInputRequestTypeDef(
     _RequiredGetTileInputRequestTypeDef, _OptionalGetTileInputRequestTypeDef
 ):
     pass
 
-GetTileOutputTypeDef = TypedDict(
-    "GetTileOutputTypeDef",
-    {
-        "BinaryFile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "GetVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
@@ -402,70 +554,128 @@
         "ViewOffNadir": float,
         "ViewSunAzimuth": float,
         "ViewSunElevation": float,
     },
     total=False,
 )
 
+_RequiredTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_RequiredTemporalStatisticsConfigInputOutputTypeDef",
+    {
+        "Statistics": List[TemporalStatisticsType],
+    },
+)
+_OptionalTemporalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_OptionalTemporalStatisticsConfigInputOutputTypeDef",
+    {
+        "GroupBy": GroupByType,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
+
+class TemporalStatisticsConfigInputOutputTypeDef(
+    _RequiredTemporalStatisticsConfigInputOutputTypeDef,
+    _OptionalTemporalStatisticsConfigInputOutputTypeDef,
+):
+    pass
+
+
+_RequiredZonalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_RequiredZonalStatisticsConfigInputOutputTypeDef",
+    {
+        "Statistics": List[ZonalStatisticsType],
+        "ZoneS3Path": str,
+    },
+)
+_OptionalZonalStatisticsConfigInputOutputTypeDef = TypedDict(
+    "_OptionalZonalStatisticsConfigInputOutputTypeDef",
+    {
+        "TargetBands": List[str],
+        "ZoneS3PathKmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class ZonalStatisticsConfigInputOutputTypeDef(
+    _RequiredZonalStatisticsConfigInputOutputTypeDef,
+    _OptionalZonalStatisticsConfigInputOutputTypeDef,
+):
+    pass
+
+
 _RequiredTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredTemporalStatisticsConfigInputTypeDef",
     {
-        "Statistics": List[TemporalStatisticsType],
+        "Statistics": Sequence[TemporalStatisticsType],
     },
 )
 _OptionalTemporalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalTemporalStatisticsConfigInputTypeDef",
     {
         "GroupBy": GroupByType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
+
 class TemporalStatisticsConfigInputTypeDef(
     _RequiredTemporalStatisticsConfigInputTypeDef, _OptionalTemporalStatisticsConfigInputTypeDef
 ):
     pass
 
+
 _RequiredZonalStatisticsConfigInputTypeDef = TypedDict(
     "_RequiredZonalStatisticsConfigInputTypeDef",
     {
-        "Statistics": List[ZonalStatisticsType],
+        "Statistics": Sequence[ZonalStatisticsType],
         "ZoneS3Path": str,
     },
 )
 _OptionalZonalStatisticsConfigInputTypeDef = TypedDict(
     "_OptionalZonalStatisticsConfigInputTypeDef",
     {
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
         "ZoneS3PathKmsKeyId": str,
     },
     total=False,
 )
 
+
 class ZonalStatisticsConfigInputTypeDef(
     _RequiredZonalStatisticsConfigInputTypeDef, _OptionalZonalStatisticsConfigInputTypeDef
 ):
     pass
 
+
+LandsatCloudCoverLandInputOutputTypeDef = TypedDict(
+    "LandsatCloudCoverLandInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
 LandsatCloudCoverLandInputTypeDef = TypedDict(
     "LandsatCloudCoverLandInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
 
-ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
-    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": EarthObservationJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListEarthObservationJobInputRequestTypeDef = TypedDict(
     "ListEarthObservationJobInputRequestTypeDef",
     {
@@ -493,27 +703,21 @@
     "_OptionalListEarthObservationJobOutputConfigTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ListEarthObservationJobOutputConfigTypeDef(
     _RequiredListEarthObservationJobOutputConfigTypeDef,
     _OptionalListEarthObservationJobOutputConfigTypeDef,
 ):
     pass
 
-ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
-    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListRasterDataCollectionsInputRequestTypeDef = TypedDict(
     "ListRasterDataCollectionsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
@@ -523,33 +727,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
-    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
-    {
-        "SortBy": str,
-        "SortOrder": SortOrderType,
-        "StatusEquals": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "ListVectorEnrichmentJobInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -573,65 +758,122 @@
     "_OptionalListVectorEnrichmentJobOutputConfigTypeDef",
     {
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ListVectorEnrichmentJobOutputConfigTypeDef(
     _RequiredListVectorEnrichmentJobOutputConfigTypeDef,
     _OptionalListVectorEnrichmentJobOutputConfigTypeDef,
 ):
     pass
 
+
+MapMatchingConfigOutputTypeDef = TypedDict(
+    "MapMatchingConfigOutputTypeDef",
+    {
+        "IdAttributeName": str,
+        "TimestampAttributeName": str,
+        "XAttributeName": str,
+        "YAttributeName": str,
+    },
+)
+
 MapMatchingConfigTypeDef = TypedDict(
     "MapMatchingConfigTypeDef",
     {
         "IdAttributeName": str,
         "TimestampAttributeName": str,
         "XAttributeName": str,
         "YAttributeName": str,
     },
 )
 
+UserDefinedOutputTypeDef = TypedDict(
+    "UserDefinedOutputTypeDef",
+    {
+        "Unit": Literal["METERS"],
+        "Value": float,
+    },
+)
+
 UserDefinedTypeDef = TypedDict(
     "UserDefinedTypeDef",
     {
         "Unit": Literal["METERS"],
         "Value": float,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredPlatformInputOutputTypeDef = TypedDict(
+    "_RequiredPlatformInputOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Value": str,
+    },
+)
+_OptionalPlatformInputOutputTypeDef = TypedDict(
+    "_OptionalPlatformInputOutputTypeDef",
+    {
+        "ComparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
+
+class PlatformInputOutputTypeDef(
+    _RequiredPlatformInputOutputTypeDef, _OptionalPlatformInputOutputTypeDef
+):
+    pass
+
+
 _RequiredPlatformInputTypeDef = TypedDict(
     "_RequiredPlatformInputTypeDef",
     {
         "Value": str,
     },
 )
 _OptionalPlatformInputTypeDef = TypedDict(
     "_OptionalPlatformInputTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
     },
     total=False,
 )
 
+
 class PlatformInputTypeDef(_RequiredPlatformInputTypeDef, _OptionalPlatformInputTypeDef):
     pass
 
+
+ViewOffNadirInputOutputTypeDef = TypedDict(
+    "ViewOffNadirInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
+ViewSunAzimuthInputOutputTypeDef = TypedDict(
+    "ViewSunAzimuthInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
+ViewSunElevationInputOutputTypeDef = TypedDict(
+    "ViewSunElevationInputOutputTypeDef",
+    {
+        "LowerBound": float,
+        "UpperBound": float,
+    },
+)
+
 ViewOffNadirInputTypeDef = TypedDict(
     "ViewOffNadirInputTypeDef",
     {
         "LowerBound": float,
         "UpperBound": float,
     },
 )
@@ -664,22 +906,19 @@
     "TimeRangeFilterOutputTypeDef",
     {
         "EndTime": datetime,
         "StartTime": datetime,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ReverseGeocodingConfigOutputTypeDef = TypedDict(
+    "ReverseGeocodingConfigOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "XAttributeName": str,
+        "YAttributeName": str,
     },
 )
 
 ReverseGeocodingConfigTypeDef = TypedDict(
     "ReverseGeocodingConfigTypeDef",
     {
         "XAttributeName": str,
@@ -713,47 +952,102 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AreaOfInterestGeometryOutputTypeDef = TypedDict(
+    "AreaOfInterestGeometryOutputTypeDef",
+    {
+        "MultiPolygonGeometry": MultiPolygonGeometryInputOutputTypeDef,
+        "PolygonGeometry": PolygonGeometryInputOutputTypeDef,
+    },
+    total=False,
+)
+
 AreaOfInterestGeometryTypeDef = TypedDict(
     "AreaOfInterestGeometryTypeDef",
     {
         "MultiPolygonGeometry": MultiPolygonGeometryInputTypeDef,
         "PolygonGeometry": PolygonGeometryInputTypeDef,
     },
     total=False,
 )
 
+CustomIndicesInputOutputTypeDef = TypedDict(
+    "CustomIndicesInputOutputTypeDef",
+    {
+        "Operations": List[OperationOutputTypeDef],
+    },
+    total=False,
+)
+
 CustomIndicesInputTypeDef = TypedDict(
     "CustomIndicesInputTypeDef",
     {
-        "Operations": List[OperationTypeDef],
+        "Operations": Sequence[OperationTypeDef],
     },
     total=False,
 )
 
+GetTileOutputTypeDef = TypedDict(
+    "GetTileOutputTypeDef",
+    {
+        "BinaryFile": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ExportErrorDetailsTypeDef = TypedDict(
     "ExportErrorDetailsTypeDef",
     {
         "ExportResults": ExportErrorDetailsOutputTypeDef,
         "ExportSourceImages": ExportErrorDetailsOutputTypeDef,
     },
     total=False,
 )
 
+OutputConfigInputOutputTypeDef = TypedDict(
+    "OutputConfigInputOutputTypeDef",
+    {
+        "S3Data": ExportS3DataInputOutputTypeDef,
+    },
+)
+
 OutputConfigInputTypeDef = TypedDict(
     "OutputConfigInputTypeDef",
     {
         "S3Data": ExportS3DataInputTypeDef,
     },
 )
 
+ExportVectorEnrichmentJobOutputConfigOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputConfigOutputTypeDef",
+    {
+        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
+    },
+)
+
+VectorEnrichmentJobDataSourceConfigInputOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobDataSourceConfigInputOutputTypeDef",
+    {
+        "S3Data": VectorEnrichmentJobS3DataOutputTypeDef,
+    },
+    total=False,
+)
+
 ExportVectorEnrichmentJobOutputConfigTypeDef = TypedDict(
     "ExportVectorEnrichmentJobOutputConfigTypeDef",
     {
         "S3Data": VectorEnrichmentJobS3DataTypeDef,
     },
 )
 
@@ -772,15 +1066,15 @@
         "Description": str,
         "DescriptionPageUrl": str,
         "ImageSourceBands": List[str],
         "Name": str,
         "SupportedFilters": List[FilterTypeDef],
         "Tags": Dict[str, str],
         "Type": DataCollectionTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRasterDataCollectionMetadataTypeDef = TypedDict(
     "_RequiredRasterDataCollectionMetadataTypeDef",
     {
         "Arn": str,
@@ -795,19 +1089,21 @@
     {
         "DescriptionPageUrl": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class RasterDataCollectionMetadataTypeDef(
     _RequiredRasterDataCollectionMetadataTypeDef, _OptionalRasterDataCollectionMetadataTypeDef
 ):
     pass
 
+
 _RequiredItemSourceTypeDef = TypedDict(
     "_RequiredItemSourceTypeDef",
     {
         "DateTime": datetime,
         "Geometry": GeometryTypeDef,
         "Id": str,
     },
@@ -817,35 +1113,83 @@
     {
         "Assets": Dict[str, AssetValueTypeDef],
         "Properties": PropertiesTypeDef,
     },
     total=False,
 )
 
+
 class ItemSourceTypeDef(_RequiredItemSourceTypeDef, _OptionalItemSourceTypeDef):
     pass
 
+
+ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef = TypedDict(
+    "ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": EarthObservationJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef = TypedDict(
+    "ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef = TypedDict(
+    "ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef",
+    {
+        "SortBy": str,
+        "SortOrder": SortOrderType,
+        "StatusEquals": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListEarthObservationJobOutputTypeDef = TypedDict(
     "ListEarthObservationJobOutputTypeDef",
     {
         "EarthObservationJobSummaries": List[ListEarthObservationJobOutputConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVectorEnrichmentJobOutputTypeDef = TypedDict(
     "ListVectorEnrichmentJobOutputTypeDef",
     {
         "NextToken": str,
         "VectorEnrichmentJobSummaries": List[ListVectorEnrichmentJobOutputConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+OutputResolutionResamplingInputOutputTypeDef = TypedDict(
+    "OutputResolutionResamplingInputOutputTypeDef",
+    {
+        "UserDefined": UserDefinedOutputTypeDef,
+    },
+)
+
+OutputResolutionStackInputOutputTypeDef = TypedDict(
+    "OutputResolutionStackInputOutputTypeDef",
+    {
+        "Predefined": PredefinedResolutionType,
+        "UserDefined": UserDefinedOutputTypeDef,
+    },
+    total=False,
+)
+
 OutputResolutionResamplingInputTypeDef = TypedDict(
     "OutputResolutionResamplingInputTypeDef",
     {
         "UserDefined": UserDefinedTypeDef,
     },
 )
 
@@ -854,53 +1198,105 @@
     {
         "Predefined": PredefinedResolutionType,
         "UserDefined": UserDefinedTypeDef,
     },
     total=False,
 )
 
+PropertyOutputTypeDef = TypedDict(
+    "PropertyOutputTypeDef",
+    {
+        "EoCloudCover": EoCloudCoverInputOutputTypeDef,
+        "LandsatCloudCoverLand": LandsatCloudCoverLandInputOutputTypeDef,
+        "Platform": PlatformInputOutputTypeDef,
+        "ViewOffNadir": ViewOffNadirInputOutputTypeDef,
+        "ViewSunAzimuth": ViewSunAzimuthInputOutputTypeDef,
+        "ViewSunElevation": ViewSunElevationInputOutputTypeDef,
+    },
+    total=False,
+)
+
 PropertyTypeDef = TypedDict(
     "PropertyTypeDef",
     {
         "EoCloudCover": EoCloudCoverInputTypeDef,
         "LandsatCloudCoverLand": LandsatCloudCoverLandInputTypeDef,
         "Platform": PlatformInputTypeDef,
         "ViewOffNadir": ViewOffNadirInputTypeDef,
         "ViewSunAzimuth": ViewSunAzimuthInputTypeDef,
         "ViewSunElevation": ViewSunElevationInputTypeDef,
     },
     total=False,
 )
 
+VectorEnrichmentJobConfigOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobConfigOutputTypeDef",
+    {
+        "MapMatchingConfig": MapMatchingConfigOutputTypeDef,
+        "ReverseGeocodingConfig": ReverseGeocodingConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 VectorEnrichmentJobConfigTypeDef = TypedDict(
     "VectorEnrichmentJobConfigTypeDef",
     {
         "MapMatchingConfig": MapMatchingConfigTypeDef,
         "ReverseGeocodingConfig": ReverseGeocodingConfigTypeDef,
     },
     total=False,
 )
 
+AreaOfInterestOutputTypeDef = TypedDict(
+    "AreaOfInterestOutputTypeDef",
+    {
+        "AreaOfInterestGeometry": AreaOfInterestGeometryOutputTypeDef,
+    },
+    total=False,
+)
+
 AreaOfInterestTypeDef = TypedDict(
     "AreaOfInterestTypeDef",
     {
         "AreaOfInterestGeometry": AreaOfInterestGeometryTypeDef,
     },
     total=False,
 )
 
+BandMathConfigInputOutputTypeDef = TypedDict(
+    "BandMathConfigInputOutputTypeDef",
+    {
+        "CustomIndices": CustomIndicesInputOutputTypeDef,
+        "PredefinedIndices": List[str],
+    },
+    total=False,
+)
+
 BandMathConfigInputTypeDef = TypedDict(
     "BandMathConfigInputTypeDef",
     {
         "CustomIndices": CustomIndicesInputTypeDef,
-        "PredefinedIndices": List[str],
+        "PredefinedIndices": Sequence[str],
     },
     total=False,
 )
 
+ExportEarthObservationJobOutputTypeDef = TypedDict(
+    "ExportEarthObservationJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionRoleArn": str,
+        "ExportSourceImages": bool,
+        "ExportStatus": EarthObservationJobExportStatusType,
+        "OutputConfig": OutputConfigInputOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredExportEarthObservationJobInputRequestTypeDef = TypedDict(
     "_RequiredExportEarthObservationJobInputRequestTypeDef",
     {
         "Arn": str,
         "ExecutionRoleArn": str,
         "OutputConfig": OutputConfigInputTypeDef,
     },
@@ -910,30 +1306,39 @@
     {
         "ClientToken": str,
         "ExportSourceImages": bool,
     },
     total=False,
 )
 
+
 class ExportEarthObservationJobInputRequestTypeDef(
     _RequiredExportEarthObservationJobInputRequestTypeDef,
     _OptionalExportEarthObservationJobInputRequestTypeDef,
 ):
     pass
 
-ExportEarthObservationJobOutputTypeDef = TypedDict(
-    "ExportEarthObservationJobOutputTypeDef",
+
+ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "ExportVectorEnrichmentJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionRoleArn": str,
-        "ExportSourceImages": bool,
-        "ExportStatus": EarthObservationJobExportStatusType,
-        "OutputConfig": OutputConfigInputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ExportStatus": VectorEnrichmentJobExportStatusType,
+        "OutputConfig": ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VectorEnrichmentJobInputConfigOutputTypeDef = TypedDict(
+    "VectorEnrichmentJobInputConfigOutputTypeDef",
+    {
+        "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
+        "DocumentType": Literal["CSV"],
     },
 )
 
 _RequiredExportVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "Arn": str,
@@ -945,88 +1350,118 @@
     "_OptionalExportVectorEnrichmentJobInputRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ExportVectorEnrichmentJobInputRequestTypeDef(
     _RequiredExportVectorEnrichmentJobInputRequestTypeDef,
     _OptionalExportVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
-ExportVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "ExportVectorEnrichmentJobOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionRoleArn": str,
-        "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "OutputConfig": ExportVectorEnrichmentJobOutputConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 VectorEnrichmentJobInputConfigTypeDef = TypedDict(
     "VectorEnrichmentJobInputConfigTypeDef",
     {
         "DataSourceConfig": VectorEnrichmentJobDataSourceConfigInputTypeDef,
         "DocumentType": Literal["CSV"],
     },
 )
 
 ListRasterDataCollectionsOutputTypeDef = TypedDict(
     "ListRasterDataCollectionsOutputTypeDef",
     {
         "NextToken": str,
         "RasterDataCollectionSummaries": List[RasterDataCollectionMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchRasterDataCollectionOutputTypeDef = TypedDict(
     "SearchRasterDataCollectionOutputTypeDef",
     {
         "ApproximateResultCount": int,
         "Items": List[ItemSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredResamplingConfigInputOutputTypeDef = TypedDict(
+    "_RequiredResamplingConfigInputOutputTypeDef",
+    {
+        "OutputResolution": OutputResolutionResamplingInputOutputTypeDef,
+    },
+)
+_OptionalResamplingConfigInputOutputTypeDef = TypedDict(
+    "_OptionalResamplingConfigInputOutputTypeDef",
+    {
+        "AlgorithmName": AlgorithmNameResamplingType,
+        "TargetBands": List[str],
+    },
+    total=False,
+)
+
+
+class ResamplingConfigInputOutputTypeDef(
+    _RequiredResamplingConfigInputOutputTypeDef, _OptionalResamplingConfigInputOutputTypeDef
+):
+    pass
+
+
+StackConfigInputOutputTypeDef = TypedDict(
+    "StackConfigInputOutputTypeDef",
+    {
+        "OutputResolution": OutputResolutionStackInputOutputTypeDef,
+        "TargetBands": List[str],
     },
+    total=False,
 )
 
 _RequiredResamplingConfigInputTypeDef = TypedDict(
     "_RequiredResamplingConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionResamplingInputTypeDef,
     },
 )
 _OptionalResamplingConfigInputTypeDef = TypedDict(
     "_OptionalResamplingConfigInputTypeDef",
     {
         "AlgorithmName": AlgorithmNameResamplingType,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
+
 class ResamplingConfigInputTypeDef(
     _RequiredResamplingConfigInputTypeDef, _OptionalResamplingConfigInputTypeDef
 ):
     pass
 
+
 StackConfigInputTypeDef = TypedDict(
     "StackConfigInputTypeDef",
     {
         "OutputResolution": OutputResolutionStackInputTypeDef,
-        "TargetBands": List[str],
+        "TargetBands": Sequence[str],
     },
     total=False,
 )
 
+PropertyFilterOutputTypeDef = TypedDict(
+    "PropertyFilterOutputTypeDef",
+    {
+        "Property": PropertyOutputTypeDef,
+    },
+)
+
 PropertyFilterTypeDef = TypedDict(
     "PropertyFilterTypeDef",
     {
         "Property": PropertyTypeDef,
     },
 )
 
@@ -1036,22 +1471,40 @@
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": VectorEnrichmentJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": VectorEnrichmentJobExportErrorDetailsTypeDef,
         "ExportStatus": VectorEnrichmentJobExportStatusType,
-        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigTypeDef,
+        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": VectorEnrichmentJobStatusType,
         "Tags": Dict[str, str],
         "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVectorEnrichmentJobOutputTypeDef = TypedDict(
+    "StartVectorEnrichmentJobOutputTypeDef",
+    {
+        "Arn": str,
+        "CreationTime": datetime,
+        "DurationInSeconds": int,
+        "ExecutionRoleArn": str,
+        "InputConfig": VectorEnrichmentJobInputConfigOutputTypeDef,
+        "JobConfig": VectorEnrichmentJobConfigOutputTypeDef,
+        "KmsKeyId": str,
+        "Name": str,
+        "Status": VectorEnrichmentJobStatusType,
+        "Tags": Dict[str, str],
+        "Type": VectorEnrichmentJobTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartVectorEnrichmentJobInputRequestTypeDef = TypedDict(
     "_RequiredStartVectorEnrichmentJobInputRequestTypeDef",
     {
         "ExecutionRoleArn": str,
@@ -1066,106 +1519,119 @@
         "ClientToken": str,
         "KmsKeyId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartVectorEnrichmentJobInputRequestTypeDef(
     _RequiredStartVectorEnrichmentJobInputRequestTypeDef,
     _OptionalStartVectorEnrichmentJobInputRequestTypeDef,
 ):
     pass
 
-StartVectorEnrichmentJobOutputTypeDef = TypedDict(
-    "StartVectorEnrichmentJobOutputTypeDef",
+
+JobConfigInputOutputTypeDef = TypedDict(
+    "JobConfigInputOutputTypeDef",
     {
-        "Arn": str,
-        "CreationTime": datetime,
-        "DurationInSeconds": int,
-        "ExecutionRoleArn": str,
-        "InputConfig": VectorEnrichmentJobInputConfigTypeDef,
-        "JobConfig": VectorEnrichmentJobConfigTypeDef,
-        "KmsKeyId": str,
-        "Name": str,
-        "Status": VectorEnrichmentJobStatusType,
-        "Tags": Dict[str, str],
-        "Type": VectorEnrichmentJobTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "BandMathConfig": BandMathConfigInputOutputTypeDef,
+        "CloudMaskingConfig": Dict[str, Any],
+        "CloudRemovalConfig": CloudRemovalConfigInputOutputTypeDef,
+        "GeoMosaicConfig": GeoMosaicConfigInputOutputTypeDef,
+        "LandCoverSegmentationConfig": Dict[str, Any],
+        "ResamplingConfig": ResamplingConfigInputOutputTypeDef,
+        "StackConfig": StackConfigInputOutputTypeDef,
+        "TemporalStatisticsConfig": TemporalStatisticsConfigInputOutputTypeDef,
+        "ZonalStatisticsConfig": ZonalStatisticsConfigInputOutputTypeDef,
     },
+    total=False,
 )
 
 JobConfigInputTypeDef = TypedDict(
     "JobConfigInputTypeDef",
     {
         "BandMathConfig": BandMathConfigInputTypeDef,
-        "CloudMaskingConfig": Dict[str, Any],
+        "CloudMaskingConfig": Mapping[str, Any],
         "CloudRemovalConfig": CloudRemovalConfigInputTypeDef,
         "GeoMosaicConfig": GeoMosaicConfigInputTypeDef,
-        "LandCoverSegmentationConfig": Dict[str, Any],
+        "LandCoverSegmentationConfig": Mapping[str, Any],
         "ResamplingConfig": ResamplingConfigInputTypeDef,
         "StackConfig": StackConfigInputTypeDef,
         "TemporalStatisticsConfig": TemporalStatisticsConfigInputTypeDef,
         "ZonalStatisticsConfig": ZonalStatisticsConfigInputTypeDef,
     },
     total=False,
 )
 
+PropertyFiltersOutputTypeDef = TypedDict(
+    "PropertyFiltersOutputTypeDef",
+    {
+        "LogicalOperator": Literal["AND"],
+        "Properties": List[PropertyFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 PropertyFiltersTypeDef = TypedDict(
     "PropertyFiltersTypeDef",
     {
         "LogicalOperator": Literal["AND"],
-        "Properties": List[PropertyFilterTypeDef],
+        "Properties": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryInputTypeDef",
+_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryOutputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
+        "RasterDataCollectionName": str,
+        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryInputTypeDef",
+_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryOutputTypeDef",
     {
-        "AreaOfInterest": AreaOfInterestTypeDef,
-        "PropertyFilters": PropertyFiltersTypeDef,
+        "AreaOfInterest": AreaOfInterestOutputTypeDef,
+        "PropertyFilters": PropertyFiltersOutputTypeDef,
     },
     total=False,
 )
 
-class RasterDataCollectionQueryInputTypeDef(
-    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
+
+class RasterDataCollectionQueryOutputTypeDef(
+    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
 ):
     pass
 
-_RequiredRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_RequiredRasterDataCollectionQueryOutputTypeDef",
+
+_RequiredRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_RequiredRasterDataCollectionQueryInputTypeDef",
     {
         "RasterDataCollectionArn": str,
-        "RasterDataCollectionName": str,
-        "TimeRangeFilter": TimeRangeFilterOutputTypeDef,
+        "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
-_OptionalRasterDataCollectionQueryOutputTypeDef = TypedDict(
-    "_OptionalRasterDataCollectionQueryOutputTypeDef",
+_OptionalRasterDataCollectionQueryInputTypeDef = TypedDict(
+    "_OptionalRasterDataCollectionQueryInputTypeDef",
     {
         "AreaOfInterest": AreaOfInterestTypeDef,
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
-class RasterDataCollectionQueryOutputTypeDef(
-    _RequiredRasterDataCollectionQueryOutputTypeDef, _OptionalRasterDataCollectionQueryOutputTypeDef
+
+class RasterDataCollectionQueryInputTypeDef(
+    _RequiredRasterDataCollectionQueryInputTypeDef, _OptionalRasterDataCollectionQueryInputTypeDef
 ):
     pass
 
+
 _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
     "_RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef",
     {
         "TimeRangeFilter": TimeRangeFilterInputTypeDef,
     },
 )
 _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef = TypedDict(
@@ -1174,34 +1640,36 @@
         "AreaOfInterest": AreaOfInterestTypeDef,
         "BandFilter": Sequence[str],
         "PropertyFilters": PropertyFiltersTypeDef,
     },
     total=False,
 )
 
+
 class RasterDataCollectionQueryWithBandFilterInputTypeDef(
     _RequiredRasterDataCollectionQueryWithBandFilterInputTypeDef,
     _OptionalRasterDataCollectionQueryWithBandFilterInputTypeDef,
 ):
     pass
 
-InputConfigInputTypeDef = TypedDict(
-    "InputConfigInputTypeDef",
+
+InputConfigOutputTypeDef = TypedDict(
+    "InputConfigOutputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
     },
     total=False,
 )
 
-InputConfigOutputTypeDef = TypedDict(
-    "InputConfigOutputTypeDef",
+InputConfigInputTypeDef = TypedDict(
+    "InputConfigInputTypeDef",
     {
         "PreviousEarthObservationJobArn": str,
-        "RasterDataCollectionQuery": RasterDataCollectionQueryOutputTypeDef,
+        "RasterDataCollectionQuery": RasterDataCollectionQueryInputTypeDef,
     },
     total=False,
 )
 
 _RequiredSearchRasterDataCollectionInputRequestTypeDef = TypedDict(
     "_RequiredSearchRasterDataCollectionInputRequestTypeDef",
     {
@@ -1213,75 +1681,78 @@
     "_OptionalSearchRasterDataCollectionInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class SearchRasterDataCollectionInputRequestTypeDef(
     _RequiredSearchRasterDataCollectionInputRequestTypeDef,
     _OptionalSearchRasterDataCollectionInputRequestTypeDef,
 ):
     pass
 
-_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_RequiredStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-        "InputConfig": InputConfigInputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
-        "Name": str,
-    },
-)
-_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
-    "_OptionalStartEarthObservationJobInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "KmsKeyId": str,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartEarthObservationJobInputRequestTypeDef(
-    _RequiredStartEarthObservationJobInputRequestTypeDef,
-    _OptionalStartEarthObservationJobInputRequestTypeDef,
-):
-    pass
 
 GetEarthObservationJobOutputTypeDef = TypedDict(
     "GetEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ErrorDetails": EarthObservationJobErrorDetailsTypeDef,
         "ExecutionRoleArn": str,
         "ExportErrorDetails": ExportErrorDetailsTypeDef,
         "ExportStatus": EarthObservationJobExportStatusType,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
+        "JobConfig": JobConfigInputOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "OutputBands": List[OutputBandTypeDef],
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartEarthObservationJobOutputTypeDef = TypedDict(
     "StartEarthObservationJobOutputTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "DurationInSeconds": int,
         "ExecutionRoleArn": str,
         "InputConfig": InputConfigOutputTypeDef,
-        "JobConfig": JobConfigInputTypeDef,
+        "JobConfig": JobConfigInputOutputTypeDef,
         "KmsKeyId": str,
         "Name": str,
         "Status": EarthObservationJobStatusType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_RequiredStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+        "InputConfig": InputConfigInputTypeDef,
+        "JobConfig": JobConfigInputTypeDef,
+        "Name": str,
+    },
+)
+_OptionalStartEarthObservationJobInputRequestTypeDef = TypedDict(
+    "_OptionalStartEarthObservationJobInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "KmsKeyId": str,
+        "Tags": Mapping[str, str],
     },
+    total=False,
 )
+
+
+class StartEarthObservationJobInputRequestTypeDef(
+    _RequiredStartEarthObservationJobInputRequestTypeDef,
+    _OptionalStartEarthObservationJobInputRequestTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sagemaker-geospatial
-Version: 1.28.0
-Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-sagemaker-geospatial"></a>
 
 # mypy-boto3-sagemaker-geospatial
 
 [![PyPI - mypy-boto3-sagemaker-geospatial](https://img.shields.io/pypi/v/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sagemaker-geospatial.svg?color=blue)](https://pypi.org/project/mypy-boto3-sagemaker-geospatial)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sagemaker-geospatial?color=blue)](https://pypistats.org/packages/mypy-boto3-sagemaker-geospatial)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sagemaker-geospatial)](https://pepy.tech/project/mypy-boto3-sagemaker-geospatial)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SageMakergeospatialcapabilities 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
+[boto3.SageMakergeospatialcapabilities 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
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
 [mypy-boto3-sagemaker-geospatial docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sagemaker_geospatial/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,111 +358,146 @@
 ### Typed dictionaries
 
 `mypy_boto3_sagemaker_geospatial.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sagemaker_geospatial.type_defs import (
+    MultiPolygonGeometryInputOutputTypeDef,
+    PolygonGeometryInputOutputTypeDef,
     MultiPolygonGeometryInputTypeDef,
     PolygonGeometryInputTypeDef,
     AssetValueTypeDef,
+    CloudRemovalConfigInputOutputTypeDef,
     CloudRemovalConfigInputTypeDef,
+    OperationOutputTypeDef,
     OperationTypeDef,
     DeleteEarthObservationJobInputRequestTypeDef,
     DeleteVectorEnrichmentJobInputRequestTypeDef,
     EarthObservationJobErrorDetailsTypeDef,
+    EoCloudCoverInputOutputTypeDef,
     EoCloudCoverInputTypeDef,
+    ResponseMetadataTypeDef,
     ExportErrorDetailsOutputTypeDef,
+    ExportS3DataInputOutputTypeDef,
     ExportS3DataInputTypeDef,
+    VectorEnrichmentJobS3DataOutputTypeDef,
     VectorEnrichmentJobS3DataTypeDef,
     FilterTypeDef,
+    GeoMosaicConfigInputOutputTypeDef,
     GeoMosaicConfigInputTypeDef,
     GeometryTypeDef,
     GetEarthObservationJobInputRequestTypeDef,
     OutputBandTypeDef,
     GetRasterDataCollectionInputRequestTypeDef,
     GetTileInputRequestTypeDef,
-    GetTileOutputTypeDef,
     GetVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobErrorDetailsTypeDef,
     VectorEnrichmentJobExportErrorDetailsTypeDef,
     PropertiesTypeDef,
+    TemporalStatisticsConfigInputOutputTypeDef,
+    ZonalStatisticsConfigInputOutputTypeDef,
     TemporalStatisticsConfigInputTypeDef,
     ZonalStatisticsConfigInputTypeDef,
+    LandsatCloudCoverLandInputOutputTypeDef,
     LandsatCloudCoverLandInputTypeDef,
-    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEarthObservationJobInputRequestTypeDef,
     ListEarthObservationJobOutputConfigTypeDef,
-    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
     ListRasterDataCollectionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListVectorEnrichmentJobInputRequestTypeDef,
     ListVectorEnrichmentJobOutputConfigTypeDef,
+    MapMatchingConfigOutputTypeDef,
     MapMatchingConfigTypeDef,
+    UserDefinedOutputTypeDef,
     UserDefinedTypeDef,
-    PaginatorConfigTypeDef,
+    PlatformInputOutputTypeDef,
     PlatformInputTypeDef,
+    ViewOffNadirInputOutputTypeDef,
+    ViewSunAzimuthInputOutputTypeDef,
+    ViewSunElevationInputOutputTypeDef,
     ViewOffNadirInputTypeDef,
     ViewSunAzimuthInputTypeDef,
     ViewSunElevationInputTypeDef,
     TimeRangeFilterInputTypeDef,
     TimeRangeFilterOutputTypeDef,
-    ResponseMetadataTypeDef,
+    ReverseGeocodingConfigOutputTypeDef,
     ReverseGeocodingConfigTypeDef,
     StopEarthObservationJobInputRequestTypeDef,
     StopVectorEnrichmentJobInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AreaOfInterestGeometryOutputTypeDef,
     AreaOfInterestGeometryTypeDef,
+    CustomIndicesInputOutputTypeDef,
     CustomIndicesInputTypeDef,
+    GetTileOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExportErrorDetailsTypeDef,
+    OutputConfigInputOutputTypeDef,
     OutputConfigInputTypeDef,
+    ExportVectorEnrichmentJobOutputConfigOutputTypeDef,
+    VectorEnrichmentJobDataSourceConfigInputOutputTypeDef,
     ExportVectorEnrichmentJobOutputConfigTypeDef,
     VectorEnrichmentJobDataSourceConfigInputTypeDef,
     GetRasterDataCollectionOutputTypeDef,
     RasterDataCollectionMetadataTypeDef,
     ItemSourceTypeDef,
+    ListEarthObservationJobInputListEarthObservationJobsPaginateTypeDef,
+    ListRasterDataCollectionsInputListRasterDataCollectionsPaginateTypeDef,
+    ListVectorEnrichmentJobInputListVectorEnrichmentJobsPaginateTypeDef,
     ListEarthObservationJobOutputTypeDef,
     ListVectorEnrichmentJobOutputTypeDef,
+    OutputResolutionResamplingInputOutputTypeDef,
+    OutputResolutionStackInputOutputTypeDef,
     OutputResolutionResamplingInputTypeDef,
     OutputResolutionStackInputTypeDef,
+    PropertyOutputTypeDef,
     PropertyTypeDef,
+    VectorEnrichmentJobConfigOutputTypeDef,
     VectorEnrichmentJobConfigTypeDef,
+    AreaOfInterestOutputTypeDef,
     AreaOfInterestTypeDef,
+    BandMathConfigInputOutputTypeDef,
     BandMathConfigInputTypeDef,
-    ExportEarthObservationJobInputRequestTypeDef,
     ExportEarthObservationJobOutputTypeDef,
-    ExportVectorEnrichmentJobInputRequestTypeDef,
+    ExportEarthObservationJobInputRequestTypeDef,
     ExportVectorEnrichmentJobOutputTypeDef,
+    VectorEnrichmentJobInputConfigOutputTypeDef,
+    ExportVectorEnrichmentJobInputRequestTypeDef,
     VectorEnrichmentJobInputConfigTypeDef,
     ListRasterDataCollectionsOutputTypeDef,
     SearchRasterDataCollectionOutputTypeDef,
+    ResamplingConfigInputOutputTypeDef,
+    StackConfigInputOutputTypeDef,
     ResamplingConfigInputTypeDef,
     StackConfigInputTypeDef,
+    PropertyFilterOutputTypeDef,
     PropertyFilterTypeDef,
     GetVectorEnrichmentJobOutputTypeDef,
-    StartVectorEnrichmentJobInputRequestTypeDef,
     StartVectorEnrichmentJobOutputTypeDef,
+    StartVectorEnrichmentJobInputRequestTypeDef,
+    JobConfigInputOutputTypeDef,
     JobConfigInputTypeDef,
+    PropertyFiltersOutputTypeDef,
     PropertyFiltersTypeDef,
-    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryOutputTypeDef,
+    RasterDataCollectionQueryInputTypeDef,
     RasterDataCollectionQueryWithBandFilterInputTypeDef,
-    InputConfigInputTypeDef,
     InputConfigOutputTypeDef,
+    InputConfigInputTypeDef,
     SearchRasterDataCollectionInputRequestTypeDef,
-    StartEarthObservationJobInputRequestTypeDef,
     GetEarthObservationJobOutputTypeDef,
     StartEarthObservationJobOutputTypeDef,
+    StartEarthObservationJobInputRequestTypeDef,
 )
 
 
-def get_structure() -> MultiPolygonGeometryInputTypeDef:
+def get_structure() -> MultiPolygonGeometryInputOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt` & `mypy-boto3-sagemaker-geospatial-1.28.12/mypy_boto3_sagemaker_geospatial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sagemaker-geospatial-1.28.0/setup.py` & `mypy-boto3-sagemaker-geospatial-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sagemaker-geospatial",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_sagemaker_geospatial"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SageMakergeospatialcapabilities 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

