# Comparing `tmp/mypy-boto3-appconfig-1.28.0.tar.gz` & `tmp/mypy-boto3-appconfig-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfig-1.28.0.tar", last modified: Thu Jul  6 20:58:55 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfig-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
```

## Comparing `mypy-boto3-appconfig-1.28.0.tar` & `mypy-boto3-appconfig-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.434214 mypy-boto3-appconfig-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-06 20:58:55.434214 mypy-boto3-appconfig-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.430214 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9186 2023-07-06 20:33:09.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-07-06 20:33:09.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31196 2023-07-06 20:33:10.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31151 2023-07-06 20:33:09.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:55.434214 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:58:55.000000 mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:55.434214 mypy-boto3-appconfig-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:33:08.000000 mypy-boto3-appconfig-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.340584 mypy-boto3-appconfig-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29069 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29020 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32185 2023-07-27 05:17:17.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32138 2023-07-27 05:17:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:16.000000 mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.340584 mypy-boto3-appconfig-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:15.000000 mypy-boto3-appconfig-1.28.12/setup.py
```

### Comparing `mypy-boto3-appconfig-1.28.0/LICENSE` & `mypy-boto3-appconfig-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.0/PKG-INFO` & `mypy-boto3-appconfig-1.28.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.0
-Summary: Type annotations for boto3.AppConfig 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,22 +304,24 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorTypeDef,
+    ValidatorOutputTypeDef,
     ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ValidatorTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
@@ -328,17 +330,19 @@
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
     DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
     EmptyResponseMetadataTypeDef,
+    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
+    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
@@ -368,24 +372,24 @@
     DeploymentEventTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
-    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
+    EnvironmentResponseMetadataTypeDef,
+    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
+    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.0/README.md` & `mypy-boto3-appconfig-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,22 +272,24 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorTypeDef,
+    ValidatorOutputTypeDef,
     ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ValidatorTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
@@ -296,17 +298,19 @@
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
     DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
     EmptyResponseMetadataTypeDef,
+    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
+    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
@@ -336,24 +340,24 @@
     DeploymentEventTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
-    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
+    EnvironmentResponseMetadataTypeDef,
+    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
+    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/__main__.py` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfig 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppConfig 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig\nOther"
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

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/client.py` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/client.pyi` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/literals.py` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
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
@@ -262,26 +263,28 @@
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

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/literals.pyi` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,15 @@
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
@@ -260,26 +261,28 @@
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

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/type_defs.py` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionInvocationTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
-    "ValidatorTypeDef",
+    "ValidatorOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ValidatorTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
@@ -56,17 +58,19 @@
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
     "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "MonitorOutputTypeDef",
     "ExtensionAssociationSummaryTypeDef",
     "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
+    "ParameterOutputTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
@@ -96,24 +100,24 @@
     "DeploymentEventTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
-    "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
+    "EnvironmentResponseMetadataTypeDef",
+    "EnvironmentTypeDef",
     "ExtensionAssociationsTypeDef",
     "ExtensionsTypeDef",
+    "ExtensionTypeDef",
     "HostedConfigurationVersionsTypeDef",
     "DeploymentTypeDef",
     "EnvironmentsTypeDef",
 )
 
 ActionInvocationTypeDef = TypedDict(
     "ActionInvocationTypeDef",
@@ -125,14 +129,25 @@
         "ErrorMessage": str,
         "ErrorCode": str,
         "InvocationId": str,
     },
     total=False,
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Uri": str,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
         "Description": str,
         "Uri": str,
         "RoleArn": str,
@@ -180,16 +195,16 @@
         "LocationUri": str,
         "ValidatorTypes": List[ValidatorTypeType],
         "Type": str,
     },
     total=False,
 )
 
-ValidatorTypeDef = TypedDict(
-    "ValidatorTypeDef",
+ValidatorOutputTypeDef = TypedDict(
+    "ValidatorOutputTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
 ConfigurationTypeDef = TypedDict(
@@ -220,14 +235,22 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+ValidatorTypeDef = TypedDict(
+    "ValidatorTypeDef",
+    {
+        "Type": ValidatorTypeType,
+        "Content": str,
+    },
+)
+
 _RequiredCreateDeploymentStrategyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentStrategyRequestRequestTypeDef",
     {
         "Name": str,
         "DeploymentDurationInMinutes": int,
         "GrowthFactor": float,
     },
@@ -450,14 +473,33 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMonitorOutputTypeDef = TypedDict(
+    "_RequiredMonitorOutputTypeDef",
+    {
+        "AlarmArn": str,
+    },
+)
+_OptionalMonitorOutputTypeDef = TypedDict(
+    "_OptionalMonitorOutputTypeDef",
+    {
+        "AlarmRoleArn": str,
+    },
+    total=False,
+)
+
+
+class MonitorOutputTypeDef(_RequiredMonitorOutputTypeDef, _OptionalMonitorOutputTypeDef):
+    pass
+
+
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
@@ -485,14 +527,23 @@
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
     },
     total=False,
 )
 
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
+    {
+        "Description": str,
+        "Required": bool,
+    },
+    total=False,
+)
+
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -942,15 +993,15 @@
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
-        "Validators": List[ValidatorTypeDef],
+        "Validators": List[ValidatorOutputTypeDef],
         "Type": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
@@ -1026,40 +1077,14 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
     },
 )
@@ -1101,28 +1126,14 @@
 
 class CreateExtensionRequestRequestTypeDef(
     _RequiredCreateExtensionRequestRequestTypeDef, _OptionalCreateExtensionRequestRequestTypeDef
 ):
     pass
 
 
-ExtensionTypeDef = TypedDict(
-    "ExtensionTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "VersionNumber": int,
-        "Arn": str,
-        "Description": str,
-        "Actions": Dict[ActionPointType, List[ActionTypeDef]],
-        "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
     },
 )
 _OptionalUpdateExtensionRequestRequestTypeDef = TypedDict(
@@ -1157,14 +1168,40 @@
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnvironmentResponseMetadataTypeDef = TypedDict(
+    "EnvironmentResponseMetadataTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorOutputTypeDef],
+    },
+    total=False,
+)
+
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1175,14 +1212,28 @@
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExtensionTypeDef = TypedDict(
+    "ExtensionTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "VersionNumber": int,
+        "Arn": str,
+        "Description": str,
+        "Actions": Dict[ActionPointType, List[ActionOutputTypeDef]],
+        "Parameters": Dict[str, ParameterOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig/type_defs.pyi` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionInvocationTypeDef",
+    "ActionOutputTypeDef",
     "ActionTypeDef",
     "ApplicationResponseMetadataTypeDef",
     "ApplicationTypeDef",
     "AppliedExtensionTypeDef",
     "ConfigurationProfileSummaryTypeDef",
-    "ValidatorTypeDef",
+    "ValidatorOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateApplicationRequestRequestTypeDef",
+    "ValidatorTypeDef",
     "CreateDeploymentStrategyRequestRequestTypeDef",
     "MonitorTypeDef",
     "CreateExtensionAssociationRequestRequestTypeDef",
     "ParameterTypeDef",
     "CreateHostedConfigurationVersionRequestRequestTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteConfigurationProfileRequestRequestTypeDef",
@@ -55,17 +57,19 @@
     "DeleteExtensionAssociationRequestRequestTypeDef",
     "DeleteExtensionRequestRequestTypeDef",
     "DeleteHostedConfigurationVersionRequestRequestTypeDef",
     "DeploymentStrategyTypeDef",
     "DeploymentStrategyResponseMetadataTypeDef",
     "DeploymentSummaryTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "MonitorOutputTypeDef",
     "ExtensionAssociationSummaryTypeDef",
     "ExtensionAssociationTypeDef",
     "ExtensionSummaryTypeDef",
+    "ParameterOutputTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetConfigurationProfileRequestRequestTypeDef",
     "GetConfigurationRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
     "GetDeploymentStrategyRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetExtensionAssociationRequestRequestTypeDef",
@@ -95,24 +99,24 @@
     "DeploymentEventTypeDef",
     "ApplicationsTypeDef",
     "ConfigurationProfilesTypeDef",
     "ConfigurationProfileTypeDef",
     "CreateConfigurationProfileRequestRequestTypeDef",
     "UpdateConfigurationProfileRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "EnvironmentResponseMetadataTypeDef",
-    "EnvironmentTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateExtensionRequestRequestTypeDef",
-    "ExtensionTypeDef",
     "UpdateExtensionRequestRequestTypeDef",
     "DeploymentStrategiesTypeDef",
     "DeploymentsTypeDef",
+    "EnvironmentResponseMetadataTypeDef",
+    "EnvironmentTypeDef",
     "ExtensionAssociationsTypeDef",
     "ExtensionsTypeDef",
+    "ExtensionTypeDef",
     "HostedConfigurationVersionsTypeDef",
     "DeploymentTypeDef",
     "EnvironmentsTypeDef",
 )
 
 ActionInvocationTypeDef = TypedDict(
     "ActionInvocationTypeDef",
@@ -124,14 +128,25 @@
         "ErrorMessage": str,
         "ErrorCode": str,
         "InvocationId": str,
     },
     total=False,
 )
 
+ActionOutputTypeDef = TypedDict(
+    "ActionOutputTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Uri": str,
+        "RoleArn": str,
+    },
+    total=False,
+)
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
         "Description": str,
         "Uri": str,
         "RoleArn": str,
@@ -179,16 +194,16 @@
         "LocationUri": str,
         "ValidatorTypes": List[ValidatorTypeType],
         "Type": str,
     },
     total=False,
 )
 
-ValidatorTypeDef = TypedDict(
-    "ValidatorTypeDef",
+ValidatorOutputTypeDef = TypedDict(
+    "ValidatorOutputTypeDef",
     {
         "Type": ValidatorTypeType,
         "Content": str,
     },
 )
 
 ConfigurationTypeDef = TypedDict(
@@ -217,14 +232,22 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
+ValidatorTypeDef = TypedDict(
+    "ValidatorTypeDef",
+    {
+        "Type": ValidatorTypeType,
+        "Content": str,
+    },
+)
+
 _RequiredCreateDeploymentStrategyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentStrategyRequestRequestTypeDef",
     {
         "Name": str,
         "DeploymentDurationInMinutes": int,
         "GrowthFactor": float,
     },
@@ -437,14 +460,31 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredMonitorOutputTypeDef = TypedDict(
+    "_RequiredMonitorOutputTypeDef",
+    {
+        "AlarmArn": str,
+    },
+)
+_OptionalMonitorOutputTypeDef = TypedDict(
+    "_OptionalMonitorOutputTypeDef",
+    {
+        "AlarmRoleArn": str,
+    },
+    total=False,
+)
+
+class MonitorOutputTypeDef(_RequiredMonitorOutputTypeDef, _OptionalMonitorOutputTypeDef):
+    pass
+
 ExtensionAssociationSummaryTypeDef = TypedDict(
     "ExtensionAssociationSummaryTypeDef",
     {
         "Id": str,
         "ExtensionArn": str,
         "ResourceArn": str,
     },
@@ -472,14 +512,23 @@
         "VersionNumber": int,
         "Arn": str,
         "Description": str,
     },
     total=False,
 )
 
+ParameterOutputTypeDef = TypedDict(
+    "ParameterOutputTypeDef",
+    {
+        "Description": str,
+        "Required": bool,
+    },
+    total=False,
+)
+
 GetApplicationRequestRequestTypeDef = TypedDict(
     "GetApplicationRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
@@ -909,15 +958,15 @@
     {
         "ApplicationId": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "LocationUri": str,
         "RetrievalRoleArn": str,
-        "Validators": List[ValidatorTypeDef],
+        "Validators": List[ValidatorOutputTypeDef],
         "Type": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateConfigurationProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationProfileRequestRequestTypeDef",
@@ -987,40 +1036,14 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-EnvironmentResponseMetadataTypeDef = TypedDict(
-    "EnvironmentResponseMetadataTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnvironmentTypeDef = TypedDict(
-    "EnvironmentTypeDef",
-    {
-        "ApplicationId": str,
-        "Id": str,
-        "Name": str,
-        "Description": str,
-        "State": EnvironmentStateType,
-        "Monitors": List[MonitorTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "EnvironmentId": str,
     },
 )
@@ -1058,28 +1081,14 @@
 )
 
 class CreateExtensionRequestRequestTypeDef(
     _RequiredCreateExtensionRequestRequestTypeDef, _OptionalCreateExtensionRequestRequestTypeDef
 ):
     pass
 
-ExtensionTypeDef = TypedDict(
-    "ExtensionTypeDef",
-    {
-        "Id": str,
-        "Name": str,
-        "VersionNumber": int,
-        "Arn": str,
-        "Description": str,
-        "Actions": Dict[ActionPointType, List[ActionTypeDef]],
-        "Parameters": Dict[str, ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateExtensionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateExtensionRequestRequestTypeDef",
     {
         "ExtensionIdentifier": str,
     },
 )
 _OptionalUpdateExtensionRequestRequestTypeDef = TypedDict(
@@ -1112,14 +1121,40 @@
     {
         "Items": List[DeploymentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+EnvironmentResponseMetadataTypeDef = TypedDict(
+    "EnvironmentResponseMetadataTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+EnvironmentTypeDef = TypedDict(
+    "EnvironmentTypeDef",
+    {
+        "ApplicationId": str,
+        "Id": str,
+        "Name": str,
+        "Description": str,
+        "State": EnvironmentStateType,
+        "Monitors": List[MonitorOutputTypeDef],
+    },
+    total=False,
+)
+
 ExtensionAssociationsTypeDef = TypedDict(
     "ExtensionAssociationsTypeDef",
     {
         "Items": List[ExtensionAssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1130,14 +1165,28 @@
     {
         "Items": List[ExtensionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ExtensionTypeDef = TypedDict(
+    "ExtensionTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "VersionNumber": int,
+        "Arn": str,
+        "Description": str,
+        "Actions": Dict[ActionPointType, List[ActionOutputTypeDef]],
+        "Parameters": Dict[str, ParameterOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 HostedConfigurationVersionsTypeDef = TypedDict(
     "HostedConfigurationVersionsTypeDef",
     {
         "Items": List[HostedConfigurationVersionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
```

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/PKG-INFO` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfig
-Version: 1.28.0
-Summary: Type annotations for boto3.AppConfig 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-appconfig"></a>
 
 # mypy-boto3-appconfig
 
 [![PyPI - mypy-boto3-appconfig](https://img.shields.io/pypi/v/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfig.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfig)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-appconfig?color=blue)](https://pypistats.org/packages/mypy-boto3-appconfig)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfig)](https://pepy.tech/project/mypy-boto3-appconfig)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfig 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
+[boto3.AppConfig 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#AppConfig)
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
 [mypy-boto3-appconfig docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfig/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,22 +304,24 @@
 
 `mypy_boto3_appconfig.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfig.type_defs import (
     ActionInvocationTypeDef,
+    ActionOutputTypeDef,
     ActionTypeDef,
     ApplicationResponseMetadataTypeDef,
     ApplicationTypeDef,
     AppliedExtensionTypeDef,
     ConfigurationProfileSummaryTypeDef,
-    ValidatorTypeDef,
+    ValidatorOutputTypeDef,
     ConfigurationTypeDef,
     CreateApplicationRequestRequestTypeDef,
+    ValidatorTypeDef,
     CreateDeploymentStrategyRequestRequestTypeDef,
     MonitorTypeDef,
     CreateExtensionAssociationRequestRequestTypeDef,
     ParameterTypeDef,
     CreateHostedConfigurationVersionRequestRequestTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteConfigurationProfileRequestRequestTypeDef,
@@ -328,17 +330,19 @@
     DeleteExtensionAssociationRequestRequestTypeDef,
     DeleteExtensionRequestRequestTypeDef,
     DeleteHostedConfigurationVersionRequestRequestTypeDef,
     DeploymentStrategyTypeDef,
     DeploymentStrategyResponseMetadataTypeDef,
     DeploymentSummaryTypeDef,
     EmptyResponseMetadataTypeDef,
+    MonitorOutputTypeDef,
     ExtensionAssociationSummaryTypeDef,
     ExtensionAssociationTypeDef,
     ExtensionSummaryTypeDef,
+    ParameterOutputTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetConfigurationProfileRequestRequestTypeDef,
     GetConfigurationRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
     GetDeploymentStrategyRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetExtensionAssociationRequestRequestTypeDef,
@@ -368,24 +372,24 @@
     DeploymentEventTypeDef,
     ApplicationsTypeDef,
     ConfigurationProfilesTypeDef,
     ConfigurationProfileTypeDef,
     CreateConfigurationProfileRequestRequestTypeDef,
     UpdateConfigurationProfileRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    EnvironmentResponseMetadataTypeDef,
-    EnvironmentTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateExtensionRequestRequestTypeDef,
-    ExtensionTypeDef,
     UpdateExtensionRequestRequestTypeDef,
     DeploymentStrategiesTypeDef,
     DeploymentsTypeDef,
+    EnvironmentResponseMetadataTypeDef,
+    EnvironmentTypeDef,
     ExtensionAssociationsTypeDef,
     ExtensionsTypeDef,
+    ExtensionTypeDef,
     HostedConfigurationVersionsTypeDef,
     DeploymentTypeDef,
     EnvironmentsTypeDef,
 )
 
 
 def get_structure() -> ActionInvocationTypeDef:
```

### Comparing `mypy-boto3-appconfig-1.28.0/mypy_boto3_appconfig.egg-info/SOURCES.txt` & `mypy-boto3-appconfig-1.28.12/mypy_boto3_appconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfig-1.28.0/setup.py` & `mypy-boto3-appconfig-1.28.12/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfig",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_appconfig"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfig 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppConfig 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

