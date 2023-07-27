# Comparing `tmp/mypy-boto3-apprunner-1.28.0.tar.gz` & `tmp/mypy-boto3-apprunner-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apprunner-1.28.0.tar", last modified: Thu Jul  6 20:58:58 2023, max compression
+gzip compressed data, was "mypy-boto3-apprunner-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
```

## Comparing `mypy-boto3-apprunner-1.28.0.tar` & `mypy-boto3-apprunner-1.28.12.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.770221 mypy-boto3-apprunner-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-07-06 20:58:58.770221 mypy-boto3-apprunner-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.766221 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-06 20:33:34.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35647 2023-07-06 20:33:35.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35612 2023-07-06 20:33:35.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:33:33.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:58:58.770221 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 20:58:58.000000 mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:58:58.770221 mypy-boto3-apprunner-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 20:33:32.000000 mypy-boto3-apprunner-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.516577 mypy-boto3-apprunner-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25678 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41889 2023-07-27 05:17:33.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41844 2023-07-27 05:17:33.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.504577 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:18.000000 mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.516577 mypy-boto3-apprunner-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:32.000000 mypy-boto3-apprunner-1.28.12/setup.py
```

### Comparing `mypy-boto3-apprunner-1.28.0/LICENSE` & `mypy-boto3-apprunner-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.0/PKG-INFO` & `mypy-boto3-apprunner-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apprunner
-Version: 1.28.0
-Summary: Type annotations for boto3.AppRunner 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,19 +315,22 @@
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     VpcDNSTargetTypeDef,
+    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
+    CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
+    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -344,79 +347,94 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
+    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
+    HealthCheckConfigurationOutputTypeDef,
+    ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
+    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
+    IngressVpcConfigurationOutputTypeDef,
+    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
+    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
+    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
-    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
-    VpcIngressConnectionTypeDef,
+    ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
+    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
+    CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.0/README.md` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-apprunner
+Version: 1.28.12
+Summary: Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 apprunner type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,19 +315,22 @@
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     VpcDNSTargetTypeDef,
+    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
+    CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
+    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -312,79 +347,94 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
+    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
+    HealthCheckConfigurationOutputTypeDef,
+    ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
+    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
+    IngressVpcConfigurationOutputTypeDef,
+    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
+    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
+    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
-    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
-    VpcIngressConnectionTypeDef,
+    ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
+    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
+    CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/__main__.py` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppRunner 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.AppRunner 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner\nOther"
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

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/client.py` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/client.pyi` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/literals.py` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.pyi`

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
     "AutoScalingConfigurationStatusType",
     "CertificateValidationRecordStatusType",
     "ConfigurationSourceType",
     "ConnectionStatusType",
     "CustomDomainAssociationStatusType",
     "EgressTypeType",
@@ -40,15 +39,14 @@
     "VpcIngressConnectionStatusType",
     "AppRunnerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AutoScalingConfigurationStatusType = Literal["ACTIVE", "INACTIVE"]
 CertificateValidationRecordStatusType = Literal["FAILED", "PENDING_VALIDATION", "SUCCESS"]
 ConfigurationSourceType = Literal["API", "REPOSITORY"]
 ConnectionStatusType = Literal["AVAILABLE", "DELETED", "ERROR", "PENDING_HANDSHAKE"]
 CustomDomainAssociationStatusType = Literal[
     "ACTIVE",
     "BINDING_CERTIFICATE",
@@ -224,14 +222,15 @@
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
@@ -310,26 +309,28 @@
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

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/literals.pyi` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/literals.py`

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
     "AutoScalingConfigurationStatusType",
     "CertificateValidationRecordStatusType",
     "ConfigurationSourceType",
     "ConnectionStatusType",
     "CustomDomainAssociationStatusType",
     "EgressTypeType",
@@ -39,14 +40,15 @@
     "VpcIngressConnectionStatusType",
     "AppRunnerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AutoScalingConfigurationStatusType = Literal["ACTIVE", "INACTIVE"]
 CertificateValidationRecordStatusType = Literal["FAILED", "PENDING_VALIDATION", "SUCCESS"]
 ConfigurationSourceType = Literal["API", "REPOSITORY"]
 ConnectionStatusType = Literal["AVAILABLE", "DELETED", "ERROR", "PENDING_HANDSHAKE"]
 CustomDomainAssociationStatusType = Literal[
     "ACTIVE",
     "BINDING_CERTIFICATE",
@@ -222,14 +224,15 @@
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
@@ -308,26 +311,28 @@
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

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/type_defs.py` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,19 +42,22 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
     "VpcDNSTargetTypeDef",
+    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
+    "CodeConfigurationValuesOutputTypeDef",
     "CodeConfigurationValuesTypeDef",
+    "SourceCodeVersionOutputTypeDef",
     "SourceCodeVersionTypeDef",
     "ConnectionSummaryTypeDef",
     "ConnectionTypeDef",
     "TagTypeDef",
     "TraceConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HealthCheckConfigurationTypeDef",
@@ -71,79 +74,94 @@
     "DescribeAutoScalingConfigurationRequestRequestTypeDef",
     "DescribeCustomDomainsRequestRequestTypeDef",
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     "DescribeServiceRequestRequestTypeDef",
     "DescribeVpcConnectorRequestRequestTypeDef",
     "DescribeVpcIngressConnectionRequestRequestTypeDef",
     "DisassociateCustomDomainRequestRequestTypeDef",
+    "EgressConfigurationOutputTypeDef",
     "EgressConfigurationTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
+    "HealthCheckConfigurationOutputTypeDef",
+    "ImageConfigurationOutputTypeDef",
     "ImageConfigurationTypeDef",
+    "IngressConfigurationOutputTypeDef",
     "IngressConfigurationTypeDef",
+    "IngressVpcConfigurationOutputTypeDef",
+    "InstanceConfigurationOutputTypeDef",
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListObservabilityConfigurationsRequestRequestTypeDef",
     "ObservabilityConfigurationSummaryTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
+    "TraceConfigurationOutputTypeDef",
     "PauseServiceRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
+    "ServiceObservabilityConfigurationOutputTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartDeploymentResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
+    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "CreateAutoScalingConfigurationRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateVpcConnectorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateObservabilityConfigurationRequestRequestTypeDef",
-    "ObservabilityConfigurationTypeDef",
     "CreateVpcConnectorResponseTypeDef",
     "DeleteVpcConnectorResponseTypeDef",
     "DescribeVpcConnectorResponseTypeDef",
     "ListVpcConnectorsResponseTypeDef",
     "CreateVpcIngressConnectionRequestRequestTypeDef",
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
-    "VpcIngressConnectionTypeDef",
+    "ImageRepositoryOutputTypeDef",
     "ImageRepositoryTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
+    "VpcIngressConnectionTypeDef",
     "ListObservabilityConfigurationsResponseTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     "ListVpcIngressConnectionsResponseTypeDef",
+    "ObservabilityConfigurationTypeDef",
     "AssociateCustomDomainResponseTypeDef",
     "DescribeCustomDomainsResponseTypeDef",
     "DisassociateCustomDomainResponseTypeDef",
+    "CodeRepositoryOutputTypeDef",
     "CodeRepositoryTypeDef",
-    "CreateObservabilityConfigurationResponseTypeDef",
-    "DeleteObservabilityConfigurationResponseTypeDef",
-    "DescribeObservabilityConfigurationResponseTypeDef",
     "CreateVpcIngressConnectionResponseTypeDef",
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
+    "CreateObservabilityConfigurationResponseTypeDef",
+    "DeleteObservabilityConfigurationResponseTypeDef",
+    "DescribeObservabilityConfigurationResponseTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServiceResponseTypeDef",
     "PauseServiceResponseTypeDef",
     "ResumeServiceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
@@ -178,14 +196,23 @@
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
     total=False,
 )
 
+AuthenticationConfigurationOutputTypeDef = TypedDict(
+    "AuthenticationConfigurationOutputTypeDef",
+    {
+        "ConnectionArn": str,
+        "AccessRoleArn": str,
+    },
+    total=False,
+)
+
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "ConnectionArn": str,
         "AccessRoleArn": str,
     },
     total=False,
@@ -225,14 +252,39 @@
         "Type": str,
         "Value": str,
         "Status": CertificateValidationRecordStatusType,
     },
     total=False,
 )
 
+_RequiredCodeConfigurationValuesOutputTypeDef = TypedDict(
+    "_RequiredCodeConfigurationValuesOutputTypeDef",
+    {
+        "Runtime": RuntimeType,
+    },
+)
+_OptionalCodeConfigurationValuesOutputTypeDef = TypedDict(
+    "_OptionalCodeConfigurationValuesOutputTypeDef",
+    {
+        "BuildCommand": str,
+        "StartCommand": str,
+        "Port": str,
+        "RuntimeEnvironmentVariables": Dict[str, str],
+        "RuntimeEnvironmentSecrets": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class CodeConfigurationValuesOutputTypeDef(
+    _RequiredCodeConfigurationValuesOutputTypeDef, _OptionalCodeConfigurationValuesOutputTypeDef
+):
+    pass
+
+
 _RequiredCodeConfigurationValuesTypeDef = TypedDict(
     "_RequiredCodeConfigurationValuesTypeDef",
     {
         "Runtime": RuntimeType,
     },
 )
 _OptionalCodeConfigurationValuesTypeDef = TypedDict(
@@ -250,14 +302,22 @@
 
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
 
+SourceCodeVersionOutputTypeDef = TypedDict(
+    "SourceCodeVersionOutputTypeDef",
+    {
+        "Type": Literal["BRANCH"],
+        "Value": str,
+    },
+)
+
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -482,42 +542,109 @@
     "DisassociateCustomDomainRequestRequestTypeDef",
     {
         "ServiceArn": str,
         "DomainName": str,
     },
 )
 
+EgressConfigurationOutputTypeDef = TypedDict(
+    "EgressConfigurationOutputTypeDef",
+    {
+        "EgressType": EgressTypeType,
+        "VpcConnectorArn": str,
+    },
+    total=False,
+)
+
 EgressConfigurationTypeDef = TypedDict(
     "EgressConfigurationTypeDef",
     {
         "EgressType": EgressTypeType,
         "VpcConnectorArn": str,
     },
     total=False,
 )
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
+HealthCheckConfigurationOutputTypeDef = TypedDict(
+    "HealthCheckConfigurationOutputTypeDef",
+    {
+        "Protocol": HealthCheckProtocolType,
+        "Path": str,
+        "Interval": int,
+        "Timeout": int,
+        "HealthyThreshold": int,
+        "UnhealthyThreshold": int,
+    },
+    total=False,
+)
+
+ImageConfigurationOutputTypeDef = TypedDict(
+    "ImageConfigurationOutputTypeDef",
+    {
+        "RuntimeEnvironmentVariables": Dict[str, str],
+        "StartCommand": str,
+        "Port": str,
+        "RuntimeEnvironmentSecrets": Dict[str, str],
+    },
+    total=False,
+)
+
 ImageConfigurationTypeDef = TypedDict(
     "ImageConfigurationTypeDef",
     {
         "RuntimeEnvironmentVariables": Mapping[str, str],
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
+IngressConfigurationOutputTypeDef = TypedDict(
+    "IngressConfigurationOutputTypeDef",
+    {
+        "IsPubliclyAccessible": bool,
+    },
+    total=False,
+)
+
 IngressConfigurationTypeDef = TypedDict(
     "IngressConfigurationTypeDef",
     {
         "IsPubliclyAccessible": bool,
     },
     total=False,
 )
 
+IngressVpcConfigurationOutputTypeDef = TypedDict(
+    "IngressVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "VpcEndpointId": str,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "Cpu": str,
+        "Memory": str,
+        "InstanceRoleArn": str,
+    },
+    total=False,
+)
+
 ListAutoScalingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
         "LatestOnly": bool,
         "MaxResults": int,
         "NextToken": str,
@@ -618,14 +745,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
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
 ListVpcConnectorsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -645,14 +781,21 @@
     {
         "VpcIngressConnectionArn": str,
         "ServiceArn": str,
     },
     total=False,
 )
 
+TraceConfigurationOutputTypeDef = TypedDict(
+    "TraceConfigurationOutputTypeDef",
+    {
+        "Vendor": Literal["AWSXRAY"],
+    },
+)
+
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
@@ -670,14 +813,36 @@
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
+_RequiredServiceObservabilityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceObservabilityConfigurationOutputTypeDef",
+    {
+        "ObservabilityEnabled": bool,
+    },
+)
+_OptionalServiceObservabilityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceObservabilityConfigurationOutputTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+    },
+    total=False,
+)
+
+
+class ServiceObservabilityConfigurationOutputTypeDef(
+    _RequiredServiceObservabilityConfigurationOutputTypeDef,
+    _OptionalServiceObservabilityConfigurationOutputTypeDef,
+):
+    pass
+
+
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
@@ -747,14 +912,35 @@
 )
 
 
 class CustomDomainTypeDef(_RequiredCustomDomainTypeDef, _OptionalCustomDomainTypeDef):
     pass
 
 
+_RequiredCodeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCodeConfigurationOutputTypeDef",
+    {
+        "ConfigurationSource": ConfigurationSourceType,
+    },
+)
+_OptionalCodeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCodeConfigurationOutputTypeDef",
+    {
+        "CodeConfigurationValues": CodeConfigurationValuesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CodeConfigurationOutputTypeDef(
+    _RequiredCodeConfigurationOutputTypeDef, _OptionalCodeConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredCodeConfigurationTypeDef = TypedDict(
     "_RequiredCodeConfigurationTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationTypeDef = TypedDict(
@@ -864,22 +1050,14 @@
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
 
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
@@ -903,29 +1081,14 @@
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-ObservabilityConfigurationTypeDef = TypedDict(
-    "ObservabilityConfigurationTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-        "ObservabilityConfigurationName": str,
-        "TraceConfiguration": TraceConfigurationTypeDef,
-        "ObservabilityConfigurationRevision": int,
-        "Latest": bool,
-        "Status": ObservabilityConfigurationStatusType,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
-    },
-    total=False,
-)
-
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -983,30 +1146,36 @@
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
 
-VpcIngressConnectionTypeDef = TypedDict(
-    "VpcIngressConnectionTypeDef",
+_RequiredImageRepositoryOutputTypeDef = TypedDict(
+    "_RequiredImageRepositoryOutputTypeDef",
     {
-        "VpcIngressConnectionArn": str,
-        "VpcIngressConnectionName": str,
-        "ServiceArn": str,
-        "Status": VpcIngressConnectionStatusType,
-        "AccountId": str,
-        "DomainName": str,
-        "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
+        "ImageIdentifier": str,
+        "ImageRepositoryType": ImageRepositoryTypeType,
+    },
+)
+_OptionalImageRepositoryOutputTypeDef = TypedDict(
+    "_OptionalImageRepositoryOutputTypeDef",
+    {
+        "ImageConfiguration": ImageConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+
+class ImageRepositoryOutputTypeDef(
+    _RequiredImageRepositoryOutputTypeDef, _OptionalImageRepositoryOutputTypeDef
+):
+    pass
+
+
 _RequiredImageRepositoryTypeDef = TypedDict(
     "_RequiredImageRepositoryTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -1019,23 +1188,48 @@
 )
 
 
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "EgressConfiguration": EgressConfigurationOutputTypeDef,
+        "IngressConfiguration": IngressConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
 )
 
+VpcIngressConnectionTypeDef = TypedDict(
+    "VpcIngressConnectionTypeDef",
+    {
+        "VpcIngressConnectionArn": str,
+        "VpcIngressConnectionName": str,
+        "ServiceArn": str,
+        "Status": VpcIngressConnectionStatusType,
+        "AccountId": str,
+        "DomainName": str,
+        "IngressVpcConfiguration": IngressVpcConfigurationOutputTypeDef,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1055,14 +1249,22 @@
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1074,14 +1276,29 @@
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ObservabilityConfigurationTypeDef = TypedDict(
+    "ObservabilityConfigurationTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+        "ObservabilityConfigurationName": str,
+        "TraceConfiguration": TraceConfigurationOutputTypeDef,
+        "ObservabilityConfigurationRevision": int,
+        "Latest": bool,
+        "Status": ObservabilityConfigurationStatusType,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
@@ -1108,14 +1325,36 @@
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCodeRepositoryOutputTypeDef = TypedDict(
+    "_RequiredCodeRepositoryOutputTypeDef",
+    {
+        "RepositoryUrl": str,
+        "SourceCodeVersion": SourceCodeVersionOutputTypeDef,
+    },
+)
+_OptionalCodeRepositoryOutputTypeDef = TypedDict(
+    "_OptionalCodeRepositoryOutputTypeDef",
+    {
+        "CodeConfiguration": CodeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class CodeRepositoryOutputTypeDef(
+    _RequiredCodeRepositoryOutputTypeDef, _OptionalCodeRepositoryOutputTypeDef
+):
+    pass
+
+
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
         "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
@@ -1128,138 +1367,149 @@
 )
 
 
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
 
-CreateObservabilityConfigurationResponseTypeDef = TypedDict(
-    "CreateObservabilityConfigurationResponseTypeDef",
+CreateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "CreateVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DeleteObservabilityConfigurationResponseTypeDef",
+DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeObservabilityConfigurationResponseTypeDef",
+DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "CreateVpcIngressConnectionResponseTypeDef",
+UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "UpdateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcIngressConnectionResponseTypeDef",
+CreateObservabilityConfigurationResponseTypeDef = TypedDict(
+    "CreateObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcIngressConnectionResponseTypeDef",
+DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DeleteObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "UpdateVpcIngressConnectionResponseTypeDef",
+DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "CodeRepository": CodeRepositoryOutputTypeDef,
+        "ImageRepository": ImageRepositoryOutputTypeDef,
+        "AutoDeploymentsEnabled": bool,
+        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "CodeRepository": CodeRepositoryTypeDef,
         "ImageRepository": ImageRepositoryTypeDef,
         "AutoDeploymentsEnabled": bool,
         "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
+_RequiredServiceTypeDef = TypedDict(
+    "_RequiredServiceTypeDef",
     {
         "ServiceName": str,
-        "SourceConfiguration": SourceConfigurationTypeDef,
+        "ServiceId": str,
+        "ServiceArn": str,
+        "CreatedAt": datetime,
+        "UpdatedAt": datetime,
+        "Status": ServiceStatusType,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "InstanceConfiguration": InstanceConfigurationOutputTypeDef,
+        "AutoScalingConfigurationSummary": AutoScalingConfigurationSummaryTypeDef,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
     },
 )
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
+_OptionalServiceTypeDef = TypedDict(
+    "_OptionalServiceTypeDef",
     {
-        "InstanceConfiguration": InstanceConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
-        "AutoScalingConfigurationArn": str,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
-        "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
+        "ServiceUrl": str,
+        "DeletedAt": datetime,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "HealthCheckConfiguration": HealthCheckConfigurationOutputTypeDef,
+        "ObservabilityConfiguration": ServiceObservabilityConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
+class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
     pass
 
 
-_RequiredServiceTypeDef = TypedDict(
-    "_RequiredServiceTypeDef",
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ServiceName": str,
-        "ServiceId": str,
-        "ServiceArn": str,
-        "CreatedAt": datetime,
-        "UpdatedAt": datetime,
-        "Status": ServiceStatusType,
         "SourceConfiguration": SourceConfigurationTypeDef,
-        "InstanceConfiguration": InstanceConfigurationTypeDef,
-        "AutoScalingConfigurationSummary": AutoScalingConfigurationSummaryTypeDef,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
     },
 )
-_OptionalServiceTypeDef = TypedDict(
-    "_OptionalServiceTypeDef",
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
     {
-        "ServiceUrl": str,
-        "DeletedAt": datetime,
+        "InstanceConfiguration": InstanceConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
+        "AutoScalingConfigurationArn": str,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
 
-class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
     pass
 
 
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
```

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner/type_defs.pyi` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -41,19 +41,22 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateCustomDomainRequestRequestTypeDef",
     "VpcDNSTargetTypeDef",
+    "AuthenticationConfigurationOutputTypeDef",
     "AuthenticationConfigurationTypeDef",
     "AutoScalingConfigurationSummaryTypeDef",
     "AutoScalingConfigurationTypeDef",
     "CertificateValidationRecordTypeDef",
+    "CodeConfigurationValuesOutputTypeDef",
     "CodeConfigurationValuesTypeDef",
+    "SourceCodeVersionOutputTypeDef",
     "SourceCodeVersionTypeDef",
     "ConnectionSummaryTypeDef",
     "ConnectionTypeDef",
     "TagTypeDef",
     "TraceConfigurationTypeDef",
     "EncryptionConfigurationTypeDef",
     "HealthCheckConfigurationTypeDef",
@@ -70,79 +73,94 @@
     "DescribeAutoScalingConfigurationRequestRequestTypeDef",
     "DescribeCustomDomainsRequestRequestTypeDef",
     "DescribeObservabilityConfigurationRequestRequestTypeDef",
     "DescribeServiceRequestRequestTypeDef",
     "DescribeVpcConnectorRequestRequestTypeDef",
     "DescribeVpcIngressConnectionRequestRequestTypeDef",
     "DisassociateCustomDomainRequestRequestTypeDef",
+    "EgressConfigurationOutputTypeDef",
     "EgressConfigurationTypeDef",
+    "EncryptionConfigurationOutputTypeDef",
+    "HealthCheckConfigurationOutputTypeDef",
+    "ImageConfigurationOutputTypeDef",
     "ImageConfigurationTypeDef",
+    "IngressConfigurationOutputTypeDef",
     "IngressConfigurationTypeDef",
+    "IngressVpcConfigurationOutputTypeDef",
+    "InstanceConfigurationOutputTypeDef",
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListObservabilityConfigurationsRequestRequestTypeDef",
     "ObservabilityConfigurationSummaryTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "OperationSummaryTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ServiceSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListVpcConnectorsRequestRequestTypeDef",
     "ListVpcIngressConnectionsFilterTypeDef",
     "VpcIngressConnectionSummaryTypeDef",
+    "TraceConfigurationOutputTypeDef",
     "PauseServiceRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResumeServiceRequestRequestTypeDef",
+    "ServiceObservabilityConfigurationOutputTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StartDeploymentResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ListAutoScalingConfigurationsResponseTypeDef",
     "CreateAutoScalingConfigurationResponseTypeDef",
     "DeleteAutoScalingConfigurationResponseTypeDef",
     "DescribeAutoScalingConfigurationResponseTypeDef",
     "CustomDomainTypeDef",
+    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "CreateAutoScalingConfigurationRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateVpcConnectorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateObservabilityConfigurationRequestRequestTypeDef",
-    "ObservabilityConfigurationTypeDef",
     "CreateVpcConnectorResponseTypeDef",
     "DeleteVpcConnectorResponseTypeDef",
     "DescribeVpcConnectorResponseTypeDef",
     "ListVpcConnectorsResponseTypeDef",
     "CreateVpcIngressConnectionRequestRequestTypeDef",
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
-    "VpcIngressConnectionTypeDef",
+    "ImageRepositoryOutputTypeDef",
     "ImageRepositoryTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
+    "VpcIngressConnectionTypeDef",
     "ListObservabilityConfigurationsResponseTypeDef",
     "ListOperationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     "ListVpcIngressConnectionsResponseTypeDef",
+    "ObservabilityConfigurationTypeDef",
     "AssociateCustomDomainResponseTypeDef",
     "DescribeCustomDomainsResponseTypeDef",
     "DisassociateCustomDomainResponseTypeDef",
+    "CodeRepositoryOutputTypeDef",
     "CodeRepositoryTypeDef",
-    "CreateObservabilityConfigurationResponseTypeDef",
-    "DeleteObservabilityConfigurationResponseTypeDef",
-    "DescribeObservabilityConfigurationResponseTypeDef",
     "CreateVpcIngressConnectionResponseTypeDef",
     "DeleteVpcIngressConnectionResponseTypeDef",
     "DescribeVpcIngressConnectionResponseTypeDef",
     "UpdateVpcIngressConnectionResponseTypeDef",
+    "CreateObservabilityConfigurationResponseTypeDef",
+    "DeleteObservabilityConfigurationResponseTypeDef",
+    "DescribeObservabilityConfigurationResponseTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "CreateServiceRequestRequestTypeDef",
     "ServiceTypeDef",
+    "CreateServiceRequestRequestTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServiceResponseTypeDef",
     "PauseServiceResponseTypeDef",
     "ResumeServiceResponseTypeDef",
     "UpdateServiceResponseTypeDef",
@@ -175,14 +193,23 @@
         "VpcIngressConnectionArn": str,
         "VpcId": str,
         "DomainName": str,
     },
     total=False,
 )
 
+AuthenticationConfigurationOutputTypeDef = TypedDict(
+    "AuthenticationConfigurationOutputTypeDef",
+    {
+        "ConnectionArn": str,
+        "AccessRoleArn": str,
+    },
+    total=False,
+)
+
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "ConnectionArn": str,
         "AccessRoleArn": str,
     },
     total=False,
@@ -222,14 +249,37 @@
         "Type": str,
         "Value": str,
         "Status": CertificateValidationRecordStatusType,
     },
     total=False,
 )
 
+_RequiredCodeConfigurationValuesOutputTypeDef = TypedDict(
+    "_RequiredCodeConfigurationValuesOutputTypeDef",
+    {
+        "Runtime": RuntimeType,
+    },
+)
+_OptionalCodeConfigurationValuesOutputTypeDef = TypedDict(
+    "_OptionalCodeConfigurationValuesOutputTypeDef",
+    {
+        "BuildCommand": str,
+        "StartCommand": str,
+        "Port": str,
+        "RuntimeEnvironmentVariables": Dict[str, str],
+        "RuntimeEnvironmentSecrets": Dict[str, str],
+    },
+    total=False,
+)
+
+class CodeConfigurationValuesOutputTypeDef(
+    _RequiredCodeConfigurationValuesOutputTypeDef, _OptionalCodeConfigurationValuesOutputTypeDef
+):
+    pass
+
 _RequiredCodeConfigurationValuesTypeDef = TypedDict(
     "_RequiredCodeConfigurationValuesTypeDef",
     {
         "Runtime": RuntimeType,
     },
 )
 _OptionalCodeConfigurationValuesTypeDef = TypedDict(
@@ -245,14 +295,22 @@
 )
 
 class CodeConfigurationValuesTypeDef(
     _RequiredCodeConfigurationValuesTypeDef, _OptionalCodeConfigurationValuesTypeDef
 ):
     pass
 
+SourceCodeVersionOutputTypeDef = TypedDict(
+    "SourceCodeVersionOutputTypeDef",
+    {
+        "Type": Literal["BRANCH"],
+        "Value": str,
+    },
+)
+
 SourceCodeVersionTypeDef = TypedDict(
     "SourceCodeVersionTypeDef",
     {
         "Type": Literal["BRANCH"],
         "Value": str,
     },
 )
@@ -473,42 +531,109 @@
     "DisassociateCustomDomainRequestRequestTypeDef",
     {
         "ServiceArn": str,
         "DomainName": str,
     },
 )
 
+EgressConfigurationOutputTypeDef = TypedDict(
+    "EgressConfigurationOutputTypeDef",
+    {
+        "EgressType": EgressTypeType,
+        "VpcConnectorArn": str,
+    },
+    total=False,
+)
+
 EgressConfigurationTypeDef = TypedDict(
     "EgressConfigurationTypeDef",
     {
         "EgressType": EgressTypeType,
         "VpcConnectorArn": str,
     },
     total=False,
 )
 
+EncryptionConfigurationOutputTypeDef = TypedDict(
+    "EncryptionConfigurationOutputTypeDef",
+    {
+        "KmsKey": str,
+    },
+)
+
+HealthCheckConfigurationOutputTypeDef = TypedDict(
+    "HealthCheckConfigurationOutputTypeDef",
+    {
+        "Protocol": HealthCheckProtocolType,
+        "Path": str,
+        "Interval": int,
+        "Timeout": int,
+        "HealthyThreshold": int,
+        "UnhealthyThreshold": int,
+    },
+    total=False,
+)
+
+ImageConfigurationOutputTypeDef = TypedDict(
+    "ImageConfigurationOutputTypeDef",
+    {
+        "RuntimeEnvironmentVariables": Dict[str, str],
+        "StartCommand": str,
+        "Port": str,
+        "RuntimeEnvironmentSecrets": Dict[str, str],
+    },
+    total=False,
+)
+
 ImageConfigurationTypeDef = TypedDict(
     "ImageConfigurationTypeDef",
     {
         "RuntimeEnvironmentVariables": Mapping[str, str],
         "StartCommand": str,
         "Port": str,
         "RuntimeEnvironmentSecrets": Mapping[str, str],
     },
     total=False,
 )
 
+IngressConfigurationOutputTypeDef = TypedDict(
+    "IngressConfigurationOutputTypeDef",
+    {
+        "IsPubliclyAccessible": bool,
+    },
+    total=False,
+)
+
 IngressConfigurationTypeDef = TypedDict(
     "IngressConfigurationTypeDef",
     {
         "IsPubliclyAccessible": bool,
     },
     total=False,
 )
 
+IngressVpcConfigurationOutputTypeDef = TypedDict(
+    "IngressVpcConfigurationOutputTypeDef",
+    {
+        "VpcId": str,
+        "VpcEndpointId": str,
+    },
+    total=False,
+)
+
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "Cpu": str,
+        "Memory": str,
+        "InstanceRoleArn": str,
+    },
+    total=False,
+)
+
 ListAutoScalingConfigurationsRequestRequestTypeDef = TypedDict(
     "ListAutoScalingConfigurationsRequestRequestTypeDef",
     {
         "AutoScalingConfigurationName": str,
         "LatestOnly": bool,
         "MaxResults": int,
         "NextToken": str,
@@ -607,14 +732,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
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
 ListVpcConnectorsRequestRequestTypeDef = TypedDict(
     "ListVpcConnectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -634,14 +768,21 @@
     {
         "VpcIngressConnectionArn": str,
         "ServiceArn": str,
     },
     total=False,
 )
 
+TraceConfigurationOutputTypeDef = TypedDict(
+    "TraceConfigurationOutputTypeDef",
+    {
+        "Vendor": Literal["AWSXRAY"],
+    },
+)
+
 PauseServiceRequestRequestTypeDef = TypedDict(
     "PauseServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
@@ -659,14 +800,34 @@
 ResumeServiceRequestRequestTypeDef = TypedDict(
     "ResumeServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
+_RequiredServiceObservabilityConfigurationOutputTypeDef = TypedDict(
+    "_RequiredServiceObservabilityConfigurationOutputTypeDef",
+    {
+        "ObservabilityEnabled": bool,
+    },
+)
+_OptionalServiceObservabilityConfigurationOutputTypeDef = TypedDict(
+    "_OptionalServiceObservabilityConfigurationOutputTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+    },
+    total=False,
+)
+
+class ServiceObservabilityConfigurationOutputTypeDef(
+    _RequiredServiceObservabilityConfigurationOutputTypeDef,
+    _OptionalServiceObservabilityConfigurationOutputTypeDef,
+):
+    pass
+
 StartDeploymentRequestRequestTypeDef = TypedDict(
     "StartDeploymentRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
 )
 
@@ -734,14 +895,33 @@
     },
     total=False,
 )
 
 class CustomDomainTypeDef(_RequiredCustomDomainTypeDef, _OptionalCustomDomainTypeDef):
     pass
 
+_RequiredCodeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredCodeConfigurationOutputTypeDef",
+    {
+        "ConfigurationSource": ConfigurationSourceType,
+    },
+)
+_OptionalCodeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalCodeConfigurationOutputTypeDef",
+    {
+        "CodeConfigurationValues": CodeConfigurationValuesOutputTypeDef,
+    },
+    total=False,
+)
+
+class CodeConfigurationOutputTypeDef(
+    _RequiredCodeConfigurationOutputTypeDef, _OptionalCodeConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredCodeConfigurationTypeDef = TypedDict(
     "_RequiredCodeConfigurationTypeDef",
     {
         "ConfigurationSource": ConfigurationSourceType,
     },
 )
 _OptionalCodeConfigurationTypeDef = TypedDict(
@@ -843,22 +1023,14 @@
 
 class CreateVpcConnectorRequestRequestTypeDef(
     _RequiredCreateVpcConnectorRequestRequestTypeDef,
     _OptionalCreateVpcConnectorRequestRequestTypeDef,
 ):
     pass
 
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
@@ -880,29 +1052,14 @@
 
 class CreateObservabilityConfigurationRequestRequestTypeDef(
     _RequiredCreateObservabilityConfigurationRequestRequestTypeDef,
     _OptionalCreateObservabilityConfigurationRequestRequestTypeDef,
 ):
     pass
 
-ObservabilityConfigurationTypeDef = TypedDict(
-    "ObservabilityConfigurationTypeDef",
-    {
-        "ObservabilityConfigurationArn": str,
-        "ObservabilityConfigurationName": str,
-        "TraceConfiguration": TraceConfigurationTypeDef,
-        "ObservabilityConfigurationRevision": int,
-        "Latest": bool,
-        "Status": ObservabilityConfigurationStatusType,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
-    },
-    total=False,
-)
-
 CreateVpcConnectorResponseTypeDef = TypedDict(
     "CreateVpcConnectorResponseTypeDef",
     {
         "VpcConnector": VpcConnectorTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -958,30 +1115,34 @@
     "UpdateVpcIngressConnectionRequestRequestTypeDef",
     {
         "VpcIngressConnectionArn": str,
         "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
     },
 )
 
-VpcIngressConnectionTypeDef = TypedDict(
-    "VpcIngressConnectionTypeDef",
+_RequiredImageRepositoryOutputTypeDef = TypedDict(
+    "_RequiredImageRepositoryOutputTypeDef",
     {
-        "VpcIngressConnectionArn": str,
-        "VpcIngressConnectionName": str,
-        "ServiceArn": str,
-        "Status": VpcIngressConnectionStatusType,
-        "AccountId": str,
-        "DomainName": str,
-        "IngressVpcConfiguration": IngressVpcConfigurationTypeDef,
-        "CreatedAt": datetime,
-        "DeletedAt": datetime,
+        "ImageIdentifier": str,
+        "ImageRepositoryType": ImageRepositoryTypeType,
+    },
+)
+_OptionalImageRepositoryOutputTypeDef = TypedDict(
+    "_OptionalImageRepositoryOutputTypeDef",
+    {
+        "ImageConfiguration": ImageConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+class ImageRepositoryOutputTypeDef(
+    _RequiredImageRepositoryOutputTypeDef, _OptionalImageRepositoryOutputTypeDef
+):
+    pass
+
 _RequiredImageRepositoryTypeDef = TypedDict(
     "_RequiredImageRepositoryTypeDef",
     {
         "ImageIdentifier": str,
         "ImageRepositoryType": ImageRepositoryTypeType,
     },
 )
@@ -992,23 +1153,48 @@
     },
     total=False,
 )
 
 class ImageRepositoryTypeDef(_RequiredImageRepositoryTypeDef, _OptionalImageRepositoryTypeDef):
     pass
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "EgressConfiguration": EgressConfigurationOutputTypeDef,
+        "IngressConfiguration": IngressConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "EgressConfiguration": EgressConfigurationTypeDef,
         "IngressConfiguration": IngressConfigurationTypeDef,
     },
     total=False,
 )
 
+VpcIngressConnectionTypeDef = TypedDict(
+    "VpcIngressConnectionTypeDef",
+    {
+        "VpcIngressConnectionArn": str,
+        "VpcIngressConnectionName": str,
+        "ServiceArn": str,
+        "Status": VpcIngressConnectionStatusType,
+        "AccountId": str,
+        "DomainName": str,
+        "IngressVpcConfiguration": IngressVpcConfigurationOutputTypeDef,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 ListObservabilityConfigurationsResponseTypeDef = TypedDict(
     "ListObservabilityConfigurationsResponseTypeDef",
     {
         "ObservabilityConfigurationSummaryList": List[ObservabilityConfigurationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1028,14 +1214,22 @@
     {
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 ListVpcIngressConnectionsRequestRequestTypeDef = TypedDict(
     "ListVpcIngressConnectionsRequestRequestTypeDef",
     {
         "Filter": ListVpcIngressConnectionsFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1047,14 +1241,29 @@
     {
         "VpcIngressConnectionSummaryList": List[VpcIngressConnectionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ObservabilityConfigurationTypeDef = TypedDict(
+    "ObservabilityConfigurationTypeDef",
+    {
+        "ObservabilityConfigurationArn": str,
+        "ObservabilityConfigurationName": str,
+        "TraceConfiguration": TraceConfigurationOutputTypeDef,
+        "ObservabilityConfigurationRevision": int,
+        "Latest": bool,
+        "Status": ObservabilityConfigurationStatusType,
+        "CreatedAt": datetime,
+        "DeletedAt": datetime,
+    },
+    total=False,
+)
+
 AssociateCustomDomainResponseTypeDef = TypedDict(
     "AssociateCustomDomainResponseTypeDef",
     {
         "DNSTarget": str,
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
@@ -1081,14 +1290,34 @@
         "ServiceArn": str,
         "CustomDomain": CustomDomainTypeDef,
         "VpcDNSTargets": List[VpcDNSTargetTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredCodeRepositoryOutputTypeDef = TypedDict(
+    "_RequiredCodeRepositoryOutputTypeDef",
+    {
+        "RepositoryUrl": str,
+        "SourceCodeVersion": SourceCodeVersionOutputTypeDef,
+    },
+)
+_OptionalCodeRepositoryOutputTypeDef = TypedDict(
+    "_OptionalCodeRepositoryOutputTypeDef",
+    {
+        "CodeConfiguration": CodeConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class CodeRepositoryOutputTypeDef(
+    _RequiredCodeRepositoryOutputTypeDef, _OptionalCodeRepositoryOutputTypeDef
+):
+    pass
+
 _RequiredCodeRepositoryTypeDef = TypedDict(
     "_RequiredCodeRepositoryTypeDef",
     {
         "RepositoryUrl": str,
         "SourceCodeVersion": SourceCodeVersionTypeDef,
     },
 )
@@ -1099,135 +1328,146 @@
     },
     total=False,
 )
 
 class CodeRepositoryTypeDef(_RequiredCodeRepositoryTypeDef, _OptionalCodeRepositoryTypeDef):
     pass
 
-CreateObservabilityConfigurationResponseTypeDef = TypedDict(
-    "CreateObservabilityConfigurationResponseTypeDef",
+CreateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "CreateVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DeleteObservabilityConfigurationResponseTypeDef",
+DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DeleteVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
-    "DescribeObservabilityConfigurationResponseTypeDef",
+DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
+    "DescribeVpcIngressConnectionResponseTypeDef",
     {
-        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
+        "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "CreateVpcIngressConnectionResponseTypeDef",
+UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
+    "UpdateVpcIngressConnectionResponseTypeDef",
     {
         "VpcIngressConnection": VpcIngressConnectionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeleteVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DeleteVpcIngressConnectionResponseTypeDef",
+CreateObservabilityConfigurationResponseTypeDef = TypedDict(
+    "CreateObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DescribeVpcIngressConnectionResponseTypeDef = TypedDict(
-    "DescribeVpcIngressConnectionResponseTypeDef",
+DeleteObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DeleteObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateVpcIngressConnectionResponseTypeDef = TypedDict(
-    "UpdateVpcIngressConnectionResponseTypeDef",
+DescribeObservabilityConfigurationResponseTypeDef = TypedDict(
+    "DescribeObservabilityConfigurationResponseTypeDef",
     {
-        "VpcIngressConnection": VpcIngressConnectionTypeDef,
+        "ObservabilityConfiguration": ObservabilityConfigurationTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-SourceConfigurationTypeDef = TypedDict(
-    "SourceConfigurationTypeDef",
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
     {
-        "CodeRepository": CodeRepositoryTypeDef,
-        "ImageRepository": ImageRepositoryTypeDef,
+        "CodeRepository": CodeRepositoryOutputTypeDef,
+        "ImageRepository": ImageRepositoryOutputTypeDef,
         "AutoDeploymentsEnabled": bool,
-        "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
+        "AuthenticationConfiguration": AuthenticationConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateServiceRequestRequestTypeDef",
-    {
-        "ServiceName": str,
-        "SourceConfiguration": SourceConfigurationTypeDef,
-    },
-)
-_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateServiceRequestRequestTypeDef",
+SourceConfigurationTypeDef = TypedDict(
+    "SourceConfigurationTypeDef",
     {
-        "InstanceConfiguration": InstanceConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
-        "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
-        "AutoScalingConfigurationArn": str,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
-        "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
+        "CodeRepository": CodeRepositoryTypeDef,
+        "ImageRepository": ImageRepositoryTypeDef,
+        "AutoDeploymentsEnabled": bool,
+        "AuthenticationConfiguration": AuthenticationConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateServiceRequestRequestTypeDef(
-    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
-):
-    pass
-
 _RequiredServiceTypeDef = TypedDict(
     "_RequiredServiceTypeDef",
     {
         "ServiceName": str,
         "ServiceId": str,
         "ServiceArn": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "Status": ServiceStatusType,
-        "SourceConfiguration": SourceConfigurationTypeDef,
-        "InstanceConfiguration": InstanceConfigurationTypeDef,
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "InstanceConfiguration": InstanceConfigurationOutputTypeDef,
         "AutoScalingConfigurationSummary": AutoScalingConfigurationSummaryTypeDef,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
     },
 )
 _OptionalServiceTypeDef = TypedDict(
     "_OptionalServiceTypeDef",
     {
         "ServiceUrl": str,
         "DeletedAt": datetime,
+        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "HealthCheckConfiguration": HealthCheckConfigurationOutputTypeDef,
+        "ObservabilityConfiguration": ServiceObservabilityConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
+    pass
+
+_RequiredCreateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateServiceRequestRequestTypeDef",
+    {
+        "ServiceName": str,
+        "SourceConfiguration": SourceConfigurationTypeDef,
+    },
+)
+_OptionalCreateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateServiceRequestRequestTypeDef",
+    {
+        "InstanceConfiguration": InstanceConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "HealthCheckConfiguration": HealthCheckConfigurationTypeDef,
+        "AutoScalingConfigurationArn": str,
+        "NetworkConfiguration": NetworkConfigurationTypeDef,
         "ObservabilityConfiguration": ServiceObservabilityConfigurationTypeDef,
     },
     total=False,
 )
 
-class ServiceTypeDef(_RequiredServiceTypeDef, _OptionalServiceTypeDef):
+class CreateServiceRequestRequestTypeDef(
+    _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
+):
     pass
 
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "ServiceArn": str,
     },
```

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/PKG-INFO` & `mypy-boto3-apprunner-1.28.12/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-apprunner
-Version: 1.28.0
-Summary: Type annotations for boto3.AppRunner 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 apprunner type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-apprunner"></a>
 
 # mypy-boto3-apprunner
 
 [![PyPI - mypy-boto3-apprunner](https://img.shields.io/pypi/v/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apprunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-apprunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-apprunner?color=blue)](https://pypistats.org/packages/mypy-boto3-apprunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apprunner)](https://pepy.tech/project/mypy-boto3-apprunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppRunner 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
+[boto3.AppRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#AppRunner)
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
 [mypy-boto3-apprunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apprunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -315,19 +283,22 @@
 `mypy_boto3_apprunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apprunner.type_defs import (
     AssociateCustomDomainRequestRequestTypeDef,
     VpcDNSTargetTypeDef,
+    AuthenticationConfigurationOutputTypeDef,
     AuthenticationConfigurationTypeDef,
     AutoScalingConfigurationSummaryTypeDef,
     AutoScalingConfigurationTypeDef,
     CertificateValidationRecordTypeDef,
+    CodeConfigurationValuesOutputTypeDef,
     CodeConfigurationValuesTypeDef,
+    SourceCodeVersionOutputTypeDef,
     SourceCodeVersionTypeDef,
     ConnectionSummaryTypeDef,
     ConnectionTypeDef,
     TagTypeDef,
     TraceConfigurationTypeDef,
     EncryptionConfigurationTypeDef,
     HealthCheckConfigurationTypeDef,
@@ -344,79 +315,94 @@
     DescribeAutoScalingConfigurationRequestRequestTypeDef,
     DescribeCustomDomainsRequestRequestTypeDef,
     DescribeObservabilityConfigurationRequestRequestTypeDef,
     DescribeServiceRequestRequestTypeDef,
     DescribeVpcConnectorRequestRequestTypeDef,
     DescribeVpcIngressConnectionRequestRequestTypeDef,
     DisassociateCustomDomainRequestRequestTypeDef,
+    EgressConfigurationOutputTypeDef,
     EgressConfigurationTypeDef,
+    EncryptionConfigurationOutputTypeDef,
+    HealthCheckConfigurationOutputTypeDef,
+    ImageConfigurationOutputTypeDef,
     ImageConfigurationTypeDef,
+    IngressConfigurationOutputTypeDef,
     IngressConfigurationTypeDef,
+    IngressVpcConfigurationOutputTypeDef,
+    InstanceConfigurationOutputTypeDef,
     ListAutoScalingConfigurationsRequestRequestTypeDef,
     ListConnectionsRequestRequestTypeDef,
     ListObservabilityConfigurationsRequestRequestTypeDef,
     ObservabilityConfigurationSummaryTypeDef,
     ListOperationsRequestRequestTypeDef,
     OperationSummaryTypeDef,
     ListServicesRequestRequestTypeDef,
     ServiceSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListVpcConnectorsRequestRequestTypeDef,
     ListVpcIngressConnectionsFilterTypeDef,
     VpcIngressConnectionSummaryTypeDef,
+    TraceConfigurationOutputTypeDef,
     PauseServiceRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResumeServiceRequestRequestTypeDef,
+    ServiceObservabilityConfigurationOutputTypeDef,
     StartDeploymentRequestRequestTypeDef,
     StartDeploymentResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     ListAutoScalingConfigurationsResponseTypeDef,
     CreateAutoScalingConfigurationResponseTypeDef,
     DeleteAutoScalingConfigurationResponseTypeDef,
     DescribeAutoScalingConfigurationResponseTypeDef,
     CustomDomainTypeDef,
+    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     ListConnectionsResponseTypeDef,
     CreateConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     CreateAutoScalingConfigurationRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateVpcConnectorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateObservabilityConfigurationRequestRequestTypeDef,
-    ObservabilityConfigurationTypeDef,
     CreateVpcConnectorResponseTypeDef,
     DeleteVpcConnectorResponseTypeDef,
     DescribeVpcConnectorResponseTypeDef,
     ListVpcConnectorsResponseTypeDef,
     CreateVpcIngressConnectionRequestRequestTypeDef,
     UpdateVpcIngressConnectionRequestRequestTypeDef,
-    VpcIngressConnectionTypeDef,
+    ImageRepositoryOutputTypeDef,
     ImageRepositoryTypeDef,
+    NetworkConfigurationOutputTypeDef,
     NetworkConfigurationTypeDef,
+    VpcIngressConnectionTypeDef,
     ListObservabilityConfigurationsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVpcIngressConnectionsRequestRequestTypeDef,
     ListVpcIngressConnectionsResponseTypeDef,
+    ObservabilityConfigurationTypeDef,
     AssociateCustomDomainResponseTypeDef,
     DescribeCustomDomainsResponseTypeDef,
     DisassociateCustomDomainResponseTypeDef,
+    CodeRepositoryOutputTypeDef,
     CodeRepositoryTypeDef,
-    CreateObservabilityConfigurationResponseTypeDef,
-    DeleteObservabilityConfigurationResponseTypeDef,
-    DescribeObservabilityConfigurationResponseTypeDef,
     CreateVpcIngressConnectionResponseTypeDef,
     DeleteVpcIngressConnectionResponseTypeDef,
     DescribeVpcIngressConnectionResponseTypeDef,
     UpdateVpcIngressConnectionResponseTypeDef,
+    CreateObservabilityConfigurationResponseTypeDef,
+    DeleteObservabilityConfigurationResponseTypeDef,
+    DescribeObservabilityConfigurationResponseTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
-    CreateServiceRequestRequestTypeDef,
     ServiceTypeDef,
+    CreateServiceRequestRequestTypeDef,
     UpdateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DescribeServiceResponseTypeDef,
     PauseServiceResponseTypeDef,
     ResumeServiceResponseTypeDef,
     UpdateServiceResponseTypeDef,
```

### Comparing `mypy-boto3-apprunner-1.28.0/mypy_boto3_apprunner.egg-info/SOURCES.txt` & `mypy-boto3-apprunner-1.28.12/mypy_boto3_apprunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apprunner-1.28.0/setup.py` & `mypy-boto3-apprunner-1.28.12/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apprunner",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_apprunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppRunner 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.AppRunner 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

