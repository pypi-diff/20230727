# Comparing `tmp/mypy-boto3-billingconductor-1.28.11.tar.gz` & `tmp/mypy-boto3-billingconductor-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-billingconductor-1.28.11.tar", last modified: Tue Jul 25 19:49:13 2023, max compression
+gzip compressed data, was "mypy-boto3-billingconductor-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-billingconductor-1.28.11.tar` & `mypy-boto3-billingconductor-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-billingconductor-1.28.11/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-07-25 19:49:13.841034 mypy-boto3-billingconductor-1.28.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.833034 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-07-25 19:46:54.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10169 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43891 2023-07-25 19:46:55.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43844 2023-07-25 19:46:54.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:49:13.841034 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20684 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 19:49:13.000000 mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:49:13.841034 mypy-boto3-billingconductor-1.28.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-25 19:46:53.000000 mypy-boto3-billingconductor-1.28.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.688567 mypy-boto3-billingconductor-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-07-27 05:34:22.688567 mypy-boto3-billingconductor-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.688567 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31684 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31636 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-07-27 05:18:00.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-27 05:18:00.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-27 05:18:00.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14433 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44518 2023-07-27 05:18:01.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44469 2023-07-27 05:18:00.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.688567 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20668 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:22.000000 mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.688567 mypy-boto3-billingconductor-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:17:59.000000 mypy-boto3-billingconductor-1.28.12/setup.py
```

### Comparing `mypy-boto3-billingconductor-1.28.11/LICENSE` & `mypy-boto3-billingconductor-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/PKG-INFO` & `mypy-boto3-billingconductor-1.28.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.28.11
-Summary: Type annotations for boto3.BillingConductor 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.BillingConductor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,89 +374,89 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceOutputTypeDef,
     ListBillingGroupAccountGroupingTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBillingGroupAccountGroupingOutputTypeDef,
     UpdateBillingGroupAccountGroupingTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigOutputTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
```

### Comparing `mypy-boto3-billingconductor-1.28.11/README.md` & `mypy-boto3-billingconductor-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,89 +342,89 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceOutputTypeDef,
     ListBillingGroupAccountGroupingTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBillingGroupAccountGroupingOutputTypeDef,
     UpdateBillingGroupAccountGroupingTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigOutputTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__init__.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__init__.pyi` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/__main__.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BillingConductor 1.28.11\nVersion:         1.28.11\nBuilder"
-        " version: 7.15.1\nDocs:           "
+        "Type annotations for boto3.BillingConductor 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.11")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/client.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/client.pyi` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/literals.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/literals.py`

 * *Files 1% similar despite different names*

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
@@ -275,14 +276,15 @@
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

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/literals.pyi` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -273,14 +274,15 @@
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

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/paginator.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 
@@ -132,15 +132,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -151,15 +151,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 
@@ -170,15 +170,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 
@@ -189,15 +189,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 
@@ -208,15 +208,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 
@@ -227,15 +227,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 
@@ -246,15 +246,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 
@@ -266,13 +266,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/paginator.pyi` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListAccountAssociationsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListAccountAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListAccountAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listaccountassociationspaginator)
         """
 
 class ListBillingGroupCostReportsPaginator(Paginator):
@@ -109,15 +109,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupCostReportsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupCostReportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroupCostReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupcostreportspaginator)
         """
 
 class ListBillingGroupsPaginator(Paginator):
@@ -127,15 +127,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListBillingGroupsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListBillingGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listbillinggroupspaginator)
         """
 
 class ListCustomLineItemVersionsPaginator(Paginator):
@@ -145,15 +145,15 @@
     """
 
     def paginate(
         self,
         *,
         Arn: str,
         Filters: ListCustomLineItemVersionsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemVersionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItemVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemversionspaginator)
         """
 
 class ListCustomLineItemsPaginator(Paginator):
@@ -163,15 +163,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListCustomLineItemsFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListCustomLineItemsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListCustomLineItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listcustomlineitemspaginator)
         """
 
 class ListPricingPlansPaginator(Paginator):
@@ -181,15 +181,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingPlansFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplanspaginator)
         """
 
 class ListPricingPlansAssociatedWithPricingRulePaginator(Paginator):
@@ -199,15 +199,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingRuleArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingPlansAssociatedWithPricingRuleOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingPlansAssociatedWithPricingRule.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingplansassociatedwithpricingrulepaginator)
         """
 
 class ListPricingRulesPaginator(Paginator):
@@ -217,15 +217,15 @@
     """
 
     def paginate(
         self,
         *,
         BillingPeriod: str = ...,
         Filters: ListPricingRulesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulespaginator)
         """
 
 class ListPricingRulesAssociatedToPricingPlanPaginator(Paginator):
@@ -235,15 +235,15 @@
     """
 
     def paginate(
         self,
         *,
         PricingPlanArn: str,
         BillingPeriod: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListPricingRulesAssociatedToPricingPlanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListPricingRulesAssociatedToPricingPlan.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listpricingrulesassociatedtopricingplanpaginator)
         """
 
 class ListResourcesAssociatedToCustomLineItemPaginator(Paginator):
@@ -254,13 +254,13 @@
 
     def paginate(
         self,
         *,
         Arn: str,
         BillingPeriod: str = ...,
         Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListResourcesAssociatedToCustomLineItemOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Paginator.ListResourcesAssociatedToCustomLineItem.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/paginators/#listresourcesassociatedtocustomlineitempaginator)
         """
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/type_defs.py` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,89 +30,89 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceOutputTypeDef",
     "ListBillingGroupAccountGroupingTypeDef",
     "ComputationPreferenceTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
+    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
+    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
+    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBillingGroupAccountGroupingOutputTypeDef",
     "UpdateBillingGroupAccountGroupingTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigOutputTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
-    "DeletePricingPlanOutputTypeDef",
-    "DeletePricingRuleOutputTypeDef",
-    "DisassociateAccountsOutputTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
-    "ListAccountAssociationsOutputTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdatePricingPlanOutputTypeDef",
+    "ListAccountAssociationsOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    "ListAccountAssociationsInputRequestTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -153,14 +153,15 @@
     "AccountAssociationsListElementTypeDef",
     {
         "AccountId": str,
         "BillingGroupArn": str,
         "AccountName": str,
         "AccountEmail": str,
     },
+    total=False,
 )
 
 _RequiredAccountGroupingTypeDef = TypedDict(
     "_RequiredAccountGroupingTypeDef",
     {
         "LinkedAccountIds": Sequence[str],
     },
@@ -182,39 +183,45 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
+    total=False,
 )
 
 _RequiredCustomLineItemBillingPeriodRangeTypeDef = TypedDict(
     "_RequiredCustomLineItemBillingPeriodRangeTypeDef",
     {
         "InclusiveStartBillingPeriod": str,
     },
@@ -241,37 +248,55 @@
         "Arn": str,
         "AWSCost": str,
         "ProformaCost": str,
         "Margin": str,
         "MarginPercentage": str,
         "Currency": str,
     },
+    total=False,
 )
 
 ComputationPreferenceOutputTypeDef = TypedDict(
     "ComputationPreferenceOutputTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
 ListBillingGroupAccountGroupingTypeDef = TypedDict(
     "ListBillingGroupAccountGroupingTypeDef",
     {
         "AutoAssociate": bool,
     },
+    total=False,
 )
 
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -295,14 +320,30 @@
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -331,44 +372,92 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -378,24 +467,14 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
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
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -440,14 +519,37 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -464,14 +566,25 @@
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
 
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -482,16 +595,40 @@
         "Name": str,
         "Arn": str,
         "Description": str,
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
+    total=False,
+)
+
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
 )
 
+
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -508,14 +645,25 @@
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
 
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -531,23 +679,53 @@
 ListResourcesAssociatedToCustomLineItemResponseElementTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     {
         "Arn": str,
         "Relationship": CustomLineItemRelationshipType,
         "EndBillingPeriod": str,
     },
+    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
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
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -561,14 +739,15 @@
 )
 
 UpdateBillingGroupAccountGroupingOutputTypeDef = TypedDict(
     "UpdateBillingGroupAccountGroupingOutputTypeDef",
     {
         "AutoAssociate": bool,
     },
+    total=False,
 )
 
 UpdateBillingGroupAccountGroupingTypeDef = TypedDict(
     "UpdateBillingGroupAccountGroupingTypeDef",
     {
         "AutoAssociate": bool,
     },
@@ -621,175 +800,51 @@
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Description": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountAssociationsOutputTypeDef = TypedDict(
     "ListAccountAssociationsOutputTypeDef",
     {
         "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
         "Error": AssociateResourceErrorTypeDef,
     },
+    total=False,
 )
 
 DisassociateResourceResponseElementTypeDef = TypedDict(
     "DisassociateResourceResponseElementTypeDef",
     {
         "Arn": str,
         "Error": AssociateResourceErrorTypeDef,
     },
+    total=False,
 )
 
 _RequiredBatchAssociateResourcesToCustomLineItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     {
         "TargetArn": str,
         "ResourceArns": Sequence[str],
@@ -857,15 +912,15 @@
 
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -876,14 +931,15 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
         "Status": BillingGroupStatusType,
         "StatusReason": str,
         "AccountGrouping": ListBillingGroupAccountGroupingTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateBillingGroupInputRequestTypeDef",
     {
         "Name": str,
         "AccountGrouping": AccountGroupingTypeDef,
@@ -940,86 +996,40 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
-    {
-        "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
-
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
     {
         "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
     },
     total=False,
 )
 
-
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
-
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -1032,15 +1042,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1048,37 +1058,50 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": ListBillingGroupsFilterTypeDef,
     },
     total=False,
 )
 
-ListCustomLineItemChargeDetailsTypeDef = TypedDict(
-    "ListCustomLineItemChargeDetailsTypeDef",
+_RequiredListCustomLineItemChargeDetailsTypeDef = TypedDict(
+    "_RequiredListCustomLineItemChargeDetailsTypeDef",
+    {
+        "Type": CustomLineItemTypeType,
+    },
+)
+_OptionalListCustomLineItemChargeDetailsTypeDef = TypedDict(
+    "_OptionalListCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": ListCustomLineItemFlatChargeDetailsTypeDef,
         "Percentage": ListCustomLineItemPercentageChargeDetailsTypeDef,
-        "Type": CustomLineItemTypeType,
     },
+    total=False,
 )
 
+
+class ListCustomLineItemChargeDetailsTypeDef(
+    _RequiredListCustomLineItemChargeDetailsTypeDef, _OptionalListCustomLineItemChargeDetailsTypeDef
+):
+    pass
+
+
 ListCustomLineItemVersionsFilterTypeDef = TypedDict(
     "ListCustomLineItemVersionsFilterTypeDef",
     {
         "BillingPeriodRange": ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     },
     total=False,
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1091,15 +1114,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1113,24 +1136,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1149,15 +1172,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1193,15 +1216,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBillingGroupOutputTypeDef = TypedDict(
     "UpdateBillingGroupOutputTypeDef",
     {
         "Arn": str,
@@ -1210,15 +1233,15 @@
         "PrimaryAccountId": str,
         "PricingPlanArn": str,
         "Size": int,
         "LastModifiedTime": int,
         "Status": BillingGroupStatusType,
         "StatusReason": str,
         "AccountGrouping": UpdateBillingGroupAccountGroupingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
@@ -1267,33 +1290,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1365,14 +1388,15 @@
         "CreationTime": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": TieringTypeDef,
         "UsageType": str,
         "Operation": str,
     },
+    total=False,
 )
 
 CustomLineItemListElementTypeDef = TypedDict(
     "CustomLineItemListElementTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -1381,14 +1405,15 @@
         "Description": str,
         "ProductCode": str,
         "BillingGroupArn": str,
         "CreationTime": int,
         "LastModifiedTime": int,
         "AssociationSize": int,
     },
+    total=False,
 )
 
 CustomLineItemVersionListElementTypeDef = TypedDict(
     "CustomLineItemVersionListElementTypeDef",
     {
         "Name": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
@@ -1400,41 +1425,42 @@
         "LastModifiedTime": int,
         "AssociationSize": int,
         "StartBillingPeriod": str,
         "EndBillingPeriod": str,
         "Arn": str,
         "StartTime": int,
     },
+    total=False,
 )
 
 UpdateCustomLineItemOutputTypeDef = TypedDict(
     "UpdateCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1504,15 +1530,15 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputOutputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
@@ -1539,28 +1565,28 @@
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor/type_defs.pyi` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,89 +29,89 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAssociationsListElementTypeDef",
     "AccountGroupingTypeDef",
     "AssociateAccountsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AssociateAccountsOutputTypeDef",
     "AssociatePricingRulesInputRequestTypeDef",
+    "AssociatePricingRulesOutputTypeDef",
     "AssociateResourceErrorTypeDef",
     "CustomLineItemBillingPeriodRangeTypeDef",
     "BillingGroupCostReportElementTypeDef",
     "ComputationPreferenceOutputTypeDef",
     "ListBillingGroupAccountGroupingTypeDef",
     "ComputationPreferenceTypeDef",
+    "CreateBillingGroupOutputTypeDef",
+    "CreateCustomLineItemOutputTypeDef",
     "CreateFreeTierConfigTypeDef",
     "CreatePricingPlanInputRequestTypeDef",
+    "CreatePricingPlanOutputTypeDef",
+    "CreatePricingRuleOutputTypeDef",
     "CustomLineItemFlatChargeDetailsTypeDef",
     "CustomLineItemPercentageChargeDetailsTypeDef",
     "DeleteBillingGroupInputRequestTypeDef",
+    "DeleteBillingGroupOutputTypeDef",
+    "DeleteCustomLineItemOutputTypeDef",
     "DeletePricingPlanInputRequestTypeDef",
+    "DeletePricingPlanOutputTypeDef",
     "DeletePricingRuleInputRequestTypeDef",
+    "DeletePricingRuleOutputTypeDef",
     "DisassociateAccountsInputRequestTypeDef",
+    "DisassociateAccountsOutputTypeDef",
     "DisassociatePricingRulesInputRequestTypeDef",
+    "DisassociatePricingRulesOutputTypeDef",
     "FreeTierConfigTypeDef",
     "ListAccountAssociationsFilterTypeDef",
-    "PaginatorConfigTypeDef",
     "ListBillingGroupCostReportsFilterTypeDef",
     "ListBillingGroupsFilterTypeDef",
     "ListCustomLineItemFlatChargeDetailsTypeDef",
     "ListCustomLineItemPercentageChargeDetailsTypeDef",
     "ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef",
     "ListCustomLineItemsFilterTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
     "ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
     "ListPricingPlansFilterTypeDef",
     "PricingPlanListElementTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
     "ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
     "ListPricingRulesFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemFilterTypeDef",
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBillingGroupAccountGroupingOutputTypeDef",
     "UpdateBillingGroupAccountGroupingTypeDef",
     "UpdateCustomLineItemFlatChargeDetailsTypeDef",
     "UpdateCustomLineItemPercentageChargeDetailsTypeDef",
     "UpdateFreeTierConfigOutputTypeDef",
     "UpdateFreeTierConfigTypeDef",
     "UpdatePricingPlanInputRequestTypeDef",
-    "AssociateAccountsOutputTypeDef",
-    "AssociatePricingRulesOutputTypeDef",
-    "CreateBillingGroupOutputTypeDef",
-    "CreateCustomLineItemOutputTypeDef",
-    "CreatePricingPlanOutputTypeDef",
-    "CreatePricingRuleOutputTypeDef",
-    "DeleteBillingGroupOutputTypeDef",
-    "DeleteCustomLineItemOutputTypeDef",
-    "DeletePricingPlanOutputTypeDef",
-    "DeletePricingRuleOutputTypeDef",
-    "DisassociateAccountsOutputTypeDef",
-    "DisassociatePricingRulesOutputTypeDef",
-    "ListAccountAssociationsOutputTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "UpdatePricingPlanOutputTypeDef",
+    "ListAccountAssociationsOutputTypeDef",
     "AssociateResourceResponseElementTypeDef",
     "DisassociateResourceResponseElementTypeDef",
     "BatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     "BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef",
     "DeleteCustomLineItemInputRequestTypeDef",
     "ListBillingGroupCostReportsOutputTypeDef",
     "BillingGroupListElementTypeDef",
     "CreateBillingGroupInputRequestTypeDef",
     "CreateTieringInputTypeDef",
     "CustomLineItemChargeDetailsTypeDef",
     "TieringTypeDef",
-    "ListAccountAssociationsInputRequestTypeDef",
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
-    "ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    "ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    "ListAccountAssociationsInputRequestTypeDef",
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     "ListBillingGroupCostReportsInputRequestTypeDef",
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsInputRequestTypeDef",
     "ListCustomLineItemChargeDetailsTypeDef",
     "ListCustomLineItemVersionsFilterTypeDef",
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
@@ -152,14 +152,15 @@
     "AccountAssociationsListElementTypeDef",
     {
         "AccountId": str,
         "BillingGroupArn": str,
         "AccountName": str,
         "AccountEmail": str,
     },
+    total=False,
 )
 
 _RequiredAccountGroupingTypeDef = TypedDict(
     "_RequiredAccountGroupingTypeDef",
     {
         "LinkedAccountIds": Sequence[str],
     },
@@ -179,39 +180,45 @@
     "AssociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AssociateAccountsOutputTypeDef = TypedDict(
+    "AssociateAccountsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociatePricingRulesInputRequestTypeDef = TypedDict(
     "AssociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+AssociatePricingRulesOutputTypeDef = TypedDict(
+    "AssociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 AssociateResourceErrorTypeDef = TypedDict(
     "AssociateResourceErrorTypeDef",
     {
         "Message": str,
         "Reason": AssociateResourceErrorReasonType,
     },
+    total=False,
 )
 
 _RequiredCustomLineItemBillingPeriodRangeTypeDef = TypedDict(
     "_RequiredCustomLineItemBillingPeriodRangeTypeDef",
     {
         "InclusiveStartBillingPeriod": str,
     },
@@ -236,37 +243,55 @@
         "Arn": str,
         "AWSCost": str,
         "ProformaCost": str,
         "Margin": str,
         "MarginPercentage": str,
         "Currency": str,
     },
+    total=False,
 )
 
 ComputationPreferenceOutputTypeDef = TypedDict(
     "ComputationPreferenceOutputTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
 ListBillingGroupAccountGroupingTypeDef = TypedDict(
     "ListBillingGroupAccountGroupingTypeDef",
     {
         "AutoAssociate": bool,
     },
+    total=False,
 )
 
 ComputationPreferenceTypeDef = TypedDict(
     "ComputationPreferenceTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 
+CreateBillingGroupOutputTypeDef = TypedDict(
+    "CreateBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreateCustomLineItemOutputTypeDef = TypedDict(
+    "CreateCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CreateFreeTierConfigTypeDef = TypedDict(
     "CreateFreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -288,14 +313,30 @@
 )
 
 class CreatePricingPlanInputRequestTypeDef(
     _RequiredCreatePricingPlanInputRequestTypeDef, _OptionalCreatePricingPlanInputRequestTypeDef
 ):
     pass
 
+CreatePricingPlanOutputTypeDef = TypedDict(
+    "CreatePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+CreatePricingRuleOutputTypeDef = TypedDict(
+    "CreatePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 CustomLineItemFlatChargeDetailsTypeDef = TypedDict(
     "CustomLineItemFlatChargeDetailsTypeDef",
     {
         "ChargeValue": float,
     },
 )
 
@@ -322,44 +363,92 @@
 DeleteBillingGroupInputRequestTypeDef = TypedDict(
     "DeleteBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeleteBillingGroupOutputTypeDef = TypedDict(
+    "DeleteBillingGroupOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DeleteCustomLineItemOutputTypeDef = TypedDict(
+    "DeleteCustomLineItemOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingPlanInputRequestTypeDef = TypedDict(
     "DeletePricingPlanInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingPlanOutputTypeDef = TypedDict(
+    "DeletePricingPlanOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeletePricingRuleInputRequestTypeDef = TypedDict(
     "DeletePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DeletePricingRuleOutputTypeDef = TypedDict(
+    "DeletePricingRuleOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociateAccountsInputRequestTypeDef = TypedDict(
     "DisassociateAccountsInputRequestTypeDef",
     {
         "Arn": str,
         "AccountIds": Sequence[str],
     },
 )
 
+DisassociateAccountsOutputTypeDef = TypedDict(
+    "DisassociateAccountsOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DisassociatePricingRulesInputRequestTypeDef = TypedDict(
     "DisassociatePricingRulesInputRequestTypeDef",
     {
         "Arn": str,
         "PricingRuleArns": Sequence[str],
     },
 )
 
+DisassociatePricingRulesOutputTypeDef = TypedDict(
+    "DisassociatePricingRulesOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 FreeTierConfigTypeDef = TypedDict(
     "FreeTierConfigTypeDef",
     {
         "Activated": bool,
     },
 )
 
@@ -369,24 +458,14 @@
         "Association": str,
         "AccountId": str,
         "AccountIds": Sequence[str],
     },
     total=False,
 )
 
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
 ListBillingGroupCostReportsFilterTypeDef = TypedDict(
     "ListBillingGroupCostReportsFilterTypeDef",
     {
         "BillingGroupArns": Sequence[str],
     },
     total=False,
 )
@@ -431,14 +510,35 @@
         "Names": Sequence[str],
         "BillingGroups": Sequence[str],
         "Arns": Sequence[str],
     },
     total=False,
 )
 
+_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "PricingRuleArn": str,
+    },
+)
+_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
+    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
+    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
+):
+    pass
+
 _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef",
     {
         "PricingRuleArn": str,
     },
 )
 _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = TypedDict(
@@ -453,14 +553,25 @@
 
 class ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef(
     _RequiredListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
     _OptionalListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
 ):
     pass
 
+ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
+    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingRuleArn": str,
+        "PricingPlanArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingPlansFilterTypeDef = TypedDict(
     "ListPricingPlansFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -471,16 +582,38 @@
         "Name": str,
         "Arn": str,
         "Description": str,
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
     },
+    total=False,
+)
+
+_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "PricingPlanArn": str,
+    },
+)
+_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
+    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+    {
+        "BillingPeriod": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
 )
 
+class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
+    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+):
+    pass
+
 _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
     "_RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef",
     {
         "PricingPlanArn": str,
     },
 )
 _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = TypedDict(
@@ -495,14 +628,25 @@
 
 class ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef(
     _RequiredListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
     _OptionalListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
 ):
     pass
 
+ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
+    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
+    {
+        "BillingPeriod": str,
+        "PricingPlanArn": str,
+        "PricingRuleArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListPricingRulesFilterTypeDef = TypedDict(
     "ListPricingRulesFilterTypeDef",
     {
         "Arns": Sequence[str],
     },
     total=False,
 )
@@ -518,23 +662,53 @@
 ListResourcesAssociatedToCustomLineItemResponseElementTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemResponseElementTypeDef",
     {
         "Arn": str,
         "Relationship": CustomLineItemRelationshipType,
         "EndBillingPeriod": str,
     },
+    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
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
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -548,14 +722,15 @@
 )
 
 UpdateBillingGroupAccountGroupingOutputTypeDef = TypedDict(
     "UpdateBillingGroupAccountGroupingOutputTypeDef",
     {
         "AutoAssociate": bool,
     },
+    total=False,
 )
 
 UpdateBillingGroupAccountGroupingTypeDef = TypedDict(
     "UpdateBillingGroupAccountGroupingTypeDef",
     {
         "AutoAssociate": bool,
     },
@@ -606,175 +781,51 @@
 )
 
 class UpdatePricingPlanInputRequestTypeDef(
     _RequiredUpdatePricingPlanInputRequestTypeDef, _OptionalUpdatePricingPlanInputRequestTypeDef
 ):
     pass
 
-AssociateAccountsOutputTypeDef = TypedDict(
-    "AssociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AssociatePricingRulesOutputTypeDef = TypedDict(
-    "AssociatePricingRulesOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateBillingGroupOutputTypeDef = TypedDict(
-    "CreateBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateCustomLineItemOutputTypeDef = TypedDict(
-    "CreateCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingPlanOutputTypeDef = TypedDict(
-    "CreatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreatePricingRuleOutputTypeDef = TypedDict(
-    "CreatePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteBillingGroupOutputTypeDef = TypedDict(
-    "DeleteBillingGroupOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteCustomLineItemOutputTypeDef = TypedDict(
-    "DeleteCustomLineItemOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingPlanOutputTypeDef = TypedDict(
-    "DeletePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeletePricingRuleOutputTypeDef = TypedDict(
-    "DeletePricingRuleOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociateAccountsOutputTypeDef = TypedDict(
-    "DisassociateAccountsOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DisassociatePricingRulesOutputTypeDef = TypedDict(
-    "DisassociatePricingRulesOutputTypeDef",
+UpdatePricingPlanOutputTypeDef = TypedDict(
+    "UpdatePricingPlanOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Name": str,
+        "Description": str,
+        "Size": int,
+        "LastModifiedTime": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListAccountAssociationsOutputTypeDef = TypedDict(
     "ListAccountAssociationsOutputTypeDef",
     {
         "LinkedAccounts": List[AccountAssociationsListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingPlansAssociatedWithPricingRuleOutputTypeDef = TypedDict(
-    "ListPricingPlansAssociatedWithPricingRuleOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingRuleArn": str,
-        "PricingPlanArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListPricingRulesAssociatedToPricingPlanOutputTypeDef = TypedDict(
-    "ListPricingRulesAssociatedToPricingPlanOutputTypeDef",
-    {
-        "BillingPeriod": str,
-        "PricingPlanArn": str,
-        "PricingRuleArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePricingPlanOutputTypeDef = TypedDict(
-    "UpdatePricingPlanOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Size": int,
-        "LastModifiedTime": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 AssociateResourceResponseElementTypeDef = TypedDict(
     "AssociateResourceResponseElementTypeDef",
     {
         "Arn": str,
         "Error": AssociateResourceErrorTypeDef,
     },
+    total=False,
 )
 
 DisassociateResourceResponseElementTypeDef = TypedDict(
     "DisassociateResourceResponseElementTypeDef",
     {
         "Arn": str,
         "Error": AssociateResourceErrorTypeDef,
     },
+    total=False,
 )
 
 _RequiredBatchAssociateResourcesToCustomLineItemInputRequestTypeDef = TypedDict(
     "_RequiredBatchAssociateResourcesToCustomLineItemInputRequestTypeDef",
     {
         "TargetArn": str,
         "ResourceArns": Sequence[str],
@@ -836,15 +887,15 @@
     pass
 
 ListBillingGroupCostReportsOutputTypeDef = TypedDict(
     "ListBillingGroupCostReportsOutputTypeDef",
     {
         "BillingGroupCostReports": List[BillingGroupCostReportElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BillingGroupListElementTypeDef = TypedDict(
     "BillingGroupListElementTypeDef",
     {
         "Name": str,
@@ -855,14 +906,15 @@
         "Size": int,
         "CreationTime": int,
         "LastModifiedTime": int,
         "Status": BillingGroupStatusType,
         "StatusReason": str,
         "AccountGrouping": ListBillingGroupAccountGroupingTypeDef,
     },
+    total=False,
 )
 
 _RequiredCreateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateBillingGroupInputRequestTypeDef",
     {
         "Name": str,
         "AccountGrouping": AccountGroupingTypeDef,
@@ -915,82 +967,40 @@
 TieringTypeDef = TypedDict(
     "TieringTypeDef",
     {
         "FreeTier": FreeTierConfigTypeDef,
     },
 )
 
-ListAccountAssociationsInputRequestTypeDef = TypedDict(
-    "ListAccountAssociationsInputRequestTypeDef",
-    {
-        "BillingPeriod": str,
-        "Filters": ListAccountAssociationsFilterTypeDef,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef = TypedDict(
     "ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListAccountAssociationsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "PricingRuleArn": str,
-    },
-)
-_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef = TypedDict(
-    "_OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef",
-    {
-        "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef(
-    _RequiredListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    _OptionalListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-):
-    pass
-
-_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
-    {
-        "PricingPlanArn": str,
-    },
-)
-_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef = TypedDict(
-    "_OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef",
+ListAccountAssociationsInputRequestTypeDef = TypedDict(
+    "ListAccountAssociationsInputRequestTypeDef",
     {
         "BillingPeriod": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Filters": ListAccountAssociationsFilterTypeDef,
+        "NextToken": str,
     },
     total=False,
 )
 
-class ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef(
-    _RequiredListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-    _OptionalListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
-):
-    pass
-
 ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupCostReportsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupCostReportsInputRequestTypeDef = TypedDict(
     "ListBillingGroupCostReportsInputRequestTypeDef",
     {
@@ -1003,15 +1013,15 @@
 )
 
 ListBillingGroupsInputListBillingGroupsPaginateTypeDef = TypedDict(
     "ListBillingGroupsInputListBillingGroupsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListBillingGroupsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListBillingGroupsInputRequestTypeDef = TypedDict(
     "ListBillingGroupsInputRequestTypeDef",
     {
@@ -1019,37 +1029,48 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": ListBillingGroupsFilterTypeDef,
     },
     total=False,
 )
 
-ListCustomLineItemChargeDetailsTypeDef = TypedDict(
-    "ListCustomLineItemChargeDetailsTypeDef",
+_RequiredListCustomLineItemChargeDetailsTypeDef = TypedDict(
+    "_RequiredListCustomLineItemChargeDetailsTypeDef",
+    {
+        "Type": CustomLineItemTypeType,
+    },
+)
+_OptionalListCustomLineItemChargeDetailsTypeDef = TypedDict(
+    "_OptionalListCustomLineItemChargeDetailsTypeDef",
     {
         "Flat": ListCustomLineItemFlatChargeDetailsTypeDef,
         "Percentage": ListCustomLineItemPercentageChargeDetailsTypeDef,
-        "Type": CustomLineItemTypeType,
     },
+    total=False,
 )
 
+class ListCustomLineItemChargeDetailsTypeDef(
+    _RequiredListCustomLineItemChargeDetailsTypeDef, _OptionalListCustomLineItemChargeDetailsTypeDef
+):
+    pass
+
 ListCustomLineItemVersionsFilterTypeDef = TypedDict(
     "ListCustomLineItemVersionsFilterTypeDef",
     {
         "BillingPeriodRange": ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     },
     total=False,
 )
 
 ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef = TypedDict(
     "ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListCustomLineItemsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListCustomLineItemsInputRequestTypeDef = TypedDict(
     "ListCustomLineItemsInputRequestTypeDef",
     {
@@ -1062,15 +1083,15 @@
 )
 
 ListPricingPlansInputListPricingPlansPaginateTypeDef = TypedDict(
     "ListPricingPlansInputListPricingPlansPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingPlansFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingPlansInputRequestTypeDef = TypedDict(
     "ListPricingPlansInputRequestTypeDef",
     {
@@ -1084,24 +1105,24 @@
 
 ListPricingPlansOutputTypeDef = TypedDict(
     "ListPricingPlansOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingPlans": List[PricingPlanListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListPricingRulesInputListPricingRulesPaginateTypeDef = TypedDict(
     "ListPricingRulesInputListPricingRulesPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListPricingRulesFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListPricingRulesInputRequestTypeDef = TypedDict(
     "ListPricingRulesInputRequestTypeDef",
     {
@@ -1120,15 +1141,15 @@
     },
 )
 _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef = TypedDict(
     "_OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef",
     {
         "BillingPeriod": str,
         "Filters": ListResourcesAssociatedToCustomLineItemFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef(
     _RequiredListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
     _OptionalListResourcesAssociatedToCustomLineItemInputListResourcesAssociatedToCustomLineItemPaginateTypeDef,
@@ -1160,15 +1181,15 @@
 
 ListResourcesAssociatedToCustomLineItemOutputTypeDef = TypedDict(
     "ListResourcesAssociatedToCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "AssociatedResources": List[ListResourcesAssociatedToCustomLineItemResponseElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateBillingGroupOutputTypeDef = TypedDict(
     "UpdateBillingGroupOutputTypeDef",
     {
         "Arn": str,
@@ -1177,15 +1198,15 @@
         "PrimaryAccountId": str,
         "PricingPlanArn": str,
         "Size": int,
         "LastModifiedTime": int,
         "Status": BillingGroupStatusType,
         "StatusReason": str,
         "AccountGrouping": UpdateBillingGroupAccountGroupingOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdateBillingGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupInputRequestTypeDef",
     {
         "Arn": str,
@@ -1232,33 +1253,33 @@
 )
 
 BatchAssociateResourcesToCustomLineItemOutputTypeDef = TypedDict(
     "BatchAssociateResourcesToCustomLineItemOutputTypeDef",
     {
         "SuccessfullyAssociatedResources": List[AssociateResourceResponseElementTypeDef],
         "FailedAssociatedResources": List[AssociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 BatchDisassociateResourcesFromCustomLineItemOutputTypeDef = TypedDict(
     "BatchDisassociateResourcesFromCustomLineItemOutputTypeDef",
     {
         "SuccessfullyDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
         "FailedDisassociatedResources": List[DisassociateResourceResponseElementTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListBillingGroupsOutputTypeDef = TypedDict(
     "ListBillingGroupsOutputTypeDef",
     {
         "BillingGroups": List[BillingGroupListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredCreatePricingRuleInputRequestTypeDef",
     {
         "Name": str,
@@ -1326,14 +1347,15 @@
         "CreationTime": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": TieringTypeDef,
         "UsageType": str,
         "Operation": str,
     },
+    total=False,
 )
 
 CustomLineItemListElementTypeDef = TypedDict(
     "CustomLineItemListElementTypeDef",
     {
         "Arn": str,
         "Name": str,
@@ -1342,14 +1364,15 @@
         "Description": str,
         "ProductCode": str,
         "BillingGroupArn": str,
         "CreationTime": int,
         "LastModifiedTime": int,
         "AssociationSize": int,
     },
+    total=False,
 )
 
 CustomLineItemVersionListElementTypeDef = TypedDict(
     "CustomLineItemVersionListElementTypeDef",
     {
         "Name": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
@@ -1361,41 +1384,42 @@
         "LastModifiedTime": int,
         "AssociationSize": int,
         "StartBillingPeriod": str,
         "EndBillingPeriod": str,
         "Arn": str,
         "StartTime": int,
     },
+    total=False,
 )
 
 UpdateCustomLineItemOutputTypeDef = TypedDict(
     "UpdateCustomLineItemOutputTypeDef",
     {
         "Arn": str,
         "BillingGroupArn": str,
         "Name": str,
         "Description": str,
         "ChargeDetails": ListCustomLineItemChargeDetailsTypeDef,
         "LastModifiedTime": int,
         "AssociationSize": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef = TypedDict(
     "_OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef",
     {
         "Filters": ListCustomLineItemVersionsFilterTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 class ListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef(
     _RequiredListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
     _OptionalListCustomLineItemVersionsInputListCustomLineItemVersionsPaginateTypeDef,
@@ -1459,15 +1483,15 @@
         "Service": str,
         "AssociatedPricingPlanCount": int,
         "LastModifiedTime": int,
         "BillingEntity": str,
         "Tiering": UpdateTieringInputOutputTypeDef,
         "UsageType": str,
         "Operation": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredUpdatePricingRuleInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingRuleInputRequestTypeDef",
     {
         "Arn": str,
@@ -1492,28 +1516,28 @@
 
 ListPricingRulesOutputTypeDef = TypedDict(
     "ListPricingRulesOutputTypeDef",
     {
         "BillingPeriod": str,
         "PricingRules": List[PricingRuleListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemsOutputTypeDef = TypedDict(
     "ListCustomLineItemsOutputTypeDef",
     {
         "CustomLineItems": List[CustomLineItemListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListCustomLineItemVersionsOutputTypeDef = TypedDict(
     "ListCustomLineItemVersionsOutputTypeDef",
     {
         "CustomLineItemVersions": List[CustomLineItemVersionListElementTypeDef],
         "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/PKG-INFO` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-billingconductor
-Version: 1.28.11
-Summary: Type annotations for boto3.BillingConductor 1.28.11 service generated with mypy-boto3-builder 7.15.1
+Version: 1.28.12
+Summary: Type annotations for boto3.BillingConductor 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-billingconductor"></a>
 
 # mypy-boto3-billingconductor
 
 [![PyPI - mypy-boto3-billingconductor](https://img.shields.io/pypi/v/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-billingconductor.svg?color=blue)](https://pypi.org/project/mypy-boto3-billingconductor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-billingconductor?color=blue)](https://pypistats.org/packages/mypy-boto3-billingconductor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-billingconductor)](https://pepy.tech/project/mypy-boto3-billingconductor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BillingConductor 1.28.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
+[boto3.BillingConductor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor)
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
 [mypy-boto3-billingconductor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_billingconductor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,89 +374,89 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_billingconductor.type_defs import (
     AccountAssociationsListElementTypeDef,
     AccountGroupingTypeDef,
     AssociateAccountsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AssociateAccountsOutputTypeDef,
     AssociatePricingRulesInputRequestTypeDef,
+    AssociatePricingRulesOutputTypeDef,
     AssociateResourceErrorTypeDef,
     CustomLineItemBillingPeriodRangeTypeDef,
     BillingGroupCostReportElementTypeDef,
     ComputationPreferenceOutputTypeDef,
     ListBillingGroupAccountGroupingTypeDef,
     ComputationPreferenceTypeDef,
+    CreateBillingGroupOutputTypeDef,
+    CreateCustomLineItemOutputTypeDef,
     CreateFreeTierConfigTypeDef,
     CreatePricingPlanInputRequestTypeDef,
+    CreatePricingPlanOutputTypeDef,
+    CreatePricingRuleOutputTypeDef,
     CustomLineItemFlatChargeDetailsTypeDef,
     CustomLineItemPercentageChargeDetailsTypeDef,
     DeleteBillingGroupInputRequestTypeDef,
+    DeleteBillingGroupOutputTypeDef,
+    DeleteCustomLineItemOutputTypeDef,
     DeletePricingPlanInputRequestTypeDef,
+    DeletePricingPlanOutputTypeDef,
     DeletePricingRuleInputRequestTypeDef,
+    DeletePricingRuleOutputTypeDef,
     DisassociateAccountsInputRequestTypeDef,
+    DisassociateAccountsOutputTypeDef,
     DisassociatePricingRulesInputRequestTypeDef,
+    DisassociatePricingRulesOutputTypeDef,
     FreeTierConfigTypeDef,
     ListAccountAssociationsFilterTypeDef,
-    PaginatorConfigTypeDef,
     ListBillingGroupCostReportsFilterTypeDef,
     ListBillingGroupsFilterTypeDef,
     ListCustomLineItemFlatChargeDetailsTypeDef,
     ListCustomLineItemPercentageChargeDetailsTypeDef,
     ListCustomLineItemVersionsBillingPeriodRangeFilterTypeDef,
     ListCustomLineItemsFilterTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
     ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef,
+    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
     ListPricingPlansFilterTypeDef,
     PricingPlanListElementTypeDef,
+    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
     ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef,
+    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
     ListPricingRulesFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemFilterTypeDef,
     ListResourcesAssociatedToCustomLineItemResponseElementTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateBillingGroupAccountGroupingOutputTypeDef,
     UpdateBillingGroupAccountGroupingTypeDef,
     UpdateCustomLineItemFlatChargeDetailsTypeDef,
     UpdateCustomLineItemPercentageChargeDetailsTypeDef,
     UpdateFreeTierConfigOutputTypeDef,
     UpdateFreeTierConfigTypeDef,
     UpdatePricingPlanInputRequestTypeDef,
-    AssociateAccountsOutputTypeDef,
-    AssociatePricingRulesOutputTypeDef,
-    CreateBillingGroupOutputTypeDef,
-    CreateCustomLineItemOutputTypeDef,
-    CreatePricingPlanOutputTypeDef,
-    CreatePricingRuleOutputTypeDef,
-    DeleteBillingGroupOutputTypeDef,
-    DeleteCustomLineItemOutputTypeDef,
-    DeletePricingPlanOutputTypeDef,
-    DeletePricingRuleOutputTypeDef,
-    DisassociateAccountsOutputTypeDef,
-    DisassociatePricingRulesOutputTypeDef,
-    ListAccountAssociationsOutputTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleOutputTypeDef,
-    ListPricingRulesAssociatedToPricingPlanOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
     UpdatePricingPlanOutputTypeDef,
+    ListAccountAssociationsOutputTypeDef,
     AssociateResourceResponseElementTypeDef,
     DisassociateResourceResponseElementTypeDef,
     BatchAssociateResourcesToCustomLineItemInputRequestTypeDef,
     BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef,
     DeleteCustomLineItemInputRequestTypeDef,
     ListBillingGroupCostReportsOutputTypeDef,
     BillingGroupListElementTypeDef,
     CreateBillingGroupInputRequestTypeDef,
     CreateTieringInputTypeDef,
     CustomLineItemChargeDetailsTypeDef,
     TieringTypeDef,
-    ListAccountAssociationsInputRequestTypeDef,
     ListAccountAssociationsInputListAccountAssociationsPaginateTypeDef,
-    ListPricingPlansAssociatedWithPricingRuleInputListPricingPlansAssociatedWithPricingRulePaginateTypeDef,
-    ListPricingRulesAssociatedToPricingPlanInputListPricingRulesAssociatedToPricingPlanPaginateTypeDef,
+    ListAccountAssociationsInputRequestTypeDef,
     ListBillingGroupCostReportsInputListBillingGroupCostReportsPaginateTypeDef,
     ListBillingGroupCostReportsInputRequestTypeDef,
     ListBillingGroupsInputListBillingGroupsPaginateTypeDef,
     ListBillingGroupsInputRequestTypeDef,
     ListCustomLineItemChargeDetailsTypeDef,
     ListCustomLineItemVersionsFilterTypeDef,
     ListCustomLineItemsInputListCustomLineItemsPaginateTypeDef,
```

### Comparing `mypy-boto3-billingconductor-1.28.11/mypy_boto3_billingconductor.egg-info/SOURCES.txt` & `mypy-boto3-billingconductor-1.28.12/mypy_boto3_billingconductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-billingconductor-1.28.11/setup.py` & `mypy-boto3-billingconductor-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-billingconductor",
-    version="1.28.11",
+    version="1.28.12",
     packages=["mypy_boto3_billingconductor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BillingConductor 1.28.11 service generated with"
-        " mypy-boto3-builder 7.15.1"
+        "Type annotations for boto3.BillingConductor 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

