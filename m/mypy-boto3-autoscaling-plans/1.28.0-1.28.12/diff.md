# Comparing `tmp/mypy-boto3-autoscaling-plans-1.28.0.tar.gz` & `tmp/mypy-boto3-autoscaling-plans-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.0.tar", last modified: Thu Jul  6 20:59:02 2023, max compression
+gzip compressed data, was "mypy-boto3-autoscaling-plans-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
```

## Comparing `mypy-boto3-autoscaling-plans-1.28.0.tar` & `mypy-boto3-autoscaling-plans-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.170228 mypy-boto3-autoscaling-plans-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-06 20:59:02.170228 mypy-boto3-autoscaling-plans-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13276 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.166228 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-07-06 20:34:03.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-06 20:34:03.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:02.170228 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:01.000000 mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:02.170228 mypy-boto3-autoscaling-plans-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:34:02.000000 mypy-boto3-autoscaling-plans-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.648572 mypy-boto3-autoscaling-plans-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19570 2023-07-27 05:17:51.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-27 05:17:51.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.640572 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:20.000000 mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.648572 mypy-boto3-autoscaling-plans-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:17:50.000000 mypy-boto3-autoscaling-plans-1.28.12/setup.py
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/LICENSE` & `mypy-boto3-autoscaling-plans-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.0
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,45 +341,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
     CreateScalingPlanResponseTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
+    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_structure() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/README.md` & `mypy-boto3-autoscaling-plans-1.28.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -309,45 +309,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
     CreateScalingPlanResponseTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
+    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_structure() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__init__.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__init__.pyi` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/__main__.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AutoScalingPlans 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.AutoScalingPlans 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/client.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/client.pyi` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/literals.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeScalingPlanResourcesPaginatorName",
     "DescribeScalingPlansPaginatorName",
     "ForecastDataTypeType",
     "LoadMetricTypeType",
     "MetricStatisticType",
     "PolicyTypeType",
@@ -37,15 +36,14 @@
     "AutoScalingPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeScalingPlanResourcesPaginatorName = Literal["describe_scaling_plan_resources"]
 DescribeScalingPlansPaginatorName = Literal["describe_scaling_plans"]
 ForecastDataTypeType = Literal[
     "CapacityForecast", "LoadForecast", "ScheduledActionMaxCapacity", "ScheduledActionMinCapacity"
 ]
 LoadMetricTypeType = Literal[
     "ALBTargetGroupRequestCount",
@@ -215,14 +213,15 @@
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
@@ -301,26 +300,28 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/literals.pyi` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeScalingPlanResourcesPaginatorName",
     "DescribeScalingPlansPaginatorName",
     "ForecastDataTypeType",
     "LoadMetricTypeType",
     "MetricStatisticType",
     "PolicyTypeType",
@@ -36,14 +37,15 @@
     "AutoScalingPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DescribeScalingPlanResourcesPaginatorName = Literal["describe_scaling_plan_resources"]
 DescribeScalingPlansPaginatorName = Literal["describe_scaling_plans"]
 ForecastDataTypeType = Literal[
     "CapacityForecast", "LoadForecast", "ScheduledActionMaxCapacity", "ScheduledActionMinCapacity"
 ]
 LoadMetricTypeType = Literal[
     "ALBTargetGroupRequestCount",
@@ -213,14 +215,15 @@
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
@@ -299,26 +302,28 @@
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

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/paginator.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/paginator.pyi` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/type_defs.py` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling_plans.type_defs import TagFilterTypeDef
+    from mypy_boto3_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterTypeDef = {...}
+    data: TagFilterOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -34,45 +34,62 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
     "CreateScalingPlanResponseTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "PredefinedLoadMetricSpecificationOutputTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
+    "PredefinedScalingMetricSpecificationOutputTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
     "ResponseMetadataTypeDef",
+    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CustomizedLoadMetricSpecificationOutputTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
-    "ScalingInstructionTypeDef",
+    "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
 )
 
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -82,14 +99,22 @@
     "CreateScalingPlanResponseTypeDef",
     {
         "ScalingPlanVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -122,22 +147,20 @@
     "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
 class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -146,22 +169,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -178,35 +199,73 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedLoadMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedLoadMetricType": LoadMetricTypeType,
+    },
+)
+_OptionalPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedLoadMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredefinedLoadMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedLoadMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedLoadMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedLoadMetricSpecificationTypeDef(
     _RequiredPredefinedLoadMetricSpecificationTypeDef,
     _OptionalPredefinedLoadMetricSpecificationTypeDef,
 ):
     pass
 
+_RequiredPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedScalingMetricType": ScalingMetricTypeType,
+    },
+)
+_OptionalPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedScalingMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+class PredefinedScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
 
 _RequiredPredefinedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedScalingMetricSpecificationTypeDef",
     {
         "PredefinedScalingMetricType": ScalingMetricTypeType,
     },
 )
@@ -214,42 +273,95 @@
     "_OptionalPredefinedScalingMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ApplicationSourceOutputTypeDef = TypedDict(
+    "ApplicationSourceOutputTypeDef",
+    {
+        "CloudFormationStackARN": str,
+        "TagFilters": List[TagFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+class CustomizedLoadMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -259,22 +371,20 @@
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
-
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
-
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -284,22 +394,20 @@
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
-
 class CustomizedScalingMetricSpecificationTypeDef(
     _RequiredCustomizedScalingMetricSpecificationTypeDef,
     _OptionalCustomizedScalingMetricSpecificationTypeDef,
 ):
     pass
 
-
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -323,14 +431,39 @@
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationOutputTypeDef,
+        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "EstimatedInstanceWarmup": int,
+    },
+    total=False,
+)
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -342,158 +475,177 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "EstimatedInstanceWarmup": int,
     },
     total=False,
 )
 
-
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
-
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
+_RequiredScalingInstructionOutputTypeDef = TypedDict(
+    "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+_OptionalScalingInstructionOutputTypeDef = TypedDict(
+    "_OptionalScalingInstructionOutputTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationOutputTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
-
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+class ScalingInstructionOutputTypeDef(
+    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
 ):
     pass
 
-
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+    },
+)
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
+    {
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "ScheduledActionBufferTime": int,
+        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
+        "PredictiveScalingMaxCapacityBuffer": int,
+        "PredictiveScalingMode": PredictiveScalingModeType,
+        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
+        "DisableDynamicScaling": bool,
     },
+    total=False,
 )
 
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+):
+    pass
+
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": List[ScalingInstructionTypeDef],
+        "ApplicationSource": ApplicationSourceOutputTypeDef,
+        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
         "StatusStartTime": datetime,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
-
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+_RequiredScalingPlanResourceTypeDef = TypedDict(
+    "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "ScalingStatusCode": ScalingStatusCodeType,
     },
 )
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+_OptionalScalingPlanResourceTypeDef = TypedDict(
+    "_OptionalScalingPlanResourceTypeDef",
     {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ScalingPolicies": List[ScalingPolicyTypeDef],
+        "ScalingStatusMessage": str,
     },
     total=False,
 )
 
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+class ScalingPlanResourceTypeDef(
+    _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+    },
+)
 
-_RequiredScalingPlanResourceTypeDef = TypedDict(
-    "_RequiredScalingPlanResourceTypeDef",
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "ScalingStatusCode": ScalingStatusCodeType,
     },
 )
-_OptionalScalingPlanResourceTypeDef = TypedDict(
-    "_OptionalScalingPlanResourceTypeDef",
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
     {
-        "ScalingPolicies": List[ScalingPolicyTypeDef],
-        "ScalingStatusMessage": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
     },
     total=False,
 )
 
-
-class ScalingPlanResourceTypeDef(
-    _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
 ):
     pass
 
-
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans/type_defs.pyi` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans/type_defs.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_autoscaling_plans.type_defs import TagFilterTypeDef
+    from mypy_boto3_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterTypeDef = {...}
+    data: TagFilterOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -34,44 +34,63 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
     "CreateScalingPlanResponseTypeDef",
+    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "PredefinedLoadMetricSpecificationOutputTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
+    "PredefinedScalingMetricSpecificationOutputTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
     "ResponseMetadataTypeDef",
+    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CustomizedLoadMetricSpecificationOutputTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "TargetTrackingConfigurationTypeDef",
-    "ScalingInstructionTypeDef",
+    "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
 )
 
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
+)
+
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -81,14 +100,22 @@
     "CreateScalingPlanResponseTypeDef",
     {
         "ScalingPlanVersion": int,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+MetricDimensionOutputTypeDef = TypedDict(
+    "MetricDimensionOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -121,20 +148,22 @@
     "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
 class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -143,20 +172,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -173,74 +204,181 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedLoadMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedLoadMetricType": LoadMetricTypeType,
+    },
+)
+_OptionalPredefinedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedLoadMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredefinedLoadMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedLoadMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedLoadMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedLoadMetricSpecificationTypeDef(
     _RequiredPredefinedLoadMetricSpecificationTypeDef,
     _OptionalPredefinedLoadMetricSpecificationTypeDef,
 ):
     pass
 
+
+_RequiredPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredefinedScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedScalingMetricType": ScalingMetricTypeType,
+    },
+)
+_OptionalPredefinedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredefinedScalingMetricSpecificationOutputTypeDef",
+    {
+        "ResourceLabel": str,
+    },
+    total=False,
+)
+
+
+class PredefinedScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredefinedScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredefinedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredefinedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedScalingMetricSpecificationTypeDef",
     {
         "PredefinedScalingMetricType": ScalingMetricTypeType,
     },
 )
 _OptionalPredefinedScalingMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedScalingMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
+ApplicationSourceOutputTypeDef = TypedDict(
+    "ApplicationSourceOutputTypeDef",
+    {
+        "CloudFormationStackARN": str,
+        "TagFilters": List[TagFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class CustomizedLoadMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -250,20 +388,22 @@
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
+
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
+
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -273,20 +413,22 @@
     {
         "Dimensions": Sequence[MetricDimensionTypeDef],
         "Unit": str,
     },
     total=False,
 )
 
+
 class CustomizedScalingMetricSpecificationTypeDef(
     _RequiredCustomizedScalingMetricSpecificationTypeDef,
     _OptionalCustomizedScalingMetricSpecificationTypeDef,
 ):
     pass
 
+
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -310,14 +452,41 @@
         "ApplicationSources": Sequence[ApplicationSourceTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationOutputTypeDef,
+        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "EstimatedInstanceWarmup": int,
+    },
+    total=False,
+)
+
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -329,120 +498,131 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "EstimatedInstanceWarmup": int,
     },
     total=False,
 )
 
+
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
+
+_RequiredScalingInstructionOutputTypeDef = TypedDict(
+    "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+_OptionalScalingInstructionOutputTypeDef = TypedDict(
+    "_OptionalScalingInstructionOutputTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationOutputTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+
+class ScalingInstructionOutputTypeDef(
+    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
 ):
     pass
 
+
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
+
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+    },
+)
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
+    {
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "ScheduledActionBufferTime": int,
+        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
+        "PredictiveScalingMaxCapacityBuffer": int,
+        "PredictiveScalingMode": PredictiveScalingModeType,
+        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
+        "DisableDynamicScaling": bool,
     },
+    total=False,
 )
 
+
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+):
+    pass
+
+
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": List[ScalingInstructionTypeDef],
+        "ApplicationSource": ApplicationSourceOutputTypeDef,
+        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
         "StatusStartTime": datetime,
         "CreationTime": datetime,
     },
     total=False,
 )
 
+
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
-):
-    pass
 
 _RequiredScalingPlanResourceTypeDef = TypedDict(
     "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
@@ -456,19 +636,53 @@
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "ScalingStatusMessage": str,
     },
     total=False,
 )
 
+
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
+
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+    },
+)
+
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+):
+    pass
+
+
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-autoscaling-plans
-Version: 1.28.0
-Summary: Type annotations for boto3.AutoScalingPlans 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-autoscaling-plans"></a>
 
 # mypy-boto3-autoscaling-plans
 
 [![PyPI - mypy-boto3-autoscaling-plans](https://img.shields.io/pypi/v/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-autoscaling-plans.svg?color=blue)](https://pypi.org/project/mypy-boto3-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-autoscaling-plans?color=blue)](https://pypistats.org/packages/mypy-boto3-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-autoscaling-plans)](https://pepy.tech/project/mypy-boto3-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AutoScalingPlans 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
+[boto3.AutoScalingPlans 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [mypy-boto3-autoscaling-plans docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -341,45 +341,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_autoscaling_plans.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
     CreateScalingPlanResponseTypeDef,
+    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
     DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
     DescribeScalingPlanResourcesRequestRequestTypeDef,
     GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    PredefinedLoadMetricSpecificationOutputTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
+    PredefinedScalingMetricSpecificationOutputTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
     ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_structure() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt` & `mypy-boto3-autoscaling-plans-1.28.12/mypy_boto3_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-autoscaling-plans-1.28.0/setup.py` & `mypy-boto3-autoscaling-plans-1.28.12/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-autoscaling-plans",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AutoScalingPlans 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.AutoScalingPlans 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

