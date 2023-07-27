# Comparing `tmp/mypy-boto3-budgets-1.28.0.tar.gz` & `tmp/mypy-boto3-budgets-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-budgets-1.28.0.tar", last modified: Thu Jul  6 20:59:05 2023, max compression
+gzip compressed data, was "mypy-boto3-budgets-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
```

## Comparing `mypy-boto3-budgets-1.28.0.tar` & `mypy-boto3-budgets-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.542235 mypy-boto3-budgets-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-06 20:59:05.538235 mypy-boto3-budgets-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16186 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.526235 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-06 20:34:22.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-07-06 20:34:23.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-06 20:34:23.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-06 20:34:23.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-06 20:34:22.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31372 2023-07-06 20:34:24.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-07-06 20:34:23.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:05.538235 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 20:59:05.000000 mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:05.542235 mypy-boto3-budgets-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-06 20:34:21.000000 mypy-boto3-budgets-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.784567 mypy-boto3-budgets-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-27 05:34:22.784567 mypy-boto3-budgets-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16623 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.780567 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21927 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10732 2023-07-27 05:18:03.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10730 2023-07-27 05:18:03.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36980 2023-07-27 05:18:04.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36919 2023-07-27 05:18:03.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.784567 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:22.000000 mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.784567 mypy-boto3-budgets-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:18:02.000000 mypy-boto3-budgets-1.28.12/setup.py
```

### Comparing `mypy-boto3-budgets-1.28.0/LICENSE` & `mypy-boto3-budgets-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/PKG-INFO` & `mypy-boto3-budgets-1.28.12/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-budgets
-Version: 1.28.0
-Summary: Type annotations for boto3.Budgets 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.Budgets 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,22 +368,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
+    ActionThresholdOutputTypeDef,
     ActionThresholdTypeDef,
-    SubscriberTypeDef,
+    SubscriberOutputTypeDef,
+    HistoricalOptionsOutputTypeDef,
     HistoricalOptionsTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
+    CostTypesOutputTypeDef,
+    SpendOutputTypeDef,
+    TimePeriodOutputTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
+    SubscriberTypeDef,
     CreateBudgetActionResponseTypeDef,
+    NotificationTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
@@ -398,56 +408,60 @@
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    CalculatedSpendOutputTypeDef,
+    BudgetedAndActualAmountsTypeDef,
+    CalculatedSpendTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    CalculatedSpendTypeDef,
-    BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    DefinitionOutputTypeDef,
     DefinitionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
-    BudgetTypeDef,
+    BudgetOutputTypeDef,
     BudgetPerformanceHistoryTypeDef,
+    BudgetTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
-    UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
+    CreateBudgetRequestRequestTypeDef,
+    UpdateBudgetRequestRequestTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_structure() -> ActionThresholdOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.0/README.md` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-budgets
+Version: 1.28.12
+Summary: Type annotations for boto3.Budgets 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,22 +368,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
+    ActionThresholdOutputTypeDef,
     ActionThresholdTypeDef,
-    SubscriberTypeDef,
+    SubscriberOutputTypeDef,
+    HistoricalOptionsOutputTypeDef,
     HistoricalOptionsTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
+    CostTypesOutputTypeDef,
+    SpendOutputTypeDef,
+    TimePeriodOutputTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
+    SubscriberTypeDef,
     CreateBudgetActionResponseTypeDef,
+    NotificationTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
@@ -366,56 +408,60 @@
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    CalculatedSpendOutputTypeDef,
+    BudgetedAndActualAmountsTypeDef,
+    CalculatedSpendTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    CalculatedSpendTypeDef,
-    BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    DefinitionOutputTypeDef,
     DefinitionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
-    BudgetTypeDef,
+    BudgetOutputTypeDef,
     BudgetPerformanceHistoryTypeDef,
+    BudgetTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
-    UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
+    CreateBudgetRequestRequestTypeDef,
+    UpdateBudgetRequestRequestTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_structure() -> ActionThresholdOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__init__.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__init__.pyi` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/__main__.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Budgets 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.Budgets 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/client.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/client.pyi` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/literals.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActionStatusType",
     "ActionSubTypeType",
     "ActionTypeType",
     "ApprovalModelType",
     "AutoAdjustTypeType",
     "BudgetTypeType",
@@ -44,15 +43,14 @@
     "TimeUnitType",
     "BudgetsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionStatusType = Literal[
     "EXECUTION_FAILURE",
     "EXECUTION_IN_PROGRESS",
     "EXECUTION_SUCCESS",
     "PENDING",
     "RESET_FAILURE",
     "RESET_IN_PROGRESS",
@@ -211,14 +209,15 @@
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
@@ -297,26 +296,28 @@
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

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/literals.pyi` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/literals.py`

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
     "ActionStatusType",
     "ActionSubTypeType",
     "ActionTypeType",
     "ApprovalModelType",
     "AutoAdjustTypeType",
     "BudgetTypeType",
@@ -43,14 +44,15 @@
     "TimeUnitType",
     "BudgetsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
+
 ActionStatusType = Literal[
     "EXECUTION_FAILURE",
     "EXECUTION_IN_PROGRESS",
     "EXECUTION_SUCCESS",
     "PENDING",
     "RESET_FAILURE",
     "RESET_IN_PROGRESS",
@@ -209,14 +211,15 @@
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
@@ -295,26 +298,28 @@
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

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/paginator.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/paginator.pyi` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/type_defs.py` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for budgets service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_budgets.type_defs import ActionThresholdTypeDef
+    from mypy_boto3_budgets.type_defs import ActionThresholdOutputTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -35,22 +35,32 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ActionThresholdOutputTypeDef",
     "ActionThresholdTypeDef",
-    "SubscriberTypeDef",
+    "SubscriberOutputTypeDef",
+    "HistoricalOptionsOutputTypeDef",
     "HistoricalOptionsTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
+    "CostTypesOutputTypeDef",
+    "SpendOutputTypeDef",
+    "TimePeriodOutputTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodTypeDef",
+    "SubscriberTypeDef",
     "CreateBudgetActionResponseTypeDef",
+    "NotificationTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
@@ -65,70 +75,103 @@
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "BudgetNotificationsForAccountTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "CalculatedSpendOutputTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
+    "CalculatedSpendTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "CalculatedSpendTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetPerformanceHistoryTypeDef",
+    "BudgetTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
-    "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
+    "UpdateBudgetRequestRequestTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
     "ActionHistoryTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
+ActionThresholdOutputTypeDef = TypedDict(
+    "ActionThresholdOutputTypeDef",
+    {
+        "ActionThresholdValue": float,
+        "ActionThresholdType": ThresholdTypeType,
+    },
+)
+
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
         "ActionThresholdValue": float,
         "ActionThresholdType": ThresholdTypeType,
     },
 )
 
-SubscriberTypeDef = TypedDict(
-    "SubscriberTypeDef",
+SubscriberOutputTypeDef = TypedDict(
+    "SubscriberOutputTypeDef",
     {
         "SubscriptionType": SubscriptionTypeType,
         "Address": str,
     },
 )
 
+_RequiredHistoricalOptionsOutputTypeDef = TypedDict(
+    "_RequiredHistoricalOptionsOutputTypeDef",
+    {
+        "BudgetAdjustmentPeriod": int,
+    },
+)
+_OptionalHistoricalOptionsOutputTypeDef = TypedDict(
+    "_OptionalHistoricalOptionsOutputTypeDef",
+    {
+        "LookBackAvailablePeriods": int,
+    },
+    total=False,
+)
+
+
+class HistoricalOptionsOutputTypeDef(
+    _RequiredHistoricalOptionsOutputTypeDef, _OptionalHistoricalOptionsOutputTypeDef
+):
+    pass
+
+
 _RequiredHistoricalOptionsTypeDef = TypedDict(
     "_RequiredHistoricalOptionsTypeDef",
     {
         "BudgetAdjustmentPeriod": int,
     },
 )
 _OptionalHistoricalOptionsTypeDef = TypedDict(
@@ -142,36 +185,73 @@
 
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
 
-_RequiredNotificationTypeDef = TypedDict(
-    "_RequiredNotificationTypeDef",
+_RequiredNotificationOutputTypeDef = TypedDict(
+    "_RequiredNotificationOutputTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
 )
-_OptionalNotificationTypeDef = TypedDict(
-    "_OptionalNotificationTypeDef",
+_OptionalNotificationOutputTypeDef = TypedDict(
+    "_OptionalNotificationOutputTypeDef",
     {
         "ThresholdType": ThresholdTypeType,
         "NotificationState": NotificationStateType,
     },
     total=False,
 )
 
 
-class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
+class NotificationOutputTypeDef(
+    _RequiredNotificationOutputTypeDef, _OptionalNotificationOutputTypeDef
+):
     pass
 
 
+CostTypesOutputTypeDef = TypedDict(
+    "CostTypesOutputTypeDef",
+    {
+        "IncludeTax": bool,
+        "IncludeSubscription": bool,
+        "UseBlended": bool,
+        "IncludeRefund": bool,
+        "IncludeCredit": bool,
+        "IncludeUpfront": bool,
+        "IncludeRecurring": bool,
+        "IncludeOtherSubscription": bool,
+        "IncludeSupport": bool,
+        "IncludeDiscount": bool,
+        "UseAmortized": bool,
+    },
+    total=False,
+)
+
+SpendOutputTypeDef = TypedDict(
+    "SpendOutputTypeDef",
+    {
+        "Amount": str,
+        "Unit": str,
+    },
+)
+
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
+    {
+        "Start": datetime,
+        "End": datetime,
+    },
+    total=False,
+)
+
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": bool,
         "IncludeSubscription": bool,
         "UseBlended": bool,
         "IncludeRefund": bool,
@@ -199,24 +279,94 @@
     {
         "Start": Union[datetime, str],
         "End": Union[datetime, str],
     },
     total=False,
 )
 
+SubscriberTypeDef = TypedDict(
+    "SubscriberTypeDef",
+    {
+        "SubscriptionType": SubscriptionTypeType,
+        "Address": str,
+    },
+)
+
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredNotificationTypeDef = TypedDict(
+    "_RequiredNotificationTypeDef",
+    {
+        "NotificationType": NotificationTypeType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Threshold": float,
+    },
+)
+_OptionalNotificationTypeDef = TypedDict(
+    "_OptionalNotificationTypeDef",
+    {
+        "ThresholdType": ThresholdTypeType,
+        "NotificationState": NotificationStateType,
+    },
+    total=False,
+)
+
+
+class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
+    pass
+
+
+_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
+    "_RequiredIamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
+    "_OptionalIamActionDefinitionOutputTypeDef",
+    {
+        "Roles": List[str],
+        "Groups": List[str],
+        "Users": List[str],
+    },
+    total=False,
+)
+
+
+class IamActionDefinitionOutputTypeDef(
+    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
+):
+    pass
+
+
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
+    },
+)
+
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalIamActionDefinitionTypeDef = TypedDict(
@@ -556,20 +706,42 @@
         "RetryAttempts": int,
     },
 )
 
 DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
     "DescribeSubscribersForNotificationResponseTypeDef",
     {
-        "Subscribers": List[SubscriberTypeDef],
+        "Subscribers": List[SubscriberOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
+    "_RequiredAutoAdjustDataOutputTypeDef",
+    {
+        "AutoAdjustType": AutoAdjustTypeType,
+    },
+)
+_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
+    "_OptionalAutoAdjustDataOutputTypeDef",
+    {
+        "HistoricalOptions": HistoricalOptionsOutputTypeDef,
+        "LastAutoAdjustTime": datetime,
+    },
+    total=False,
+)
+
+
+class AutoAdjustDataOutputTypeDef(
+    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
+):
+    pass
+
+
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -585,146 +757,60 @@
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
 
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
-        "Notifications": List[NotificationTypeDef],
+        "Notifications": List[NotificationOutputTypeDef],
         "BudgetName": str,
     },
     total=False,
 )
 
-CreateNotificationRequestRequestTypeDef = TypedDict(
-    "CreateNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscribers": Sequence[SubscriberTypeDef],
-    },
-)
-
-CreateSubscriberRequestRequestTypeDef = TypedDict(
-    "CreateSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscriber": SubscriberTypeDef,
-    },
-)
-
-DeleteNotificationRequestRequestTypeDef = TypedDict(
-    "DeleteNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-
-DeleteSubscriberRequestRequestTypeDef = TypedDict(
-    "DeleteSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscriber": SubscriberTypeDef,
-    },
-)
-
 DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
     "DescribeNotificationsForBudgetResponseTypeDef",
     {
-        "Notifications": List[NotificationTypeDef],
+        "Notifications": List[NotificationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+_RequiredCalculatedSpendOutputTypeDef = TypedDict(
+    "_RequiredCalculatedSpendOutputTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
+        "ActualSpend": SpendOutputTypeDef,
     },
 )
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+_OptionalCalculatedSpendOutputTypeDef = TypedDict(
+    "_OptionalCalculatedSpendOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ForecastedSpend": SpendOutputTypeDef,
     },
     total=False,
 )
 
 
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+class CalculatedSpendOutputTypeDef(
+    _RequiredCalculatedSpendOutputTypeDef, _OptionalCalculatedSpendOutputTypeDef
 ):
     pass
 
 
-_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef",
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "BudgetedAmount": SpendOutputTypeDef,
+        "ActualAmount": SpendOutputTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
     },
     total=False,
 )
 
-
-class DescribeSubscribersForNotificationRequestRequestTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
-):
-    pass
-
-
-NotificationWithSubscribersTypeDef = TypedDict(
-    "NotificationWithSubscribersTypeDef",
-    {
-        "Notification": NotificationTypeDef,
-        "Subscribers": Sequence[SubscriberTypeDef],
-    },
-)
-
-UpdateNotificationRequestRequestTypeDef = TypedDict(
-    "UpdateNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "OldNotification": NotificationTypeDef,
-        "NewNotification": NotificationTypeDef,
-    },
-)
-
-UpdateSubscriberRequestRequestTypeDef = TypedDict(
-    "UpdateSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "OldSubscriber": SubscriberTypeDef,
-        "NewSubscriber": SubscriberTypeDef,
-    },
-)
-
 _RequiredCalculatedSpendTypeDef = TypedDict(
     "_RequiredCalculatedSpendTypeDef",
     {
         "ActualSpend": SpendTypeDef,
     },
 )
 _OptionalCalculatedSpendTypeDef = TypedDict(
@@ -736,24 +822,14 @@
 )
 
 
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
 
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": SpendTypeDef,
-        "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -850,14 +926,141 @@
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+CreateNotificationRequestRequestTypeDef = TypedDict(
+    "CreateNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscribers": Sequence[SubscriberTypeDef],
+    },
+)
+
+CreateSubscriberRequestRequestTypeDef = TypedDict(
+    "CreateSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscriber": SubscriberTypeDef,
+    },
+)
+
+DeleteNotificationRequestRequestTypeDef = TypedDict(
+    "DeleteNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+
+DeleteSubscriberRequestRequestTypeDef = TypedDict(
+    "DeleteSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscriber": SubscriberTypeDef,
+    },
+)
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class DescribeSubscribersForNotificationRequestRequestTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
+):
+    pass
+
+
+NotificationWithSubscribersTypeDef = TypedDict(
+    "NotificationWithSubscribersTypeDef",
+    {
+        "Notification": NotificationTypeDef,
+        "Subscribers": Sequence[SubscriberTypeDef],
+    },
+)
+
+UpdateNotificationRequestRequestTypeDef = TypedDict(
+    "UpdateNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "OldNotification": NotificationTypeDef,
+        "NewNotification": NotificationTypeDef,
+    },
+)
+
+UpdateSubscriberRequestRequestTypeDef = TypedDict(
+    "UpdateSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "OldSubscriber": SubscriberTypeDef,
+        "NewSubscriber": SubscriberTypeDef,
+    },
+)
+
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
@@ -869,14 +1072,55 @@
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBudgetOutputTypeDef = TypedDict(
+    "_RequiredBudgetOutputTypeDef",
+    {
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+    },
+)
+_OptionalBudgetOutputTypeDef = TypedDict(
+    "_OptionalBudgetOutputTypeDef",
+    {
+        "BudgetLimit": SpendOutputTypeDef,
+        "PlannedBudgetLimits": Dict[str, SpendOutputTypeDef],
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesOutputTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+        "CalculatedSpend": CalculatedSpendOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
+    pass
+
+
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
+    {
+        "BudgetName": str,
+        "BudgetType": BudgetTypeType,
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesOutputTypeDef,
+        "TimeUnit": TimeUnitType,
+        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -897,40 +1141,27 @@
 )
 
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
 
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
-    {
-        "BudgetName": str,
-        "BudgetType": BudgetTypeType,
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimeUnit": TimeUnitType,
-        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
-        "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "ActionThreshold": ActionThresholdOutputTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
-        "Subscribers": List[SubscriberTypeDef],
+        "Subscribers": List[SubscriberOutputTypeDef],
     },
 )
 
 CreateBudgetActionRequestRequestTypeDef = TypedDict(
     "CreateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -970,14 +1201,40 @@
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
+    {
+        "Budget": BudgetOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
+    {
+        "Budgets": List[BudgetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    {
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -992,48 +1249,22 @@
 
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
 
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
 
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets/type_defs.pyi` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for budgets service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_budgets.type_defs import ActionThresholdTypeDef
+    from mypy_boto3_budgets.type_defs import ActionThresholdOutputTypeDef
 
-    data: ActionThresholdTypeDef = {...}
+    data: ActionThresholdOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -34,22 +34,32 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ActionThresholdOutputTypeDef",
     "ActionThresholdTypeDef",
-    "SubscriberTypeDef",
+    "SubscriberOutputTypeDef",
+    "HistoricalOptionsOutputTypeDef",
     "HistoricalOptionsTypeDef",
-    "NotificationTypeDef",
+    "NotificationOutputTypeDef",
+    "CostTypesOutputTypeDef",
+    "SpendOutputTypeDef",
+    "TimePeriodOutputTypeDef",
     "CostTypesTypeDef",
     "SpendTypeDef",
     "TimePeriodTypeDef",
+    "SubscriberTypeDef",
     "CreateBudgetActionResponseTypeDef",
+    "NotificationTypeDef",
+    "IamActionDefinitionOutputTypeDef",
+    "ScpActionDefinitionOutputTypeDef",
+    "SsmActionDefinitionOutputTypeDef",
     "IamActionDefinitionTypeDef",
     "ScpActionDefinitionTypeDef",
     "SsmActionDefinitionTypeDef",
     "DeleteBudgetActionRequestRequestTypeDef",
     "DeleteBudgetRequestRequestTypeDef",
     "DescribeBudgetActionRequestRequestTypeDef",
     "DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef",
@@ -64,70 +74,101 @@
     "DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef",
     "DescribeNotificationsForBudgetRequestRequestTypeDef",
     "ExecuteBudgetActionRequestRequestTypeDef",
     "ExecuteBudgetActionResponseTypeDef",
     "PaginatorConfigTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSubscribersForNotificationResponseTypeDef",
+    "AutoAdjustDataOutputTypeDef",
     "AutoAdjustDataTypeDef",
     "BudgetNotificationsForAccountTypeDef",
+    "DescribeNotificationsForBudgetResponseTypeDef",
+    "CalculatedSpendOutputTypeDef",
+    "BudgetedAndActualAmountsTypeDef",
+    "CalculatedSpendTypeDef",
+    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
+    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
+    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
     "CreateNotificationRequestRequestTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "DeleteNotificationRequestRequestTypeDef",
     "DeleteSubscriberRequestRequestTypeDef",
-    "DescribeNotificationsForBudgetResponseTypeDef",
     "DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
     "DescribeSubscribersForNotificationRequestRequestTypeDef",
     "NotificationWithSubscribersTypeDef",
     "UpdateNotificationRequestRequestTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
-    "CalculatedSpendTypeDef",
-    "BudgetedAndActualAmountsTypeDef",
-    "DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
-    "DescribeBudgetActionHistoriesRequestRequestTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef",
-    "DescribeBudgetPerformanceHistoryRequestRequestTypeDef",
+    "DefinitionOutputTypeDef",
     "DefinitionTypeDef",
     "DescribeBudgetNotificationsForAccountResponseTypeDef",
-    "BudgetTypeDef",
+    "BudgetOutputTypeDef",
     "BudgetPerformanceHistoryTypeDef",
+    "BudgetTypeDef",
     "ActionTypeDef",
     "CreateBudgetActionRequestRequestTypeDef",
     "UpdateBudgetActionRequestRequestTypeDef",
-    "CreateBudgetRequestRequestTypeDef",
     "DescribeBudgetResponseTypeDef",
     "DescribeBudgetsResponseTypeDef",
-    "UpdateBudgetRequestRequestTypeDef",
     "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    "CreateBudgetRequestRequestTypeDef",
+    "UpdateBudgetRequestRequestTypeDef",
     "ActionHistoryDetailsTypeDef",
     "DeleteBudgetActionResponseTypeDef",
     "DescribeBudgetActionResponseTypeDef",
     "DescribeBudgetActionsForAccountResponseTypeDef",
     "DescribeBudgetActionsForBudgetResponseTypeDef",
     "UpdateBudgetActionResponseTypeDef",
     "ActionHistoryTypeDef",
     "DescribeBudgetActionHistoriesResponseTypeDef",
 )
 
+ActionThresholdOutputTypeDef = TypedDict(
+    "ActionThresholdOutputTypeDef",
+    {
+        "ActionThresholdValue": float,
+        "ActionThresholdType": ThresholdTypeType,
+    },
+)
+
 ActionThresholdTypeDef = TypedDict(
     "ActionThresholdTypeDef",
     {
         "ActionThresholdValue": float,
         "ActionThresholdType": ThresholdTypeType,
     },
 )
 
-SubscriberTypeDef = TypedDict(
-    "SubscriberTypeDef",
+SubscriberOutputTypeDef = TypedDict(
+    "SubscriberOutputTypeDef",
     {
         "SubscriptionType": SubscriptionTypeType,
         "Address": str,
     },
 )
 
+_RequiredHistoricalOptionsOutputTypeDef = TypedDict(
+    "_RequiredHistoricalOptionsOutputTypeDef",
+    {
+        "BudgetAdjustmentPeriod": int,
+    },
+)
+_OptionalHistoricalOptionsOutputTypeDef = TypedDict(
+    "_OptionalHistoricalOptionsOutputTypeDef",
+    {
+        "LookBackAvailablePeriods": int,
+    },
+    total=False,
+)
+
+class HistoricalOptionsOutputTypeDef(
+    _RequiredHistoricalOptionsOutputTypeDef, _OptionalHistoricalOptionsOutputTypeDef
+):
+    pass
+
 _RequiredHistoricalOptionsTypeDef = TypedDict(
     "_RequiredHistoricalOptionsTypeDef",
     {
         "BudgetAdjustmentPeriod": int,
     },
 )
 _OptionalHistoricalOptionsTypeDef = TypedDict(
@@ -139,34 +180,71 @@
 )
 
 class HistoricalOptionsTypeDef(
     _RequiredHistoricalOptionsTypeDef, _OptionalHistoricalOptionsTypeDef
 ):
     pass
 
-_RequiredNotificationTypeDef = TypedDict(
-    "_RequiredNotificationTypeDef",
+_RequiredNotificationOutputTypeDef = TypedDict(
+    "_RequiredNotificationOutputTypeDef",
     {
         "NotificationType": NotificationTypeType,
         "ComparisonOperator": ComparisonOperatorType,
         "Threshold": float,
     },
 )
-_OptionalNotificationTypeDef = TypedDict(
-    "_OptionalNotificationTypeDef",
+_OptionalNotificationOutputTypeDef = TypedDict(
+    "_OptionalNotificationOutputTypeDef",
     {
         "ThresholdType": ThresholdTypeType,
         "NotificationState": NotificationStateType,
     },
     total=False,
 )
 
-class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
+class NotificationOutputTypeDef(
+    _RequiredNotificationOutputTypeDef, _OptionalNotificationOutputTypeDef
+):
     pass
 
+CostTypesOutputTypeDef = TypedDict(
+    "CostTypesOutputTypeDef",
+    {
+        "IncludeTax": bool,
+        "IncludeSubscription": bool,
+        "UseBlended": bool,
+        "IncludeRefund": bool,
+        "IncludeCredit": bool,
+        "IncludeUpfront": bool,
+        "IncludeRecurring": bool,
+        "IncludeOtherSubscription": bool,
+        "IncludeSupport": bool,
+        "IncludeDiscount": bool,
+        "UseAmortized": bool,
+    },
+    total=False,
+)
+
+SpendOutputTypeDef = TypedDict(
+    "SpendOutputTypeDef",
+    {
+        "Amount": str,
+        "Unit": str,
+    },
+)
+
+TimePeriodOutputTypeDef = TypedDict(
+    "TimePeriodOutputTypeDef",
+    {
+        "Start": datetime,
+        "End": datetime,
+    },
+    total=False,
+)
+
 CostTypesTypeDef = TypedDict(
     "CostTypesTypeDef",
     {
         "IncludeTax": bool,
         "IncludeSubscription": bool,
         "UseBlended": bool,
         "IncludeRefund": bool,
@@ -194,24 +272,90 @@
     {
         "Start": Union[datetime, str],
         "End": Union[datetime, str],
     },
     total=False,
 )
 
+SubscriberTypeDef = TypedDict(
+    "SubscriberTypeDef",
+    {
+        "SubscriptionType": SubscriptionTypeType,
+        "Address": str,
+    },
+)
+
 CreateBudgetActionResponseTypeDef = TypedDict(
     "CreateBudgetActionResponseTypeDef",
     {
         "AccountId": str,
         "BudgetName": str,
         "ActionId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredNotificationTypeDef = TypedDict(
+    "_RequiredNotificationTypeDef",
+    {
+        "NotificationType": NotificationTypeType,
+        "ComparisonOperator": ComparisonOperatorType,
+        "Threshold": float,
+    },
+)
+_OptionalNotificationTypeDef = TypedDict(
+    "_OptionalNotificationTypeDef",
+    {
+        "ThresholdType": ThresholdTypeType,
+        "NotificationState": NotificationStateType,
+    },
+    total=False,
+)
+
+class NotificationTypeDef(_RequiredNotificationTypeDef, _OptionalNotificationTypeDef):
+    pass
+
+_RequiredIamActionDefinitionOutputTypeDef = TypedDict(
+    "_RequiredIamActionDefinitionOutputTypeDef",
+    {
+        "PolicyArn": str,
+    },
+)
+_OptionalIamActionDefinitionOutputTypeDef = TypedDict(
+    "_OptionalIamActionDefinitionOutputTypeDef",
+    {
+        "Roles": List[str],
+        "Groups": List[str],
+        "Users": List[str],
+    },
+    total=False,
+)
+
+class IamActionDefinitionOutputTypeDef(
+    _RequiredIamActionDefinitionOutputTypeDef, _OptionalIamActionDefinitionOutputTypeDef
+):
+    pass
+
+ScpActionDefinitionOutputTypeDef = TypedDict(
+    "ScpActionDefinitionOutputTypeDef",
+    {
+        "PolicyId": str,
+        "TargetIds": List[str],
+    },
+)
+
+SsmActionDefinitionOutputTypeDef = TypedDict(
+    "SsmActionDefinitionOutputTypeDef",
+    {
+        "ActionSubType": ActionSubTypeType,
+        "Region": str,
+        "InstanceIds": List[str],
+    },
+)
+
 _RequiredIamActionDefinitionTypeDef = TypedDict(
     "_RequiredIamActionDefinitionTypeDef",
     {
         "PolicyArn": str,
     },
 )
 _OptionalIamActionDefinitionTypeDef = TypedDict(
@@ -529,20 +673,40 @@
         "RetryAttempts": int,
     },
 )
 
 DescribeSubscribersForNotificationResponseTypeDef = TypedDict(
     "DescribeSubscribersForNotificationResponseTypeDef",
     {
-        "Subscribers": List[SubscriberTypeDef],
+        "Subscribers": List[SubscriberOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredAutoAdjustDataOutputTypeDef = TypedDict(
+    "_RequiredAutoAdjustDataOutputTypeDef",
+    {
+        "AutoAdjustType": AutoAdjustTypeType,
+    },
+)
+_OptionalAutoAdjustDataOutputTypeDef = TypedDict(
+    "_OptionalAutoAdjustDataOutputTypeDef",
+    {
+        "HistoricalOptions": HistoricalOptionsOutputTypeDef,
+        "LastAutoAdjustTime": datetime,
+    },
+    total=False,
+)
+
+class AutoAdjustDataOutputTypeDef(
+    _RequiredAutoAdjustDataOutputTypeDef, _OptionalAutoAdjustDataOutputTypeDef
+):
+    pass
+
 _RequiredAutoAdjustDataTypeDef = TypedDict(
     "_RequiredAutoAdjustDataTypeDef",
     {
         "AutoAdjustType": AutoAdjustTypeType,
     },
 )
 _OptionalAutoAdjustDataTypeDef = TypedDict(
@@ -556,142 +720,58 @@
 
 class AutoAdjustDataTypeDef(_RequiredAutoAdjustDataTypeDef, _OptionalAutoAdjustDataTypeDef):
     pass
 
 BudgetNotificationsForAccountTypeDef = TypedDict(
     "BudgetNotificationsForAccountTypeDef",
     {
-        "Notifications": List[NotificationTypeDef],
+        "Notifications": List[NotificationOutputTypeDef],
         "BudgetName": str,
     },
     total=False,
 )
 
-CreateNotificationRequestRequestTypeDef = TypedDict(
-    "CreateNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscribers": Sequence[SubscriberTypeDef],
-    },
-)
-
-CreateSubscriberRequestRequestTypeDef = TypedDict(
-    "CreateSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscriber": SubscriberTypeDef,
-    },
-)
-
-DeleteNotificationRequestRequestTypeDef = TypedDict(
-    "DeleteNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-
-DeleteSubscriberRequestRequestTypeDef = TypedDict(
-    "DeleteSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "Subscriber": SubscriberTypeDef,
-    },
-)
-
 DescribeNotificationsForBudgetResponseTypeDef = TypedDict(
     "DescribeNotificationsForBudgetResponseTypeDef",
     {
-        "Notifications": List[NotificationTypeDef],
+        "Notifications": List[NotificationOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+_RequiredCalculatedSpendOutputTypeDef = TypedDict(
+    "_RequiredCalculatedSpendOutputTypeDef",
     {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
+        "ActualSpend": SpendOutputTypeDef,
     },
 )
-_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+_OptionalCalculatedSpendOutputTypeDef = TypedDict(
+    "_OptionalCalculatedSpendOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ForecastedSpend": SpendOutputTypeDef,
     },
     total=False,
 )
 
-class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+class CalculatedSpendOutputTypeDef(
+    _RequiredCalculatedSpendOutputTypeDef, _OptionalCalculatedSpendOutputTypeDef
 ):
     pass
 
-_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-    },
-)
-_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef",
+BudgetedAndActualAmountsTypeDef = TypedDict(
+    "BudgetedAndActualAmountsTypeDef",
     {
-        "MaxResults": int,
-        "NextToken": str,
+        "BudgetedAmount": SpendOutputTypeDef,
+        "ActualAmount": SpendOutputTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
     },
     total=False,
 )
 
-class DescribeSubscribersForNotificationRequestRequestTypeDef(
-    _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
-    _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
-):
-    pass
-
-NotificationWithSubscribersTypeDef = TypedDict(
-    "NotificationWithSubscribersTypeDef",
-    {
-        "Notification": NotificationTypeDef,
-        "Subscribers": Sequence[SubscriberTypeDef],
-    },
-)
-
-UpdateNotificationRequestRequestTypeDef = TypedDict(
-    "UpdateNotificationRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "OldNotification": NotificationTypeDef,
-        "NewNotification": NotificationTypeDef,
-    },
-)
-
-UpdateSubscriberRequestRequestTypeDef = TypedDict(
-    "UpdateSubscriberRequestRequestTypeDef",
-    {
-        "AccountId": str,
-        "BudgetName": str,
-        "Notification": NotificationTypeDef,
-        "OldSubscriber": SubscriberTypeDef,
-        "NewSubscriber": SubscriberTypeDef,
-    },
-)
-
 _RequiredCalculatedSpendTypeDef = TypedDict(
     "_RequiredCalculatedSpendTypeDef",
     {
         "ActualSpend": SpendTypeDef,
     },
 )
 _OptionalCalculatedSpendTypeDef = TypedDict(
@@ -701,24 +781,14 @@
     },
     total=False,
 )
 
 class CalculatedSpendTypeDef(_RequiredCalculatedSpendTypeDef, _OptionalCalculatedSpendTypeDef):
     pass
 
-BudgetedAndActualAmountsTypeDef = TypedDict(
-    "BudgetedAndActualAmountsTypeDef",
-    {
-        "BudgetedAmount": SpendTypeDef,
-        "ActualAmount": SpendTypeDef,
-        "TimePeriod": TimePeriodTypeDef,
-    },
-    total=False,
-)
-
 _RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef = (
     TypedDict(
         "_RequiredDescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef",
         {
             "AccountId": str,
             "BudgetName": str,
             "ActionId": str,
@@ -807,14 +877,137 @@
 
 class DescribeBudgetPerformanceHistoryRequestRequestTypeDef(
     _RequiredDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     _OptionalDescribeBudgetPerformanceHistoryRequestRequestTypeDef,
 ):
     pass
 
+CreateNotificationRequestRequestTypeDef = TypedDict(
+    "CreateNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscribers": Sequence[SubscriberTypeDef],
+    },
+)
+
+CreateSubscriberRequestRequestTypeDef = TypedDict(
+    "CreateSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscriber": SubscriberTypeDef,
+    },
+)
+
+DeleteNotificationRequestRequestTypeDef = TypedDict(
+    "DeleteNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+
+DeleteSubscriberRequestRequestTypeDef = TypedDict(
+    "DeleteSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "Subscriber": SubscriberTypeDef,
+    },
+)
+
+_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
+class DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeSubscribersForNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+    },
+)
+_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeSubscribersForNotificationRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class DescribeSubscribersForNotificationRequestRequestTypeDef(
+    _RequiredDescribeSubscribersForNotificationRequestRequestTypeDef,
+    _OptionalDescribeSubscribersForNotificationRequestRequestTypeDef,
+):
+    pass
+
+NotificationWithSubscribersTypeDef = TypedDict(
+    "NotificationWithSubscribersTypeDef",
+    {
+        "Notification": NotificationTypeDef,
+        "Subscribers": Sequence[SubscriberTypeDef],
+    },
+)
+
+UpdateNotificationRequestRequestTypeDef = TypedDict(
+    "UpdateNotificationRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "OldNotification": NotificationTypeDef,
+        "NewNotification": NotificationTypeDef,
+    },
+)
+
+UpdateSubscriberRequestRequestTypeDef = TypedDict(
+    "UpdateSubscriberRequestRequestTypeDef",
+    {
+        "AccountId": str,
+        "BudgetName": str,
+        "Notification": NotificationTypeDef,
+        "OldSubscriber": SubscriberTypeDef,
+        "NewSubscriber": SubscriberTypeDef,
+    },
+)
+
+DefinitionOutputTypeDef = TypedDict(
+    "DefinitionOutputTypeDef",
+    {
+        "IamActionDefinition": IamActionDefinitionOutputTypeDef,
+        "ScpActionDefinition": ScpActionDefinitionOutputTypeDef,
+        "SsmActionDefinition": SsmActionDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 DefinitionTypeDef = TypedDict(
     "DefinitionTypeDef",
     {
         "IamActionDefinition": IamActionDefinitionTypeDef,
         "ScpActionDefinition": ScpActionDefinitionTypeDef,
         "SsmActionDefinition": SsmActionDefinitionTypeDef,
     },
@@ -826,14 +1019,53 @@
     {
         "BudgetNotificationsForAccount": List[BudgetNotificationsForAccountTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredBudgetOutputTypeDef = TypedDict(
+    "_RequiredBudgetOutputTypeDef",
+    {
+        "BudgetName": str,
+        "TimeUnit": TimeUnitType,
+        "BudgetType": BudgetTypeType,
+    },
+)
+_OptionalBudgetOutputTypeDef = TypedDict(
+    "_OptionalBudgetOutputTypeDef",
+    {
+        "BudgetLimit": SpendOutputTypeDef,
+        "PlannedBudgetLimits": Dict[str, SpendOutputTypeDef],
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesOutputTypeDef,
+        "TimePeriod": TimePeriodOutputTypeDef,
+        "CalculatedSpend": CalculatedSpendOutputTypeDef,
+        "LastUpdatedTime": datetime,
+        "AutoAdjustData": AutoAdjustDataOutputTypeDef,
+    },
+    total=False,
+)
+
+class BudgetOutputTypeDef(_RequiredBudgetOutputTypeDef, _OptionalBudgetOutputTypeDef):
+    pass
+
+BudgetPerformanceHistoryTypeDef = TypedDict(
+    "BudgetPerformanceHistoryTypeDef",
+    {
+        "BudgetName": str,
+        "BudgetType": BudgetTypeType,
+        "CostFilters": Dict[str, List[str]],
+        "CostTypes": CostTypesOutputTypeDef,
+        "TimeUnit": TimeUnitType,
+        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
+    },
+    total=False,
+)
+
 _RequiredBudgetTypeDef = TypedDict(
     "_RequiredBudgetTypeDef",
     {
         "BudgetName": str,
         "TimeUnit": TimeUnitType,
         "BudgetType": BudgetTypeType,
     },
@@ -852,40 +1084,27 @@
     },
     total=False,
 )
 
 class BudgetTypeDef(_RequiredBudgetTypeDef, _OptionalBudgetTypeDef):
     pass
 
-BudgetPerformanceHistoryTypeDef = TypedDict(
-    "BudgetPerformanceHistoryTypeDef",
-    {
-        "BudgetName": str,
-        "BudgetType": BudgetTypeType,
-        "CostFilters": Dict[str, List[str]],
-        "CostTypes": CostTypesTypeDef,
-        "TimeUnit": TimeUnitType,
-        "BudgetedAndActualAmountsList": List[BudgetedAndActualAmountsTypeDef],
-    },
-    total=False,
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "ActionId": str,
         "BudgetName": str,
         "NotificationType": NotificationTypeType,
         "ActionType": ActionTypeType,
-        "ActionThreshold": ActionThresholdTypeDef,
-        "Definition": DefinitionTypeDef,
+        "ActionThreshold": ActionThresholdOutputTypeDef,
+        "Definition": DefinitionOutputTypeDef,
         "ExecutionRoleArn": str,
         "ApprovalModel": ApprovalModelType,
         "Status": ActionStatusType,
-        "Subscribers": List[SubscriberTypeDef],
+        "Subscribers": List[SubscriberOutputTypeDef],
     },
 )
 
 CreateBudgetActionRequestRequestTypeDef = TypedDict(
     "CreateBudgetActionRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -923,14 +1142,40 @@
 
 class UpdateBudgetActionRequestRequestTypeDef(
     _RequiredUpdateBudgetActionRequestRequestTypeDef,
     _OptionalUpdateBudgetActionRequestRequestTypeDef,
 ):
     pass
 
+DescribeBudgetResponseTypeDef = TypedDict(
+    "DescribeBudgetResponseTypeDef",
+    {
+        "Budget": BudgetOutputTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBudgetsResponseTypeDef = TypedDict(
+    "DescribeBudgetsResponseTypeDef",
+    {
+        "Budgets": List[BudgetOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
+    "DescribeBudgetPerformanceHistoryResponseTypeDef",
+    {
+        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredCreateBudgetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "Budget": BudgetTypeDef,
     },
 )
@@ -943,48 +1188,22 @@
 )
 
 class CreateBudgetRequestRequestTypeDef(
     _RequiredCreateBudgetRequestRequestTypeDef, _OptionalCreateBudgetRequestRequestTypeDef
 ):
     pass
 
-DescribeBudgetResponseTypeDef = TypedDict(
-    "DescribeBudgetResponseTypeDef",
-    {
-        "Budget": BudgetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBudgetsResponseTypeDef = TypedDict(
-    "DescribeBudgetsResponseTypeDef",
-    {
-        "Budgets": List[BudgetTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateBudgetRequestRequestTypeDef = TypedDict(
     "UpdateBudgetRequestRequestTypeDef",
     {
         "AccountId": str,
         "NewBudget": BudgetTypeDef,
     },
 )
 
-DescribeBudgetPerformanceHistoryResponseTypeDef = TypedDict(
-    "DescribeBudgetPerformanceHistoryResponseTypeDef",
-    {
-        "BudgetPerformanceHistory": BudgetPerformanceHistoryTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActionHistoryDetailsTypeDef = TypedDict(
     "ActionHistoryDetailsTypeDef",
     {
         "Message": str,
         "Action": ActionTypeDef,
     },
 )
```

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/PKG-INFO` & `mypy-boto3-budgets-1.28.12/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-budgets
-Version: 1.28.0
-Summary: Type annotations for boto3.Budgets 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 budgets type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-budgets"></a>
 
 # mypy-boto3-budgets
 
 [![PyPI - mypy-boto3-budgets](https://img.shields.io/pypi/v/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-budgets.svg?color=blue)](https://pypi.org/project/mypy-boto3-budgets)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-budgets?color=blue)](https://pypistats.org/packages/mypy-boto3-budgets)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-budgets)](https://pepy.tech/project/mypy-boto3-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Budgets 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[boto3.Budgets 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [mypy-boto3-budgets docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_budgets/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,22 +336,32 @@
 ### Typed dictionaries
 
 `mypy_boto3_budgets.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_budgets.type_defs import (
+    ActionThresholdOutputTypeDef,
     ActionThresholdTypeDef,
-    SubscriberTypeDef,
+    SubscriberOutputTypeDef,
+    HistoricalOptionsOutputTypeDef,
     HistoricalOptionsTypeDef,
-    NotificationTypeDef,
+    NotificationOutputTypeDef,
+    CostTypesOutputTypeDef,
+    SpendOutputTypeDef,
+    TimePeriodOutputTypeDef,
     CostTypesTypeDef,
     SpendTypeDef,
     TimePeriodTypeDef,
+    SubscriberTypeDef,
     CreateBudgetActionResponseTypeDef,
+    NotificationTypeDef,
+    IamActionDefinitionOutputTypeDef,
+    ScpActionDefinitionOutputTypeDef,
+    SsmActionDefinitionOutputTypeDef,
     IamActionDefinitionTypeDef,
     ScpActionDefinitionTypeDef,
     SsmActionDefinitionTypeDef,
     DeleteBudgetActionRequestRequestTypeDef,
     DeleteBudgetRequestRequestTypeDef,
     DescribeBudgetActionRequestRequestTypeDef,
     DescribeBudgetActionsForAccountRequestDescribeBudgetActionsForAccountPaginateTypeDef,
@@ -398,56 +376,60 @@
     DescribeNotificationsForBudgetRequestDescribeNotificationsForBudgetPaginateTypeDef,
     DescribeNotificationsForBudgetRequestRequestTypeDef,
     ExecuteBudgetActionRequestRequestTypeDef,
     ExecuteBudgetActionResponseTypeDef,
     PaginatorConfigTypeDef,
     ResponseMetadataTypeDef,
     DescribeSubscribersForNotificationResponseTypeDef,
+    AutoAdjustDataOutputTypeDef,
     AutoAdjustDataTypeDef,
     BudgetNotificationsForAccountTypeDef,
+    DescribeNotificationsForBudgetResponseTypeDef,
+    CalculatedSpendOutputTypeDef,
+    BudgetedAndActualAmountsTypeDef,
+    CalculatedSpendTypeDef,
+    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
+    DescribeBudgetActionHistoriesRequestRequestTypeDef,
+    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
+    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
     CreateNotificationRequestRequestTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     DeleteNotificationRequestRequestTypeDef,
     DeleteSubscriberRequestRequestTypeDef,
-    DescribeNotificationsForBudgetResponseTypeDef,
     DescribeSubscribersForNotificationRequestDescribeSubscribersForNotificationPaginateTypeDef,
     DescribeSubscribersForNotificationRequestRequestTypeDef,
     NotificationWithSubscribersTypeDef,
     UpdateNotificationRequestRequestTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
-    CalculatedSpendTypeDef,
-    BudgetedAndActualAmountsTypeDef,
-    DescribeBudgetActionHistoriesRequestDescribeBudgetActionHistoriesPaginateTypeDef,
-    DescribeBudgetActionHistoriesRequestRequestTypeDef,
-    DescribeBudgetPerformanceHistoryRequestDescribeBudgetPerformanceHistoryPaginateTypeDef,
-    DescribeBudgetPerformanceHistoryRequestRequestTypeDef,
+    DefinitionOutputTypeDef,
     DefinitionTypeDef,
     DescribeBudgetNotificationsForAccountResponseTypeDef,
-    BudgetTypeDef,
+    BudgetOutputTypeDef,
     BudgetPerformanceHistoryTypeDef,
+    BudgetTypeDef,
     ActionTypeDef,
     CreateBudgetActionRequestRequestTypeDef,
     UpdateBudgetActionRequestRequestTypeDef,
-    CreateBudgetRequestRequestTypeDef,
     DescribeBudgetResponseTypeDef,
     DescribeBudgetsResponseTypeDef,
-    UpdateBudgetRequestRequestTypeDef,
     DescribeBudgetPerformanceHistoryResponseTypeDef,
+    CreateBudgetRequestRequestTypeDef,
+    UpdateBudgetRequestRequestTypeDef,
     ActionHistoryDetailsTypeDef,
     DeleteBudgetActionResponseTypeDef,
     DescribeBudgetActionResponseTypeDef,
     DescribeBudgetActionsForAccountResponseTypeDef,
     DescribeBudgetActionsForBudgetResponseTypeDef,
     UpdateBudgetActionResponseTypeDef,
     ActionHistoryTypeDef,
     DescribeBudgetActionHistoriesResponseTypeDef,
 )
 
 
-def get_structure() -> ActionThresholdTypeDef:
+def get_structure() -> ActionThresholdOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-budgets-1.28.0/mypy_boto3_budgets.egg-info/SOURCES.txt` & `mypy-boto3-budgets-1.28.12/mypy_boto3_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-budgets-1.28.0/setup.py` & `mypy-boto3-budgets-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-budgets",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Budgets 1.28.0 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.Budgets 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

