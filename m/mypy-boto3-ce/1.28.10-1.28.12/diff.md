# Comparing `tmp/mypy-boto3-ce-1.28.10.tar.gz` & `tmp/mypy-boto3-ce-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.28.10.tar", last modified: Mon Jul 24 19:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-ce-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-ce-1.28.10.tar` & `mypy-boto3-ce-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18167 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:46:56.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    68270 2023-07-24 19:46:58.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68211 2023-07-24 19:46:57.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 19:49:46.000000 mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:49:46.284631 mypy-boto3-ce-1.28.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-24 19:46:55.000000 mypy-boto3-ce-1.28.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.796567 mypy-boto3-ce-1.28.12/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32603 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-07-27 05:18:06.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:05.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71661 2023-07-27 05:18:07.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71586 2023-07-27 05:18:06.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19628 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:34:22.000000 mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.804567 mypy-boto3-ce-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:18:04.000000 mypy-boto3-ce-1.28.12/setup.py
```

### Comparing `mypy-boto3-ce-1.28.10/LICENSE` & `mypy-boto3-ce-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.10/PKG-INFO` & `mypy-boto3-ce-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.10
-Summary: Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,20 +351,23 @@
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesOutputTypeDef,
     DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
@@ -378,71 +381,68 @@
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationOutputTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.10/README.md` & `mypy-boto3-ce-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -319,20 +319,23 @@
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesOutputTypeDef,
     DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
@@ -346,71 +349,68 @@
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationOutputTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/__main__.py` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.28.10\nVersion:         1.28.10\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.CostExplorer 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.10")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.py` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/client.pyi` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.py` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
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
@@ -382,14 +383,15 @@
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

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/literals.pyi` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -294,14 +294,15 @@
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
@@ -380,14 +381,15 @@
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

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.py` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,20 +77,23 @@
     "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalOutputTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
     "TagValuesOutputTypeDef",
     "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
@@ -104,71 +107,68 @@
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
+    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
+    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
     "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
-    "GetCostCategoriesResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationOutputTypeDef",
@@ -251,29 +251,42 @@
 
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
 
-AnomalyMonitorOutputTypeDef = TypedDict(
-    "AnomalyMonitorOutputTypeDef",
+_RequiredAnomalyMonitorOutputTypeDef = TypedDict(
+    "_RequiredAnomalyMonitorOutputTypeDef",
     {
-        "MonitorArn": str,
         "MonitorName": str,
+        "MonitorType": MonitorTypeType,
+    },
+)
+_OptionalAnomalyMonitorOutputTypeDef = TypedDict(
+    "_OptionalAnomalyMonitorOutputTypeDef",
+    {
+        "MonitorArn": str,
         "CreationDate": str,
         "LastUpdatedDate": str,
         "LastEvaluatedDate": str,
-        "MonitorType": MonitorTypeType,
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionOutputTypeDef",
         "DimensionalValueCount": int,
     },
+    total=False,
 )
 
+
+class AnomalyMonitorOutputTypeDef(
+    _RequiredAnomalyMonitorOutputTypeDef, _OptionalAnomalyMonitorOutputTypeDef
+):
+    pass
+
+
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -307,46 +320,59 @@
 SubscriberOutputTypeDef = TypedDict(
     "SubscriberOutputTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
+    total=False,
 )
 
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
     total=False,
 )
 
-ImpactTypeDef = TypedDict(
-    "ImpactTypeDef",
+_RequiredImpactTypeDef = TypedDict(
+    "_RequiredImpactTypeDef",
     {
         "MaxImpact": float,
+    },
+)
+_OptionalImpactTypeDef = TypedDict(
+    "_OptionalImpactTypeDef",
+    {
         "TotalImpact": float,
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
+    total=False,
 )
 
+
+class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
+    pass
+
+
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
         "LinkedAccountName": str,
     },
+    total=False,
 )
 
 CostAllocationTagStatusEntryTypeDef = TypedDict(
     "CostAllocationTagStatusEntryTypeDef",
     {
         "TagKey": str,
         "Status": CostAllocationTagStatusType,
@@ -364,14 +390,15 @@
 
 CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionOutputTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
+    total=False,
 )
 
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
@@ -381,14 +408,15 @@
 
 CostCategoryProcessingStatusTypeDef = TypedDict(
     "CostCategoryProcessingStatusTypeDef",
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
+    total=False,
 )
 
 CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterOutputTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": List[str],
@@ -406,14 +434,15 @@
 CostCategoryValuesOutputTypeDef = TypedDict(
     "CostCategoryValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -431,62 +460,80 @@
 )
 
 CoverageCostTypeDef = TypedDict(
     "CoverageCostTypeDef",
     {
         "OnDemandCost": str,
     },
+    total=False,
 )
 
 CoverageHoursTypeDef = TypedDict(
     "CoverageHoursTypeDef",
     {
         "OnDemandHours": str,
         "ReservedHours": str,
         "TotalRunningHours": str,
         "CoverageHoursPercentage": str,
     },
+    total=False,
 )
 
 CoverageNormalizedUnitsTypeDef = TypedDict(
     "CoverageNormalizedUnitsTypeDef",
     {
         "OnDemandNormalizedUnits": str,
         "ReservedNormalizedUnits": str,
         "TotalRunningNormalizedUnits": str,
         "CoverageNormalizedUnitsPercentage": str,
     },
+    total=False,
 )
 
 ResourceTagTypeDef = TypedDict(
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagValuesOutputTypeDef = TypedDict(
     "TagValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 DateIntervalTypeDef = TypedDict(
     "DateIntervalTypeDef",
     {
         "Start": str,
         "End": str,
@@ -510,14 +557,23 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -539,14 +595,15 @@
 DimensionValuesOutputTypeDef = TypedDict(
     "DimensionValuesOutputTypeDef",
     {
         "Key": DimensionType,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
@@ -557,48 +614,52 @@
 
 DimensionValuesWithAttributesTypeDef = TypedDict(
     "DimensionValuesWithAttributesTypeDef",
     {
         "Value": str,
         "Attributes": Dict[str, str],
     },
+    total=False,
 )
 
 DiskResourceUtilizationTypeDef = TypedDict(
     "DiskResourceUtilizationTypeDef",
     {
         "DiskReadOpsPerSecond": str,
         "DiskWriteOpsPerSecond": str,
         "DiskReadBytesPerSecond": str,
         "DiskWriteBytesPerSecond": str,
     },
+    total=False,
 )
 
 EBSResourceUtilizationTypeDef = TypedDict(
     "EBSResourceUtilizationTypeDef",
     {
         "EbsReadOpsPerSecond": str,
         "EbsWriteOpsPerSecond": str,
         "EbsReadBytesPerSecond": str,
         "EbsWriteBytesPerSecond": str,
     },
+    total=False,
 )
 
 EC2InstanceDetailsTypeDef = TypedDict(
     "EC2InstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "AvailabilityZone": str,
         "Platform": str,
         "Tenancy": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 EC2ResourceDetailsTypeDef = TypedDict(
     "EC2ResourceDetailsTypeDef",
     {
         "HourlyOnDemandRate": str,
         "InstanceType": str,
@@ -606,31 +667,34 @@
         "Region": str,
         "Sku": str,
         "Memory": str,
         "NetworkPerformance": str,
         "Storage": str,
         "Vcpu": str,
     },
+    total=False,
 )
 
 NetworkResourceUtilizationTypeDef = TypedDict(
     "NetworkResourceUtilizationTypeDef",
     {
         "NetworkInBytesPerSecond": str,
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
+    total=False,
 )
 
 EC2SpecificationOutputTypeDef = TypedDict(
     "EC2SpecificationOutputTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
+    total=False,
 )
 
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
@@ -642,26 +706,28 @@
     {
         "InstanceClass": str,
         "InstanceSize": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 ElastiCacheInstanceDetailsTypeDef = TypedDict(
     "ElastiCacheInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 TagValuesTypeDef = TypedDict(
     "TagValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -675,14 +741,15 @@
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
         "EstimatedCompletionTime": str,
     },
+    total=False,
 )
 
 _RequiredTotalImpactFilterTypeDef = TypedDict(
     "_RequiredTotalImpactFilterTypeDef",
     {
         "NumericOperator": NumericOperatorType,
         "StartValue": float,
@@ -735,14 +802,15 @@
 
 GroupDefinitionOutputTypeDef = TypedDict(
     "GroupDefinitionOutputTypeDef",
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
+    total=False,
 )
 
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
@@ -756,28 +824,42 @@
 )
 
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
 
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
     },
+    total=False,
 )
 
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": str,
         "UtilizationPercentageInUnits": str,
@@ -793,14 +875,15 @@
         "AmortizedUpfrontFee": str,
         "AmortizedRecurringFee": str,
         "TotalAmortizedFee": str,
         "RICostForUnusedHours": str,
         "RealizedSavings": str,
         "UnrealizedSavings": str,
     },
+    total=False,
 )
 
 RightsizingRecommendationConfigurationTypeDef = TypedDict(
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
@@ -819,24 +902,26 @@
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
     },
+    total=False,
 )
 
 RightsizingRecommendationSummaryTypeDef = TypedDict(
     "RightsizingRecommendationSummaryTypeDef",
     {
         "TotalRecommendationCount": str,
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
+    total=False,
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     {
         "RecommendationDetailId": str,
     },
@@ -873,14 +958,26 @@
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
+    total=False,
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
@@ -888,25 +985,27 @@
         "DatabaseEngine": str,
         "DatabaseEdition": str,
         "DeploymentOption": str,
         "LicenseModel": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 RedshiftInstanceDetailsTypeDef = TypedDict(
     "RedshiftInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 ListCostAllocationTagsRequestRequestTypeDef = TypedDict(
     "ListCostAllocationTagsRequestRequestTypeDef",
     {
         "Status": CostAllocationTagStatusType,
         "TagKeys": Sequence[str],
@@ -957,68 +1056,93 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecommendationDetailHourlyMetricsTypeDef = TypedDict(
     "RecommendationDetailHourlyMetricsTypeDef",
     {
         "StartTime": str,
         "EstimatedOnDemandCost": str,
         "CurrentCoverage": str,
         "EstimatedCoverage": str,
         "EstimatedNewCommitmentUtilization": str,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
+    total=False,
 )
 
 SavingsPlansAmortizedCommitmentTypeDef = TypedDict(
     "SavingsPlansAmortizedCommitmentTypeDef",
     {
         "AmortizedRecurringCommitment": str,
         "AmortizedUpfrontCommitment": str,
         "TotalAmortizedCommitment": str,
     },
+    total=False,
 )
 
 SavingsPlansCoverageDataTypeDef = TypedDict(
     "SavingsPlansCoverageDataTypeDef",
     {
         "SpendCoveredBySavingsPlans": str,
         "OnDemandCost": str,
         "TotalCost": str,
         "CoveragePercentage": str,
     },
+    total=False,
 )
 
 SavingsPlansDetailsTypeDef = TypedDict(
     "SavingsPlansDetailsTypeDef",
     {
         "Region": str,
         "InstanceFamily": str,
         "OfferingId": str,
     },
+    total=False,
 )
 
 SavingsPlansPurchaseRecommendationSummaryTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     {
         "EstimatedROI": str,
         "CurrencyCode": str,
@@ -1028,32 +1152,45 @@
         "TotalRecommendationCount": str,
         "DailyCommitmentToPurchase": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedSavingsPercentage": str,
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedOnDemandCostWithCurrentCommitment": str,
     },
+    total=False,
 )
 
 SavingsPlansSavingsTypeDef = TypedDict(
     "SavingsPlansSavingsTypeDef",
     {
         "NetSavings": str,
         "OnDemandCostEquivalent": str,
     },
+    total=False,
 )
 
 SavingsPlansUtilizationTypeDef = TypedDict(
     "SavingsPlansUtilizationTypeDef",
     {
         "TotalCommitment": str,
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
+    total=False,
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
@@ -1078,37 +1215,85 @@
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
+    total=False,
 )
 
-AnomalySubscriptionOutputTypeDef = TypedDict(
-    "AnomalySubscriptionOutputTypeDef",
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_RequiredAnomalySubscriptionOutputTypeDef",
     {
-        "SubscriptionArn": str,
-        "AccountId": str,
         "MonitorArnList": List[str],
         "Subscribers": List[SubscriberOutputTypeDef],
-        "Threshold": float,
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
+    },
+)
+_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_OptionalAnomalySubscriptionOutputTypeDef",
+    {
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "Threshold": float,
         "ThresholdExpression": "ExpressionOutputTypeDef",
     },
+    total=False,
 )
 
+
+class AnomalySubscriptionOutputTypeDef(
+    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
+):
+    pass
+
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1155,44 +1340,65 @@
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+_RequiredAnomalyTypeDef = TypedDict(
+    "_RequiredAnomalyTypeDef",
     {
         "AnomalyId": str,
+        "AnomalyScore": AnomalyScoreTypeDef,
+        "Impact": ImpactTypeDef,
+        "MonitorArn": str,
+    },
+)
+_OptionalAnomalyTypeDef = TypedDict(
+    "_OptionalAnomalyTypeDef",
+    {
         "AnomalyStartDate": str,
         "AnomalyEndDate": str,
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
-        "AnomalyScore": AnomalyScoreTypeDef,
-        "Impact": ImpactTypeDef,
-        "MonitorArn": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
+    total=False,
 )
 
+
+class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
+    pass
+
+
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CostCategoryRuleOutputTypeDef = TypedDict(
     "CostCategoryRuleOutputTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionOutputTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
         "Type": CostCategoryRuleTypeType,
     },
+    total=False,
 )
 
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
@@ -1210,26 +1416,41 @@
         "EffectiveStart": str,
         "EffectiveEnd": str,
         "NumberOfRules": int,
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
+    total=False,
 )
 
-CostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "CostCategorySplitChargeRuleOutputTypeDef",
+_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
     {
         "Source": str,
         "Targets": List[str],
         "Method": CostCategorySplitChargeMethodType,
+    },
+)
+_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
+    {
         "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
     },
+    total=False,
 )
 
+
+class CostCategorySplitChargeRuleOutputTypeDef(
+    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
+    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
+):
+    pass
+
+
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1253,23 +1474,25 @@
     "ForecastResultTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
+    total=False,
 )
 
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
     {
         "AnomalyMonitor": AnomalyMonitorTypeDef,
     },
@@ -1294,132 +1517,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1470,51 +1575,55 @@
         "Or": List[Dict[str, Any]],
         "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
         "Dimensions": DimensionValuesOutputTypeDef,
         "Tags": TagValuesOutputTypeDef,
         "CostCategories": CostCategoryValuesOutputTypeDef,
     },
+    total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
     },
+    total=False,
 )
 
 EC2ResourceUtilizationTypeDef = TypedDict(
     "EC2ResourceUtilizationTypeDef",
     {
         "MaxCpuUtilizationPercentage": str,
         "MaxMemoryUtilizationPercentage": str,
         "MaxStorageUtilizationPercentage": str,
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
 ServiceSpecificationOutputTypeDef = TypedDict(
     "ServiceSpecificationOutputTypeDef",
     {
         "EC2Specification": EC2SpecificationOutputTypeDef,
     },
+    total=False,
 )
 
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
@@ -1535,15 +1644,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1834,24 +1943,26 @@
 
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
+    total=False,
 )
 
 ReservationUtilizationGroupTypeDef = TypedDict(
     "ReservationUtilizationGroupTypeDef",
     {
         "Key": str,
         "Value": str,
         "Attributes": Dict[str, str],
         "Utilization": ReservationAggregatesTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetRightsizingRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetRightsizingRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -1880,21 +1991,22 @@
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDetailDataTypeDef = TypedDict(
     "RecommendationDetailDataTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -1923,23 +2035,25 @@
         "ExistingHourlyCommitment": str,
         "HourlyCommitmentToPurchase": str,
         "UpfrontCost": str,
         "CurrentAverageCoverage": str,
         "EstimatedAverageCoverage": str,
         "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
     },
+    total=False,
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
         "TimePeriod": DateIntervalOutputTypeDef,
     },
+    total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
         "SavingsPlansDetails": SavingsPlansDetailsTypeDef,
         "AccountId": str,
@@ -1955,60 +2069,89 @@
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
         "RecommendationDetailId": str,
     },
+    total=False,
 )
 
-SavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "SavingsPlansUtilizationAggregatesTypeDef",
+_RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
     {
         "Utilization": SavingsPlansUtilizationTypeDef,
+    },
+)
+_OptionalSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "_OptionalSavingsPlansUtilizationAggregatesTypeDef",
+    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
-SavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "SavingsPlansUtilizationByTimeTypeDef",
+
+class SavingsPlansUtilizationAggregatesTypeDef(
+    _RequiredSavingsPlansUtilizationAggregatesTypeDef,
+    _OptionalSavingsPlansUtilizationAggregatesTypeDef,
+):
+    pass
+
+
+_RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
+    },
+)
+_OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "_OptionalSavingsPlansUtilizationByTimeTypeDef",
+    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
+
+class SavingsPlansUtilizationByTimeTypeDef(
+    _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
+):
+    pass
+
+
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -2031,42 +2174,53 @@
 
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CostCategoryTypeDef = TypedDict(
-    "CostCategoryTypeDef",
+_RequiredCostCategoryTypeDef = TypedDict(
+    "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
-        "EffectiveEnd": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": List[CostCategoryRuleOutputTypeDef],
+    },
+)
+_OptionalCostCategoryTypeDef = TypedDict(
+    "_OptionalCostCategoryTypeDef",
+    {
+        "EffectiveEnd": str,
         "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
+    total=False,
 )
 
+
+class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
+    pass
+
+
 _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -2117,40 +2271,42 @@
 
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": CoverageTypeDef,
     },
+    total=False,
 )
 
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "EC2ResourceUtilization": EC2ResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -2183,23 +2339,25 @@
     "ResultByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
+    total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
     "ReservationPurchaseRecommendationDetailTypeDef",
     {
         "AccountId": str,
         "InstanceDetails": InstanceDetailsTypeDef,
@@ -2217,31 +2375,32 @@
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedMonthlySavingsPercentage": str,
         "EstimatedMonthlyOnDemandCost": str,
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
+    total=False,
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     {
         "RecommendationDetailId": str,
         "RecommendationDetailData": RecommendationDetailDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2252,51 +2411,53 @@
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
         "SavingsPlansPurchaseRecommendationSummary": (
             SavingsPlansPurchaseRecommendationSummaryTypeDef
         ),
     },
+    total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalOutputTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
+    total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
@@ -2306,127 +2467,132 @@
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
         "CurrencyCode": str,
     },
+    total=False,
 )
 
 TargetInstanceTypeDef = TypedDict(
     "TargetInstanceTypeDef",
     {
         "EstimatedMonthlyCost": str,
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
         "DefaultTargetInstance": bool,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ExpectedResourceUtilization": ResourceUtilizationTypeDef,
         "PlatformDifferences": List[PlatformDifferenceType],
     },
+    total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "ServiceSpecification": ServiceSpecificationOutputTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
+    total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
     },
+    total=False,
 )
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
         "CurrentInstance": CurrentInstanceTypeDef,
         "RightsizingType": RightsizingTypeType,
         "ModifyRecommendationDetail": ModifyRecommendationDetailTypeDef,
         "TerminateRecommendationDetail": TerminateRecommendationDetailTypeDef,
         "FindingReasonCodes": List[FindingReasonCodeType],
     },
+    total=False,
 )
 
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce/type_defs.pyi` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -76,20 +76,23 @@
     "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalOutputTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "ResponseMetadataTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
     "TagValuesOutputTypeDef",
     "DateIntervalTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
     "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
@@ -103,71 +106,68 @@
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "GroupDefinitionOutputTypeDef",
     "SortDefinitionTypeDef",
+    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationConfigurationOutputTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
+    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagOutputTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
     "RecommendationDetailHourlyMetricsTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
     "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleOutputTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
     "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
-    "GetCostCategoriesResponseTypeDef",
-    "GetTagsResponseTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationOutputTypeDef",
@@ -248,29 +248,40 @@
 )
 
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
-AnomalyMonitorOutputTypeDef = TypedDict(
-    "AnomalyMonitorOutputTypeDef",
+_RequiredAnomalyMonitorOutputTypeDef = TypedDict(
+    "_RequiredAnomalyMonitorOutputTypeDef",
     {
-        "MonitorArn": str,
         "MonitorName": str,
+        "MonitorType": MonitorTypeType,
+    },
+)
+_OptionalAnomalyMonitorOutputTypeDef = TypedDict(
+    "_OptionalAnomalyMonitorOutputTypeDef",
+    {
+        "MonitorArn": str,
         "CreationDate": str,
         "LastUpdatedDate": str,
         "LastEvaluatedDate": str,
-        "MonitorType": MonitorTypeType,
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionOutputTypeDef",
         "DimensionalValueCount": int,
     },
+    total=False,
 )
 
+class AnomalyMonitorOutputTypeDef(
+    _RequiredAnomalyMonitorOutputTypeDef, _OptionalAnomalyMonitorOutputTypeDef
+):
+    pass
+
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -302,46 +313,57 @@
 SubscriberOutputTypeDef = TypedDict(
     "SubscriberOutputTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
+    total=False,
 )
 
 SubscriberTypeDef = TypedDict(
     "SubscriberTypeDef",
     {
         "Address": str,
         "Type": SubscriberTypeType,
         "Status": SubscriberStatusType,
     },
     total=False,
 )
 
-ImpactTypeDef = TypedDict(
-    "ImpactTypeDef",
+_RequiredImpactTypeDef = TypedDict(
+    "_RequiredImpactTypeDef",
     {
         "MaxImpact": float,
+    },
+)
+_OptionalImpactTypeDef = TypedDict(
+    "_OptionalImpactTypeDef",
+    {
         "TotalImpact": float,
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
+    total=False,
 )
 
+class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
+    pass
+
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
         "LinkedAccountName": str,
     },
+    total=False,
 )
 
 CostAllocationTagStatusEntryTypeDef = TypedDict(
     "CostAllocationTagStatusEntryTypeDef",
     {
         "TagKey": str,
         "Status": CostAllocationTagStatusType,
@@ -359,14 +381,15 @@
 
 CostCategoryInheritedValueDimensionOutputTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionOutputTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
     },
+    total=False,
 )
 
 CostCategoryInheritedValueDimensionTypeDef = TypedDict(
     "CostCategoryInheritedValueDimensionTypeDef",
     {
         "DimensionName": CostCategoryInheritedValueDimensionNameType,
         "DimensionKey": str,
@@ -376,14 +399,15 @@
 
 CostCategoryProcessingStatusTypeDef = TypedDict(
     "CostCategoryProcessingStatusTypeDef",
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
+    total=False,
 )
 
 CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterOutputTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": List[str],
@@ -401,14 +425,15 @@
 CostCategoryValuesOutputTypeDef = TypedDict(
     "CostCategoryValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -426,62 +451,80 @@
 )
 
 CoverageCostTypeDef = TypedDict(
     "CoverageCostTypeDef",
     {
         "OnDemandCost": str,
     },
+    total=False,
 )
 
 CoverageHoursTypeDef = TypedDict(
     "CoverageHoursTypeDef",
     {
         "OnDemandHours": str,
         "ReservedHours": str,
         "TotalRunningHours": str,
         "CoverageHoursPercentage": str,
     },
+    total=False,
 )
 
 CoverageNormalizedUnitsTypeDef = TypedDict(
     "CoverageNormalizedUnitsTypeDef",
     {
         "OnDemandNormalizedUnits": str,
         "ReservedNormalizedUnits": str,
         "TotalRunningNormalizedUnits": str,
         "CoverageNormalizedUnitsPercentage": str,
     },
+    total=False,
 )
 
 ResourceTagTypeDef = TypedDict(
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 TagValuesOutputTypeDef = TypedDict(
     "TagValuesOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 DateIntervalTypeDef = TypedDict(
     "DateIntervalTypeDef",
     {
         "Start": str,
         "End": str,
@@ -505,14 +548,23 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
@@ -532,14 +584,15 @@
 DimensionValuesOutputTypeDef = TypedDict(
     "DimensionValuesOutputTypeDef",
     {
         "Key": DimensionType,
         "Values": List[str],
         "MatchOptions": List[MatchOptionType],
     },
+    total=False,
 )
 
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
@@ -550,48 +603,52 @@
 
 DimensionValuesWithAttributesTypeDef = TypedDict(
     "DimensionValuesWithAttributesTypeDef",
     {
         "Value": str,
         "Attributes": Dict[str, str],
     },
+    total=False,
 )
 
 DiskResourceUtilizationTypeDef = TypedDict(
     "DiskResourceUtilizationTypeDef",
     {
         "DiskReadOpsPerSecond": str,
         "DiskWriteOpsPerSecond": str,
         "DiskReadBytesPerSecond": str,
         "DiskWriteBytesPerSecond": str,
     },
+    total=False,
 )
 
 EBSResourceUtilizationTypeDef = TypedDict(
     "EBSResourceUtilizationTypeDef",
     {
         "EbsReadOpsPerSecond": str,
         "EbsWriteOpsPerSecond": str,
         "EbsReadBytesPerSecond": str,
         "EbsWriteBytesPerSecond": str,
     },
+    total=False,
 )
 
 EC2InstanceDetailsTypeDef = TypedDict(
     "EC2InstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "AvailabilityZone": str,
         "Platform": str,
         "Tenancy": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 EC2ResourceDetailsTypeDef = TypedDict(
     "EC2ResourceDetailsTypeDef",
     {
         "HourlyOnDemandRate": str,
         "InstanceType": str,
@@ -599,31 +656,34 @@
         "Region": str,
         "Sku": str,
         "Memory": str,
         "NetworkPerformance": str,
         "Storage": str,
         "Vcpu": str,
     },
+    total=False,
 )
 
 NetworkResourceUtilizationTypeDef = TypedDict(
     "NetworkResourceUtilizationTypeDef",
     {
         "NetworkInBytesPerSecond": str,
         "NetworkOutBytesPerSecond": str,
         "NetworkPacketsInPerSecond": str,
         "NetworkPacketsOutPerSecond": str,
     },
+    total=False,
 )
 
 EC2SpecificationOutputTypeDef = TypedDict(
     "EC2SpecificationOutputTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
+    total=False,
 )
 
 EC2SpecificationTypeDef = TypedDict(
     "EC2SpecificationTypeDef",
     {
         "OfferingClass": OfferingClassType,
     },
@@ -635,26 +695,28 @@
     {
         "InstanceClass": str,
         "InstanceSize": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 ElastiCacheInstanceDetailsTypeDef = TypedDict(
     "ElastiCacheInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 TagValuesTypeDef = TypedDict(
     "TagValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -668,14 +730,15 @@
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
         "EstimatedCompletionTime": str,
     },
+    total=False,
 )
 
 _RequiredTotalImpactFilterTypeDef = TypedDict(
     "_RequiredTotalImpactFilterTypeDef",
     {
         "NumericOperator": NumericOperatorType,
         "StartValue": float,
@@ -726,14 +789,15 @@
 
 GroupDefinitionOutputTypeDef = TypedDict(
     "GroupDefinitionOutputTypeDef",
     {
         "Type": GroupDefinitionTypeType,
         "Key": str,
     },
+    total=False,
 )
 
 _RequiredSortDefinitionTypeDef = TypedDict(
     "_RequiredSortDefinitionTypeDef",
     {
         "Key": str,
     },
@@ -745,28 +809,42 @@
     },
     total=False,
 )
 
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
     },
+    total=False,
 )
 
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": str,
         "UtilizationPercentageInUnits": str,
@@ -782,14 +860,15 @@
         "AmortizedUpfrontFee": str,
         "AmortizedRecurringFee": str,
         "TotalAmortizedFee": str,
         "RICostForUnusedHours": str,
         "RealizedSavings": str,
         "UnrealizedSavings": str,
     },
+    total=False,
 )
 
 RightsizingRecommendationConfigurationTypeDef = TypedDict(
     "RightsizingRecommendationConfigurationTypeDef",
     {
         "RecommendationTarget": RecommendationTargetType,
         "BenefitsConsidered": bool,
@@ -808,24 +887,26 @@
     "RightsizingRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "AdditionalMetadata": str,
     },
+    total=False,
 )
 
 RightsizingRecommendationSummaryTypeDef = TypedDict(
     "RightsizingRecommendationSummaryTypeDef",
     {
         "TotalRecommendationCount": str,
         "EstimatedTotalMonthlySavingsAmount": str,
         "SavingsCurrencyCode": str,
         "SavingsPercentage": str,
     },
+    total=False,
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef",
     {
         "RecommendationDetailId": str,
     },
@@ -860,14 +941,26 @@
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
+    total=False,
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
@@ -875,25 +968,27 @@
         "DatabaseEngine": str,
         "DatabaseEdition": str,
         "DeploymentOption": str,
         "LicenseModel": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 RedshiftInstanceDetailsTypeDef = TypedDict(
     "RedshiftInstanceDetailsTypeDef",
     {
         "Family": str,
         "NodeType": str,
         "Region": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
+    total=False,
 )
 
 ListCostAllocationTagsRequestRequestTypeDef = TypedDict(
     "ListCostAllocationTagsRequestRequestTypeDef",
     {
         "Status": CostAllocationTagStatusType,
         "TagKeys": Sequence[str],
@@ -944,68 +1039,93 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    {
+        "AnomalyId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RecommendationDetailHourlyMetricsTypeDef = TypedDict(
     "RecommendationDetailHourlyMetricsTypeDef",
     {
         "StartTime": str,
         "EstimatedOnDemandCost": str,
         "CurrentCoverage": str,
         "EstimatedCoverage": str,
         "EstimatedNewCommitmentUtilization": str,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
     },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
 )
 
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
+    total=False,
 )
 
 SavingsPlansAmortizedCommitmentTypeDef = TypedDict(
     "SavingsPlansAmortizedCommitmentTypeDef",
     {
         "AmortizedRecurringCommitment": str,
         "AmortizedUpfrontCommitment": str,
         "TotalAmortizedCommitment": str,
     },
+    total=False,
 )
 
 SavingsPlansCoverageDataTypeDef = TypedDict(
     "SavingsPlansCoverageDataTypeDef",
     {
         "SpendCoveredBySavingsPlans": str,
         "OnDemandCost": str,
         "TotalCost": str,
         "CoveragePercentage": str,
     },
+    total=False,
 )
 
 SavingsPlansDetailsTypeDef = TypedDict(
     "SavingsPlansDetailsTypeDef",
     {
         "Region": str,
         "InstanceFamily": str,
         "OfferingId": str,
     },
+    total=False,
 )
 
 SavingsPlansPurchaseRecommendationSummaryTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     {
         "EstimatedROI": str,
         "CurrencyCode": str,
@@ -1015,32 +1135,45 @@
         "TotalRecommendationCount": str,
         "DailyCommitmentToPurchase": str,
         "HourlyCommitmentToPurchase": str,
         "EstimatedSavingsPercentage": str,
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedOnDemandCostWithCurrentCommitment": str,
     },
+    total=False,
 )
 
 SavingsPlansSavingsTypeDef = TypedDict(
     "SavingsPlansSavingsTypeDef",
     {
         "NetSavings": str,
         "OnDemandCostEquivalent": str,
     },
+    total=False,
 )
 
 SavingsPlansUtilizationTypeDef = TypedDict(
     "SavingsPlansUtilizationTypeDef",
     {
         "TotalCommitment": str,
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
+    total=False,
+)
+
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    {
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
 )
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
@@ -1063,37 +1196,83 @@
 
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
+    total=False,
 )
 
-AnomalySubscriptionOutputTypeDef = TypedDict(
-    "AnomalySubscriptionOutputTypeDef",
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_RequiredAnomalySubscriptionOutputTypeDef",
     {
-        "SubscriptionArn": str,
-        "AccountId": str,
         "MonitorArnList": List[str],
         "Subscribers": List[SubscriberOutputTypeDef],
-        "Threshold": float,
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
+    },
+)
+_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_OptionalAnomalySubscriptionOutputTypeDef",
+    {
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "Threshold": float,
         "ThresholdExpression": "ExpressionOutputTypeDef",
     },
+    total=False,
 )
 
+class AnomalySubscriptionOutputTypeDef(
+    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
+):
+    pass
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1136,44 +1315,63 @@
 
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+_RequiredAnomalyTypeDef = TypedDict(
+    "_RequiredAnomalyTypeDef",
     {
         "AnomalyId": str,
+        "AnomalyScore": AnomalyScoreTypeDef,
+        "Impact": ImpactTypeDef,
+        "MonitorArn": str,
+    },
+)
+_OptionalAnomalyTypeDef = TypedDict(
+    "_OptionalAnomalyTypeDef",
+    {
         "AnomalyStartDate": str,
         "AnomalyEndDate": str,
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
-        "AnomalyScore": AnomalyScoreTypeDef,
-        "Impact": ImpactTypeDef,
-        "MonitorArn": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
+    total=False,
 )
 
+class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
+    pass
+
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CostCategoryRuleOutputTypeDef = TypedDict(
     "CostCategoryRuleOutputTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionOutputTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionOutputTypeDef,
         "Type": CostCategoryRuleTypeType,
     },
+    total=False,
 )
 
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
@@ -1191,26 +1389,39 @@
         "EffectiveStart": str,
         "EffectiveEnd": str,
         "NumberOfRules": int,
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
+    total=False,
 )
 
-CostCategorySplitChargeRuleOutputTypeDef = TypedDict(
-    "CostCategorySplitChargeRuleOutputTypeDef",
+_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
     {
         "Source": str,
         "Targets": List[str],
         "Method": CostCategorySplitChargeMethodType,
+    },
+)
+_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
+    {
         "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
     },
+    total=False,
 )
 
+class CostCategorySplitChargeRuleOutputTypeDef(
+    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
+    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
+):
+    pass
+
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1232,23 +1443,25 @@
     "ForecastResultTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
     },
+    total=False,
 )
 
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyMonitorRequestRequestTypeDef",
     {
         "AnomalyMonitor": AnomalyMonitorTypeDef,
     },
@@ -1271,132 +1484,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
-    {
-        "AnomalyMonitors": List[AnomalyMonitorOutputTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredGetCostForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1443,51 +1538,55 @@
         "Or": List[Dict[str, Any]],
         "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
         "Dimensions": DimensionValuesOutputTypeDef,
         "Tags": TagValuesOutputTypeDef,
         "CostCategories": CostCategoryValuesOutputTypeDef,
     },
+    total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
     },
+    total=False,
 )
 
 EC2ResourceUtilizationTypeDef = TypedDict(
     "EC2ResourceUtilizationTypeDef",
     {
         "MaxCpuUtilizationPercentage": str,
         "MaxMemoryUtilizationPercentage": str,
         "MaxStorageUtilizationPercentage": str,
         "EBSResourceUtilization": EBSResourceUtilizationTypeDef,
         "DiskResourceUtilization": DiskResourceUtilizationTypeDef,
         "NetworkResourceUtilization": NetworkResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
 ServiceSpecificationOutputTypeDef = TypedDict(
     "ServiceSpecificationOutputTypeDef",
     {
         "EC2Specification": EC2SpecificationOutputTypeDef,
     },
+    total=False,
 )
 
 ServiceSpecificationTypeDef = TypedDict(
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
@@ -1508,15 +1607,15 @@
 )
 
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1785,24 +1884,26 @@
 
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
+    total=False,
 )
 
 ReservationUtilizationGroupTypeDef = TypedDict(
     "ReservationUtilizationGroupTypeDef",
     {
         "Key": str,
         "Value": str,
         "Attributes": Dict[str, str],
         "Utilization": ReservationAggregatesTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetRightsizingRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetRightsizingRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -1829,21 +1930,22 @@
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
         "ESInstanceDetails": ESInstanceDetailsTypeDef,
     },
+    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RecommendationDetailDataTypeDef = TypedDict(
     "RecommendationDetailDataTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -1872,23 +1974,25 @@
         "ExistingHourlyCommitment": str,
         "HourlyCommitmentToPurchase": str,
         "UpfrontCost": str,
         "CurrentAverageCoverage": str,
         "EstimatedAverageCoverage": str,
         "MetricsOverLookbackPeriod": List[RecommendationDetailHourlyMetricsTypeDef],
     },
+    total=False,
 )
 
 SavingsPlansCoverageTypeDef = TypedDict(
     "SavingsPlansCoverageTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": SavingsPlansCoverageDataTypeDef,
         "TimePeriod": DateIntervalOutputTypeDef,
     },
+    total=False,
 )
 
 SavingsPlansPurchaseRecommendationDetailTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     {
         "SavingsPlansDetails": SavingsPlansDetailsTypeDef,
         "AccountId": str,
@@ -1904,60 +2008,85 @@
         "EstimatedAverageUtilization": str,
         "EstimatedMonthlySavingsAmount": str,
         "CurrentMinimumHourlyOnDemandSpend": str,
         "CurrentMaximumHourlyOnDemandSpend": str,
         "CurrentAverageHourlyOnDemandSpend": str,
         "RecommendationDetailId": str,
     },
+    total=False,
 )
 
-SavingsPlansUtilizationAggregatesTypeDef = TypedDict(
-    "SavingsPlansUtilizationAggregatesTypeDef",
+_RequiredSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "_RequiredSavingsPlansUtilizationAggregatesTypeDef",
     {
         "Utilization": SavingsPlansUtilizationTypeDef,
+    },
+)
+_OptionalSavingsPlansUtilizationAggregatesTypeDef = TypedDict(
+    "_OptionalSavingsPlansUtilizationAggregatesTypeDef",
+    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
-SavingsPlansUtilizationByTimeTypeDef = TypedDict(
-    "SavingsPlansUtilizationByTimeTypeDef",
+class SavingsPlansUtilizationAggregatesTypeDef(
+    _RequiredSavingsPlansUtilizationAggregatesTypeDef,
+    _OptionalSavingsPlansUtilizationAggregatesTypeDef,
+):
+    pass
+
+_RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
+    },
+)
+_OptionalSavingsPlansUtilizationByTimeTypeDef = TypedDict(
+    "_OptionalSavingsPlansUtilizationByTimeTypeDef",
+    {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
+class SavingsPlansUtilizationByTimeTypeDef(
+    _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
+):
+    pass
+
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
+    total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAnomalySubscriptionsResponseTypeDef = TypedDict(
     "GetAnomalySubscriptionsResponseTypeDef",
     {
         "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
@@ -1978,42 +2107,51 @@
     pass
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CostCategoryTypeDef = TypedDict(
-    "CostCategoryTypeDef",
+_RequiredCostCategoryTypeDef = TypedDict(
+    "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
         "EffectiveStart": str,
-        "EffectiveEnd": str,
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": List[CostCategoryRuleOutputTypeDef],
+    },
+)
+_OptionalCostCategoryTypeDef = TypedDict(
+    "_OptionalCostCategoryTypeDef",
+    {
+        "EffectiveEnd": str,
         "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
+    total=False,
 )
 
+class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
+    pass
+
 _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
     {
         "Name": str,
         "RuleVersion": Literal["CostCategoryExpression.v1"],
         "Rules": Sequence[CostCategoryRuleTypeDef],
     },
@@ -2060,40 +2198,42 @@
     pass
 
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
         "Coverage": CoverageTypeDef,
     },
+    total=False,
 )
 
 ResourceUtilizationTypeDef = TypedDict(
     "ResourceUtilizationTypeDef",
     {
         "EC2ResourceUtilization": EC2ResourceUtilizationTypeDef,
     },
+    total=False,
 )
 
 _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef",
     {
         "Service": str,
     },
@@ -2124,23 +2264,25 @@
     "ResultByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
     },
+    total=False,
 )
 
 UtilizationByTimeTypeDef = TypedDict(
     "UtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationUtilizationGroupTypeDef],
         "Total": ReservationAggregatesTypeDef,
     },
+    total=False,
 )
 
 ReservationPurchaseRecommendationDetailTypeDef = TypedDict(
     "ReservationPurchaseRecommendationDetailTypeDef",
     {
         "AccountId": str,
         "InstanceDetails": InstanceDetailsTypeDef,
@@ -2158,31 +2300,32 @@
         "EstimatedMonthlySavingsAmount": str,
         "EstimatedMonthlySavingsPercentage": str,
         "EstimatedMonthlyOnDemandCost": str,
         "EstimatedReservationCostForLookbackPeriod": str,
         "UpfrontCost": str,
         "RecurringStandardMonthlyCost": str,
     },
+    total=False,
 )
 
 GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlanPurchaseRecommendationDetailsResponseTypeDef",
     {
         "RecommendationDetailId": str,
         "RecommendationDetailData": RecommendationDetailDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2193,51 +2336,53 @@
         "SavingsPlansPurchaseRecommendationDetails": List[
             SavingsPlansPurchaseRecommendationDetailTypeDef
         ],
         "SavingsPlansPurchaseRecommendationSummary": (
             SavingsPlansPurchaseRecommendationSummaryTypeDef
         ),
     },
+    total=False,
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalOutputTypeDef,
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalOutputTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
+    total=False,
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
@@ -2247,127 +2392,132 @@
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
         "CurrencyCode": str,
     },
+    total=False,
 )
 
 TargetInstanceTypeDef = TypedDict(
     "TargetInstanceTypeDef",
     {
         "EstimatedMonthlyCost": str,
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
         "DefaultTargetInstance": bool,
         "ResourceDetails": ResourceDetailsTypeDef,
         "ExpectedResourceUtilization": ResourceUtilizationTypeDef,
         "PlatformDifferences": List[PlatformDifferenceType],
     },
+    total=False,
 )
 
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionOutputTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
         "LookbackPeriodInDays": LookbackPeriodInDaysType,
         "TermInYears": TermInYearsType,
         "PaymentOption": PaymentOptionType,
         "ServiceSpecification": ServiceSpecificationOutputTypeDef,
         "RecommendationDetails": List[ReservationPurchaseRecommendationDetailTypeDef],
         "RecommendationSummary": ReservationPurchaseRecommendationSummaryTypeDef,
     },
+    total=False,
 )
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
     },
+    total=False,
 )
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
         "CurrentInstance": CurrentInstanceTypeDef,
         "RightsizingType": RightsizingTypeType,
         "ModifyRecommendationDetail": ModifyRecommendationDetailTypeDef,
         "TerminateRecommendationDetail": TerminateRecommendationDetailTypeDef,
         "FindingReasonCodes": List[FindingReasonCodeType],
     },
+    total=False,
 )
 
 GetRightsizingRecommendationResponseTypeDef = TypedDict(
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.28.10
-Summary: Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-ce"></a>
 
 # mypy-boto3-ce
 
 [![PyPI - mypy-boto3-ce](https://img.shields.io/pypi/v/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-ce?color=blue)](https://pypistats.org/packages/mypy-boto3-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.28.10](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [mypy-boto3-ce docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/).
 
 See how it helps to find and fix potential bugs:
 
@@ -351,20 +351,23 @@
     CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalOutputTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    ResponseMetadataTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
     TagValuesOutputTypeDef,
     DateIntervalTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
     DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
@@ -378,71 +381,68 @@
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     GroupDefinitionOutputTypeDef,
     SortDefinitionTypeDef,
+    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationConfigurationOutputTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlanPurchaseRecommendationDetailsRequestRequestTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
+    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagOutputTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
     RecommendationDetailHourlyMetricsTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
+    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
     AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleOutputTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
     CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
-    GetCostCategoriesResponseTypeDef,
-    GetTagsResponseTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationOutputTypeDef,
```

### Comparing `mypy-boto3-ce-1.28.10/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy-boto3-ce-1.28.12/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.28.10/setup.py` & `mypy-boto3-ce-1.28.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.28.10",
+    version="1.28.12",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostExplorer 1.28.10 service generated with mypy-boto3-builder"
-        " 7.15.1"
+        "Type annotations for boto3.CostExplorer 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

