# Comparing `tmp/mypy-boto3-servicecatalog-1.28.0.tar.gz` & `tmp/mypy-boto3-servicecatalog-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-1.28.0.tar", last modified: Thu Jul  6 21:00:37 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-1.28.12.tar", last modified: Thu Jul 27 11:49:38 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-1.28.0.tar` & `mypy-boto3-servicecatalog-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.266430 mypy-boto3-servicecatalog-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27667 2023-07-06 21:00:37.266430 mypy-boto3-servicecatalog-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.266430 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-06 20:55:35.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-07-06 20:55:35.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-07-06 20:55:36.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-07-06 20:55:35.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21879 2023-07-06 20:55:35.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21860 2023-07-06 20:55:35.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102853 2023-07-06 20:55:42.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102708 2023-07-06 20:55:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:37.266430 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27667 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 21:00:37.000000 mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:37.266430 mypy-boto3-servicecatalog-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-06 20:55:34.000000 mypy-boto3-servicecatalog-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.589291 mypy-boto3-servicecatalog-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26324 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14864 2023-07-27 11:46:42.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-07-27 11:46:41.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   103851 2023-07-27 11:46:46.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103706 2023-07-27 11:46:45.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:38.585291 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27839 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:38.000000 mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:38.589291 mypy-boto3-servicecatalog-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:46:40.000000 mypy-boto3-servicecatalog-1.28.12/setup.py
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/LICENSE` & `mypy-boto3-servicecatalog-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceCatalog 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,44 +439,42 @@
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
+    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
+    TagOutputTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -503,110 +501,101 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
+    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
+    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
+    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
-    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
+    CreatePortfolioOutputTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -614,28 +603,44 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/README.md` & `mypy-boto3-servicecatalog-1.28.12/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -407,44 +407,42 @@
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
+    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
+    TagOutputTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -471,110 +469,101 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
+    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
+    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
+    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
-    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
+    CreatePortfolioOutputTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -582,28 +571,44 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__init__.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__init__.pyi` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/__main__.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceCatalog 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ServiceCatalog 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/client.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/client.pyi` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/literals.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
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
@@ -364,26 +365,28 @@
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

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/literals.pyi` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,15 @@
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
@@ -362,26 +363,28 @@
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

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/paginator.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 
@@ -147,15 +147,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 
@@ -166,15 +166,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 
@@ -186,30 +186,30 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 
 class ListPortfoliosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliospaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortfoliosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliospaginator)
         """
 
 
@@ -220,15 +220,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 
@@ -239,15 +239,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 
@@ -259,15 +259,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 
@@ -278,15 +278,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 
@@ -298,15 +298,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 
@@ -317,30 +317,30 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 
 class ListServiceActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionspaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionspaginator)
         """
 
 
@@ -352,15 +352,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 
@@ -370,15 +370,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 
@@ -389,15 +389,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 
@@ -412,13 +412,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/paginator.pyi` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         PortfolioShareType: PortfolioShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAcceptedPortfolioSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListAcceptedPortfolioShares.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listacceptedportfoliosharespaginator)
         """
 
 class ListConstraintsForPortfolioPaginator(Paginator):
@@ -142,15 +142,15 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConstraintsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListConstraintsForPortfolio.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listconstraintsforportfoliopaginator)
         """
 
 class ListLaunchPathsPaginator(Paginator):
@@ -160,15 +160,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLaunchPathsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListLaunchPaths.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listlaunchpathspaginator)
         """
 
 class ListOrganizationPortfolioAccessPaginator(Paginator):
@@ -179,29 +179,29 @@
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         OrganizationNodeType: OrganizationNodeTypeType,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationPortfolioAccessOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListOrganizationPortfolioAccess.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listorganizationportfolioaccesspaginator)
         """
 
 class ListPortfoliosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliospaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortfoliosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfolios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliospaginator)
         """
 
 class ListPortfoliosForProductPaginator(Paginator):
@@ -211,15 +211,15 @@
     """
 
     def paginate(
         self,
         *,
         ProductId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPortfoliosForProductOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPortfoliosForProduct.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listportfoliosforproductpaginator)
         """
 
 class ListPrincipalsForPortfolioPaginator(Paginator):
@@ -229,15 +229,15 @@
     """
 
     def paginate(
         self,
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalsForPortfolioOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListPrincipalsForPortfolio.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprincipalsforportfoliopaginator)
         """
 
 class ListProvisionedProductPlansPaginator(Paginator):
@@ -248,15 +248,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisionProductId: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisionedProductPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisionedProductPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprovisionedproductplanspaginator)
         """
 
 class ListProvisioningArtifactsForServiceActionPaginator(Paginator):
@@ -266,15 +266,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceActionId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningArtifactsForServiceActionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListProvisioningArtifactsForServiceAction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listprovisioningartifactsforserviceactionpaginator)
         """
 
 class ListRecordHistoryPaginator(Paginator):
@@ -285,15 +285,15 @@
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
         SearchFilter: ListRecordHistorySearchFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRecordHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListRecordHistory.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listrecordhistorypaginator)
         """
 
 class ListResourcesForTagOptionPaginator(Paginator):
@@ -303,29 +303,29 @@
     """
 
     def paginate(
         self,
         *,
         TagOptionId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesForTagOptionOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListResourcesForTagOption.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listresourcesfortagoptionpaginator)
         """
 
 class ListServiceActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionspaginator)
     """
 
     def paginate(
-        self, *, AcceptLanguage: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceptLanguage: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionspaginator)
         """
 
 class ListServiceActionsForProvisioningArtifactPaginator(Paginator):
@@ -336,15 +336,15 @@
 
     def paginate(
         self,
         *,
         ProductId: str,
         ProvisioningArtifactId: str,
         AcceptLanguage: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServiceActionsForProvisioningArtifactOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListServiceActionsForProvisioningArtifact.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listserviceactionsforprovisioningartifactpaginator)
         """
 
 class ListTagOptionsPaginator(Paginator):
@@ -353,15 +353,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listtagoptionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListTagOptionsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagOptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ListTagOptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#listtagoptionspaginator)
         """
 
 class ScanProvisionedProductsPaginator(Paginator):
@@ -371,15 +371,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceptLanguage: str = ...,
         AccessLevelFilter: AccessLevelFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ScanProvisionedProductsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.ScanProvisionedProducts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#scanprovisionedproductspaginator)
         """
 
 class SearchProductsAsAdminPaginator(Paginator):
@@ -393,13 +393,13 @@
         *,
         AcceptLanguage: str = ...,
         PortfolioId: str = ...,
         Filters: Mapping[ProductViewFilterByType, Sequence[str]] = ...,
         SortBy: ProductViewSortByType = ...,
         SortOrder: SortOrderType = ...,
         ProductSource: Literal["ACCOUNT"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchProductsAsAdminOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Paginator.SearchProductsAsAdmin.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/paginators/#searchproductsasadminpaginator)
         """
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/type_defs.py` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,44 +64,42 @@
     "AssociateBudgetWithResourceInputRequestTypeDef",
     "AssociatePrincipalWithPortfolioInputRequestTypeDef",
     "AssociateProductWithPortfolioInputRequestTypeDef",
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
+    "CodeStarParametersOutputTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
-    "CopyProductOutputTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
+    "TagOutputTypeDef",
     "OrganizationNodeTypeDef",
-    "CreatePortfolioShareOutputTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
-    "CreateProvisionedProductPlanOutputTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
     "DeleteConstraintInputRequestTypeDef",
     "DeletePortfolioInputRequestTypeDef",
-    "DeletePortfolioShareOutputTypeDef",
     "DeleteProductInputRequestTypeDef",
     "DeleteProvisionedProductPlanInputRequestTypeDef",
     "DeleteProvisioningArtifactInputRequestTypeDef",
     "DeleteServiceActionInputRequestTypeDef",
     "DeleteTagOptionInputRequestTypeDef",
     "DescribeConstraintInputRequestTypeDef",
     "DescribeCopyProductStatusInputRequestTypeDef",
-    "DescribeCopyProductStatusOutputTypeDef",
     "DescribePortfolioInputRequestTypeDef",
     "DescribePortfolioShareStatusInputRequestTypeDef",
     "DescribePortfolioSharesInputRequestTypeDef",
     "PortfolioShareDetailTypeDef",
     "DescribeProductAsAdminInputRequestTypeDef",
     "ProvisioningArtifactSummaryTypeDef",
     "DescribeProductInputRequestTypeDef",
@@ -128,110 +126,101 @@
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
-    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
-    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
+    "OrganizationNodeOutputTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
-    "ListPortfolioAccessOutputTypeDef",
-    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPortfoliosInputRequestTypeDef",
-    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
-    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     "ListProvisioningArtifactsInputRequestTypeDef",
     "ListRecordHistorySearchFilterTypeDef",
-    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListResourcesForTagOptionInputRequestTypeDef",
     "ResourceDetailTypeDef",
-    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
+    "UpdateProvisioningParameterOutputTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
     "TerminateProvisionedProductInputRequestTypeDef",
     "UpdateConstraintInputRequestTypeDef",
-    "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisioningPreferencesTypeDef",
     "UpdateProvisionedProductPropertiesInputRequestTypeDef",
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "UpdateProvisioningArtifactInputRequestTypeDef",
     "UpdateServiceActionInputRequestTypeDef",
     "UpdateTagOptionInputRequestTypeDef",
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisionedProductPlansInputRequestTypeDef",
     "ScanProvisionedProductsInputRequestTypeDef",
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProvisionedProductsInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
+    "CopyProductOutputTypeDef",
+    "CreatePortfolioShareOutputTypeDef",
+    "CreateProvisionedProductPlanOutputTypeDef",
+    "DeletePortfolioShareOutputTypeDef",
+    "DescribeCopyProductStatusOutputTypeDef",
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    "ListPortfolioAccessOutputTypeDef",
+    "UpdatePortfolioShareOutputTypeDef",
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
+    "SourceConnectionParametersOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
-    "LaunchPathSummaryTypeDef",
-    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioInputRequestTypeDef",
-    "CreatePortfolioOutputTypeDef",
     "ListAcceptedPortfolioSharesOutputTypeDef",
     "ListPortfoliosForProductOutputTypeDef",
     "ListPortfoliosOutputTypeDef",
+    "CreatePortfolioOutputTypeDef",
+    "LaunchPathSummaryTypeDef",
+    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
-    "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
     "ListTagOptionsOutputTypeDef",
     "UpdateTagOptionOutputTypeDef",
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
@@ -239,28 +228,44 @@
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
     "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     "EngineWorkflowResourceIdentifierTypeDef",
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    "ListOrganizationPortfolioAccessOutputTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
     "ServiceActionDetailTypeDef",
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     "ListTagOptionsInputRequestTypeDef",
     "ProvisioningArtifactParameterTypeDef",
     "SearchProductsOutputTypeDef",
     "ProvisionProductInputRequestTypeDef",
+    "ProvisionedProductPlanDetailsTypeDef",
     "RecordDetailTypeDef",
     "ResourceChangeDetailTypeDef",
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
@@ -429,14 +434,25 @@
         "ProvisioningArtifactId": str,
         "ErrorCode": ServiceActionAssociationErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
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
 BudgetDetailTypeDef = TypedDict(
     "BudgetDetailTypeDef",
     {
         "BudgetName": str,
     },
     total=False,
 )
@@ -445,14 +461,24 @@
     "CloudWatchDashboardTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+CodeStarParametersOutputTypeDef = TypedDict(
+    "CodeStarParametersOutputTypeDef",
+    {
+        "ConnectionArn": str,
+        "Repository": str,
+        "Branch": str,
+        "ArtifactPath": str,
+    },
+)
+
 CodeStarParametersTypeDef = TypedDict(
     "CodeStarParametersTypeDef",
     {
         "ConnectionArn": str,
         "Repository": str,
         "Branch": str,
         "ArtifactPath": str,
@@ -503,22 +529,14 @@
 
 class CopyProductInputRequestTypeDef(
     _RequiredCopyProductInputRequestTypeDef, _OptionalCopyProductInputRequestTypeDef
 ):
     pass
 
 
-CopyProductOutputTypeDef = TypedDict(
-    "CopyProductOutputTypeDef",
-    {
-        "CopyProductToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredCreateConstraintInputRequestTypeDef",
     {
         "PortfolioId": str,
         "ProductId": str,
         "Parameters": str,
         "Type": str,
@@ -558,29 +576,29 @@
         "Description": str,
         "CreatedTime": datetime,
         "ProviderName": str,
     },
     total=False,
 )
 
-OrganizationNodeTypeDef = TypedDict(
-    "OrganizationNodeTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Type": OrganizationNodeTypeType,
+        "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
-CreatePortfolioShareOutputTypeDef = TypedDict(
-    "CreatePortfolioShareOutputTypeDef",
+OrganizationNodeTypeDef = TypedDict(
+    "OrganizationNodeTypeDef",
     {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": OrganizationNodeTypeType,
+        "Value": str,
     },
+    total=False,
 )
 
 ProvisioningArtifactPropertiesTypeDef = TypedDict(
     "ProvisioningArtifactPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
@@ -612,26 +630,14 @@
         "Key": str,
         "Value": str,
         "UsePreviousValue": bool,
     },
     total=False,
 )
 
-CreateProvisionedProductPlanOutputTypeDef = TypedDict(
-    "CreateProvisionedProductPlanOutputTypeDef",
-    {
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionedProductName": str,
-        "ProvisioningArtifactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceActionInputRequestTypeDef",
     {
         "Name": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "IdempotencyToken": str,
@@ -711,22 +717,14 @@
 
 class DeletePortfolioInputRequestTypeDef(
     _RequiredDeletePortfolioInputRequestTypeDef, _OptionalDeletePortfolioInputRequestTypeDef
 ):
     pass
 
 
-DeletePortfolioShareOutputTypeDef = TypedDict(
-    "DeletePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProductInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteProductInputRequestTypeDef = TypedDict(
@@ -857,24 +855,14 @@
 class DescribeCopyProductStatusInputRequestTypeDef(
     _RequiredDescribeCopyProductStatusInputRequestTypeDef,
     _OptionalDescribeCopyProductStatusInputRequestTypeDef,
 ):
     pass
 
 
-DescribeCopyProductStatusOutputTypeDef = TypedDict(
-    "DescribeCopyProductStatusOutputTypeDef",
-    {
-        "CopyProductStatus": CopyProductStatusType,
-        "TargetProductId": str,
-        "StatusDetail": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDescribePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribePortfolioInputRequestTypeDef = TypedDict(
@@ -1382,22 +1370,14 @@
 class ExecuteProvisionedProductServiceActionInputRequestTypeDef(
     _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef,
     _OptionalExecuteProvisionedProductServiceActionInputRequestTypeDef,
 ):
     pass
 
 
-GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
-    {
-        "AccessStatus": AccessStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProvisionedProductOutputsInputRequestTypeDef = TypedDict(
     "GetProvisionedProductOutputsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionedProductId": str,
         "ProvisionedProductName": str,
         "OutputKeys": Sequence[str],
@@ -1441,20 +1421,20 @@
         "LastSyncStatusMessage": str,
         "LastSuccessfulSyncTime": datetime,
         "LastSuccessfulSyncProvisioningArtifactId": str,
     },
     total=False,
 )
 
-ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AcceptLanguage": str,
-        "PortfolioShareType": PortfolioShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAcceptedPortfolioSharesInputRequestTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     {
@@ -1486,38 +1466,14 @@
 class ListBudgetsForResourceInputRequestTypeDef(
     _RequiredListBudgetsForResourceInputRequestTypeDef,
     _OptionalListBudgetsForResourceInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProductId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
-    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListConstraintsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1535,37 +1491,14 @@
 class ListConstraintsForPortfolioInputRequestTypeDef(
     _RequiredListConstraintsForPortfolioInputRequestTypeDef,
     _OptionalListConstraintsForPortfolioInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
-    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchPathsInputRequestTypeDef = TypedDict(
     "_RequiredListLaunchPathsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListLaunchPathsInputRequestTypeDef = TypedDict(
@@ -1581,38 +1514,14 @@
 
 class ListLaunchPathsInputRequestTypeDef(
     _RequiredListLaunchPathsInputRequestTypeDef, _OptionalListLaunchPathsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "PortfolioId": str,
-        "OrganizationNodeType": OrganizationNodeTypeType,
-    },
-)
-_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
-    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListOrganizationPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListOrganizationPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
         "OrganizationNodeType": OrganizationNodeTypeType,
     },
 )
@@ -1630,14 +1539,23 @@
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
 
+OrganizationNodeOutputTypeDef = TypedDict(
+    "OrganizationNodeOutputTypeDef",
+    {
+        "Type": OrganizationNodeTypeType,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1654,46 +1572,14 @@
 
 class ListPortfolioAccessInputRequestTypeDef(
     _RequiredListPortfolioAccessInputRequestTypeDef, _OptionalListPortfolioAccessInputRequestTypeDef
 ):
     pass
 
 
-ListPortfolioAccessOutputTypeDef = TypedDict(
-    "ListPortfolioAccessOutputTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
-    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPortfoliosForProductInputRequestTypeDef = TypedDict(
     "_RequiredListPortfoliosForProductInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListPortfoliosForProductInputRequestTypeDef = TypedDict(
@@ -1710,56 +1596,24 @@
 class ListPortfoliosForProductInputRequestTypeDef(
     _RequiredListPortfoliosForProductInputRequestTypeDef,
     _OptionalListPortfoliosForProductInputRequestTypeDef,
 ):
     pass
 
 
-ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPortfoliosInputRequestTypeDef = TypedDict(
     "ListPortfoliosInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
-    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1798,37 +1652,14 @@
         "ProvisionProductName": str,
         "PlanType": Literal["CLOUDFORMATION"],
         "ProvisioningArtifactId": str,
     },
     total=False,
 )
 
-_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "ServiceActionId": str,
-    },
-)
-_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
-    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     {
         "ServiceActionId": str,
     },
 )
 _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
@@ -1876,37 +1707,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "TagOptionId": str,
-    },
-)
-_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
-    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesForTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesForTagOptionInputRequestTypeDef",
     {
         "TagOptionId": str,
     },
 )
 _OptionalListResourcesForTagOptionInputRequestTypeDef = TypedDict(
@@ -1935,38 +1743,14 @@
         "Name": str,
         "Description": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "ProductId": str,
-        "ProvisioningArtifactId": str,
-    },
-)
-_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
-    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -1995,23 +1779,14 @@
         "Name": str,
         "Description": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
     },
     total=False,
 )
 
-ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceActionsInputRequestTypeDef = TypedDict(
     "ListServiceActionsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
@@ -2083,24 +1858,14 @@
 class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
         "MaxLength": str,
@@ -2138,14 +1903,24 @@
         "StackSetFailureTolerancePercentage": int,
         "StackSetMaxConcurrencyCount": int,
         "StackSetMaxConcurrencyPercentage": int,
     },
     total=False,
 )
 
+UpdateProvisioningParameterOutputTypeDef = TypedDict(
+    "UpdateProvisioningParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "UsePreviousValue": bool,
+    },
+    total=False,
+)
+
 RecordErrorTypeDef = TypedDict(
     "RecordErrorTypeDef",
     {
         "Code": str,
         "Description": str,
     },
     total=False,
@@ -2189,25 +1964,14 @@
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SearchProductsAsAdminInputRequestTypeDef = TypedDict(
     "SearchProductsAsAdminInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioId": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "SortBy": ProductViewSortByType,
@@ -2215,28 +1979,14 @@
         "PageToken": str,
         "PageSize": int,
         "ProductSource": Literal["ACCOUNT"],
     },
     total=False,
 )
 
-SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PortfolioId": str,
-        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
-        "SortBy": ProductViewSortByType,
-        "SortOrder": SortOrderType,
-        "ProductSource": Literal["ACCOUNT"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProductsInputRequestTypeDef = TypedDict(
     "SearchProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "PageSize": int,
         "SortBy": ProductViewSortByType,
@@ -2301,23 +2051,14 @@
 
 class UpdateConstraintInputRequestTypeDef(
     _RequiredUpdateConstraintInputRequestTypeDef, _OptionalUpdateConstraintInputRequestTypeDef
 ):
     pass
 
 
-UpdatePortfolioShareOutputTypeDef = TypedDict(
-    "UpdatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "Status": ShareStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateProvisioningPreferencesTypeDef = TypedDict(
     "UpdateProvisioningPreferencesTypeDef",
     {
         "StackSetAccounts": Sequence[str],
         "StackSetRegions": Sequence[str],
         "StackSetFailureToleranceCount": int,
         "StackSetFailureTolerancePercentage": int,
@@ -2348,25 +2089,14 @@
 class UpdateProvisionedProductPropertiesInputRequestTypeDef(
     _RequiredUpdateProvisionedProductPropertiesInputRequestTypeDef,
     _OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef,
 ):
     pass
 
 
-UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
-    {
-        "ProvisionedProductId": str,
-        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
-        "RecordId": str,
-        "Status": RecordStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -2432,25 +2162,14 @@
 
 class UpdateTagOptionInputRequestTypeDef(
     _RequiredUpdateTagOptionInputRequestTypeDef, _OptionalUpdateTagOptionInputRequestTypeDef
 ):
     pass
 
 
-ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProvisionProductId": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisionedProductPlansInputRequestTypeDef = TypedDict(
     "ListProvisionedProductPlansInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionProductId": str,
         "PageSize": int,
         "PageToken": str,
@@ -2466,24 +2185,14 @@
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProvisionedProductsInputRequestTypeDef = TypedDict(
     "SearchProvisionedProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "Filters": Mapping[Literal["SearchQuery"], Sequence[str]],
         "SortBy": str,
@@ -2538,33 +2247,124 @@
     pass
 
 
 BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyProductOutputTypeDef = TypedDict(
+    "CopyProductOutputTypeDef",
+    {
+        "CopyProductToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortfolioShareOutputTypeDef = TypedDict(
+    "CreatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisionedProductPlanOutputTypeDef = TypedDict(
+    "CreateProvisionedProductPlanOutputTypeDef",
+    {
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionedProductName": str,
+        "ProvisioningArtifactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePortfolioShareOutputTypeDef = TypedDict(
+    "DeletePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCopyProductStatusOutputTypeDef = TypedDict(
+    "DescribeCopyProductStatusOutputTypeDef",
+    {
+        "CopyProductStatus": CopyProductStatusType,
+        "TargetProductId": str,
+        "StatusDetail": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    {
+        "AccessStatus": AccessStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPortfolioAccessOutputTypeDef = TypedDict(
+    "ListPortfolioAccessOutputTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePortfolioShareOutputTypeDef = TypedDict(
+    "UpdatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "Status": ShareStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
+    {
+        "ProvisionedProductId": str,
+        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
+        "RecordId": str,
+        "Status": RecordStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBudgetsForResourceOutputTypeDef = TypedDict(
     "ListBudgetsForResourceOutputTypeDef",
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SourceConnectionParametersOutputTypeDef = TypedDict(
+    "SourceConnectionParametersOutputTypeDef",
+    {
+        "CodeStar": CodeStarParametersOutputTypeDef,
     },
+    total=False,
 )
 
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
     },
@@ -2573,44 +2373,44 @@
 
 CreateConstraintOutputTypeDef = TypedDict(
     "CreateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConstraintOutputTypeDef = TypedDict(
     "DescribeConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConstraintsForPortfolioOutputTypeDef = TypedDict(
     "ListConstraintsForPortfolioOutputTypeDef",
     {
         "ConstraintDetails": List[ConstraintDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConstraintOutputTypeDef = TypedDict(
     "UpdateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioInputRequestTypeDef",
     {
         "DisplayName": str,
@@ -2631,51 +2431,14 @@
 
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
 
-LaunchPathSummaryTypeDef = TypedDict(
-    "LaunchPathSummaryTypeDef",
-    {
-        "Id": str,
-        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
-        "Tags": List[TagTypeDef],
-        "Name": str,
-    },
-    total=False,
-)
-
-ProvisionedProductAttributeTypeDef = TypedDict(
-    "ProvisionedProductAttributeTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Type": str,
-        "Id": str,
-        "Status": ProvisionedProductStatusType,
-        "StatusMessage": str,
-        "CreatedTime": datetime,
-        "IdempotencyToken": str,
-        "LastRecordId": str,
-        "LastProvisioningRecordId": str,
-        "LastSuccessfulProvisioningRecordId": str,
-        "Tags": List[TagTypeDef],
-        "PhysicalId": str,
-        "ProductId": str,
-        "ProductName": str,
-        "ProvisioningArtifactId": str,
-        "ProvisioningArtifactName": str,
-        "UserArn": str,
-        "UserArnSession": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePortfolioInputRequestTypeDef = TypedDict(
@@ -2694,56 +2457,93 @@
 
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
 
-CreatePortfolioOutputTypeDef = TypedDict(
-    "CreatePortfolioOutputTypeDef",
-    {
-        "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosForProductOutputTypeDef = TypedDict(
     "ListPortfoliosForProductOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosOutputTypeDef = TypedDict(
     "ListPortfoliosOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreatePortfolioOutputTypeDef = TypedDict(
+    "CreatePortfolioOutputTypeDef",
+    {
+        "PortfolioDetail": PortfolioDetailTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LaunchPathSummaryTypeDef = TypedDict(
+    "LaunchPathSummaryTypeDef",
+    {
+        "Id": str,
+        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "Name": str,
+    },
+    total=False,
+)
+
+ProvisionedProductAttributeTypeDef = TypedDict(
+    "ProvisionedProductAttributeTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Type": str,
+        "Id": str,
+        "Status": ProvisionedProductStatusType,
+        "StatusMessage": str,
+        "CreatedTime": datetime,
+        "IdempotencyToken": str,
+        "LastRecordId": str,
+        "LastProvisioningRecordId": str,
+        "LastSuccessfulProvisioningRecordId": str,
+        "Tags": List[TagOutputTypeDef],
+        "PhysicalId": str,
+        "ProductId": str,
+        "ProductName": str,
+        "ProvisioningArtifactId": str,
+        "ProvisioningArtifactName": str,
+        "UserArn": str,
+        "UserArnSession": str,
+    },
+    total=False,
+)
+
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2789,23 +2589,14 @@
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
 
-ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
-    "ListOrganizationPortfolioAccessOutputTypeDef",
-    {
-        "OrganizationNodes": List[OrganizationNodeTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalUpdatePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2854,34 +2645,34 @@
 
 CreateProvisioningArtifactOutputTypeDef = TypedDict(
     "CreateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisioningArtifactOutputTypeDef = TypedDict(
     "UpdateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanName": str,
@@ -2908,106 +2699,84 @@
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
 
-ProvisionedProductPlanDetailsTypeDef = TypedDict(
-    "ProvisionedProductPlanDetailsTypeDef",
-    {
-        "CreatedTime": datetime,
-        "PathId": str,
-        "ProductId": str,
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionProductName": str,
-        "PlanType": Literal["CLOUDFORMATION"],
-        "ProvisioningArtifactId": str,
-        "Status": ProvisionedProductPlanStatusType,
-        "UpdatedTime": datetime,
-        "NotificationArns": List[str],
-        "ProvisioningParameters": List[UpdateProvisioningParameterTypeDef],
-        "Tags": List[TagTypeDef],
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
     "DescribeTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsOutputTypeDef = TypedDict(
     "ListTagOptionsOutputTypeDef",
     {
         "TagOptionDetails": List[TagOptionDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTagOptionOutputTypeDef = TypedDict(
     "UpdateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioSharesOutputTypeDef = TypedDict(
     "DescribePortfolioSharesOutputTypeDef",
     {
         "NextPageToken": str,
         "PortfolioShareDetails": List[PortfolioShareDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductOutputTypeDef = TypedDict(
     "DescribeProductOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "LaunchPaths": List[LaunchPathTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductViewOutputTypeDef = TypedDict(
     "DescribeProductViewOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisioningArtifactViewTypeDef = TypedDict(
     "ProvisioningArtifactViewTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3017,33 +2786,33 @@
 )
 
 DescribeProvisionedProductOutputTypeDef = TypedDict(
     "DescribeProvisionedProductOutputTypeDef",
     {
         "ProvisionedProductDetail": ProvisionedProductDetailTypeDef,
         "CloudWatchDashboards": List[CloudWatchDashboardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanProvisionedProductsOutputTypeDef = TypedDict(
     "ScanProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProvisionedProductOutputsOutputTypeDef = TypedDict(
     "GetProvisionedProductOutputsOutputTypeDef",
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3069,51 +2838,310 @@
     pass
 
 
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineWorkflowResourceIdentifierTypeDef = TypedDict(
     "EngineWorkflowResourceIdentifierTypeDef",
     {
         "UniqueTag": UniqueTagResourceIdentifierTypeDef,
     },
     total=False,
 )
 
+ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioShareType": PortfolioShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProductId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
+    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
+    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "PortfolioId": str,
+        "OrganizationNodeType": OrganizationNodeTypeType,
+    },
+)
+_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
+    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
+    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+):
+    pass
+
+
+ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
+    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+):
+    pass
+
+
+ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProvisionProductId": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "ServiceActionId": str,
+    },
+)
+_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
+    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "TagOptionId": str,
+    },
+)
+_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
+    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": str,
+    },
+)
+_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
+    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+):
+    pass
+
+
+ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioId": str,
+        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
+        "SortBy": ProductViewSortByType,
+        "SortOrder": SortOrderType,
+        "ProductSource": Literal["ACCOUNT"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
+    "ListOrganizationPortfolioAccessOutputTypeDef",
+    {
+        "OrganizationNodes": List[OrganizationNodeOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedProductPlansOutputTypeDef = TypedDict(
     "ListProvisionedProductPlansOutputTypeDef",
     {
         "ProvisionedProductPlans": List[ProvisionedProductPlanSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryInputListRecordHistoryPaginateTypeDef = TypedDict(
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "SearchFilter": ListRecordHistorySearchFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRecordHistoryInputRequestTypeDef = TypedDict(
     "ListRecordHistoryInputRequestTypeDef",
     {
@@ -3127,33 +3155,33 @@
 )
 
 ListResourcesForTagOptionOutputTypeDef = TypedDict(
     "ListResourcesForTagOptionOutputTypeDef",
     {
         "ResourceDetails": List[ResourceDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsForProvisioningArtifactOutputTypeDef = TypedDict(
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsOutputTypeDef = TypedDict(
     "ListServiceActionsOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceActionDetailTypeDef = TypedDict(
     "ServiceActionDetailTypeDef",
     {
         "ServiceActionSummary": ServiceActionSummaryTypeDef,
@@ -3163,23 +3191,23 @@
 )
 
 ListStackInstancesForProvisionedProductOutputTypeDef = TypedDict(
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     {
         "StackInstances": List[StackInstanceTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsInputListTagOptionsPaginateTypeDef = TypedDict(
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     {
         "Filters": ListTagOptionsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTagOptionsInputRequestTypeDef = TypedDict(
     "ListTagOptionsInputRequestTypeDef",
     {
@@ -3205,15 +3233,15 @@
 
 SearchProductsOutputTypeDef = TypedDict(
     "SearchProductsOutputTypeDef",
     {
         "ProductViewSummaries": List[ProductViewSummaryTypeDef],
         "ProductViewAggregations": Dict[str, List[ProductViewAggregationValueTypeDef]],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionProductInputRequestTypeDef = TypedDict(
     "_RequiredProvisionProductInputRequestTypeDef",
     {
         "ProvisionedProductName": str,
@@ -3241,14 +3269,36 @@
 
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
 
+ProvisionedProductPlanDetailsTypeDef = TypedDict(
+    "ProvisionedProductPlanDetailsTypeDef",
+    {
+        "CreatedTime": datetime,
+        "PathId": str,
+        "ProductId": str,
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionProductName": str,
+        "PlanType": Literal["CLOUDFORMATION"],
+        "ProvisioningArtifactId": str,
+        "Status": ProvisionedProductPlanStatusType,
+        "UpdatedTime": datetime,
+        "NotificationArns": List[str],
+        "ProvisioningParameters": List[UpdateProvisioningParameterOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3318,15 +3368,15 @@
     pass
 
 
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
-        "ConnectionParameters": SourceConnectionParametersTypeDef,
+        "ConnectionParameters": SourceConnectionParametersOutputTypeDef,
         "LastSync": LastSyncTypeDef,
     },
     total=False,
 )
 
 _RequiredSourceConnectionTypeDef = TypedDict(
     "_RequiredSourceConnectionTypeDef",
@@ -3348,34 +3398,34 @@
 
 
 ListLaunchPathsOutputTypeDef = TypedDict(
     "ListLaunchPathsOutputTypeDef",
     {
         "LaunchPathSummaries": List[LaunchPathSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProvisionedProductsOutputTypeDef = TypedDict(
     "SearchProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductAttributeTypeDef],
         "TotalResultsCount": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsForServiceActionOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3402,123 +3452,123 @@
     pass
 
 
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceActionOutputTypeDef = TypedDict(
     "DescribeServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceActionOutputTypeDef = TypedDict(
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningArtifactOutputTypeDef = TypedDict(
     "DescribeProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
         "ProvisioningArtifactPreferences": ProvisioningArtifactPreferencesTypeDef,
         "ProvisioningArtifactOutputs": List[ProvisioningArtifactOutputTypeDef],
         "ProvisioningArtifactOutputKeys": List[ProvisioningArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecordOutputTypeDef = TypedDict(
     "DescribeRecordOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
         "RecordOutputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductPlanOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductPlanOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductServiceActionOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportAsProvisionedProductOutputTypeDef = TypedDict(
     "ImportAsProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryOutputTypeDef = TypedDict(
     "ListRecordHistoryOutputTypeDef",
     {
         "RecordDetails": List[RecordDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionProductOutputTypeDef = TypedDict(
     "ProvisionProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateProvisionedProductOutputTypeDef = TypedDict(
     "TerminateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisionedProductOutputTypeDef = TypedDict(
     "UpdateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3536,15 +3586,15 @@
     "DescribePortfolioShareStatusOutputTypeDef",
     {
         "PortfolioShareToken": str,
         "PortfolioId": str,
         "OrganizationNodeValue": str,
         "Status": ShareStatusType,
         "ShareDetails": ShareDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProductViewDetailTypeDef = TypedDict(
     "ProductViewDetailTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3621,50 +3671,50 @@
 
 DescribeProvisionedProductPlanOutputTypeDef = TypedDict(
     "DescribeProvisionedProductPlanOutputTypeDef",
     {
         "ProvisionedProductPlanDetails": ProvisionedProductPlanDetailsTypeDef,
         "ResourceChanges": List[ResourceChangeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
     "SearchProductsAsAdminOutputTypeDef",
     {
         "ProductViewDetails": List[ProductViewDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog/type_defs.pyi` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,44 +63,42 @@
     "AssociateBudgetWithResourceInputRequestTypeDef",
     "AssociatePrincipalWithPortfolioInputRequestTypeDef",
     "AssociateProductWithPortfolioInputRequestTypeDef",
     "AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "AssociateTagOptionWithResourceInputRequestTypeDef",
     "ServiceActionAssociationTypeDef",
     "FailedServiceActionAssociationTypeDef",
+    "ResponseMetadataTypeDef",
     "BudgetDetailTypeDef",
     "CloudWatchDashboardTypeDef",
+    "CodeStarParametersOutputTypeDef",
     "CodeStarParametersTypeDef",
     "ConstraintDetailTypeDef",
     "ConstraintSummaryTypeDef",
     "CopyProductInputRequestTypeDef",
-    "CopyProductOutputTypeDef",
     "CreateConstraintInputRequestTypeDef",
     "TagTypeDef",
     "PortfolioDetailTypeDef",
+    "TagOutputTypeDef",
     "OrganizationNodeTypeDef",
-    "CreatePortfolioShareOutputTypeDef",
     "ProvisioningArtifactPropertiesTypeDef",
     "ProvisioningArtifactDetailTypeDef",
     "UpdateProvisioningParameterTypeDef",
-    "CreateProvisionedProductPlanOutputTypeDef",
     "CreateServiceActionInputRequestTypeDef",
     "CreateTagOptionInputRequestTypeDef",
     "TagOptionDetailTypeDef",
     "DeleteConstraintInputRequestTypeDef",
     "DeletePortfolioInputRequestTypeDef",
-    "DeletePortfolioShareOutputTypeDef",
     "DeleteProductInputRequestTypeDef",
     "DeleteProvisionedProductPlanInputRequestTypeDef",
     "DeleteProvisioningArtifactInputRequestTypeDef",
     "DeleteServiceActionInputRequestTypeDef",
     "DeleteTagOptionInputRequestTypeDef",
     "DescribeConstraintInputRequestTypeDef",
     "DescribeCopyProductStatusInputRequestTypeDef",
-    "DescribeCopyProductStatusOutputTypeDef",
     "DescribePortfolioInputRequestTypeDef",
     "DescribePortfolioShareStatusInputRequestTypeDef",
     "DescribePortfolioSharesInputRequestTypeDef",
     "PortfolioShareDetailTypeDef",
     "DescribeProductAsAdminInputRequestTypeDef",
     "ProvisioningArtifactSummaryTypeDef",
     "DescribeProductInputRequestTypeDef",
@@ -127,110 +125,101 @@
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     "ListBudgetsForResourceInputRequestTypeDef",
-    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListConstraintsForPortfolioInputRequestTypeDef",
-    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListLaunchPathsInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputRequestTypeDef",
+    "OrganizationNodeOutputTypeDef",
     "ListPortfolioAccessInputRequestTypeDef",
-    "ListPortfolioAccessOutputTypeDef",
-    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosForProductInputRequestTypeDef",
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPortfoliosInputRequestTypeDef",
-    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
     "ListPrincipalsForPortfolioInputRequestTypeDef",
     "PrincipalTypeDef",
     "ProvisionedProductPlanSummaryTypeDef",
-    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
     "ListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     "ListProvisioningArtifactsInputRequestTypeDef",
     "ListRecordHistorySearchFilterTypeDef",
-    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
     "ListResourcesForTagOptionInputRequestTypeDef",
     "ResourceDetailTypeDef",
-    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
     "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
+    "UpdateProvisioningParameterOutputTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchProductsAsAdminInputRequestTypeDef",
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
     "SearchProductsInputRequestTypeDef",
     "ShareErrorTypeDef",
     "TerminateProvisionedProductInputRequestTypeDef",
     "UpdateConstraintInputRequestTypeDef",
-    "UpdatePortfolioShareOutputTypeDef",
     "UpdateProvisioningPreferencesTypeDef",
     "UpdateProvisionedProductPropertiesInputRequestTypeDef",
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "UpdateProvisioningArtifactInputRequestTypeDef",
     "UpdateServiceActionInputRequestTypeDef",
     "UpdateTagOptionInputRequestTypeDef",
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
     "ListProvisionedProductPlansInputRequestTypeDef",
     "ScanProvisionedProductsInputRequestTypeDef",
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
     "SearchProvisionedProductsInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
+    "CopyProductOutputTypeDef",
+    "CreatePortfolioShareOutputTypeDef",
+    "CreateProvisionedProductPlanOutputTypeDef",
+    "DeletePortfolioShareOutputTypeDef",
+    "DescribeCopyProductStatusOutputTypeDef",
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    "ListPortfolioAccessOutputTypeDef",
+    "UpdatePortfolioShareOutputTypeDef",
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
     "ListBudgetsForResourceOutputTypeDef",
+    "SourceConnectionParametersOutputTypeDef",
     "SourceConnectionParametersTypeDef",
     "CreateConstraintOutputTypeDef",
     "DescribeConstraintOutputTypeDef",
     "ListConstraintsForPortfolioOutputTypeDef",
     "UpdateConstraintOutputTypeDef",
     "CreatePortfolioInputRequestTypeDef",
-    "LaunchPathSummaryTypeDef",
-    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioInputRequestTypeDef",
-    "CreatePortfolioOutputTypeDef",
     "ListAcceptedPortfolioSharesOutputTypeDef",
     "ListPortfoliosForProductOutputTypeDef",
     "ListPortfoliosOutputTypeDef",
+    "CreatePortfolioOutputTypeDef",
+    "LaunchPathSummaryTypeDef",
+    "ProvisionedProductAttributeTypeDef",
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
-    "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
-    "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
     "ListTagOptionsOutputTypeDef",
     "UpdateTagOptionOutputTypeDef",
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
@@ -238,28 +227,44 @@
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
     "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     "EngineWorkflowResourceIdentifierTypeDef",
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    "ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    "ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    "ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    "ListOrganizationPortfolioAccessOutputTypeDef",
     "ListPrincipalsForPortfolioOutputTypeDef",
     "ListProvisionedProductPlansOutputTypeDef",
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     "ListRecordHistoryInputRequestTypeDef",
     "ListResourcesForTagOptionOutputTypeDef",
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     "ListServiceActionsOutputTypeDef",
     "ServiceActionDetailTypeDef",
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     "ListTagOptionsInputRequestTypeDef",
     "ProvisioningArtifactParameterTypeDef",
     "SearchProductsOutputTypeDef",
     "ProvisionProductInputRequestTypeDef",
+    "ProvisionedProductPlanDetailsTypeDef",
     "RecordDetailTypeDef",
     "ResourceChangeDetailTypeDef",
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
@@ -420,14 +425,25 @@
         "ProvisioningArtifactId": str,
         "ErrorCode": ServiceActionAssociationErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
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
 BudgetDetailTypeDef = TypedDict(
     "BudgetDetailTypeDef",
     {
         "BudgetName": str,
     },
     total=False,
 )
@@ -436,14 +452,24 @@
     "CloudWatchDashboardTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+CodeStarParametersOutputTypeDef = TypedDict(
+    "CodeStarParametersOutputTypeDef",
+    {
+        "ConnectionArn": str,
+        "Repository": str,
+        "Branch": str,
+        "ArtifactPath": str,
+    },
+)
+
 CodeStarParametersTypeDef = TypedDict(
     "CodeStarParametersTypeDef",
     {
         "ConnectionArn": str,
         "Repository": str,
         "Branch": str,
         "ArtifactPath": str,
@@ -492,22 +518,14 @@
 )
 
 class CopyProductInputRequestTypeDef(
     _RequiredCopyProductInputRequestTypeDef, _OptionalCopyProductInputRequestTypeDef
 ):
     pass
 
-CopyProductOutputTypeDef = TypedDict(
-    "CopyProductOutputTypeDef",
-    {
-        "CopyProductToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateConstraintInputRequestTypeDef = TypedDict(
     "_RequiredCreateConstraintInputRequestTypeDef",
     {
         "PortfolioId": str,
         "ProductId": str,
         "Parameters": str,
         "Type": str,
@@ -545,29 +563,29 @@
         "Description": str,
         "CreatedTime": datetime,
         "ProviderName": str,
     },
     total=False,
 )
 
-OrganizationNodeTypeDef = TypedDict(
-    "OrganizationNodeTypeDef",
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
     {
-        "Type": OrganizationNodeTypeType,
+        "Key": str,
         "Value": str,
     },
-    total=False,
 )
 
-CreatePortfolioShareOutputTypeDef = TypedDict(
-    "CreatePortfolioShareOutputTypeDef",
+OrganizationNodeTypeDef = TypedDict(
+    "OrganizationNodeTypeDef",
     {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Type": OrganizationNodeTypeType,
+        "Value": str,
     },
+    total=False,
 )
 
 ProvisioningArtifactPropertiesTypeDef = TypedDict(
     "ProvisioningArtifactPropertiesTypeDef",
     {
         "Name": str,
         "Description": str,
@@ -599,26 +617,14 @@
         "Key": str,
         "Value": str,
         "UsePreviousValue": bool,
     },
     total=False,
 )
 
-CreateProvisionedProductPlanOutputTypeDef = TypedDict(
-    "CreateProvisionedProductPlanOutputTypeDef",
-    {
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionedProductName": str,
-        "ProvisioningArtifactId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredCreateServiceActionInputRequestTypeDef",
     {
         "Name": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
         "Definition": Mapping[ServiceActionDefinitionKeyType, str],
         "IdempotencyToken": str,
@@ -692,22 +698,14 @@
 )
 
 class DeletePortfolioInputRequestTypeDef(
     _RequiredDeletePortfolioInputRequestTypeDef, _OptionalDeletePortfolioInputRequestTypeDef
 ):
     pass
 
-DeletePortfolioShareOutputTypeDef = TypedDict(
-    "DeletePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteProductInputRequestTypeDef = TypedDict(
     "_RequiredDeleteProductInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDeleteProductInputRequestTypeDef = TypedDict(
@@ -826,24 +824,14 @@
 
 class DescribeCopyProductStatusInputRequestTypeDef(
     _RequiredDescribeCopyProductStatusInputRequestTypeDef,
     _OptionalDescribeCopyProductStatusInputRequestTypeDef,
 ):
     pass
 
-DescribeCopyProductStatusOutputTypeDef = TypedDict(
-    "DescribeCopyProductStatusOutputTypeDef",
-    {
-        "CopyProductStatus": CopyProductStatusType,
-        "TargetProductId": str,
-        "StatusDetail": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredDescribePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribePortfolioInputRequestTypeDef = TypedDict(
@@ -1327,22 +1315,14 @@
 
 class ExecuteProvisionedProductServiceActionInputRequestTypeDef(
     _RequiredExecuteProvisionedProductServiceActionInputRequestTypeDef,
     _OptionalExecuteProvisionedProductServiceActionInputRequestTypeDef,
 ):
     pass
 
-GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
-    "GetAWSOrganizationsAccessStatusOutputTypeDef",
-    {
-        "AccessStatus": AccessStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProvisionedProductOutputsInputRequestTypeDef = TypedDict(
     "GetProvisionedProductOutputsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionedProductId": str,
         "ProvisionedProductName": str,
         "OutputKeys": Sequence[str],
@@ -1384,20 +1364,20 @@
         "LastSyncStatusMessage": str,
         "LastSuccessfulSyncTime": datetime,
         "LastSuccessfulSyncProvisioningArtifactId": str,
     },
     total=False,
 )
 
-ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
-    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AcceptLanguage": str,
-        "PortfolioShareType": PortfolioShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAcceptedPortfolioSharesInputRequestTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
     {
@@ -1427,36 +1407,14 @@
 
 class ListBudgetsForResourceInputRequestTypeDef(
     _RequiredListBudgetsForResourceInputRequestTypeDef,
     _OptionalListBudgetsForResourceInputRequestTypeDef,
 ):
     pass
 
-_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProductId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
-    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
-):
-    pass
-
 _RequiredListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListConstraintsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListConstraintsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1472,35 +1430,14 @@
 
 class ListConstraintsForPortfolioInputRequestTypeDef(
     _RequiredListConstraintsForPortfolioInputRequestTypeDef,
     _OptionalListConstraintsForPortfolioInputRequestTypeDef,
 ):
     pass
 
-_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
-    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
-):
-    pass
-
 _RequiredListLaunchPathsInputRequestTypeDef = TypedDict(
     "_RequiredListLaunchPathsInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListLaunchPathsInputRequestTypeDef = TypedDict(
@@ -1514,36 +1451,14 @@
 )
 
 class ListLaunchPathsInputRequestTypeDef(
     _RequiredListLaunchPathsInputRequestTypeDef, _OptionalListLaunchPathsInputRequestTypeDef
 ):
     pass
 
-_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "PortfolioId": str,
-        "OrganizationNodeType": OrganizationNodeTypeType,
-    },
-)
-_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
-    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
-):
-    pass
-
 _RequiredListOrganizationPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListOrganizationPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
         "OrganizationNodeType": OrganizationNodeTypeType,
     },
 )
@@ -1559,14 +1474,23 @@
 
 class ListOrganizationPortfolioAccessInputRequestTypeDef(
     _RequiredListOrganizationPortfolioAccessInputRequestTypeDef,
     _OptionalListOrganizationPortfolioAccessInputRequestTypeDef,
 ):
     pass
 
+OrganizationNodeOutputTypeDef = TypedDict(
+    "OrganizationNodeOutputTypeDef",
+    {
+        "Type": OrganizationNodeTypeType,
+        "Value": str,
+    },
+    total=False,
+)
+
 _RequiredListPortfolioAccessInputRequestTypeDef = TypedDict(
     "_RequiredListPortfolioAccessInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPortfolioAccessInputRequestTypeDef = TypedDict(
@@ -1581,44 +1505,14 @@
 )
 
 class ListPortfolioAccessInputRequestTypeDef(
     _RequiredListPortfolioAccessInputRequestTypeDef, _OptionalListPortfolioAccessInputRequestTypeDef
 ):
     pass
 
-ListPortfolioAccessOutputTypeDef = TypedDict(
-    "ListPortfolioAccessOutputTypeDef",
-    {
-        "AccountIds": List[str],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
-    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
-    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
-):
-    pass
-
 _RequiredListPortfoliosForProductInputRequestTypeDef = TypedDict(
     "_RequiredListPortfoliosForProductInputRequestTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalListPortfoliosForProductInputRequestTypeDef = TypedDict(
@@ -1633,54 +1527,24 @@
 
 class ListPortfoliosForProductInputRequestTypeDef(
     _RequiredListPortfoliosForProductInputRequestTypeDef,
     _OptionalListPortfoliosForProductInputRequestTypeDef,
 ):
     pass
 
-ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
-    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPortfoliosInputRequestTypeDef = TypedDict(
     "ListPortfoliosInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageToken": str,
         "PageSize": int,
     },
     total=False,
 )
 
-_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "PortfolioId": str,
-    },
-)
-_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
-    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
     "_RequiredListPrincipalsForPortfolioInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalListPrincipalsForPortfolioInputRequestTypeDef = TypedDict(
@@ -1717,35 +1581,14 @@
         "ProvisionProductName": str,
         "PlanType": Literal["CLOUDFORMATION"],
         "ProvisioningArtifactId": str,
     },
     total=False,
 )
 
-_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "ServiceActionId": str,
-    },
-)
-_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
-    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
-):
-    pass
-
 _RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
     "_RequiredListProvisioningArtifactsForServiceActionInputRequestTypeDef",
     {
         "ServiceActionId": str,
     },
 )
 _OptionalListProvisioningArtifactsForServiceActionInputRequestTypeDef = TypedDict(
@@ -1789,35 +1632,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "TagOptionId": str,
-    },
-)
-_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
-    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesForTagOptionInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesForTagOptionInputRequestTypeDef",
     {
         "TagOptionId": str,
     },
 )
 _OptionalListResourcesForTagOptionInputRequestTypeDef = TypedDict(
@@ -1844,36 +1666,14 @@
         "Name": str,
         "Description": str,
         "CreatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "ProductId": str,
-        "ProvisioningArtifactId": str,
-    },
-)
-_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
-    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
-    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
-):
-    pass
-
 _RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -1900,23 +1700,14 @@
         "Name": str,
         "Description": str,
         "DefinitionType": Literal["SSM_AUTOMATION"],
     },
     total=False,
 )
 
-ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
-    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceActionsInputRequestTypeDef = TypedDict(
     "ListServiceActionsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PageSize": int,
         "PageToken": str,
     },
@@ -1984,24 +1775,14 @@
 
 class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
     _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
         "MaxLength": str,
@@ -2039,14 +1820,24 @@
         "StackSetFailureTolerancePercentage": int,
         "StackSetMaxConcurrencyCount": int,
         "StackSetMaxConcurrencyPercentage": int,
     },
     total=False,
 )
 
+UpdateProvisioningParameterOutputTypeDef = TypedDict(
+    "UpdateProvisioningParameterOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+        "UsePreviousValue": bool,
+    },
+    total=False,
+)
+
 RecordErrorTypeDef = TypedDict(
     "RecordErrorTypeDef",
     {
         "Code": str,
         "Description": str,
     },
     total=False,
@@ -2088,25 +1879,14 @@
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SearchProductsAsAdminInputRequestTypeDef = TypedDict(
     "SearchProductsAsAdminInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioId": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "SortBy": ProductViewSortByType,
@@ -2114,28 +1894,14 @@
         "PageToken": str,
         "PageSize": int,
         "ProductSource": Literal["ACCOUNT"],
     },
     total=False,
 )
 
-SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
-    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "PortfolioId": str,
-        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
-        "SortBy": ProductViewSortByType,
-        "SortOrder": SortOrderType,
-        "ProductSource": Literal["ACCOUNT"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProductsInputRequestTypeDef = TypedDict(
     "SearchProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
         "PageSize": int,
         "SortBy": ProductViewSortByType,
@@ -2196,23 +1962,14 @@
 )
 
 class UpdateConstraintInputRequestTypeDef(
     _RequiredUpdateConstraintInputRequestTypeDef, _OptionalUpdateConstraintInputRequestTypeDef
 ):
     pass
 
-UpdatePortfolioShareOutputTypeDef = TypedDict(
-    "UpdatePortfolioShareOutputTypeDef",
-    {
-        "PortfolioShareToken": str,
-        "Status": ShareStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateProvisioningPreferencesTypeDef = TypedDict(
     "UpdateProvisioningPreferencesTypeDef",
     {
         "StackSetAccounts": Sequence[str],
         "StackSetRegions": Sequence[str],
         "StackSetFailureToleranceCount": int,
         "StackSetFailureTolerancePercentage": int,
@@ -2241,25 +1998,14 @@
 
 class UpdateProvisionedProductPropertiesInputRequestTypeDef(
     _RequiredUpdateProvisionedProductPropertiesInputRequestTypeDef,
     _OptionalUpdateProvisionedProductPropertiesInputRequestTypeDef,
 ):
     pass
 
-UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
-    "UpdateProvisionedProductPropertiesOutputTypeDef",
-    {
-        "ProvisionedProductId": str,
-        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
-        "RecordId": str,
-        "Status": RecordStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateProvisioningArtifactInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningArtifactInputRequestTypeDef",
     {
         "ProductId": str,
         "ProvisioningArtifactId": str,
     },
 )
@@ -2319,25 +2065,14 @@
 )
 
 class UpdateTagOptionInputRequestTypeDef(
     _RequiredUpdateTagOptionInputRequestTypeDef, _OptionalUpdateTagOptionInputRequestTypeDef
 ):
     pass
 
-ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
-    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "ProvisionProductId": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisionedProductPlansInputRequestTypeDef = TypedDict(
     "ListProvisionedProductPlansInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "ProvisionProductId": str,
         "PageSize": int,
         "PageToken": str,
@@ -2353,24 +2088,14 @@
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "PageSize": int,
         "PageToken": str,
     },
     total=False,
 )
 
-ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
-    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
-    {
-        "AcceptLanguage": str,
-        "AccessLevelFilter": AccessLevelFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 SearchProvisionedProductsInputRequestTypeDef = TypedDict(
     "SearchProvisionedProductsInputRequestTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "Filters": Mapping[Literal["SearchQuery"], Sequence[str]],
         "SortBy": str,
@@ -2421,79 +2146,170 @@
 ):
     pass
 
 BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef = TypedDict(
     "BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef",
     {
         "FailedServiceActionAssociations": List[FailedServiceActionAssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CopyProductOutputTypeDef = TypedDict(
+    "CopyProductOutputTypeDef",
+    {
+        "CopyProductToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortfolioShareOutputTypeDef = TypedDict(
+    "CreatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisionedProductPlanOutputTypeDef = TypedDict(
+    "CreateProvisionedProductPlanOutputTypeDef",
+    {
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionedProductName": str,
+        "ProvisioningArtifactId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePortfolioShareOutputTypeDef = TypedDict(
+    "DeletePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCopyProductStatusOutputTypeDef = TypedDict(
+    "DescribeCopyProductStatusOutputTypeDef",
+    {
+        "CopyProductStatus": CopyProductStatusType,
+        "TargetProductId": str,
+        "StatusDetail": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAWSOrganizationsAccessStatusOutputTypeDef = TypedDict(
+    "GetAWSOrganizationsAccessStatusOutputTypeDef",
+    {
+        "AccessStatus": AccessStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPortfolioAccessOutputTypeDef = TypedDict(
+    "ListPortfolioAccessOutputTypeDef",
+    {
+        "AccountIds": List[str],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePortfolioShareOutputTypeDef = TypedDict(
+    "UpdatePortfolioShareOutputTypeDef",
+    {
+        "PortfolioShareToken": str,
+        "Status": ShareStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateProvisionedProductPropertiesOutputTypeDef = TypedDict(
+    "UpdateProvisionedProductPropertiesOutputTypeDef",
+    {
+        "ProvisionedProductId": str,
+        "ProvisionedProductProperties": Dict[PropertyKeyType, str],
+        "RecordId": str,
+        "Status": RecordStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBudgetsForResourceOutputTypeDef = TypedDict(
     "ListBudgetsForResourceOutputTypeDef",
     {
         "Budgets": List[BudgetDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SourceConnectionParametersOutputTypeDef = TypedDict(
+    "SourceConnectionParametersOutputTypeDef",
+    {
+        "CodeStar": CodeStarParametersOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConnectionParametersTypeDef = TypedDict(
     "SourceConnectionParametersTypeDef",
     {
         "CodeStar": CodeStarParametersTypeDef,
     },
     total=False,
 )
 
 CreateConstraintOutputTypeDef = TypedDict(
     "CreateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConstraintOutputTypeDef = TypedDict(
     "DescribeConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConstraintsForPortfolioOutputTypeDef = TypedDict(
     "ListConstraintsForPortfolioOutputTypeDef",
     {
         "ConstraintDetails": List[ConstraintDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConstraintOutputTypeDef = TypedDict(
     "UpdateConstraintOutputTypeDef",
     {
         "ConstraintDetail": ConstraintDetailTypeDef,
         "ConstraintParameters": str,
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioInputRequestTypeDef",
     {
         "DisplayName": str,
@@ -2512,51 +2328,14 @@
 )
 
 class CreatePortfolioInputRequestTypeDef(
     _RequiredCreatePortfolioInputRequestTypeDef, _OptionalCreatePortfolioInputRequestTypeDef
 ):
     pass
 
-LaunchPathSummaryTypeDef = TypedDict(
-    "LaunchPathSummaryTypeDef",
-    {
-        "Id": str,
-        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
-        "Tags": List[TagTypeDef],
-        "Name": str,
-    },
-    total=False,
-)
-
-ProvisionedProductAttributeTypeDef = TypedDict(
-    "ProvisionedProductAttributeTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Type": str,
-        "Id": str,
-        "Status": ProvisionedProductStatusType,
-        "StatusMessage": str,
-        "CreatedTime": datetime,
-        "IdempotencyToken": str,
-        "LastRecordId": str,
-        "LastProvisioningRecordId": str,
-        "LastSuccessfulProvisioningRecordId": str,
-        "Tags": List[TagTypeDef],
-        "PhysicalId": str,
-        "ProductId": str,
-        "ProductName": str,
-        "ProvisioningArtifactId": str,
-        "ProvisioningArtifactName": str,
-        "UserArn": str,
-        "UserArnSession": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePortfolioInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioInputRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePortfolioInputRequestTypeDef = TypedDict(
@@ -2573,56 +2352,93 @@
 )
 
 class UpdatePortfolioInputRequestTypeDef(
     _RequiredUpdatePortfolioInputRequestTypeDef, _OptionalUpdatePortfolioInputRequestTypeDef
 ):
     pass
 
-CreatePortfolioOutputTypeDef = TypedDict(
-    "CreatePortfolioOutputTypeDef",
-    {
-        "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAcceptedPortfolioSharesOutputTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosForProductOutputTypeDef = TypedDict(
     "ListPortfoliosForProductOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPortfoliosOutputTypeDef = TypedDict(
     "ListPortfoliosOutputTypeDef",
     {
         "PortfolioDetails": List[PortfolioDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePortfolioOutputTypeDef = TypedDict(
+    "CreatePortfolioOutputTypeDef",
+    {
+        "PortfolioDetail": PortfolioDetailTypeDef,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LaunchPathSummaryTypeDef = TypedDict(
+    "LaunchPathSummaryTypeDef",
+    {
+        "Id": str,
+        "ConstraintSummaries": List[ConstraintSummaryTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "Name": str,
+    },
+    total=False,
+)
+
+ProvisionedProductAttributeTypeDef = TypedDict(
+    "ProvisionedProductAttributeTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Type": str,
+        "Id": str,
+        "Status": ProvisionedProductStatusType,
+        "StatusMessage": str,
+        "CreatedTime": datetime,
+        "IdempotencyToken": str,
+        "LastRecordId": str,
+        "LastProvisioningRecordId": str,
+        "LastSuccessfulProvisioningRecordId": str,
+        "Tags": List[TagOutputTypeDef],
+        "PhysicalId": str,
+        "ProductId": str,
+        "ProductName": str,
+        "ProvisioningArtifactId": str,
+        "ProvisioningArtifactName": str,
+        "UserArn": str,
+        "UserArnSession": str,
+    },
+    total=False,
+)
+
 UpdatePortfolioOutputTypeDef = TypedDict(
     "UpdatePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredCreatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
@@ -2664,23 +2480,14 @@
 
 class DeletePortfolioShareInputRequestTypeDef(
     _RequiredDeletePortfolioShareInputRequestTypeDef,
     _OptionalDeletePortfolioShareInputRequestTypeDef,
 ):
     pass
 
-ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
-    "ListOrganizationPortfolioAccessOutputTypeDef",
-    {
-        "OrganizationNodes": List[OrganizationNodeTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePortfolioShareInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePortfolioShareInputRequestTypeDef",
     {
         "PortfolioId": str,
     },
 )
 _OptionalUpdatePortfolioShareInputRequestTypeDef = TypedDict(
@@ -2725,34 +2532,34 @@
 
 CreateProvisioningArtifactOutputTypeDef = TypedDict(
     "CreateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisioningArtifactOutputTypeDef = TypedDict(
     "UpdateProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredCreateProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanName": str,
@@ -2777,106 +2584,84 @@
 
 class CreateProvisionedProductPlanInputRequestTypeDef(
     _RequiredCreateProvisionedProductPlanInputRequestTypeDef,
     _OptionalCreateProvisionedProductPlanInputRequestTypeDef,
 ):
     pass
 
-ProvisionedProductPlanDetailsTypeDef = TypedDict(
-    "ProvisionedProductPlanDetailsTypeDef",
-    {
-        "CreatedTime": datetime,
-        "PathId": str,
-        "ProductId": str,
-        "PlanName": str,
-        "PlanId": str,
-        "ProvisionProductId": str,
-        "ProvisionProductName": str,
-        "PlanType": Literal["CLOUDFORMATION"],
-        "ProvisioningArtifactId": str,
-        "Status": ProvisionedProductPlanStatusType,
-        "UpdatedTime": datetime,
-        "NotificationArns": List[str],
-        "ProvisioningParameters": List[UpdateProvisioningParameterTypeDef],
-        "Tags": List[TagTypeDef],
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 CreateTagOptionOutputTypeDef = TypedDict(
     "CreateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioOutputTypeDef = TypedDict(
     "DescribePortfolioOutputTypeDef",
     {
         "PortfolioDetail": PortfolioDetailTypeDef,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagOptionOutputTypeDef = TypedDict(
     "DescribeTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsOutputTypeDef = TypedDict(
     "ListTagOptionsOutputTypeDef",
     {
         "TagOptionDetails": List[TagOptionDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTagOptionOutputTypeDef = TypedDict(
     "UpdateTagOptionOutputTypeDef",
     {
         "TagOptionDetail": TagOptionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePortfolioSharesOutputTypeDef = TypedDict(
     "DescribePortfolioSharesOutputTypeDef",
     {
         "NextPageToken": str,
         "PortfolioShareDetails": List[PortfolioShareDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductOutputTypeDef = TypedDict(
     "DescribeProductOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
         "LaunchPaths": List[LaunchPathTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductViewOutputTypeDef = TypedDict(
     "DescribeProductViewOutputTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
         "ProvisioningArtifacts": List[ProvisioningArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisioningArtifactViewTypeDef = TypedDict(
     "ProvisioningArtifactViewTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -2886,33 +2671,33 @@
 )
 
 DescribeProvisionedProductOutputTypeDef = TypedDict(
     "DescribeProvisionedProductOutputTypeDef",
     {
         "ProvisionedProductDetail": ProvisionedProductDetailTypeDef,
         "CloudWatchDashboards": List[CloudWatchDashboardTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanProvisionedProductsOutputTypeDef = TypedDict(
     "ScanProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProvisionedProductOutputsOutputTypeDef = TypedDict(
     "GetProvisionedProductOutputsOutputTypeDef",
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -2936,51 +2721,294 @@
 ):
     pass
 
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineWorkflowResourceIdentifierTypeDef = TypedDict(
     "EngineWorkflowResourceIdentifierTypeDef",
     {
         "UniqueTag": UniqueTagResourceIdentifierTypeDef,
     },
     total=False,
 )
 
+ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
+    "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioShareType": PortfolioShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProductId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(
+    _RequiredListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    _OptionalListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+):
+    pass
+
+_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(
+    _RequiredListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    _OptionalListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "PortfolioId": str,
+        "OrganizationNodeType": OrganizationNodeTypeType,
+    },
+)
+_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(
+    _RequiredListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    _OptionalListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+):
+    pass
+
+_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "ProductId": str,
+    },
+)
+_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef = TypedDict(
+    "_OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(
+    _RequiredListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    _OptionalListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+):
+    pass
+
+ListPortfoliosInputListPortfoliosPaginateTypeDef = TypedDict(
+    "ListPortfoliosInputListPortfoliosPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "PortfolioId": str,
+    },
+)
+_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(
+    _RequiredListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    _OptionalListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+):
+    pass
+
+ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef = TypedDict(
+    "ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "ProvisionProductId": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "ServiceActionId": str,
+    },
+)
+_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(
+    _RequiredListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    _OptionalListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "TagOptionId": str,
+    },
+)
+_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(
+    _RequiredListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    _OptionalListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+):
+    pass
+
+_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "ProductId": str,
+        "ProvisioningArtifactId": str,
+    },
+)
+_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef = TypedDict(
+    "_OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(
+    _RequiredListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    _OptionalListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+):
+    pass
+
+ListServiceActionsInputListServiceActionsPaginateTypeDef = TypedDict(
+    "ListServiceActionsInputListServiceActionsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef = TypedDict(
+    "ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "AccessLevelFilter": AccessLevelFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef = TypedDict(
+    "SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef",
+    {
+        "AcceptLanguage": str,
+        "PortfolioId": str,
+        "Filters": Mapping[ProductViewFilterByType, Sequence[str]],
+        "SortBy": ProductViewSortByType,
+        "SortOrder": SortOrderType,
+        "ProductSource": Literal["ACCOUNT"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationPortfolioAccessOutputTypeDef = TypedDict(
+    "ListOrganizationPortfolioAccessOutputTypeDef",
+    {
+        "OrganizationNodes": List[OrganizationNodeOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPrincipalsForPortfolioOutputTypeDef = TypedDict(
     "ListPrincipalsForPortfolioOutputTypeDef",
     {
         "Principals": List[PrincipalTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisionedProductPlansOutputTypeDef = TypedDict(
     "ListProvisionedProductPlansOutputTypeDef",
     {
         "ProvisionedProductPlans": List[ProvisionedProductPlanSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryInputListRecordHistoryPaginateTypeDef = TypedDict(
     "ListRecordHistoryInputListRecordHistoryPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "AccessLevelFilter": AccessLevelFilterTypeDef,
         "SearchFilter": ListRecordHistorySearchFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListRecordHistoryInputRequestTypeDef = TypedDict(
     "ListRecordHistoryInputRequestTypeDef",
     {
@@ -2994,33 +3022,33 @@
 )
 
 ListResourcesForTagOptionOutputTypeDef = TypedDict(
     "ListResourcesForTagOptionOutputTypeDef",
     {
         "ResourceDetails": List[ResourceDetailTypeDef],
         "PageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsForProvisioningArtifactOutputTypeDef = TypedDict(
     "ListServiceActionsForProvisioningArtifactOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceActionsOutputTypeDef = TypedDict(
     "ListServiceActionsOutputTypeDef",
     {
         "ServiceActionSummaries": List[ServiceActionSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceActionDetailTypeDef = TypedDict(
     "ServiceActionDetailTypeDef",
     {
         "ServiceActionSummary": ServiceActionSummaryTypeDef,
@@ -3030,23 +3058,23 @@
 )
 
 ListStackInstancesForProvisionedProductOutputTypeDef = TypedDict(
     "ListStackInstancesForProvisionedProductOutputTypeDef",
     {
         "StackInstances": List[StackInstanceTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagOptionsInputListTagOptionsPaginateTypeDef = TypedDict(
     "ListTagOptionsInputListTagOptionsPaginateTypeDef",
     {
         "Filters": ListTagOptionsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTagOptionsInputRequestTypeDef = TypedDict(
     "ListTagOptionsInputRequestTypeDef",
     {
@@ -3072,15 +3100,15 @@
 
 SearchProductsOutputTypeDef = TypedDict(
     "SearchProductsOutputTypeDef",
     {
         "ProductViewSummaries": List[ProductViewSummaryTypeDef],
         "ProductViewAggregations": Dict[str, List[ProductViewAggregationValueTypeDef]],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProvisionProductInputRequestTypeDef = TypedDict(
     "_RequiredProvisionProductInputRequestTypeDef",
     {
         "ProvisionedProductName": str,
@@ -3106,14 +3134,36 @@
 )
 
 class ProvisionProductInputRequestTypeDef(
     _RequiredProvisionProductInputRequestTypeDef, _OptionalProvisionProductInputRequestTypeDef
 ):
     pass
 
+ProvisionedProductPlanDetailsTypeDef = TypedDict(
+    "ProvisionedProductPlanDetailsTypeDef",
+    {
+        "CreatedTime": datetime,
+        "PathId": str,
+        "ProductId": str,
+        "PlanName": str,
+        "PlanId": str,
+        "ProvisionProductId": str,
+        "ProvisionProductName": str,
+        "PlanType": Literal["CLOUDFORMATION"],
+        "ProvisioningArtifactId": str,
+        "Status": ProvisionedProductPlanStatusType,
+        "UpdatedTime": datetime,
+        "NotificationArns": List[str],
+        "ProvisioningParameters": List[UpdateProvisioningParameterOutputTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "StatusMessage": str,
+    },
+    total=False,
+)
+
 RecordDetailTypeDef = TypedDict(
     "RecordDetailTypeDef",
     {
         "RecordId": str,
         "ProvisionedProductName": str,
         "Status": RecordStatusType,
         "CreatedTime": datetime,
@@ -3181,15 +3231,15 @@
 ):
     pass
 
 SourceConnectionDetailTypeDef = TypedDict(
     "SourceConnectionDetailTypeDef",
     {
         "Type": Literal["CODESTAR"],
-        "ConnectionParameters": SourceConnectionParametersTypeDef,
+        "ConnectionParameters": SourceConnectionParametersOutputTypeDef,
         "LastSync": LastSyncTypeDef,
     },
     total=False,
 )
 
 _RequiredSourceConnectionTypeDef = TypedDict(
     "_RequiredSourceConnectionTypeDef",
@@ -3209,34 +3259,34 @@
     pass
 
 ListLaunchPathsOutputTypeDef = TypedDict(
     "ListLaunchPathsOutputTypeDef",
     {
         "LaunchPathSummaries": List[LaunchPathSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProvisionedProductsOutputTypeDef = TypedDict(
     "SearchProvisionedProductsOutputTypeDef",
     {
         "ProvisionedProducts": List[ProvisionedProductAttributeTypeDef],
         "TotalResultsCount": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningArtifactsForServiceActionOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
     "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     {
         "WorkflowToken": str,
@@ -3261,123 +3311,123 @@
 ):
     pass
 
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServiceActionOutputTypeDef = TypedDict(
     "DescribeServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceActionOutputTypeDef = TypedDict(
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningArtifactOutputTypeDef = TypedDict(
     "DescribeProvisioningArtifactOutputTypeDef",
     {
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
         "ProvisioningArtifactPreferences": ProvisioningArtifactPreferencesTypeDef,
         "ProvisioningArtifactOutputs": List[ProvisioningArtifactOutputTypeDef],
         "ProvisioningArtifactOutputKeys": List[ProvisioningArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecordOutputTypeDef = TypedDict(
     "DescribeRecordOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
         "RecordOutputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductPlanOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductPlanOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteProvisionedProductServiceActionOutputTypeDef = TypedDict(
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportAsProvisionedProductOutputTypeDef = TypedDict(
     "ImportAsProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRecordHistoryOutputTypeDef = TypedDict(
     "ListRecordHistoryOutputTypeDef",
     {
         "RecordDetails": List[RecordDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionProductOutputTypeDef = TypedDict(
     "ProvisionProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateProvisionedProductOutputTypeDef = TypedDict(
     "TerminateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProvisionedProductOutputTypeDef = TypedDict(
     "UpdateProvisionedProductOutputTypeDef",
     {
         "RecordDetail": RecordDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3395,15 +3445,15 @@
     "DescribePortfolioShareStatusOutputTypeDef",
     {
         "PortfolioShareToken": str,
         "PortfolioId": str,
         "OrganizationNodeValue": str,
         "Status": ShareStatusType,
         "ShareDetails": ShareDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProductViewDetailTypeDef = TypedDict(
     "ProductViewDetailTypeDef",
     {
         "ProductViewSummary": ProductViewSummaryTypeDef,
@@ -3476,50 +3526,50 @@
 
 DescribeProvisionedProductPlanOutputTypeDef = TypedDict(
     "DescribeProvisionedProductPlanOutputTypeDef",
     {
         "ProvisionedProductPlanDetails": ProvisionedProductPlanDetailsTypeDef,
         "ResourceChanges": List[ResourceChangeTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProductOutputTypeDef = TypedDict(
     "CreateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProductAsAdminOutputTypeDef = TypedDict(
     "DescribeProductAsAdminOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
         "ProvisioningArtifactSummaries": List[ProvisioningArtifactSummaryTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "TagOptions": List[TagOptionDetailTypeDef],
         "Budgets": List[BudgetDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchProductsAsAdminOutputTypeDef = TypedDict(
     "SearchProductsAsAdminOutputTypeDef",
     {
         "ProductViewDetails": List[ProductViewDetailTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProductOutputTypeDef = TypedDict(
     "UpdateProductOutputTypeDef",
     {
         "ProductViewDetail": ProductViewDetailTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.28.0
-Summary: Type annotations for boto3.ServiceCatalog 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.ServiceCatalog 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-servicecatalog)](https://pepy.tech/project/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -439,44 +439,42 @@
     AssociateBudgetWithResourceInputRequestTypeDef,
     AssociatePrincipalWithPortfolioInputRequestTypeDef,
     AssociateProductWithPortfolioInputRequestTypeDef,
     AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     AssociateTagOptionWithResourceInputRequestTypeDef,
     ServiceActionAssociationTypeDef,
     FailedServiceActionAssociationTypeDef,
+    ResponseMetadataTypeDef,
     BudgetDetailTypeDef,
     CloudWatchDashboardTypeDef,
+    CodeStarParametersOutputTypeDef,
     CodeStarParametersTypeDef,
     ConstraintDetailTypeDef,
     ConstraintSummaryTypeDef,
     CopyProductInputRequestTypeDef,
-    CopyProductOutputTypeDef,
     CreateConstraintInputRequestTypeDef,
     TagTypeDef,
     PortfolioDetailTypeDef,
+    TagOutputTypeDef,
     OrganizationNodeTypeDef,
-    CreatePortfolioShareOutputTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningArtifactDetailTypeDef,
     UpdateProvisioningParameterTypeDef,
-    CreateProvisionedProductPlanOutputTypeDef,
     CreateServiceActionInputRequestTypeDef,
     CreateTagOptionInputRequestTypeDef,
     TagOptionDetailTypeDef,
     DeleteConstraintInputRequestTypeDef,
     DeletePortfolioInputRequestTypeDef,
-    DeletePortfolioShareOutputTypeDef,
     DeleteProductInputRequestTypeDef,
     DeleteProvisionedProductPlanInputRequestTypeDef,
     DeleteProvisioningArtifactInputRequestTypeDef,
     DeleteServiceActionInputRequestTypeDef,
     DeleteTagOptionInputRequestTypeDef,
     DescribeConstraintInputRequestTypeDef,
     DescribeCopyProductStatusInputRequestTypeDef,
-    DescribeCopyProductStatusOutputTypeDef,
     DescribePortfolioInputRequestTypeDef,
     DescribePortfolioShareStatusInputRequestTypeDef,
     DescribePortfolioSharesInputRequestTypeDef,
     PortfolioShareDetailTypeDef,
     DescribeProductAsAdminInputRequestTypeDef,
     ProvisioningArtifactSummaryTypeDef,
     DescribeProductInputRequestTypeDef,
@@ -503,110 +501,101 @@
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
     UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
-    GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
-    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
     ListBudgetsForResourceInputRequestTypeDef,
-    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListConstraintsForPortfolioInputRequestTypeDef,
-    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListLaunchPathsInputRequestTypeDef,
-    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListOrganizationPortfolioAccessInputRequestTypeDef,
+    OrganizationNodeOutputTypeDef,
     ListPortfolioAccessInputRequestTypeDef,
-    ListPortfolioAccessOutputTypeDef,
-    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosForProductInputRequestTypeDef,
-    ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPortfoliosInputRequestTypeDef,
-    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
     ListPrincipalsForPortfolioInputRequestTypeDef,
     PrincipalTypeDef,
     ProvisionedProductPlanSummaryTypeDef,
-    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
     ListProvisioningArtifactsForServiceActionInputRequestTypeDef,
     ListProvisioningArtifactsInputRequestTypeDef,
     ListRecordHistorySearchFilterTypeDef,
-    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
     ListResourcesForTagOptionInputRequestTypeDef,
     ResourceDetailTypeDef,
-    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
-    ListServiceActionsInputListServiceActionsPaginateTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
     NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
+    UpdateProvisioningParameterOutputTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     SearchProductsAsAdminInputRequestTypeDef,
-    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
     SearchProductsInputRequestTypeDef,
     ShareErrorTypeDef,
     TerminateProvisionedProductInputRequestTypeDef,
     UpdateConstraintInputRequestTypeDef,
-    UpdatePortfolioShareOutputTypeDef,
     UpdateProvisioningPreferencesTypeDef,
     UpdateProvisionedProductPropertiesInputRequestTypeDef,
-    UpdateProvisionedProductPropertiesOutputTypeDef,
     UpdateProvisioningArtifactInputRequestTypeDef,
     UpdateServiceActionInputRequestTypeDef,
     UpdateTagOptionInputRequestTypeDef,
-    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
     ListProvisionedProductPlansInputRequestTypeDef,
     ScanProvisionedProductsInputRequestTypeDef,
-    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
     SearchProvisionedProductsInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef,
     BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef,
+    CopyProductOutputTypeDef,
+    CreatePortfolioShareOutputTypeDef,
+    CreateProvisionedProductPlanOutputTypeDef,
+    DeletePortfolioShareOutputTypeDef,
+    DescribeCopyProductStatusOutputTypeDef,
+    GetAWSOrganizationsAccessStatusOutputTypeDef,
+    ListPortfolioAccessOutputTypeDef,
+    UpdatePortfolioShareOutputTypeDef,
+    UpdateProvisionedProductPropertiesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
+    SourceConnectionParametersOutputTypeDef,
     SourceConnectionParametersTypeDef,
     CreateConstraintOutputTypeDef,
     DescribeConstraintOutputTypeDef,
     ListConstraintsForPortfolioOutputTypeDef,
     UpdateConstraintOutputTypeDef,
     CreatePortfolioInputRequestTypeDef,
-    LaunchPathSummaryTypeDef,
-    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioInputRequestTypeDef,
-    CreatePortfolioOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListPortfoliosForProductOutputTypeDef,
     ListPortfoliosOutputTypeDef,
+    CreatePortfolioOutputTypeDef,
+    LaunchPathSummaryTypeDef,
+    ProvisionedProductAttributeTypeDef,
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
-    ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
-    ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
     ListTagOptionsOutputTypeDef,
     UpdateTagOptionOutputTypeDef,
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
@@ -614,28 +603,44 @@
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     EngineWorkflowResourceIdentifierTypeDef,
+    ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
+    ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
+    ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
+    ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
+    ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
+    ListPortfoliosInputListPortfoliosPaginateTypeDef,
+    ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
+    ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef,
+    ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef,
+    ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef,
+    ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef,
+    ListServiceActionsInputListServiceActionsPaginateTypeDef,
+    ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef,
+    SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef,
+    ListOrganizationPortfolioAccessOutputTypeDef,
     ListPrincipalsForPortfolioOutputTypeDef,
     ListProvisionedProductPlansOutputTypeDef,
     ListRecordHistoryInputListRecordHistoryPaginateTypeDef,
     ListRecordHistoryInputRequestTypeDef,
     ListResourcesForTagOptionOutputTypeDef,
     ListServiceActionsForProvisioningArtifactOutputTypeDef,
     ListServiceActionsOutputTypeDef,
     ServiceActionDetailTypeDef,
     ListStackInstancesForProvisionedProductOutputTypeDef,
     ListTagOptionsInputListTagOptionsPaginateTypeDef,
     ListTagOptionsInputRequestTypeDef,
     ProvisioningArtifactParameterTypeDef,
     SearchProductsOutputTypeDef,
     ProvisionProductInputRequestTypeDef,
+    ProvisionedProductPlanDetailsTypeDef,
     RecordDetailTypeDef,
     ResourceChangeDetailTypeDef,
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
```

### Comparing `mypy-boto3-servicecatalog-1.28.0/mypy_boto3_servicecatalog.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-1.28.12/mypy_boto3_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.28.0/setup.py` & `mypy-boto3-servicecatalog-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-servicecatalog",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceCatalog 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.ServiceCatalog 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

