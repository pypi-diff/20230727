# Comparing `tmp/mypy-boto3-license-manager-1.28.0.tar.gz` & `tmp/mypy-boto3-license-manager-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-license-manager-1.28.0.tar", last modified: Thu Jul  6 20:59:59 2023, max compression
+gzip compressed data, was "mypy-boto3-license-manager-1.28.12.tar", last modified: Thu Jul 27 05:34:56 2023, max compression
```

## Comparing `mypy-boto3-license-manager-1.28.0.tar` & `mypy-boto3-license-manager-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:58.986353 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-06 20:45:42.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-06 20:45:45.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55080 2023-07-06 20:45:44.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 20:59:58.000000 mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:59.002353 mypy-boto3-license-manager-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-06 20:45:41.000000 mypy-boto3-license-manager-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40707 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40645 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7589 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60234 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60153 2023-07-27 05:25:20.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:19.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:56.000000 mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:56.392458 mypy-boto3-license-manager-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 05:25:18.000000 mypy-boto3-license-manager-1.28.12/setup.py
```

### Comparing `mypy-boto3-license-manager-1.28.0/LICENSE` & `mypy-boto3-license-manager-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/PKG-INFO` & `mypy-boto3-license-manager-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,19 +366,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
+    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
+    EntitlementDataOutputTypeDef,
+    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
+    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateGrantResponseTypeDef,
     OptionsTypeDef,
     CreateGrantVersionResponseTypeDef,
     TagTypeDef,
     CreateLicenseConfigurationResponseTypeDef,
@@ -390,70 +394,77 @@
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
     CreateLicenseResponseTypeDef,
     CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
     DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
     DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
+    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
     ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
     GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
+    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationTypeDef,
+    OrganizationConfigurationOutputTypeDef,
+    OptionsOutputTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
+    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
     ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    OrganizationConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
     RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
+    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
+    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
+    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
-    GrantTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
     ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
@@ -462,40 +473,45 @@
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
+    GrantTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    CreateLicenseRequestRequestTypeDef,
-    CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    CreateLicenseRequestRequestTypeDef,
+    CreateLicenseVersionRequestRequestTypeDef,
+    GetLicenseUsageResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.0/README.md` & `mypy-boto3-license-manager-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,19 +334,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
+    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
+    EntitlementDataOutputTypeDef,
+    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
+    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateGrantResponseTypeDef,
     OptionsTypeDef,
     CreateGrantVersionResponseTypeDef,
     TagTypeDef,
     CreateLicenseConfigurationResponseTypeDef,
@@ -358,70 +362,77 @@
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
     CreateLicenseResponseTypeDef,
     CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
     DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
     DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
+    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
     ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
     GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
+    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationTypeDef,
+    OrganizationConfigurationOutputTypeDef,
+    OptionsOutputTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
+    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
     ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    OrganizationConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
     RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
+    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
+    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
+    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
-    GrantTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
     ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
@@ -430,40 +441,45 @@
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
+    GrantTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    CreateLicenseRequestRequestTypeDef,
-    CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    CreateLicenseRequestRequestTypeDef,
+    CreateLicenseVersionRequestRequestTypeDef,
+    GetLicenseUsageResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__init__.pyi` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/__main__.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LicenseManager 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.LicenseManager 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/client.pyi` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.pyi`

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
     "ActivationOverrideBehaviorType",
     "AllowedOperationType",
     "CheckoutTypeType",
     "DigitalSignatureMethodType",
     "EntitlementDataUnitType",
     "EntitlementUnitType",
@@ -47,15 +46,14 @@
     "LicenseManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivationOverrideBehaviorType = Literal[
     "ALL_GRANTS_PERMITTED_BY_ISSUER", "DISTRIBUTED_GRANTS_ONLY"
 ]
 AllowedOperationType = Literal[
     "CheckInLicense",
     "CheckoutBorrowLicense",
     "CheckoutLicense",
@@ -291,14 +289,15 @@
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
@@ -377,26 +376,28 @@
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

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/literals.pyi` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/literals.py`

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
     "ActivationOverrideBehaviorType",
     "AllowedOperationType",
     "CheckoutTypeType",
     "DigitalSignatureMethodType",
     "EntitlementDataUnitType",
     "EntitlementUnitType",
@@ -46,14 +47,15 @@
     "LicenseManagerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActivationOverrideBehaviorType = Literal[
     "ALL_GRANTS_PERMITTED_BY_ISSUER", "DISTRIBUTED_GRANTS_ONLY"
 ]
 AllowedOperationType = Literal[
     "CheckInLicense",
     "CheckoutBorrowLicense",
     "CheckoutLicense",
@@ -289,14 +291,15 @@
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
@@ -375,26 +378,28 @@
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

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/paginator.pyi` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.py` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,19 +45,23 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
     "AcceptGrantResponseTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
+    "BorrowConfigurationOutputTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
+    "EntitlementDataOutputTypeDef",
+    "MetadataOutputTypeDef",
     "ConsumedLicenseSummaryTypeDef",
+    "ProvisionalConfigurationOutputTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
     "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
     "CreateLicenseConfigurationResponseTypeDef",
@@ -69,70 +73,77 @@
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
     "CreateLicenseResponseTypeDef",
     "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "CreateTokenResponseTypeDef",
+    "DatetimeRangeOutputTypeDef",
     "DeleteGrantRequestRequestTypeDef",
     "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
     "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
+    "EntitlementOutputTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
     "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
     "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
+    "TagOutputTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
+    "LicenseConversionContextOutputTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
-    "OrganizationConfigurationTypeDef",
+    "OrganizationConfigurationOutputTypeDef",
+    "OptionsOutputTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
+    "LicenseSpecificationOutputTypeDef",
     "LicenseSpecificationTypeDef",
     "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
+    "OrganizationConfigurationTypeDef",
     "PaginatorConfigTypeDef",
+    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
     "RejectGrantResponseTypeDef",
+    "ReportContextOutputTypeDef",
+    "ReportFrequencyOutputTypeDef",
     "S3LocationTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
-    "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
+    "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
+    "ConsumptionConfigurationOutputTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
-    "GrantTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
-    "GetLicenseConversionTaskResponseTypeDef",
-    "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
@@ -141,40 +152,45 @@
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetLicenseConversionTaskResponseTypeDef",
+    "LicenseConversionTaskTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
+    "GrantTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
+    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
-    "CreateLicenseRequestRequestTypeDef",
-    "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
+    "CreateLicenseRequestRequestTypeDef",
+    "CreateLicenseVersionRequestRequestTypeDef",
+    "GetLicenseUsageResponseTypeDef",
+    "ListLicenseConversionTasksResponseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
-    "ListLicenseConversionTasksResponseTypeDef",
-    "GetLicenseUsageResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
@@ -203,14 +219,22 @@
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
     },
     total=False,
 )
 
+BorrowConfigurationOutputTypeDef = TypedDict(
+    "BorrowConfigurationOutputTypeDef",
+    {
+        "AllowEarlyCheckIn": bool,
+        "MaxTimeToLiveInMinutes": int,
+    },
+)
+
 BorrowConfigurationTypeDef = TypedDict(
     "BorrowConfigurationTypeDef",
     {
         "AllowEarlyCheckIn": bool,
         "MaxTimeToLiveInMinutes": int,
     },
 )
@@ -261,23 +285,61 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredEntitlementDataOutputTypeDef = TypedDict(
+    "_RequiredEntitlementDataOutputTypeDef",
+    {
+        "Name": str,
+        "Unit": EntitlementDataUnitType,
+    },
+)
+_OptionalEntitlementDataOutputTypeDef = TypedDict(
+    "_OptionalEntitlementDataOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+
+class EntitlementDataOutputTypeDef(
+    _RequiredEntitlementDataOutputTypeDef, _OptionalEntitlementDataOutputTypeDef
+):
+    pass
+
+
+MetadataOutputTypeDef = TypedDict(
+    "MetadataOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ConsumedLicenseSummaryTypeDef = TypedDict(
     "ConsumedLicenseSummaryTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
+ProvisionalConfigurationOutputTypeDef = TypedDict(
+    "ProvisionalConfigurationOutputTypeDef",
+    {
+        "MaxTimeToLiveInMinutes": int,
+    },
+)
+
 ProvisionalConfigurationTypeDef = TypedDict(
     "ProvisionalConfigurationTypeDef",
     {
         "MaxTimeToLiveInMinutes": int,
     },
 )
 
@@ -489,14 +551,35 @@
         "TokenId": str,
         "TokenType": Literal["REFRESH_TOKEN"],
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDatetimeRangeOutputTypeDef = TypedDict(
+    "_RequiredDatetimeRangeOutputTypeDef",
+    {
+        "Begin": str,
+    },
+)
+_OptionalDatetimeRangeOutputTypeDef = TypedDict(
+    "_OptionalDatetimeRangeOutputTypeDef",
+    {
+        "End": str,
+    },
+    total=False,
+)
+
+
+class DatetimeRangeOutputTypeDef(
+    _RequiredDatetimeRangeOutputTypeDef, _OptionalDatetimeRangeOutputTypeDef
+):
+    pass
+
+
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -559,14 +642,39 @@
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
+_RequiredEntitlementOutputTypeDef = TypedDict(
+    "_RequiredEntitlementOutputTypeDef",
+    {
+        "Name": str,
+        "Unit": EntitlementUnitType,
+    },
+)
+_OptionalEntitlementOutputTypeDef = TypedDict(
+    "_OptionalEntitlementOutputTypeDef",
+    {
+        "Value": str,
+        "MaxCount": int,
+        "Overage": bool,
+        "AllowCheckIn": bool,
+    },
+    total=False,
+)
+
+
+class EntitlementOutputTypeDef(
+    _RequiredEntitlementOutputTypeDef, _OptionalEntitlementOutputTypeDef
+):
+    pass
+
+
 _RequiredEntitlementUsageTypeDef = TypedDict(
     "_RequiredEntitlementUsageTypeDef",
     {
         "Name": str,
         "ConsumedValue": str,
         "Unit": EntitlementDataUnitType,
     },
@@ -686,21 +794,38 @@
     {
         "ResourceType": ResourceTypeType,
         "AssociationCount": int,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 GetLicenseConversionTaskRequestRequestTypeDef = TypedDict(
     "GetLicenseConversionTaskRequestRequestTypeDef",
     {
         "LicenseConversionTaskId": str,
     },
 )
 
+LicenseConversionContextOutputTypeDef = TypedDict(
+    "LicenseConversionContextOutputTypeDef",
+    {
+        "UsageOperation": str,
+    },
+    total=False,
+)
+
 GetLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
     },
 )
 
@@ -728,21 +853,29 @@
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
-OrganizationConfigurationTypeDef = TypedDict(
-    "OrganizationConfigurationTypeDef",
+OrganizationConfigurationOutputTypeDef = TypedDict(
+    "OrganizationConfigurationOutputTypeDef",
     {
         "EnableIntegration": bool,
     },
 )
 
+OptionsOutputTypeDef = TypedDict(
+    "OptionsOutputTypeDef",
+    {
+        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
+    },
+    total=False,
+)
+
 IssuerDetailsTypeDef = TypedDict(
     "IssuerDetailsTypeDef",
     {
         "Name": str,
         "SignKey": str,
         "KeyFingerprint": str,
     },
@@ -800,14 +933,35 @@
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
+_RequiredLicenseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredLicenseSpecificationOutputTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalLicenseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalLicenseSpecificationOutputTypeDef",
+    {
+        "AmiAssociationScope": str,
+    },
+    total=False,
+)
+
+
+class LicenseSpecificationOutputTypeDef(
+    _RequiredLicenseSpecificationOutputTypeDef, _OptionalLicenseSpecificationOutputTypeDef
+):
+    pass
+
+
 _RequiredLicenseSpecificationTypeDef = TypedDict(
     "_RequiredLicenseSpecificationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalLicenseSpecificationTypeDef = TypedDict(
@@ -991,24 +1145,53 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
+OrganizationConfigurationTypeDef = TypedDict(
+    "OrganizationConfigurationTypeDef",
+    {
+        "EnableIntegration": bool,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredProductInformationFilterOutputTypeDef = TypedDict(
+    "_RequiredProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterName": str,
+        "ProductInformationFilterComparator": str,
+    },
+)
+_OptionalProductInformationFilterOutputTypeDef = TypedDict(
+    "_OptionalProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterValue": List[str],
+    },
+    total=False,
+)
+
+
+class ProductInformationFilterOutputTypeDef(
+    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -1040,14 +1223,30 @@
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
+    {
+        "licenseConfigurationArns": List[str],
+    },
+)
+
+ReportFrequencyOutputTypeDef = TypedDict(
+    "ReportFrequencyOutputTypeDef",
+    {
+        "value": int,
+        "period": ReportFrequencyTypeType,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -1094,29 +1293,14 @@
 
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
 
-CheckoutLicenseResponseTypeDef = TypedDict(
-    "CheckoutLicenseResponseTypeDef",
-    {
-        "CheckoutType": CheckoutTypeType,
-        "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataTypeDef],
-        "SignedToken": str,
-        "NodeId": str,
-        "IssuedAt": str,
-        "Expiration": str,
-        "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
         "DigitalSignatureMethod": Literal["JWT_PS384"],
         "ClientToken": str,
@@ -1135,40 +1319,65 @@
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
 
+CheckoutLicenseResponseTypeDef = TypedDict(
+    "CheckoutLicenseResponseTypeDef",
+    {
+        "CheckoutType": CheckoutTypeType,
+        "LicenseConsumptionToken": str,
+        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
+        "SignedToken": str,
+        "NodeId": str,
+        "IssuedAt": str,
+        "Expiration": str,
+        "LicenseArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataTypeDef],
+        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
-        "CheckoutMetadata": List[MetadataTypeDef],
+        "CheckoutMetadata": List[MetadataOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ErrorMessage": str,
         "FailureTime": datetime,
         "OperationName": str,
         "ResourceOwnerId": str,
         "OperationRequestedBy": str,
-        "MetadataList": List[MetadataTypeDef],
+        "MetadataList": List[MetadataOutputTypeDef],
+    },
+    total=False,
+)
+
+ConsumptionConfigurationOutputTypeDef = TypedDict(
+    "ConsumptionConfigurationOutputTypeDef",
+    {
+        "RenewType": RenewTypeType,
+        "ProvisionalConfiguration": ProvisionalConfigurationOutputTypeDef,
+        "BorrowConfiguration": BorrowConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ConsumptionConfigurationTypeDef = TypedDict(
     "ConsumptionConfigurationTypeDef",
     {
@@ -1203,50 +1412,14 @@
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
-    },
-)
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-        "Options": OptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
-
-
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
@@ -1256,46 +1429,14 @@
     {
         "ResourceArn": str,
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
     },
 )
 
-GetLicenseConversionTaskResponseTypeDef = TypedDict(
-    "GetLicenseConversionTaskResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextTypeDef,
-        "StatusMessage": str,
-        "Status": LicenseConversionTaskStatusType,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LicenseConversionTaskTypeDef = TypedDict(
-    "LicenseConversionTaskTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextTypeDef,
-        "Status": LicenseConversionTaskStatusType,
-        "StatusMessage": str,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1527,37 +1668,94 @@
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLicenseConversionTaskResponseTypeDef = TypedDict(
+    "GetLicenseConversionTaskResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
+        "StatusMessage": str,
+        "Status": LicenseConversionTaskStatusType,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LicenseConversionTaskTypeDef = TypedDict(
+    "LicenseConversionTaskTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
+        "Status": LicenseConversionTaskStatusType,
+        "StatusMessage": str,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "OrganizationConfiguration": OrganizationConfigurationOutputTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateServiceSettingsRequestRequestTypeDef",
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
     {
-        "S3BucketArn": str,
-        "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
-        "EnableCrossAccountsDiscovery": bool,
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsOutputTypeDef,
     },
     total=False,
 )
 
+
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
+
 ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1590,15 +1788,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
-        "LicenseSpecifications": List[LicenseSpecificationTypeDef],
+        "LicenseSpecifications": List[LicenseSpecificationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
@@ -1637,51 +1835,113 @@
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "S3BucketArn": str,
+        "SnsTopicArn": str,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "EnableCrossAccountsDiscovery": bool,
+    },
+    total=False,
+)
+
+ProductInformationOutputTypeDef = TypedDict(
+    "ProductInformationOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
+    },
+)
+
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextTypeDef,
-        "ReportFrequency": ReportFrequencyTypeDef,
+        "ReportContext": ReportContextOutputTypeDef,
+        "ReportFrequency": ReportFrequencyOutputTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
         "S3Location": S3LocationTypeDef,
         "CreateTime": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrantedLicenseTypeDef = TypedDict(
+    "GrantedLicenseTypeDef",
+    {
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeOutputTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementOutputTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
+        "LicenseMetadata": List[MetadataOutputTypeDef],
+        "CreateTime": str,
+        "Version": str,
+        "ReceivedMetadata": ReceivedMetadataTypeDef,
+    },
+    total=False,
+)
+
+LicenseTypeDef = TypedDict(
+    "LicenseTypeDef",
+    {
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeOutputTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementOutputTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
+        "LicenseMetadata": List[MetadataOutputTypeDef],
+        "CreateTime": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
         "Issuer": IssuerTypeDef,
@@ -1736,55 +1996,29 @@
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
 
-GrantedLicenseTypeDef = TypedDict(
-    "GrantedLicenseTypeDef",
+GetLicenseUsageResponseTypeDef = TypedDict(
+    "GetLicenseUsageResponseTypeDef",
     {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
-        "LicenseMetadata": List[MetadataTypeDef],
-        "CreateTime": str,
-        "Version": str,
-        "ReceivedMetadata": ReceivedMetadataTypeDef,
+        "LicenseUsage": LicenseUsageTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-LicenseTypeDef = TypedDict(
-    "LicenseTypeDef",
+ListLicenseConversionTasksResponseTypeDef = TypedDict(
+    "ListLicenseConversionTasksResponseTypeDef",
     {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
-        "LicenseMetadata": List[MetadataTypeDef],
-        "CreateTime": str,
-        "Version": str,
+        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1814,60 +2048,14 @@
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListLicenseConversionTasksResponseTypeDef = TypedDict(
-    "ListLicenseConversionTasksResponseTypeDef",
-    {
-        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLicenseUsageResponseTypeDef = TypedDict(
-    "GetLicenseUsageResponseTypeDef",
-    {
-        "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1876,16 +2064,16 @@
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
@@ -1901,20 +2089,49 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager/type_defs.pyi` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -44,19 +44,23 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
     "AcceptGrantResponseTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
+    "BorrowConfigurationOutputTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
     "MetadataTypeDef",
+    "EntitlementDataOutputTypeDef",
+    "MetadataOutputTypeDef",
     "ConsumedLicenseSummaryTypeDef",
+    "ProvisionalConfigurationOutputTypeDef",
     "ProvisionalConfigurationTypeDef",
     "CreateGrantRequestRequestTypeDef",
     "CreateGrantResponseTypeDef",
     "OptionsTypeDef",
     "CreateGrantVersionResponseTypeDef",
     "TagTypeDef",
     "CreateLicenseConfigurationResponseTypeDef",
@@ -68,70 +72,77 @@
     "DatetimeRangeTypeDef",
     "EntitlementTypeDef",
     "IssuerTypeDef",
     "CreateLicenseResponseTypeDef",
     "CreateLicenseVersionResponseTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "CreateTokenResponseTypeDef",
+    "DatetimeRangeOutputTypeDef",
     "DeleteGrantRequestRequestTypeDef",
     "DeleteGrantResponseTypeDef",
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     "DeleteLicenseManagerReportGeneratorRequestRequestTypeDef",
     "DeleteLicenseRequestRequestTypeDef",
     "DeleteLicenseResponseTypeDef",
     "DeleteTokenRequestRequestTypeDef",
+    "EntitlementOutputTypeDef",
     "EntitlementUsageTypeDef",
     "ExtendLicenseConsumptionRequestRequestTypeDef",
     "ExtendLicenseConsumptionResponseTypeDef",
     "FilterTypeDef",
     "GetAccessTokenRequestRequestTypeDef",
     "GetAccessTokenResponseTypeDef",
     "GetGrantRequestRequestTypeDef",
     "GetLicenseConfigurationRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
+    "TagOutputTypeDef",
     "GetLicenseConversionTaskRequestRequestTypeDef",
+    "LicenseConversionContextOutputTypeDef",
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     "GetLicenseRequestRequestTypeDef",
     "GetLicenseUsageRequestRequestTypeDef",
-    "OrganizationConfigurationTypeDef",
+    "OrganizationConfigurationOutputTypeDef",
+    "OptionsOutputTypeDef",
     "IssuerDetailsTypeDef",
     "ReceivedMetadataTypeDef",
     "InventoryFilterTypeDef",
     "LicenseConfigurationAssociationTypeDef",
     "LicenseConfigurationUsageTypeDef",
+    "LicenseSpecificationOutputTypeDef",
     "LicenseSpecificationTypeDef",
     "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
+    "OrganizationConfigurationTypeDef",
     "PaginatorConfigTypeDef",
+    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
     "RejectGrantResponseTypeDef",
+    "ReportContextOutputTypeDef",
+    "ReportFrequencyOutputTypeDef",
     "S3LocationTypeDef",
     "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CheckoutLicenseRequestRequestTypeDef",
-    "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseRequestRequestTypeDef",
+    "CheckoutLicenseResponseTypeDef",
     "CheckoutBorrowLicenseResponseTypeDef",
     "LicenseOperationFailureTypeDef",
+    "ConsumptionConfigurationOutputTypeDef",
     "ConsumptionConfigurationTypeDef",
     "CreateGrantVersionRequestRequestTypeDef",
-    "GrantTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateLicenseConversionTaskForResourceRequestRequestTypeDef",
-    "GetLicenseConversionTaskResponseTypeDef",
-    "LicenseConversionTaskTypeDef",
     "CreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "UpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     "LicenseUsageTypeDef",
     "ListDistributedGrantsRequestRequestTypeDef",
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseConfigurationsRequestRequestTypeDef",
     "ListLicenseConversionTasksRequestRequestTypeDef",
@@ -140,40 +151,45 @@
     "ListReceivedGrantsForOrganizationRequestRequestTypeDef",
     "ListReceivedGrantsRequestRequestTypeDef",
     "ListReceivedLicensesForOrganizationRequestRequestTypeDef",
     "ListReceivedLicensesRequestRequestTypeDef",
     "ListTokensRequestRequestTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "GetLicenseConversionTaskResponseTypeDef",
+    "LicenseConversionTaskTypeDef",
     "GetServiceSettingsResponseTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
+    "GrantTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListResourceInventoryRequestRequestTypeDef",
     "ListAssociationsForLicenseConfigurationResponseTypeDef",
     "ListUsageForLicenseConfigurationResponseTypeDef",
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     "UpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
+    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
-    "CreateLicenseRequestRequestTypeDef",
-    "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
+    "CreateLicenseRequestRequestTypeDef",
+    "CreateLicenseVersionRequestRequestTypeDef",
+    "GetLicenseUsageResponseTypeDef",
+    "ListLicenseConversionTasksResponseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
-    "ListLicenseConversionTasksResponseTypeDef",
-    "GetLicenseUsageResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
     "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
@@ -202,14 +218,22 @@
     "AutomatedDiscoveryInformationTypeDef",
     {
         "LastRunTime": datetime,
     },
     total=False,
 )
 
+BorrowConfigurationOutputTypeDef = TypedDict(
+    "BorrowConfigurationOutputTypeDef",
+    {
+        "AllowEarlyCheckIn": bool,
+        "MaxTimeToLiveInMinutes": int,
+    },
+)
+
 BorrowConfigurationTypeDef = TypedDict(
     "BorrowConfigurationTypeDef",
     {
         "AllowEarlyCheckIn": bool,
         "MaxTimeToLiveInMinutes": int,
     },
 )
@@ -256,23 +280,59 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredEntitlementDataOutputTypeDef = TypedDict(
+    "_RequiredEntitlementDataOutputTypeDef",
+    {
+        "Name": str,
+        "Unit": EntitlementDataUnitType,
+    },
+)
+_OptionalEntitlementDataOutputTypeDef = TypedDict(
+    "_OptionalEntitlementDataOutputTypeDef",
+    {
+        "Value": str,
+    },
+    total=False,
+)
+
+class EntitlementDataOutputTypeDef(
+    _RequiredEntitlementDataOutputTypeDef, _OptionalEntitlementDataOutputTypeDef
+):
+    pass
+
+MetadataOutputTypeDef = TypedDict(
+    "MetadataOutputTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 ConsumedLicenseSummaryTypeDef = TypedDict(
     "ConsumedLicenseSummaryTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
+ProvisionalConfigurationOutputTypeDef = TypedDict(
+    "ProvisionalConfigurationOutputTypeDef",
+    {
+        "MaxTimeToLiveInMinutes": int,
+    },
+)
+
 ProvisionalConfigurationTypeDef = TypedDict(
     "ProvisionalConfigurationTypeDef",
     {
         "MaxTimeToLiveInMinutes": int,
     },
 )
 
@@ -476,14 +536,33 @@
         "TokenId": str,
         "TokenType": Literal["REFRESH_TOKEN"],
         "Token": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredDatetimeRangeOutputTypeDef = TypedDict(
+    "_RequiredDatetimeRangeOutputTypeDef",
+    {
+        "Begin": str,
+    },
+)
+_OptionalDatetimeRangeOutputTypeDef = TypedDict(
+    "_OptionalDatetimeRangeOutputTypeDef",
+    {
+        "End": str,
+    },
+    total=False,
+)
+
+class DatetimeRangeOutputTypeDef(
+    _RequiredDatetimeRangeOutputTypeDef, _OptionalDatetimeRangeOutputTypeDef
+):
+    pass
+
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -544,14 +623,37 @@
 DeleteTokenRequestRequestTypeDef = TypedDict(
     "DeleteTokenRequestRequestTypeDef",
     {
         "TokenId": str,
     },
 )
 
+_RequiredEntitlementOutputTypeDef = TypedDict(
+    "_RequiredEntitlementOutputTypeDef",
+    {
+        "Name": str,
+        "Unit": EntitlementUnitType,
+    },
+)
+_OptionalEntitlementOutputTypeDef = TypedDict(
+    "_OptionalEntitlementOutputTypeDef",
+    {
+        "Value": str,
+        "MaxCount": int,
+        "Overage": bool,
+        "AllowCheckIn": bool,
+    },
+    total=False,
+)
+
+class EntitlementOutputTypeDef(
+    _RequiredEntitlementOutputTypeDef, _OptionalEntitlementOutputTypeDef
+):
+    pass
+
 _RequiredEntitlementUsageTypeDef = TypedDict(
     "_RequiredEntitlementUsageTypeDef",
     {
         "Name": str,
         "ConsumedValue": str,
         "Unit": EntitlementDataUnitType,
     },
@@ -663,21 +765,38 @@
     {
         "ResourceType": ResourceTypeType,
         "AssociationCount": int,
     },
     total=False,
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+    total=False,
+)
+
 GetLicenseConversionTaskRequestRequestTypeDef = TypedDict(
     "GetLicenseConversionTaskRequestRequestTypeDef",
     {
         "LicenseConversionTaskId": str,
     },
 )
 
+LicenseConversionContextOutputTypeDef = TypedDict(
+    "LicenseConversionContextOutputTypeDef",
+    {
+        "UsageOperation": str,
+    },
+    total=False,
+)
+
 GetLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
     },
 )
 
@@ -703,21 +822,29 @@
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
-OrganizationConfigurationTypeDef = TypedDict(
-    "OrganizationConfigurationTypeDef",
+OrganizationConfigurationOutputTypeDef = TypedDict(
+    "OrganizationConfigurationOutputTypeDef",
     {
         "EnableIntegration": bool,
     },
 )
 
+OptionsOutputTypeDef = TypedDict(
+    "OptionsOutputTypeDef",
+    {
+        "ActivationOverrideBehavior": ActivationOverrideBehaviorType,
+    },
+    total=False,
+)
+
 IssuerDetailsTypeDef = TypedDict(
     "IssuerDetailsTypeDef",
     {
         "Name": str,
         "SignKey": str,
         "KeyFingerprint": str,
     },
@@ -773,14 +900,33 @@
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
         "ConsumedLicenses": int,
     },
     total=False,
 )
 
+_RequiredLicenseSpecificationOutputTypeDef = TypedDict(
+    "_RequiredLicenseSpecificationOutputTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalLicenseSpecificationOutputTypeDef = TypedDict(
+    "_OptionalLicenseSpecificationOutputTypeDef",
+    {
+        "AmiAssociationScope": str,
+    },
+    total=False,
+)
+
+class LicenseSpecificationOutputTypeDef(
+    _RequiredLicenseSpecificationOutputTypeDef, _OptionalLicenseSpecificationOutputTypeDef
+):
+    pass
+
 _RequiredLicenseSpecificationTypeDef = TypedDict(
     "_RequiredLicenseSpecificationTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalLicenseSpecificationTypeDef = TypedDict(
@@ -950,24 +1096,51 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
+OrganizationConfigurationTypeDef = TypedDict(
+    "OrganizationConfigurationTypeDef",
+    {
+        "EnableIntegration": bool,
+    },
+)
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+_RequiredProductInformationFilterOutputTypeDef = TypedDict(
+    "_RequiredProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterName": str,
+        "ProductInformationFilterComparator": str,
+    },
+)
+_OptionalProductInformationFilterOutputTypeDef = TypedDict(
+    "_OptionalProductInformationFilterOutputTypeDef",
+    {
+        "ProductInformationFilterValue": List[str],
+    },
+    total=False,
+)
+
+class ProductInformationFilterOutputTypeDef(
+    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
+):
+    pass
+
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -997,14 +1170,30 @@
         "GrantArn": str,
         "Status": GrantStatusType,
         "Version": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReportContextOutputTypeDef = TypedDict(
+    "ReportContextOutputTypeDef",
+    {
+        "licenseConfigurationArns": List[str],
+    },
+)
+
+ReportFrequencyOutputTypeDef = TypedDict(
+    "ReportFrequencyOutputTypeDef",
+    {
+        "value": int,
+        "period": ReportFrequencyTypeType,
+    },
+    total=False,
+)
+
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -1049,29 +1238,14 @@
 )
 
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
-CheckoutLicenseResponseTypeDef = TypedDict(
-    "CheckoutLicenseResponseTypeDef",
-    {
-        "CheckoutType": CheckoutTypeType,
-        "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataTypeDef],
-        "SignedToken": str,
-        "NodeId": str,
-        "IssuedAt": str,
-        "Expiration": str,
-        "LicenseArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCheckoutBorrowLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCheckoutBorrowLicenseRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "Entitlements": Sequence[EntitlementDataTypeDef],
         "DigitalSignatureMethod": Literal["JWT_PS384"],
         "ClientToken": str,
@@ -1088,40 +1262,65 @@
 
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
+CheckoutLicenseResponseTypeDef = TypedDict(
+    "CheckoutLicenseResponseTypeDef",
+    {
+        "CheckoutType": CheckoutTypeType,
+        "LicenseConsumptionToken": str,
+        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
+        "SignedToken": str,
+        "NodeId": str,
+        "IssuedAt": str,
+        "Expiration": str,
+        "LicenseArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
-        "EntitlementsAllowed": List[EntitlementDataTypeDef],
+        "EntitlementsAllowed": List[EntitlementDataOutputTypeDef],
         "NodeId": str,
         "SignedToken": str,
         "IssuedAt": str,
         "Expiration": str,
-        "CheckoutMetadata": List[MetadataTypeDef],
+        "CheckoutMetadata": List[MetadataOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseOperationFailureTypeDef = TypedDict(
     "LicenseOperationFailureTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ErrorMessage": str,
         "FailureTime": datetime,
         "OperationName": str,
         "ResourceOwnerId": str,
         "OperationRequestedBy": str,
-        "MetadataList": List[MetadataTypeDef],
+        "MetadataList": List[MetadataOutputTypeDef],
+    },
+    total=False,
+)
+
+ConsumptionConfigurationOutputTypeDef = TypedDict(
+    "ConsumptionConfigurationOutputTypeDef",
+    {
+        "RenewType": RenewTypeType,
+        "ProvisionalConfiguration": ProvisionalConfigurationOutputTypeDef,
+        "BorrowConfiguration": BorrowConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 ConsumptionConfigurationTypeDef = TypedDict(
     "ConsumptionConfigurationTypeDef",
     {
@@ -1154,48 +1353,14 @@
 
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGrantTypeDef = TypedDict(
-    "_RequiredGrantTypeDef",
-    {
-        "GrantArn": str,
-        "GrantName": str,
-        "ParentArn": str,
-        "LicenseArn": str,
-        "GranteePrincipalArn": str,
-        "HomeRegion": str,
-        "GrantStatus": GrantStatusType,
-        "Version": str,
-        "GrantedOperations": List[AllowedOperationType],
-    },
-)
-_OptionalGrantTypeDef = TypedDict(
-    "_OptionalGrantTypeDef",
-    {
-        "StatusReason": str,
-        "Options": OptionsTypeDef,
-    },
-    total=False,
-)
-
-class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
-    pass
-
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
@@ -1205,46 +1370,14 @@
     {
         "ResourceArn": str,
         "SourceLicenseContext": LicenseConversionContextTypeDef,
         "DestinationLicenseContext": LicenseConversionContextTypeDef,
     },
 )
 
-GetLicenseConversionTaskResponseTypeDef = TypedDict(
-    "GetLicenseConversionTaskResponseTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextTypeDef,
-        "StatusMessage": str,
-        "Status": LicenseConversionTaskStatusType,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LicenseConversionTaskTypeDef = TypedDict(
-    "LicenseConversionTaskTypeDef",
-    {
-        "LicenseConversionTaskId": str,
-        "ResourceArn": str,
-        "SourceLicenseContext": LicenseConversionContextTypeDef,
-        "DestinationLicenseContext": LicenseConversionContextTypeDef,
-        "Status": LicenseConversionTaskStatusType,
-        "StatusMessage": str,
-        "StartTime": datetime,
-        "LicenseConversionTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
@@ -1466,37 +1599,92 @@
 
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+GetLicenseConversionTaskResponseTypeDef = TypedDict(
+    "GetLicenseConversionTaskResponseTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
+        "StatusMessage": str,
+        "Status": LicenseConversionTaskStatusType,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+LicenseConversionTaskTypeDef = TypedDict(
+    "LicenseConversionTaskTypeDef",
+    {
+        "LicenseConversionTaskId": str,
+        "ResourceArn": str,
+        "SourceLicenseContext": LicenseConversionContextOutputTypeDef,
+        "DestinationLicenseContext": LicenseConversionContextOutputTypeDef,
+        "Status": LicenseConversionTaskStatusType,
+        "StatusMessage": str,
+        "StartTime": datetime,
+        "LicenseConversionTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "OrganizationConfiguration": OrganizationConfigurationOutputTypeDef,
         "EnableCrossAccountsDiscovery": bool,
         "LicenseManagerResourceShareArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "UpdateServiceSettingsRequestRequestTypeDef",
+_RequiredGrantTypeDef = TypedDict(
+    "_RequiredGrantTypeDef",
     {
-        "S3BucketArn": str,
-        "SnsTopicArn": str,
-        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
-        "EnableCrossAccountsDiscovery": bool,
+        "GrantArn": str,
+        "GrantName": str,
+        "ParentArn": str,
+        "LicenseArn": str,
+        "GranteePrincipalArn": str,
+        "HomeRegion": str,
+        "GrantStatus": GrantStatusType,
+        "Version": str,
+        "GrantedOperations": List[AllowedOperationType],
+    },
+)
+_OptionalGrantTypeDef = TypedDict(
+    "_OptionalGrantTypeDef",
+    {
+        "StatusReason": str,
+        "Options": OptionsOutputTypeDef,
     },
     total=False,
 )
 
+class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
+    pass
+
 ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
@@ -1529,15 +1717,15 @@
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListLicenseSpecificationsForResourceResponseTypeDef = TypedDict(
     "ListLicenseSpecificationsForResourceResponseTypeDef",
     {
-        "LicenseSpecifications": List[LicenseSpecificationTypeDef],
+        "LicenseSpecifications": List[LicenseSpecificationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef",
@@ -1574,51 +1762,113 @@
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+UpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "UpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "S3BucketArn": str,
+        "SnsTopicArn": str,
+        "OrganizationConfiguration": OrganizationConfigurationTypeDef,
+        "EnableCrossAccountsDiscovery": bool,
+    },
+    total=False,
+)
+
+ProductInformationOutputTypeDef = TypedDict(
+    "ProductInformationOutputTypeDef",
+    {
+        "ResourceType": str,
+        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
+    },
+)
+
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextTypeDef,
-        "ReportFrequency": ReportFrequencyTypeDef,
+        "ReportContext": ReportContextOutputTypeDef,
+        "ReportFrequency": ReportFrequencyOutputTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
         "S3Location": S3LocationTypeDef,
         "CreateTime": str,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
     total=False,
 )
 
 ListFailuresForLicenseConfigurationOperationsResponseTypeDef = TypedDict(
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     {
         "LicenseOperationFailureList": List[LicenseOperationFailureTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+GrantedLicenseTypeDef = TypedDict(
+    "GrantedLicenseTypeDef",
+    {
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeOutputTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementOutputTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
+        "LicenseMetadata": List[MetadataOutputTypeDef],
+        "CreateTime": str,
+        "Version": str,
+        "ReceivedMetadata": ReceivedMetadataTypeDef,
+    },
+    total=False,
+)
+
+LicenseTypeDef = TypedDict(
+    "LicenseTypeDef",
+    {
+        "LicenseArn": str,
+        "LicenseName": str,
+        "ProductName": str,
+        "ProductSKU": str,
+        "Issuer": IssuerDetailsTypeDef,
+        "HomeRegion": str,
+        "Status": LicenseStatusType,
+        "Validity": DatetimeRangeOutputTypeDef,
+        "Beneficiary": str,
+        "Entitlements": List[EntitlementOutputTypeDef],
+        "ConsumptionConfiguration": ConsumptionConfigurationOutputTypeDef,
+        "LicenseMetadata": List[MetadataOutputTypeDef],
+        "CreateTime": str,
+        "Version": str,
+    },
+    total=False,
+)
+
 _RequiredCreateLicenseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseRequestRequestTypeDef",
     {
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
         "Issuer": IssuerTypeDef,
@@ -1669,55 +1919,29 @@
 
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
-GrantedLicenseTypeDef = TypedDict(
-    "GrantedLicenseTypeDef",
+GetLicenseUsageResponseTypeDef = TypedDict(
+    "GetLicenseUsageResponseTypeDef",
     {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
-        "LicenseMetadata": List[MetadataTypeDef],
-        "CreateTime": str,
-        "Version": str,
-        "ReceivedMetadata": ReceivedMetadataTypeDef,
+        "LicenseUsage": LicenseUsageTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-LicenseTypeDef = TypedDict(
-    "LicenseTypeDef",
+ListLicenseConversionTasksResponseTypeDef = TypedDict(
+    "ListLicenseConversionTasksResponseTypeDef",
     {
-        "LicenseArn": str,
-        "LicenseName": str,
-        "ProductName": str,
-        "ProductSKU": str,
-        "Issuer": IssuerDetailsTypeDef,
-        "HomeRegion": str,
-        "Status": LicenseStatusType,
-        "Validity": DatetimeRangeTypeDef,
-        "Beneficiary": str,
-        "Entitlements": List[EntitlementTypeDef],
-        "ConsumptionConfiguration": ConsumptionConfigurationTypeDef,
-        "LicenseMetadata": List[MetadataTypeDef],
-        "CreateTime": str,
-        "Version": str,
+        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 GetGrantResponseTypeDef = TypedDict(
     "GetGrantResponseTypeDef",
     {
         "Grant": GrantTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
@@ -1747,58 +1971,14 @@
     {
         "Grants": List[GrantTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListLicenseConversionTasksResponseTypeDef = TypedDict(
-    "ListLicenseConversionTasksResponseTypeDef",
-    {
-        "LicenseConversionTasks": List[LicenseConversionTaskTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLicenseUsageResponseTypeDef = TypedDict(
-    "GetLicenseUsageResponseTypeDef",
-    {
-        "LicenseUsage": LicenseUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationTypeDef],
-    },
-    total=False,
-)
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1807,16 +1987,16 @@
         "LicenseCount": int,
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "Tags": List[TagOutputTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
@@ -1832,20 +2012,47 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationTypeDef],
+        "ProductInformationList": List[ProductInformationOutputTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+    },
+    total=False,
+)
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/PKG-INFO` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-license-manager
-Version: 1.28.0
-Summary: Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.LicenseManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-license-manager"></a>
 
 # mypy-boto3-license-manager
 
 [![PyPI - mypy-boto3-license-manager](https://img.shields.io/pypi/v/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-license-manager.svg?color=blue)](https://pypi.org/project/mypy-boto3-license-manager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-license-manager?color=blue)](https://pypistats.org/packages/mypy-boto3-license-manager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-license-manager)](https://pepy.tech/project/mypy-boto3-license-manager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LicenseManager 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
+[boto3.LicenseManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager)
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
 [mypy-boto3-license-manager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_license_manager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -366,19 +366,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_license_manager.type_defs import (
     AcceptGrantRequestRequestTypeDef,
     AcceptGrantResponseTypeDef,
     AutomatedDiscoveryInformationTypeDef,
+    BorrowConfigurationOutputTypeDef,
     BorrowConfigurationTypeDef,
     CheckInLicenseRequestRequestTypeDef,
     EntitlementDataTypeDef,
     MetadataTypeDef,
+    EntitlementDataOutputTypeDef,
+    MetadataOutputTypeDef,
     ConsumedLicenseSummaryTypeDef,
+    ProvisionalConfigurationOutputTypeDef,
     ProvisionalConfigurationTypeDef,
     CreateGrantRequestRequestTypeDef,
     CreateGrantResponseTypeDef,
     OptionsTypeDef,
     CreateGrantVersionResponseTypeDef,
     TagTypeDef,
     CreateLicenseConfigurationResponseTypeDef,
@@ -390,70 +394,77 @@
     DatetimeRangeTypeDef,
     EntitlementTypeDef,
     IssuerTypeDef,
     CreateLicenseResponseTypeDef,
     CreateLicenseVersionResponseTypeDef,
     CreateTokenRequestRequestTypeDef,
     CreateTokenResponseTypeDef,
+    DatetimeRangeOutputTypeDef,
     DeleteGrantRequestRequestTypeDef,
     DeleteGrantResponseTypeDef,
     DeleteLicenseConfigurationRequestRequestTypeDef,
     DeleteLicenseManagerReportGeneratorRequestRequestTypeDef,
     DeleteLicenseRequestRequestTypeDef,
     DeleteLicenseResponseTypeDef,
     DeleteTokenRequestRequestTypeDef,
+    EntitlementOutputTypeDef,
     EntitlementUsageTypeDef,
     ExtendLicenseConsumptionRequestRequestTypeDef,
     ExtendLicenseConsumptionResponseTypeDef,
     FilterTypeDef,
     GetAccessTokenRequestRequestTypeDef,
     GetAccessTokenResponseTypeDef,
     GetGrantRequestRequestTypeDef,
     GetLicenseConfigurationRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
+    TagOutputTypeDef,
     GetLicenseConversionTaskRequestRequestTypeDef,
+    LicenseConversionContextOutputTypeDef,
     GetLicenseManagerReportGeneratorRequestRequestTypeDef,
     GetLicenseRequestRequestTypeDef,
     GetLicenseUsageRequestRequestTypeDef,
-    OrganizationConfigurationTypeDef,
+    OrganizationConfigurationOutputTypeDef,
+    OptionsOutputTypeDef,
     IssuerDetailsTypeDef,
     ReceivedMetadataTypeDef,
     InventoryFilterTypeDef,
     LicenseConfigurationAssociationTypeDef,
     LicenseConfigurationUsageTypeDef,
+    LicenseSpecificationOutputTypeDef,
     LicenseSpecificationTypeDef,
     ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     ListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     ListLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListLicenseVersionsRequestRequestTypeDef,
     ResourceInventoryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TokenDataTypeDef,
+    OrganizationConfigurationTypeDef,
     PaginatorConfigTypeDef,
+    ProductInformationFilterOutputTypeDef,
     ProductInformationFilterTypeDef,
     RejectGrantRequestRequestTypeDef,
     RejectGrantResponseTypeDef,
+    ReportContextOutputTypeDef,
+    ReportFrequencyOutputTypeDef,
     S3LocationTypeDef,
     ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     CheckoutLicenseRequestRequestTypeDef,
-    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseRequestRequestTypeDef,
+    CheckoutLicenseResponseTypeDef,
     CheckoutBorrowLicenseResponseTypeDef,
     LicenseOperationFailureTypeDef,
+    ConsumptionConfigurationOutputTypeDef,
     ConsumptionConfigurationTypeDef,
     CreateGrantVersionRequestRequestTypeDef,
-    GrantTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateLicenseConversionTaskForResourceRequestRequestTypeDef,
-    GetLicenseConversionTaskResponseTypeDef,
-    LicenseConversionTaskTypeDef,
     CreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     UpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     LicenseUsageTypeDef,
     ListDistributedGrantsRequestRequestTypeDef,
     ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef,
     ListLicenseConfigurationsRequestRequestTypeDef,
     ListLicenseConversionTasksRequestRequestTypeDef,
@@ -462,40 +473,45 @@
     ListReceivedGrantsForOrganizationRequestRequestTypeDef,
     ListReceivedGrantsRequestRequestTypeDef,
     ListReceivedLicensesForOrganizationRequestRequestTypeDef,
     ListReceivedLicensesRequestRequestTypeDef,
     ListTokensRequestRequestTypeDef,
     ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     ListUsageForLicenseConfigurationRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    GetLicenseConversionTaskResponseTypeDef,
+    LicenseConversionTaskTypeDef,
     GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
+    GrantTypeDef,
     ListResourceInventoryRequestListResourceInventoryPaginateTypeDef,
     ListResourceInventoryRequestRequestTypeDef,
     ListAssociationsForLicenseConfigurationResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     ListLicenseSpecificationsForResourceResponseTypeDef,
     UpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     ListResourceInventoryResponseTypeDef,
     ListTokensResponseTypeDef,
+    UpdateServiceSettingsRequestRequestTypeDef,
+    ProductInformationOutputTypeDef,
     ProductInformationTypeDef,
     ReportGeneratorTypeDef,
     ListFailuresForLicenseConfigurationOperationsResponseTypeDef,
-    CreateLicenseRequestRequestTypeDef,
-    CreateLicenseVersionRequestRequestTypeDef,
     GrantedLicenseTypeDef,
     LicenseTypeDef,
+    CreateLicenseRequestRequestTypeDef,
+    CreateLicenseVersionRequestRequestTypeDef,
+    GetLicenseUsageResponseTypeDef,
+    ListLicenseConversionTasksResponseTypeDef,
     GetGrantResponseTypeDef,
     ListDistributedGrantsResponseTypeDef,
     ListReceivedGrantsForOrganizationResponseTypeDef,
     ListReceivedGrantsResponseTypeDef,
-    ListLicenseConversionTasksResponseTypeDef,
-    GetLicenseUsageResponseTypeDef,
-    CreateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseConfigurationResponseTypeDef,
     LicenseConfigurationTypeDef,
+    CreateLicenseConfigurationRequestRequestTypeDef,
     UpdateLicenseConfigurationRequestRequestTypeDef,
     GetLicenseManagerReportGeneratorResponseTypeDef,
     ListLicenseManagerReportGeneratorsResponseTypeDef,
     ListReceivedLicensesForOrganizationResponseTypeDef,
     ListReceivedLicensesResponseTypeDef,
     GetLicenseResponseTypeDef,
     ListLicenseVersionsResponseTypeDef,
```

### Comparing `mypy-boto3-license-manager-1.28.0/mypy_boto3_license_manager.egg-info/SOURCES.txt` & `mypy-boto3-license-manager-1.28.12/mypy_boto3_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-license-manager-1.28.0/setup.py` & `mypy-boto3-license-manager-1.28.12/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-license-manager",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LicenseManager 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.LicenseManager 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

